---
title: "Extractor primitives: the language-agnostic tree-sitter toolkit"
type: concept
provenance: mixed
concept: understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts
concepts: [multi-language-extraction]
updated: 2026-07-04
status: fresh
---
# Extractor primitives: the language-agnostic tree-sitter toolkit

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [multi-language-extraction](../../../concepts/multi-language-extraction.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview
`base-extractor.ts` is the four-function toolbox that every one of Understand-Anything's
twelve per-language extractors is built on. It contains no language knowledge at all — just
generic ways to walk a tree-sitter **concrete syntax tree** (CST) and pull text out of it:
[`traverse`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#traverse)
(recurse over every node),
[`findChild`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChild) /
[`findChildren`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChildren)
(pick children by their grammar node **type string**), and
[`getStringValue`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#getStringValue)
(unquote a string literal). All of them operate on a single opaque node type,
[`TreeSitterNode`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#TreeSitterNode).

The key idea — and what makes this repo comparable to wikify-repo and graphify along the
**multi-language-extraction** axis — is *where the language-specificity lives*. Understand-Anything
does **not** resolve symbols semantically (no SCIP, no type-checker, no cross-file name resolution).
Its grounding substrate is the raw tree-sitter CST, and each language is handled by a hand-written
extractor that recognises that grammar's node-type strings (`"class_declaration"`,
`"function_item"`, `"impl_item"`, …) and maps them onto one shared, language-neutral output shape
(`StructuralAnalysis` = functions/classes/imports/exports, plus a `CallGraphEntry[]`). This file is
the thin waist those twelve extractors all pass through.

## Diagram
```mermaid
flowchart TD
  subgraph barrel["extractors/index.ts (barrel + builtinExtractors)"]
    IDX["index.ts"]
  end
  subgraph prims["base-extractor.ts — shared primitives"]
    TRAV["traverse"]
    FC["findChild"]
    FCS["findChildren"]
    GSV["getStringValue"]
  end
  TSN["TreeSitterNode (web-tree-sitter Node)"]

  IDX -->|re-exports| TRAV
  IDX -->|re-exports| FC
  IDX -->|re-exports| FCS
  IDX -->|re-exports| GSV

  WS["PhpExtractor.walkStatements"] --> FC
  WTL["CppExtractor.walkTopLevel"] --> FC
  CCB["collectClassBody (dart)"] --> FC
  CCB --> FCS
  IMPL["RustExtractor.extractImpl"] --> FCS
  ECLD["DartExtractor.extractClassLikeDeclaration"] --> FC
  CG["SwiftExtractor.extractCallGraph"] --> FC

  TRAV -->|reads .childCount / .child(i)| TSN
  FC --> TSN
  FCS --> TSN
  GSV --> TSN
```

## Design rationale (why it's built this way)
The whole file is a deliberate refusal to over-engineer. Rather than a base *class* with template
methods, it exposes four free **functions** and lets each extractor compose them however that
language's grammar demands. The author docstrings state the intent plainly — `traverse` is to
"Recursively traverse an AST tree, calling the visitor for each node"
([`traverse`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#traverse)),
`findChild` to "Find the first child matching a type"
([`findChild`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChild)) —
and nothing more. Because a tree-sitter CST is uniform (every node answers `childCount` / `child(i)`),
one traversal implementation genuinely serves all twelve languages; the variation is pushed entirely
into *which node-type strings each extractor asks for*.

The matching key throughout is the grammar **node type as a string**, not a resolved symbol. That is
the central grounding decision and its consequence: extraction is fast, dependency-free, and works on
broken/partial files, but it is also *lexical-structural* rather than semantic — the tool sees that a
`class_declaration` node exists at some line, not what it refers to elsewhere. This is the substrate
that distinguishes Understand-Anything from a SCIP-grounded tool: comparability across the survey is
"same job, different depth of grounding."

> [!inferred]
> `getStringValue` encodes a small resilience trick: it first looks for a `"string_fragment"` child
> (tree-sitter models the *content* of a quoted literal as a separate child from the quote tokens),
> and only if none exists falls back to stripping surrounding quote characters off the node's own
> text. The two-path design lets one function unquote import paths across grammars whose string
> nodes are shaped differently — an import-source extraction convenience, read from the source rather
> than any docstring.

## Entry points
Control reaches this file from *inside* a language extractor, never from the top of the pipeline. A
language plugin resolves a file to an extractor, parses it to a CST, then that extractor's
`extractStructure` / `extractCallGraph` walk begins calling these helpers.

- [`findChild`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChild)
  and [`findChildren`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChildren)
  are the workhorses — the single-vs-many pair used everywhere an extractor needs to descend one level
  by grammar type. `findChild` scans children in order and returns the first whose `.type` equals the
  requested string (or `null`); `findChildren` collects all of them. They are the two most-referenced
  symbols in the whole extractor subsystem, invoked from essentially every language:
  [`PhpExtractor.walkStatements`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts.md#PhpExtractor.walkStatements)
  uses `findChild` to reach a block-namespace's `compound_statement` body,
  [`RustExtractor.extractImpl`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts.md#RustExtractor.extractImpl)
  uses `findChildren` to gather every `function_item` in an impl block.
- [`getStringValue`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#getStringValue)
  is the narrow-purpose helper for turning a quoted literal node (an import path, a module name) into
  its bare text. It is reached mainly from import/export extraction paths.
- [`traverse`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#traverse)
  is the whole-subtree visitor primitive — the escape hatch for "I don't know where in the subtree the
  interesting nodes are" — and the only recursive primitive here (it calls itself for each child). It is
  exported from the barrel for call-graph-style scans, but is in fact **unused**: it has no call sites, and
  the shipped call-graph builders (e.g.
  [`SwiftExtractor.extractCallGraph`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/swift-extractor.ts.md#SwiftExtractor.extractCallGraph))
  implement the same visit-then-descend shape with their own local recursive `walk` closure rather than
  calling it.

## Mechanism (step-by-step)
1. **Uniform CST access.** Every primitive treats a node as nothing more than an ordered bag of typed
   children, iterated with the tree-sitter `childCount` / `child(i)` API on
   [`TreeSitterNode`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#TreeSitterNode).
   Because that node type is simply `web-tree-sitter`'s WASM `Node`, the same code runs in Node and in
   the browser dashboard, and the extractors never depend on a native binding.
2. **Type-string selection.** An extractor that has, say, a class body node in hand pulls out the parts
   it wants by grammar type via
   [`findChild`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChild) /
   [`findChildren`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChildren).
   In [`DartExtractor.extractClassLikeDeclaration`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/dart-extractor.ts.md#DartExtractor.extractClassLikeDeclaration)
   the flow is exactly this: `findChild(declNode, "identifier")` for the name, then `findChild(declNode, bodyNodeType)`
   for the body — only descending if the child exists, which is how the extractors tolerate bodyless
   declarations (`class Empty`) without crashing.
2b. **Recursive descent into nested scopes.** Where declarations nest, the extractor recurses on the
    same helper set rather than a generic walk. `walkStatements` re-invokes itself on a namespace body
    found with `findChild`
    ([`PhpExtractor.walkStatements`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts.md#PhpExtractor.walkStatements)),
    and C++'s [`CppExtractor.walkTopLevel`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts.md#CppExtractor.walkTopLevel)
    recurses into `namespace_definition` bodies the same way — the primitives handle one level, the
    extractor supplies the recursion policy.
3. **Batch collection of members.** For "all the methods / fields of this type," an extractor calls
   `findChildren` once and loops. [`RustExtractor.extractImpl`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts.md#RustExtractor.extractImpl)
   collects every `function_item` this way and, importantly, mixes the *field-name* API
   (`childForFieldName("type")`, `childForFieldName("body")`) with the type-string API — a reminder that
   `findChild`/`findChildren` are a convenience over positional children, not the only access path an
   extractor uses. Dart's [`collectClassBody`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/dart-extractor.ts.md#collectClassBody)
   likewise leans on both `findChild` and `findChildren` to sweep a `class_body`.
4. **Literal unquoting.** When a matched child is a string (an import URI, a module path), the extractor
   normalises it with [`getStringValue`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#getStringValue),
   which prefers the `string_fragment` child and otherwise strips quotes — giving import extraction a
   single grammar-agnostic unquote step.
5. **Whole-subtree scans for call graphs.** When position is unpredictable, an extractor needs a
   whole-subtree, visit-then-descend walk — the shape
   [`traverse`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#traverse)
   provides (visit the node, then recurse into every child). In practice, though, the shipped call-graph
   builders such as
   [`SwiftExtractor.extractCallGraph`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/swift-extractor.ts.md#SwiftExtractor.extractCallGraph)
   implement this shape with their own local recursive `walk` closure rather than calling `traverse`
   (which has no call sites), since call sites are scattered through function bodies.
6. **One shared output shape.** Whichever primitives an extractor composes, the result is pushed into the
   common `StructuralAnalysis` arrays and `CallGraphEntry[]` defined by
   [`TreeSitterNode`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#TreeSitterNode)'s
   sibling `LanguageExtractor` interface — so twelve grammars converge on one representation the rest of
   the tool (graph assembly, dashboard) can consume uniformly.

## Key data structures
- [`TreeSitterNode`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#TreeSitterNode)
  — a bare `import("web-tree-sitter").Node`. This is the *only* input type the primitives know. It carries
  `type` (the grammar node-kind string these helpers match on), `childCount`/`child(i)` for positional
  descent, `childForFieldName` for named-field descent, `text`, and `startPosition`/`endPosition` (used by
  callers to compute 1-based line ranges). The primitives touch only `type`, `childCount`, `child`, and
  `text`.
- The **output** contract these helpers feed (defined alongside `TreeSitterNode` in the extractors'
  `types.ts` as `LanguageExtractor`): `extractStructure(root) -> StructuralAnalysis` and
  `extractCallGraph(root) -> CallGraphEntry[]`. `StructuralAnalysis` is the language-neutral target —
  `functions`, `classes`, `imports`, `exports` arrays with line ranges — that every extractor populates.

## Dynamics (design intent)
There is no concurrency here: all four primitives are synchronous, side-effect-free traversals over an
already-parsed tree (`traverse`'s visitor is the only place a side effect happens, and it's the caller's).
Ordering is deterministic — `findChild` returns the *first* matching child in source order and
`findChildren` preserves source order — which is why extractors can rely on positional assumptions after a
match. `traverse` is pre-order (visit-then-descend), relevant to any visitor that mutates shared
accumulator state as it goes.

## Edge cases
- **`findChild` returns `null`, not throw.** Every caller must null-check; the extractors uniformly do
  (`if (!nameNode) return;`). A missing expected child silently drops that declaration rather than erroring —
  resilient, but it means malformed or unusual code is under-reported, not flagged.
- **`getStringValue` double-strategy.** If a grammar doesn't model a `string_fragment` child, the
  quote-stripping fallback only removes a *single* leading/trailing `'`, `"`, or `` ` `` — nested or escaped
  quotes are not handled.
- **`traverse` visits the root itself first**, then all descendants, with no depth guard or cycle check
  (safe because a CST is a finite tree, but a visitor that re-enters `traverse` could blow the stack on
  pathological input).
- **Type widening in the index.** The SCIP-indexed signatures render these as `node: any` because the
  `web-tree-sitter` types don't fully resolve through the indexer; the actual source is strictly typed as
  `TreeSitterNode`. A reader trusting the catalog signature alone would understate the typing.

## Open questions
- The barrel also exports `hasChildOfType` (a boolean "does a child of this type exist," used for
  export/visibility checks), but it is outside this packet's subgraph, so its exact call sites aren't
  grounded here — worth a look when documenting export detection.
- These primitives cover *type-string* and *whole-tree* access, but many extractors also use tree-sitter's
  `childForFieldName` (named fields) directly (seen in `extractImpl`). Whether a field-name helper was
  deliberately left out of the shared toolbox, or just never factored out, isn't answerable from this file.

## See also
- [Dart extractor](./understand-anything-plugin-packages-core-src-plugins-extractors-dart-extractor.ts.md) — heaviest consumer of `collectClassBody` / `findChild` for class-like and enum declarations.
- [Swift extractor](./understand-anything-plugin-packages-core-src-plugins-extractors-swift-extractor.ts.md) — call-graph extraction built on a local recursive `walk` closure plus `findChild`.
- [Extractor types (`LanguageExtractor`, `TreeSitterNode`)](./understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md) — the interface these primitives serve.
- [Tree-sitter plugin](./understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md) — parses source into the CST these helpers walk.
- [Plugin registry](./understand-anything-plugin-packages-core-src-plugins-registry.ts.md) — dispatches a file to the right language extractor.
