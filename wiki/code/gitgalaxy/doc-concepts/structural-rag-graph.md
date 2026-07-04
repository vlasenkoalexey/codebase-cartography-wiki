---
title: The Structural RAG Graph — how much of gitgalaxy's "3D knowledge graph" is a real graph
type: doc-concept
provenance: doc
source: docs/wiki/01-06-the-structural-rag-graph.md
updated: 2026-07-04
status: fresh
---
# The Structural RAG Graph — how much of gitgalaxy's "3D knowledge graph" is a real graph

## Definition
The doc's pitch: standard RAG chunking "rips functions in half" by slicing on arbitrary token
counts, so gitgalaxy instead chunks "biologically" at exact structural boundaries and rolls the
result up through **five scales of architectural resolution** — Satellites (functions/methods) →
Entities (classes) → Stars (files) → Constellations (folders) → the Galaxy (the repo) — into what
it calls a "highly relational Knowledge Graph" and a "queryable Code Knowledge Graph," explicitly
positioned against "heavy graph databases (like Neo4j)." The companion project-overview doc (docs/wiki/01-01-project-overview.md
§1.1/§1.4) frames the same claim as a "deterministic function-level knowledge graph" and gives it a
visual vocabulary — files are stars, imports are spatial proximity, inbound-import count is a
star's pulse rate, functions are orbiting satellites.

