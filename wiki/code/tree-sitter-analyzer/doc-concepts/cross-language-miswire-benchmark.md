---
title: Cross-language mis-wire benchmark — the "moat" claim
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Cross-language mis-wire benchmark — the "moat" claim

## Definition
The README frames cross-language correctness as TSA's central differentiator against name-only code
indexes (its comparator is "CodeGraph"): *"A name-only index wires Python `sorted()` to a Swift `func
sorted`. TSA doesn't."* It backs this with a head-to-head measurement on TSA's own repo — CodeGraph:
745 cross-language mis-wires out of 38,103 call edges (1.96%); TSA: 6 out of 114,160 (0.005%) — stated
as "~390× cleaner on cross-language correctness, while resolving 3× more call edges." A second,
independently reproducible run on HuggingFace's `tokenizers` (Rust+Python+JS+TS) reports a name-only
resolver would mis-wire 1,259 edges where TSA mis-wires 0.

## In tree-sitter-analyzer (grounded)
The mechanism behind the claim is documented in this silo's own concept page,
[`tree_sitter_analyzer-call_graph`](../concepts/tree_sitter_analyzer-call_graph.md): the call graph's
unscoped, project-wide name-search tier is the only one that can mis-wire across languages, and it is
gated by
[`languages_compatible`](../catalog/tree_sitter_analyzer/_language_family.md#languages_compatible) —
symmetric for the JS/TS dialect family, directional for C/C++/Objective-C. The README's own reproduction
tool is a real, catalogued CLI entry point: `miswire-audit` corresponds to
[`audit`](../catalog/tree_sitter_analyzer/miswire_audit.md#audit) in
[`tree_sitter_analyzer/miswire_audit.py`](../catalog/tree_sitter_analyzer/miswire_audit.md), which the
module's own catalog also shows rendering output via
[`render_terminal`](../catalog/tree_sitter_analyzer/miswire_audit.md#render_terminal) and
[`render_card`](../catalog/tree_sitter_analyzer/miswire_audit.md#render_card), and reporting results
through an [`AuditResult`](../catalog/tree_sitter_analyzer/miswire_audit.md#AuditResult.naive_miswires)
dataclass (`naive_miswires`, `tsa_miswires`, `total_call_edges`, `genuine_offenders`,
[`multiplier`](../catalog/tree_sitter_analyzer/miswire_audit.md#AuditResult.multiplier) — almost
certainly the source of the "~390×" figure itself). The README also names a concrete worked example TSA
gets right that a name-only index gets wrong: `fts_search()` binding to the real
`_ast_cache_query.py`/`ast_cache.py` method rather than a same-named test mock (`FallbackCache`) — the
same test-shadow-demotion behavior the call-graph concept page documents for
[`CalleeResolver`](../catalog/tree_sitter_analyzer/callee_resolution.md#CalleeResolver)'s tier-3 fallback.

## Why it matters / when it applies
The README is explicit that this is the *first* axis it wants judged, ahead of token cost: *"Token cost
is one axis; a code-intelligence tool's first job is a correct graph."* It also draws the honest
boundary of the claim — TSA's own 6 residual cross-language edges are attributed to `java→python/php`
single-word Java method names, and the doc frames the remaining ~4% "unknown" call edges (dominated by
genuinely-unresolvable dynamic dispatch like `BaseTool.execute()`) as "the false-positive floor of
static analysis, left honest rather than guessed" — i.e. the design goal is a graph that never claims
false precision, not a graph with zero unresolved edges. The doc also documents a *layered* resolver
beyond the single family gate this silo's call-graph packet captured: a per-language **resolver
registry** (its own RFC-0010) adds conservative stdlib-method tiers (RFC-0004, e.g. `str`/`Path`/`dict`
methods → `stdlib`) and external-library tiers (RFC-0005, e.g. pytest/hypothesis/mock → `external`),
raising classified call edges from 83.9% to 96.3% — none of which is grounded in this silo's call-graph
concept packet, since those RFC-driven resolver modules weren't in that packet's cited subgraph.

## Connections
- Code concepts: [`tree_sitter_analyzer-call_graph`](../concepts/tree_sitter_analyzer-call_graph.md) —
  the family-gating mechanism this benchmark measures.
- Module catalogs: [`miswire_audit.py`](../catalog/tree_sitter_analyzer/miswire_audit.md) (the
  reproduction tool), [`_language_family.py`](../catalog/tree_sitter_analyzer/_language_family.md) (the
  gate itself), [`callee_resolution.py`](../catalog/tree_sitter_analyzer/callee_resolution.md) (the
  resolver tiers the gate sits inside).
- Related doc-concepts: [`supported-language-tiers`](supported-language-tiers.md) (the 13-language
  scope this benchmark applies to).

## Source
Extracted from `README.md` (kept in place) — sections "Why it's different", "How TSA compares to
CodeGraph", and "Call-graph correctness — TSA resolves what CodeGraph mis-wires".
