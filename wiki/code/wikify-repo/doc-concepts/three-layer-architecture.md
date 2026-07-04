---
title: The three-layer architecture — grounding, static evidence, comprehension
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# The three-layer architecture — grounding, static evidence, comprehension

## Definition
wikify-repo's core mental model (design decision 2): **AST/SCIP is the *grounding*
layer, never the comprehension engine.** Understanding is stacked in layers so that
each claim in the top layer rests on a deterministic layer below it:
- **L1 Grounding** — the SCIP symbol graph. Deterministic, exhaustive, no LLM.
- **L2 Static evidence** — tests-as-spec, dynamics-bearing source surfaces, in-repo
  docs/comments, and per-symbol docstrings. All available without running anything.
- **L3 Comprehension** — concept-driven mechanism pages. LLM, every claim cited into
  L1/L2.
- **L4 (optional, downstream)** — runtime enrichment from IR/HLO + traces, only when
  hardware + a workload exist. Never a precondition for ingest.

## In wikify-repo (grounded)
**L1** is the [`SymbolGraph`](../catalog/wikify/graph.md#SymbolGraph) built by
[`build_graph`](../catalog/wikify/scip_index.md#build_graph) from the SCIP index —
symbols, edges, and monikers reused as anchors, citation targets, and diff keys.

**L2** is the highest-grounding, zero-cost comprehension layer. Its realized arm is
tests-as-spec: [`collect_tests`](../catalog/wikify/evidence.md#collect_tests) maps
each test → asserted behavior → exercised symbols as
[`TestEvidence`](../catalog/wikify/evidence.md#TestEvidence). The other L2 arm that
*did* land is **docstrings** — the author's own "what this does",
[`Symbol.docstring`](../catalog/wikify/graph.md#Symbol.docstring) /
[`Symbol.doc_summary`](../catalog/wikify/graph.md#Symbol.doc_summary), `extracted`
provenance, rendered inline on catalogs and surfaced to synthesis so the model quotes
intent instead of guessing it. (Dynamics-bearing-source and in-repo-docs evidence
were planned but not realized as separate L2 emitters; the repo's own docs are
instead ingested as doc-concepts.)

**L3** is the LLM mechanism pages: per concept, traverse the L1 graph, read the real
source + L2, emit one page, every non-trivial claim ending in a citation. **L4** is
gated behind hardware and appends an `## Observed dynamics` block — clearly separated
from the static `## Dynamics (design intent)` section so a design guess is never
confused with a measured runtime fact.

## Why it matters / when it applies
The layering is *the* anti-hallucination discipline: dynamics ("how does overlap /
scheduling work") is invisible to bare structure but recoverable **statically** at
ingest, and design-intent is labeled as such so it is never confused with measured
behavior. Each layer is only trusted to the degree the layer below it grounds it.

## Connections
- Code concepts: [SymbolGraph](../concepts/wikify-graph.md) — L1; [SCIP indexing](../concepts/wikify-scip_index.md) — L1 extraction; [Coverage](../concepts/wikify-coverage.md) — L1 docstrings on catalogs.
- Module catalogs: [graph](../catalog/wikify/graph.md), [scip_index](../catalog/wikify/scip_index.md), [evidence](../catalog/wikify/evidence.md).
- Related doc-concepts: [scip-vs-ast-grounding](scip-vs-ast-grounding.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [packet-based-synthesis](packet-based-synthesis.md), [citation-linter-grounding-gate](citation-linter-grounding-gate.md).

## Source
Extracted from `docs/design.md` (load-bearing decision 2 "Three layers, not one";
the Architecture diagram; Stage 4 static-evidence sources), with the docstring/tests
realization from `docs/implementation.md` (§5.6). Kept in place.
