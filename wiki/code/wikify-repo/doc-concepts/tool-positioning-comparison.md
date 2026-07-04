---
title: Tool positioning — wikify-repo vs graphify, understand-anything, Code Wiki
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Tool positioning — wikify-repo vs graphify, understand-anything, Code Wiki

## Definition
The survey-comparability lens made explicit: the README positions wikify-repo
against three peer code-comprehension tools along seven axes. The other three
optimize for **navigation and reach** — a graph to traverse
([graphify](https://github.com/safishamsi/graphify)), a visual dashboard to explore
([understand-anything](https://github.com/labolado/understand-anything)), a
zero-setup hosted site (Google Code Wiki). **wikify-repo optimizes for trust and
ownership.** This page is the anchor for cross-repo concept pages in the wider
code-comprehension survey.

## In wikify-repo (grounded)
The distinguishing choices are all realized in code, not marketing:

| Axis | wikify-repo's realized answer | grounded in |
|---|---|---|
| Code structure | **SCIP** (compiler-grade), not name-based tree-sitter | [`build_graph`](../catalog/wikify/scip_index.md#build_graph), [`parse_symbol`](../catalog/wikify/monikers.md#parse_symbol) |
| Faithfulness | citation linter is a **hard build gate**; uncited → `[!inferred]` | [`lint_silo`](../catalog/wikify/lint.md#lint_silo) |
| Coverage | deterministic **set-difference** — every module gets a page | [`documentable_symbols`](../catalog/wikify/coverage.md#documentable_symbols), [`emit_catalogs`](../catalog/wikify/coverage.md#emit_catalogs) |
| Retrieval | `grep` + `index.md` — no embeddings, no DB | [`write_top_index`](../catalog/wikify/assemble.md#write_top_index) |
| Updates | idempotent reconcile — `--ref` rebuilds only changed *symbols* | [`compute_plan`](../catalog/wikify/diff.md#compute_plan) |
| Multi-repo | inline cross-repo concept links, selective | [`apply_connections`](../catalog/wikify/connect.md#apply_connections) |
| Ownership | plain markdown in your own git repo | (the whole `wiki/` product) |

**Borrowed ideas, no code reuse** (design.md "Prior art"): graphify contributes the
`extracted / inferred / ambiguous` confidence vocabulary (mapped onto wikify's
provenance model) and its markdown-wiki emission as a rendering reference; its
tree-sitter core is explicitly out of scope. context-sherpa contributes the symbol
pruning + reference-count importance formula (reimplemented over wikify's own SCIP
read — see [`SymbolGraph.importance`](../catalog/wikify/graph.md#SymbolGraph.importance)).
CodeGraphContext is explicitly *not* adopted — its name-based dead-code detector is
the exact failure mode devirtualization + set-difference coverage avoid.

## Why it matters / when it applies
For the survey, this is the map of *what is comparable to what*. wikify-repo trades
tree-sitter's breadth (20+ languages, zero build) for SCIP's precision (citeable
grounding behind a gate), and trades a queryable graph runtime for materialized
markdown you own. Use this page when asking "which tool for navigation vs trusted
retrieval" — the answer is on the axis, not absolute.

## Connections
- Code concepts: [SCIP indexing](../concepts/wikify-scip_index.md), [The citation linter](../concepts/wikify-lint.md), [Coverage](../concepts/wikify-coverage.md), [wikify connect](../concepts/wikify-connect.md).
- Module catalogs: [scip_index](../catalog/wikify/scip_index.md), [lint](../catalog/wikify/lint.md), [coverage](../catalog/wikify/coverage.md), [connect](../catalog/wikify/connect.md), [monikers](../catalog/wikify/monikers.md), [graph](../catalog/wikify/graph.md), [assemble](../catalog/wikify/assemble.md), [diff](../catalog/wikify/diff.md).
- Related doc-concepts: [scip-vs-ast-grounding](scip-vs-ast-grounding.md), [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [markdown-as-interface](markdown-as-interface.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [devirtualization-dispatch-seam](devirtualization-dispatch-seam.md).

## Source
Extracted from `README.md` ("How wikify-repo compares" table; "SCIP vs AST
parsing"), with prior-art attributions from `docs/design.md` ("Prior art — borrowed
concepts"). Kept in place.
