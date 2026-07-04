---
title: Devirtualization — crossing the dynamic-dispatch seam name-based graphs miss
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# Devirtualization — crossing the dynamic-dispatch seam name-based graphs miss

## Definition
The comprehension seam that defeats every name-based call graph: a framework invokes
a subclass polymorphically — e.g. `model_parts[0](inputs)` through
`nn.Module.__call__` — a **dynamic dispatch with no static call edge**. Walking out
from entry points cannot cross it (the model looks unreachable); a per-file
"is it connected?" check is worse, false-flagging model files as dead code (the exact
failure mode of CodeGraphContext's dead-code detector). wikify-repo's answer is
**devirtualization**: Class Hierarchy Analysis (CHA) over SCIP's explicit
`is_implementation` relationships builds the base→override edges reference-scoping
misses. The Decisions log records it as "**Devirtualization IS the connection op**"
— the concrete realization of the "connection" that coverage decision 7 deferred.

## In wikify-repo (grounded)
It is a step inside graph construction:
[`build_graph`](../catalog/wikify/scip_index.md#build_graph) calls
[`devirtualize`](../catalog/wikify/graph.md#devirtualize), which reads each symbol's
[`Symbol.relationships`](../catalog/wikify/graph.md#Symbol.relationships)
(`is_implementation`, explicit in SCIP) and adds base→override / class→subclass edges
to the [`SymbolGraph`](../catalog/wikify/graph.md#SymbolGraph). The added edges are
tracked in [`SymbolGraph.virtual_edges`](../catalog/wikify/graph.md#SymbolGraph.virtual_edges)
and queryable via [`SymbolGraph.is_virtual`](../catalog/wikify/graph.md#SymbolGraph.is_virtual),
so they render as `(virtual)` in packets and are never confused with resolved static
calls. On pytorch this recovered 8026 virtual edges (`nn.Module` → its ~400
subclasses).

**Coverage is still ≠ connection.** Devirtualization is the *bridge* over the seam;
it does not replace the enumeration floor. Coverage represents every module (via
[set-difference](concept-driven-synthesis-and-coverage.md)); devirtualization adds
the cross-hierarchy edges that let synthesis and connect reason across the dispatch
boundary.

## Why it matters / when it applies
This is a direct differentiator for the code-comprehension survey: tree-sitter /
name-based tools "guess" inheritance and overrides, so they cannot cross this seam
*correctly*; wikify-repo gets it from SCIP's compiler-resolved `is_implementation`,
CHA-expanded. It also made a planned Stage 3 dispatch/registration extractor
unnecessary — devirtualization crossed the dynamic-dispatch seam generically, so the
`native_functions.yaml` / `TORCH_LIBRARY_IMPL` map was descoped and never built.

## Connections
- Code concepts: [SymbolGraph](../concepts/wikify-graph.md) — where devirtualize lives; [SCIP indexing](../concepts/wikify-scip_index.md) — build_graph orchestration.
- Module catalogs: [graph](../catalog/wikify/graph.md), [scip_index](../catalog/wikify/scip_index.md).
- Related doc-concepts: [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [scip-vs-ast-grounding](scip-vs-ast-grounding.md), [multi-repo-connect](multi-repo-connect.md), [tool-positioning-comparison](tool-positioning-comparison.md).

## Source
Extracted from `docs/design.md` (load-bearing decision 7; Decisions log
"Devirtualization IS the connection op"; Stage 3 descope note), with the realized
mechanism from `docs/implementation.md` (§10.2 `build_graph` — devirtualization).
Kept in place.
