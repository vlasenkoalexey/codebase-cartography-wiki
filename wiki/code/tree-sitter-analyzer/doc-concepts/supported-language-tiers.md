---
title: Supported-language tiers — 21 plugins, 4 levels of support
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Supported-language tiers — 21 plugins, 4 levels of support

## Definition
The README is explicit that "13 languages with full call-graph indexing" is not the same claim as "TSA
supports 21 language plugins" — it tiers the two deliberately: **13** languages get full symbol *and*
call-graph indexing (Python, Java, JavaScript, TypeScript, Go, Rust, C, C++, C#, Swift, Kotlin, Ruby,
PHP); **2** more (Bash, Scala) are fully symbol-indexed but call-graph wiring is still pending; **5**
(HTML, CSS, Markdown, SQL, YAML) are reachable only via the single-file CLI path, not the project-wide
indexer; **1** (JSON) is a "scaffold" — the plugin class exists but indexer wiring is pending. The doc
also names a real historical bug: "the 2026-05-24 patch unblocked Swift / Kotlin / Ruby / PHP / C# that
had been silently skipped for months."

## In tree-sitter-analyzer (grounded)
The plugin count checks out against the repo's own module layout: `tree_sitter_analyzer/languages/`
contains 21 per-language plugin modules, matching the README's total, including
[`JSONPlugin`](../catalog/tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin) (the "scaffold" tier
— it has a working
[`create_extractor`](../catalog/tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.create_extractor)
and [`analyze_file`](../catalog/tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.analyze_file)
but is not part of the indexer's call-graph extension set documented in this silo's
[`tree_sitter_analyzer-call_graph`](../concepts/tree_sitter_analyzer-call_graph.md) page, whose
`CallGraph.build` only walks `.py .js .ts .jsx .tsx .java .go .c .cpp .cc .cxx`). The registry that
discovers and loads every one of these 21 plugins on demand is documented in
[`tree_sitter_analyzer-plugins-manager`](../concepts/tree_sitter_analyzer-plugins-manager.md); the two
concrete implementations this silo documents in depth,
[`tree_sitter_analyzer-languages-csharp_plugin`](../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
and
[`tree_sitter_analyzer-languages-scala_plugin`](../concepts/tree_sitter_analyzer-languages-scala_plugin.md),
sit in the README's "full index" and "symbol-indexed, call-graph pending" tiers respectively — which
means the Scala concept page documents a plugin whose extraction the README says is real but whose
call-graph wiring is, per the README's own tiering, not yet complete.

## Why it matters / when it applies
The historical bug the README names — five languages "silently skipped for months" — is the exact
failure mode
[`tree_sitter_analyzer-call_graph`](../concepts/tree_sitter_analyzer-call_graph.md)'s source comments
reference obliquely (the call graph packet's own source excerpt for `_language_from_ext` calls out "the
history of why duplicating this dict in two files was a multi-month silent bug (Swift/Kotlin/Ruby/PHP/C#
silently dropped — fixed 2026-05-24)"), tying this doc-level claim directly to a specific code fix date
already visible in the code concept's own grounding. The broader lesson the tiering communicates: adding
a language plugin and wiring it into the call graph are two separate, independently-completable steps —
a plugin existing does not imply its edges are trustworthy for cross-language resolution, which is
exactly the distinction the [`tree_sitter_analyzer-plugins-manager`](../concepts/tree_sitter_analyzer-plugins-manager.md)
page's own inferred note draws between "how many languages get a structural extractor" and "how many
languages the call-graph resolver classifies."

## Connections
- Code concepts: [`tree_sitter_analyzer-plugins-manager`](../concepts/tree_sitter_analyzer-plugins-manager.md),
  [`tree_sitter_analyzer-plugins-base`](../concepts/tree_sitter_analyzer-plugins-base.md),
  [`tree_sitter_analyzer-languages-csharp_plugin`](../concepts/tree_sitter_analyzer-languages-csharp_plugin.md),
  [`tree_sitter_analyzer-languages-scala_plugin`](../concepts/tree_sitter_analyzer-languages-scala_plugin.md),
  [`tree_sitter_analyzer-call_graph`](../concepts/tree_sitter_analyzer-call_graph.md) (the narrower
  13-language call-graph extension set).
- Module catalogs: [`languages/json_plugin.py`](../catalog/tree_sitter_analyzer/languages/json_plugin.md)
  (the scaffold tier), [`languages/`](../catalog/tree_sitter_analyzer/languages/) directory generally.
- Related doc-concepts: [`cross-language-miswire-benchmark`](cross-language-miswire-benchmark.md) (the
  benchmark applies to the 13-language call-graph tier specifically, not all 21 plugins).

## Source
Extracted from `README.md` (kept in place) — section "Supported Languages".