## In gitgalaxy (grounded)
This packet's earlier concept pages left the answer to "is there really a graph here" partly open
(the Detector page's Open questions flags that `calls_out_to` *might* feed a downstream graph but
the module that would do so, `network_risk_sensor.py`, wasn't in that packet). Reading it directly
resolves the question, with a real, nuanced split:

**Yes, a real file-level graph exists.** [`NetworkRiskSensor.build_dependency_graph`](../catalog/gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph)
(guarded by [`HAS_NETWORKX`](../catalog/gitgalaxy/core/network_risk_sensor.md#HAS_NETWORKX)) builds
an actual `networkx.DiGraph`: one node per file (carrying `risk_vector`/`max_big_o`/`is_recursive`
as node attributes), one weighted edge per resolved import. The *same* method computes real graph
math over it — not just PageRank/betweenness/closeness centrality, but also modularity (via
`community.louvain_communities`/`greedy_modularity_communities`), degree assortativity, cyclic
density (from `strongly_connected_components`), and articulation points — exactly the "3.5
MACRO-NETWORK TOPOLOGY" table `docs/gitgalaxy_architecture_brief.md` prints. This is genuine graph
theory over a genuine graph object, not a metaphor.

**Yes, a real queryable relational export exists.** [`LLMRecorder.generate_artifacts`](../catalog/gitgalaxy/recorders/llm_recorder.md#LLMRecorder.generate_artifacts)
writes its output database to a file literally named `{target}_galaxy_graph.sqlite`, produced by
[`LLMRecorder._generate_sqlite_graph`](../catalog/gitgalaxy/recorders/llm_recorder.md#LLMRecorder._generate_sqlite_graph) —
a method whose own inline comment calls it "Build the Relational Knowledge Graph (SQLite)." It
creates real, foreign-keyed tables (`artifacts`, `functions`, `dna_hits`, `outbound_dependencies`,
`inbound_dependencies`, `directory_groups`), independently re-deriving the same import-resolution
edges `generate_artifacts` computes inline (not by reusing the `NetworkRiskSensor` DiGraph object).
[`RecordKeeper.record_mission`](../catalog/gitgalaxy/recorders/record_keeper.md#RecordKeeper.record_mission)
does the equivalent for the primary mission database. This is a real, normalized, SQL-queryable
structure — the doc's own example query (`SELECT s.file_name, s.pagerank ... FROM stars s INNER
JOIN dna_hits d ...`) is illustrative rather than copy-pasted from the schema (the real table is
`artifacts`, not `stars`), but the *shape* of the claim — a local relational graph an agent can
`SELECT`/`JOIN` against — is real.

**No, there is no function-level call graph.** [`FunctionNode`](../catalog/gitgalaxy/core/detector.md#FunctionNode)'s
`calls_out_to` field (a list of bare callee names, produced per-function by the Detector) is the one
piece of data that *could* wire functions to each other. Tracing every place it is written after
extraction shows it is only ever `json.dumps()`'d into a flat `functions.calls_out_to TEXT` column
in both `llm_recorder.py` and `record_keeper.py` — never resolved to a target function ID, never
joined against another row, never turned into an edge. The graph that exists is file-to-file
(import-level); the doc's claim that the engine builds "full function call graphs" is not backed by
a resolved call-edge structure anywhere in this codebase.

**No, the 3D layout does not encode the graph's topology.** [`SpatialMapper.map_repository`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper.map_repository)
computes every file's `(pos_x, pos_y, pos_z)` from three inputs only: its directory ("sector"),
its own structural magnitude (via `_get_magnitude`), and a deterministic hash of its own filename
([`SpatialMapper._hash_jitter`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper._hash_jitter),
explicitly chosen so re-running on the same repo reproduces identical geometry). It never reads an
edge, a weight, a PageRank score, or a centrality value from `NetworkRiskSensor`'s DiGraph when
choosing a position — two files that heavily import each other are not pulled visually closer. The
1.4 "Files = Stars ... Inbound Imports = a star's pulse rate" metaphor from `01-01-project-overview.md`
is describing a *color/pulse overlay* on top of an angular, directory-clustered packing algorithm,
not a force-directed graph layout — position is a treemap-with-golden-angle-jitter wearing a galaxy
metaphor, independent of the dependency graph itself. See [the-cartographer-spatial-positioning](the-cartographer-spatial-positioning.md)
for the full mechanism (Hull Calculation, the ray-casting collision avoidance, the Golden Angle and
MD5 jitter) — this page only needed the one finding it establishes: node position is graph-independent.

## Why it matters / when it applies
This is the single most direct place to answer this survey's `symbol-graph` axis question for
gitgalaxy: it earns a **partial yes**. There is a real, computed, centrality-scored import graph and
a real, foreign-keyed, SQL-queryable export of it — genuinely comparable in spirit (not in
grounding fidelity) to the graph structures wikify-repo/graphify build from SCIP/embeddings. But the
graph's *granularity* stops at the file boundary: there is no cross-file symbol resolution, no
resolved call graph, and the 3D visualization a human actually looks at is decorative rather than
topological. This matches, rather than contradicts, [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md)'s
own finding that gitgalaxy has "no cross-file symbol resolution" — that page inferred it from the
Detector's file-scoped subgraph; this page confirms it directly from the one module that *could*
have added cross-file resolution and didn't.

## Connections
- Code concepts: [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — Phase 4 (network
  topology) must run before Phase 9 (ML inference) precisely because centrality feeds the threat
  model, and Phase 7 (spatial layout) runs after both, consuming their output only as node
  attributes, not edges; [The Detector](../concepts/gitgalaxy-core-detector.md) — where
  `calls_out_to` is produced and whose Open Questions section this page resolves; [Signal
  Processor](../concepts/gitgalaxy-metrics-signal_processor.md) — the `risk_vector` every graph node
  and every `dna_hits` row carries.
- Module catalogs: [galaxyscope](../catalog/gitgalaxy/galaxyscope.md), [detector](../catalog/gitgalaxy/core/detector.md),
  [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md); no catalog page yet exists
  for `network_risk_sensor.py`, `spatial_mapper.py`, or `recorders/llm_recorder.py` — the symbols
  cited above are read directly from source since this doc names subsystems the code-concept packets
  didn't cover.
- Related doc-concepts: [risk-exposure-physics](risk-exposure-physics.md) — what actually rides on
  top of this graph's per-file `risk_vector`; [blast-paradigm](blast-paradigm.md) — why there is no
  AST/LLM anywhere in this pipeline in the first place; [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md) —
  the "no cross-file symbol resolution" finding this page grounds directly;
  [the-cartographer-spatial-positioning](the-cartographer-spatial-positioning.md) — the detailed,
  independently-grounded mechanism behind this page's "spatial layout ≠ graph topology" finding.

## Source
Extracted from `docs/wiki/01-06-the-structural-rag-graph.md` (primary); also draws on
`docs/wiki/01-01-project-overview.md` §1.1 ("The Deterministic Knowledge Graph") and §1.4 (the
visual-metaphor mapping), and `docs/gitgalaxy_architecture_brief.md` §3.5 ("Macro-Network Topology")
as the live numeric example of the same mechanism. All three kept in place.
