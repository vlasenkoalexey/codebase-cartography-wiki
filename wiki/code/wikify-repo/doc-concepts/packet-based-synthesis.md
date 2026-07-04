---
title: Packet-based synthesis — the relevance-bounded Python→LLM handoff
type: doc-concept
provenance: doc
source: docs/implementation.md
updated: 2026-07-04
status: fresh
---
# Packet-based synthesis — the relevance-bounded Python→LLM handoff

## Definition
The concrete interface across the Python/LLM boundary: for each concept, the
deterministic side writes **one synthesis packet** — a markdown file bundling the
grounded subgraph the LLM may cite from — and the agent reads it (plus the real
source it points to) to write one mechanism page. The packet is *the* grounding
contract: it carries the seeds, the relevant subgraph with each symbol's verbatim
`cite:` catalog anchor, truncated source snippets, L2 evidence (tests + docstrings),
and the template + citation rules. Synthesis is **heavy processing, not annotation** —
a page that merely traces the code with a citation per clause is a failure even if it
lints.

## In wikify-repo (grounded)
[`build_packet`](../catalog/wikify/packet.md#build_packet) assembles the packet;
[`write_packet`](../catalog/wikify/packet.md#write_packet) writes it to
`.cache/packets/<slug>/<concept>.md` (+ a `.subgraph.txt` of monikers that lint rule
3 gates against). Seeds come from
[`resolve_seeds`](../catalog/wikify/packet.md#resolve_seeds) (config-named) or
[`auto_seeds`](../catalog/wikify/packet.md#auto_seeds) (discovered top-centrality).

**Relevance-bounded subgraph.** [`gather_subgraph`](../catalog/wikify/packet.md#gather_subgraph)
replaces a flat BFS cap with a frontier scored by *importance ÷ (1 + distance from a
seed)*, filling a budget ([`MAX_SUBGRAPH`](../catalog/wikify/packet.md#MAX_SUBGRAPH))
by relevance — so a hub like `nn.Module` (1000+ callers) keeps its load-bearing
collaborators instead of an alphabetical slice; seeds are always kept. Importance is
[`SymbolGraph.importance`](../catalog/wikify/graph.md#SymbolGraph.importance) (the
context-sherpa reference-count formula). [`read_subgraph`](../catalog/wikify/packet.md#read_subgraph)
pulls the source snippets.

**Lens-aware emphasis.** When
[`RepoConfig.synthesis_focus`](../catalog/wikify/config.md#RepoConfig.synthesis_focus)
is set, `build_packet` emits a "Synthesis focus (lens)" block so synthesis
*foregrounds* the domain framing — the lens moves emphasis, never grounding, so every
claim still cites a real symbol. (This very doc-concept extraction was run through
such a lens: code-comprehension / survey comparability.)

## Why it matters / when it applies
The packet is what makes grounding *enforceable at the source*: the agent cites only
symbols the deterministic side already resolved and handed over, so lint rule 3
(no out-of-subgraph symbol) is a mechanical check. The relevance bound is what keeps
synthesis focused on a hub's *important* neighbors rather than truncating arbitrarily —
the difference between an insightful mechanism page and a shallow trace.

## Connections
- Code concepts: [SymbolGraph](../concepts/wikify-graph.md) — the graph packets walk + importance ranking; [wikify config](../concepts/wikify-config.md) — the synthesis lens.
- Module catalogs: [packet](../catalog/wikify/packet.md), [graph](../catalog/wikify/graph.md), [config](../catalog/wikify/config.md).
- Related doc-concepts: [python-llm-split](python-llm-split.md), [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [three-layer-architecture](three-layer-architecture.md).

## Source
Extracted from `docs/implementation.md` (§5.4 synthesis packet; §10.3
relevance-bounded subgraph; §10.9 lens), with the "heavy processing, not annotation"
bar and Stage 5 from `docs/design.md`. Kept in place.
