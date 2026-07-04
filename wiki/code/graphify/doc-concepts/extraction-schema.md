---
title: The extraction (node/edge) schema
type: doc-concept
provenance: doc
source: ARCHITECTURE.md
updated: 2026-07-04
status: fresh
---
# The extraction (node/edge) schema

## Definition
Every extractor — code or semantic — returns the same JSON shape: a list of `nodes` (`id`, `label`, `source_file`, `source_location`) and a list of `edges` (`source`, `target`, `relation`, `confidence`). This one contract is what lets 36 language extractors and LLM subagents all feed a single graph builder. `validate.py` enforces the schema before `build_graph()` consumes it, so a malformed extraction fails fast rather than corrupting the graph.

## In graphify (grounded)
- The schema gate is [`validate_extraction`](../catalog/graphify/validate.md#validate_extraction) (and [`assert_valid`](../catalog/graphify/validate.md#assert_valid)), backed by the field constants [`REQUIRED_NODE_FIELDS`](../catalog/graphify/validate.md#REQUIRED_NODE_FIELDS), [`REQUIRED_EDGE_FIELDS`](../catalog/graphify/validate.md#REQUIRED_EDGE_FIELDS), [`VALID_CONFIDENCES`](../catalog/graphify/validate.md#VALID_CONFIDENCES), and [`VALID_FILE_TYPES`](../catalog/graphify/validate.md#VALID_FILE_TYPES).
- Consumption is [`build`](../catalog/graphify/build.md#build) / [`build_from_json`](../catalog/graphify/build.md#build_from_json), which merge validated extraction dicts into one `nx.Graph`.
- The persisted form (`graph.json`) is NetworkX node-link JSON, where nodes carry `file_type` (`code`, `document`, `paper`, `image`, `rationale`) and edges add `confidence_score` (INFERRED only) plus `source_file`; group relationships over 3+ nodes are stored as hyperedges in `G.graph["hyperedges"]`.

## Why it matters / when it applies
The uniform schema is the seam that makes graphify extensible: a new language or a new source type only has to emit this shape to join the graph. It is also the grounding for every downstream claim — clustering, god-node analysis, and query all operate over these typed nodes and edges.

## Connections
- Code concepts: [build](../concepts/graphify-build.md), [extract](../concepts/graphify-extract.md)
- Module catalogs: [validate](../catalog/graphify/validate.md), [build](../catalog/graphify/build.md)
- Related doc-concepts: [ingest-pipeline](ingest-pipeline.md), [confidence-labels](confidence-labels.md), [output-artifacts](output-artifacts.md), [adding-a-language](adding-a-language.md)

## Source
Extracted from `ARCHITECTURE.md` (kept in place); the `graph.json` field detail is corroborated by `docs/how-it-works.md`.
