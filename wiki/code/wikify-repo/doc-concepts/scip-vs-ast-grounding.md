---
title: SCIP vs AST grounding — the compiler-grade structural substrate
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# SCIP vs AST grounding — the compiler-grade structural substrate

## Definition
wikify-repo's central comprehension bet: extract a repo's structure with **SCIP**
(Sourcegraph's Code Intelligence Protocol) via the language's *real* name-and-type
resolver — `scip-python` (pyright) and `scip-clang` (clang) — rather than a
tree-sitter AST. An AST parse is fast and build-free but resolves references
**syntactically by name**: it sees a call to something *called* `forward`, not
*which* `forward`. SCIP binds every definition and reference to a globally-unique
**moniker**, so a citation points at *the* symbol across files — not a string that
happens to match. That precision is what makes the wiki's grounding *enforceable*
rather than best-effort, and it is the axis on which the README's comparison table
separates wikify-repo from graphify and understand-anything (both tree-sitter,
name-based).

## In wikify-repo (grounded)
The indexers are invoked as external subprocesses and their `.scip` output parsed
into a symbol graph — no per-language AST lives downstream. [`index_repo`](../catalog/wikify/scip_index.md#index_repo)
drives [`run_indexer`](../catalog/wikify/scip_index.md#run_indexer), then
[`parse_index`](../catalog/wikify/scip_index.md#parse_index) reads the protobuf and
[`build_graph`](../catalog/wikify/scip_index.md#build_graph) assembles a
[`SymbolGraph`](../catalog/wikify/graph.md#SymbolGraph) of
[`Symbol`](../catalog/wikify/graph.md#Symbol) nodes. Each symbol carries its
compiler-resolved [`Symbol.moniker`](../catalog/wikify/graph.md#Symbol.moniker),
parsed into descriptors by [`parse_symbol`](../catalog/wikify/monikers.md#parse_symbol)
→ [`ParsedSymbol`](../catalog/wikify/monikers.md#ParsedSymbol). The moniker is
reused three ways (design decision 1): wiki anchor, citation target, and diff key.

**The callers/callees approximation (the risky foundation).** SCIP has *no "call"
role*, so [`SymbolGraph.callers`](../catalog/wikify/graph.md#SymbolGraph.callers) /
[`SymbolGraph.callees`](../catalog/wikify/graph.md#SymbolGraph.callees) are derived
from a *reference* occurrence of a callable whose range falls inside a function's
enclosing range (implementation.md §5.1). This is **reference-scoped, not true call
resolution** — but it is *symbol-accurate* (the name is bound to the right symbol by
the compiler frontend), which is the whole gain over tree-sitter. Inheritance and
override edges, by contrast, are explicit in SCIP via
[`Symbol.relationships`](../catalog/wikify/graph.md#Symbol.relationships)
(`is_implementation`).

**Languages are pluggable because grounding is SCIP.** Since the downstream reads
the symbol table, not an AST, a language is just a pluggable indexer
([`LANGS.LANGS`](../catalog/wikify/languages.md#LANGS.LANGS) →
[`Lang`](../catalog/wikify/languages.md#Lang)). Python + C++ are bundled;
[`detect_languages`](../catalog/wikify/languages.md#detect_languages) plus
[`ensure_indexer`](../catalog/wikify/languages.md#ensure_indexer) install TS/JS, Go,
and Rust indexers *on demand* (asking, never silently). See the deeper page on this.

## Why it matters / when it applies
Grounding is only *enforceable* if a citation resolves to a real symbol; a name-based
graph can only guess at cross-file bindings, aliases, overloads, and inheritance, so
its "citations" cannot be gated. SCIP's honest cost is a real indexer (npm for
`scip-python`; a `compile_commands.json` for C++) — heavier than a zero-build parse,
which is the price of precision. Tree-sitter trades precision for breadth: the right
call for navigation, the wrong one for *citeable* grounding.

## Connections
- Code concepts: [SCIP indexing](../concepts/wikify-scip_index.md) — the extraction pipeline; [SymbolGraph](../concepts/wikify-graph.md) — the citation namespace; [Monikers](../concepts/wikify-monikers.md) — symbol-string parsing; [Language detection](../concepts/wikify-languages.md) — on-demand indexers.
- Module catalogs: [scip_index](../catalog/wikify/scip_index.md), [graph](../catalog/wikify/graph.md), [monikers](../catalog/wikify/monikers.md), [languages](../catalog/wikify/languages.md).
- Related doc-concepts: [three-layer-architecture](three-layer-architecture.md), [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [indexing-at-scale](indexing-at-scale.md), [devirtualization-dispatch-seam](devirtualization-dispatch-seam.md), [tool-positioning-comparison](tool-positioning-comparison.md).

## Source
Extracted from `README.md` ("SCIP vs AST parsing", "languages are pluggable"),
with corroborating detail from `docs/design.md` (load-bearing decision 1; Stage 1
table) and `docs/implementation.md` (§5.1 callers/callees derivation; §10.8
multi-language). All kept in place.
