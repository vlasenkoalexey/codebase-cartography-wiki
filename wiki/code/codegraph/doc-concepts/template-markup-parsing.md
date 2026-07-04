---
title: Template / markup parsing
type: doc-concept
provenance: doc
source: docs/design/template-markup-parser.md
updated: 2026-07-04
status: fresh
---
# Template / markup parsing

## Definition
CodeGraph's impact graph is built only from code the engine parses, so any class,
component, view-model, or DTO that is referenced **only from template markup**
(Razor `.cshtml`/`.razor`, Blazor components, Vue SFC `<template>`, Liquid, Svelte,
Thymeleaf, Django) looks like it has no in-repo dependent — a graph hole. On
convention-heavy frameworks this markup-only reference is *the dominant residual
gap* after framework-entry exclusions (e.g. eShopOnWeb ASP.NET: 77% FAIR coverage,
with Razor/Blazor referencing `.cs` the engine never parsed). Template-markup
parsing closes it by scanning the stylized markup and emitting ordinary
`references` edges from the template file into the symbol graph, so a `<Child/>`
component tag or an `@model Foo` directive becomes a real edge to `Foo`.

## In codegraph (grounded)
The mental model is a **standalone extractor per markup family**, mirroring the
non-tree-sitter extractors the engine already has — a class taking
`(filePath, source)` and returning `{ nodes, references }`, wired into the
extension→language map and the dispatch switch, with **no new resolver**.

