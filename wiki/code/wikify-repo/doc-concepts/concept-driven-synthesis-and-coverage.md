---
title: Concept-driven synthesis + the coverage floor + graded comprehension
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# Concept-driven synthesis + the coverage floor + graded comprehension

## Definition
Three interlocking design decisions (3, 7, 8) that together answer "what gets
understood, how deeply, and how do we guarantee nothing is dropped":
- **Concept-driven (top-down), not file-driven (decision 3).** Bottom-up "summarize
  the repo" is the root cause of shallow answers; synthesis is driven from an
  explicit list of architectural concepts. This is deliberately *selective*.
- **Coverage floor (decision 7).** Selectivity means a forgotten concept = a missing
  subsystem. The floor is a deterministic **set-difference over the SCIP symbol
  table** — `coverage = documentable_symbols − concept-cited` — emitting one catalog
  page per module. "The idea is simple: spend the LLM annotating only the most
  central ~20% of nodes — enough to explain ~80% — while the rest still get a
  deterministic catalog page so nothing is dropped."
- **Graded comprehension (decision 8).** The agenda is *derived from the code's own
  topology*, not authored, and LLM effort is *monotonic in centrality*.

## In wikify-repo (grounded)
**Coverage is representation, not connection.** It never asks "what is reachable?"
(traversal dies at dynamic-dispatch seams like `model_parts[0](inputs)`); it asks
"what is *represented*?" [`documentable_symbols`](../catalog/wikify/coverage.md#documentable_symbols)
enumerates every in-repo class/function/method/module-value SCIP found;
[`covered_monikers`](../catalog/wikify/coverage.md#covered_monikers) reads back what
concept pages cited; [`compute_report`](../catalog/wikify/coverage.md#compute_report)
→ [`CoverageReport`](../catalog/wikify/coverage.md#CoverageReport) classifies each
symbol as deep / catalog-only / unrepresented, and
[`emit_catalogs`](../catalog/wikify/coverage.md#emit_catalogs) writes one
[`render_catalog`](../catalog/wikify/coverage.md#render_catalog) page per module so
the catalogued set == the documentable set. Deterministic, no LLM, cannot miss a
file.

**The agenda is derived, the effort is graded.**
[`discover_concepts`](../catalog/wikify/discover.md#discover_concepts) clusters the
symbol graph ([`detect_communities`](../catalog/wikify/discover.md#detect_communities)
→ [`Community`](../catalog/wikify/discover.md#Community)), ranks by
[`module_importance`](../catalog/wikify/discover.md#module_importance) /
[`SymbolGraph.importance`](../catalog/wikify/graph.md#SymbolGraph.importance), and
assigns tiers, auto-seeding each unit ([`DiscoveredConcept`](../catalog/wikify/discover.md#DiscoveredConcept)).
Effort then follows a four-band gradient: deep **mechanism page** (high centrality) →
**docstring annotation** ([`Symbol.doc_summary`](../catalog/wikify/graph.md#Symbol.doc_summary),
`extracted`, free — preferred over synthesis) → **purpose blurb** (mid-centrality,
undocumented) → **structural catalog** (the trivial tail). No important unit is
un-annotated; no trivial unit burns a deep page.

## Why it matters / when it applies
The first torchtitan ingest proved the failure this fixes: three Trainer concepts,
and **every model** (`Transformer`, `Attention`, …) — the essence of the repo — was
absent. Two "obvious" fixes fail: reachability traversal can't cross the dynamic
dispatch seam, and a per-file "is it connected?" check false-flags model files as
dead code (the name-based-graph blind spot). Enumeration sidesteps dispatch entirely.
The bridge that *does* connect across the seam is a separate op — see
[devirtualization](devirtualization-dispatch-seam.md).

## Connections
- Code concepts: [Coverage](../concepts/wikify-coverage.md) — the set-difference + catalogs; [Discover](../concepts/wikify-discover.md) — the derived, ranked agenda; [SymbolGraph](../concepts/wikify-graph.md) — centrality + docstrings.
- Module catalogs: [coverage](../catalog/wikify/coverage.md), [discover](../catalog/wikify/discover.md), [graph](../catalog/wikify/graph.md).
- Related doc-concepts: [devirtualization-dispatch-seam](devirtualization-dispatch-seam.md), [packet-based-synthesis](packet-based-synthesis.md), [markdown-as-interface](markdown-as-interface.md), [three-layer-architecture](three-layer-architecture.md).

## Source
Extracted from `docs/design.md` (load-bearing decisions 3, 7, 8; "Coverage is
representation, not connection"), with the README's 20/80 framing and the coverage
contracts from `docs/implementation.md` (§5.6, Stage 6b). Kept in place.