- **Extension → synthetic language.** `.cshtml`/`.razor` map to a synthetic `razor`
  language in the grammar registry — the [`EXTENSION_MAP`](../catalog/src/extraction/grammars.ts.md#EXTENSION_MAP)
  / [`detectLanguage`](../catalog/src/extraction/grammars.ts.md#detectLanguage) in
  [grammars.ts](../catalog/src/extraction/grammars.ts.md). A template file is a
  file-level graph citizen (cf. [`isFileLevelOnlyLanguage`](../catalog/src/extraction/grammars.ts.md#isFileLevelOnlyLanguage)),
  not a full tree-sitter parse.
- **Dispatch by extension.** [`extractFromSource`](../catalog/src/extraction/tree-sitter.ts.md#extractFromSource)
  in [tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md) routes each
  markup extension to its standalone extractor, exactly as it already dispatches the
  [`SvelteExtractor`](../catalog/src/extraction/svelte-extractor.ts.md#SvelteExtractor),
  [`VueExtractor`](../catalog/src/extraction/vue-extractor.ts.md#VueExtractor), and
  [`LiquidExtractor`](../catalog/src/extraction/liquid-extractor.ts.md#LiquidExtractor) —
  none of which use a tree-sitter grammar for the markup itself.
- **The Razor/Blazor extractor.** [`RazorExtractor`](../catalog/src/extraction/razor-extractor.ts.md#RazorExtractor)
  in [razor-extractor.ts](../catalog/src/extraction/razor-extractor.ts.md) does a
  regex/line scan (markup is highly stylized — no grammar needed). It emits **one
  `component` node for the whole file** via
  [`createComponentNode`](../catalog/src/extraction/razor-extractor.ts.md#RazorExtractor.createComponentNode)
  so the `.razor` file is linkable as a `<X/>` target, then emits `references` for
  each markup construct:
  [`extractDirectives`](../catalog/src/extraction/razor-extractor.ts.md#RazorExtractor.extractDirectives)
  handles `@model Foo`, `@inherits X<Foo>`, `@inject IBar bar`, `@typeof(T)`;
  [`extractComponentTags`](../catalog/src/extraction/razor-extractor.ts.md#RazorExtractor.extractComponentTags)
  handles `<PascalComponent/>` element tags (only `[A-Z]`-initial tags are Blazor
  components — a safe discriminator against lowercase HTML), skipping framework
  built-ins via the [`BLAZOR_BUILTIN_COMPONENTS`](../catalog/src/extraction/razor-extractor.ts.md#BLAZOR_BUILTIN_COMPONENTS)
  set; and [`processCodeBlocks`](../catalog/src/extraction/razor-extractor.ts.md#RazorExtractor.processCodeBlocks)
  delegates `@code`/`@functions`/`@{ }` C# blocks to the tree-sitter C# path.
- **Vue SFC templates — a resolver pass, not an extractor.** The `.vue` extractor
  only parses `<script>`, so template-only references (`<Child/>` components,
  `@click="handler"` bound handlers) are recovered later by
  [`vueTemplateEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#vueTemplateEdges)
  in the callback synthesizer — a second shape of the same idea (bridge template
  markup into the graph), applied at resolution time rather than extraction time.
- **Resolution: no new resolver.** Emitted refs are ordinary `references` to a
  class/component **by name**, so the existing name-matcher resolves them
  ([`matchReference`](../catalog/src/resolution/name-matcher.ts.md#matchReference) /
  [`matchByExactName`](../catalog/src/resolution/name-matcher.ts.md#matchByExactName)).
  The **one** resolver-side change is the cross-family language gate: a `razor` ref
  must be allowed to resolve to a `csharp` symbol, so `razor`↔`csharp` must be
  treated as same-family in [`applyLanguageGate`](../catalog/src/resolution/name-matcher.ts.md#applyLanguageGate) —
  otherwise the family gate drops every markup edge.

## Why it matters / when it applies
This is primarily an **ASP.NET (Razor + Blazor) win**: it lifts the honest coverage
ceiling from ~77% toward ~90% on convention-heavy .NET apps, recovering the
markup-only ViewModels, DTOs (via component params / `@bind`), and `.cs`
`ComponentBase` components that a plain host-language parse never sees. Key
invariants: **+1 `component` node per template file only** (component tags become
`references` edges, not nodes — no per-tag node explosion), all edges are
`references` (counted by impact / `affected` / `getFileDependents`, not
callers/callees), and re-indexing is idempotent (node count stable across re-runs).
It applies wherever a framework routes real code references through markup; it is
explicitly *lower priority* for Thymeleaf and Django, whose template links to code
are weak (template→template fragments, fuzzy model-attribute strings) and whose real
gaps lie elsewhere. Out of scope by design: property-string data bindings
(`asp-for`, `th:field`) that would need model-type inference, and the
reflection/proxy + static-const value-read frontier (AutoMapper, Swagger, DI
registration, `Constants.X`) — separate features needed to reach literal 95%.

## Connections
- Code concepts:
  [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md) —
  the `vueTemplateEdges` pass and the synthesizer that bridges template markup at
  resolution time;
  [extraction-tree-sitter.ts](../concepts/extraction-tree-sitter.ts.md) — the
  extractor dispatch (`extractFromSource`) that routes markup to standalone
  extractors;
  [extraction-tree-sitter-types.ts](../concepts/extraction-tree-sitter-types.ts.md) —
  the `{ nodes, references }` extraction-result shape every markup extractor returns.
- Module catalogs:
  [razor-extractor.ts](../catalog/src/extraction/razor-extractor.ts.md),
  [grammars.ts](../catalog/src/extraction/grammars.ts.md),
  [tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md),
  [svelte-extractor.ts](../catalog/src/extraction/svelte-extractor.ts.md),
  [vue-extractor.ts](../catalog/src/extraction/vue-extractor.ts.md),
  [liquid-extractor.ts](../catalog/src/extraction/liquid-extractor.ts.md),
  [callback-synthesizer.ts](../catalog/src/resolution/callback-synthesizer.ts.md),
  [name-matcher.ts](../catalog/src/resolution/name-matcher.ts.md).
- Related doc-concepts:
  [dynamic-dispatch-coverage.md](dynamic-dispatch-coverage.md) — template edges are
  one channel of the same "make the flow exist in the graph" coverage program;
  [value-reference-edges.md](value-reference-edges.md) — the static-const value-read
  frontier this feature explicitly does *not* close;
  [cross-language-native-bridging.md](cross-language-native-bridging.md) — the same
  cross-family language-gate machinery that lets a `razor` ref resolve to a `csharp`
  symbol.

## Source
Extracted from `docs/design/template-markup-parser.md` (kept in place).
