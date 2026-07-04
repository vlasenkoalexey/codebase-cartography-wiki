---
title: Community detection (Leiden)
type: doc-concept
provenance: doc
source: docs/how-it-works.md
updated: 2026-07-04
status: fresh
---
# Community detection (Leiden)

## Definition
graphify groups nodes into communities with the Leiden algorithm, a graph-clustering method that clusters by edge density — nodes with many connections between them land in the same community. Crucially, **no embeddings are needed**: the `semantically_similar_to` edges the LLM already extracted are in the graph, so semantic similarity influences community shape directly. The graph structure *is* the similarity signal; there is no separate embedding step or vector database.

## In graphify (grounded)
- Clustering is [`cluster`](../catalog/graphify/cluster.md#cluster), which runs Leiden via [`_partition`](../catalog/graphify/cluster.md#_partition) and can further split loose communities with a second pass [`_split_community`](../catalog/graphify/cluster.md#_split_community) guided by [`cohesion_score`](../catalog/graphify/cluster.md#cohesion_score).
- Communities get LLM-free names deterministically from their hub node via [`label_communities_by_hub`](../catalog/graphify/cluster.md#label_communities_by_hub); membership is fingerprinted by [`community_member_sigs`](../catalog/graphify/cluster.md#community_member_sigs) so re-clusters stay stable.
- CLI knobs map to real parameters: `--resolution` sets the `resolution` of [`cluster`](../catalog/graphify/cluster.md#cluster) (more, smaller communities), and `--exclude-hubs` feeds its `exclude_hubs_percentile`.

## Why it matters / when it applies
Community detection is how graphify goes from a flat node/edge soup to an architectural map — the communities become the sections of the call-flow view and the frame for god-node ranking. Doing it purely from graph topology (no vector DB) keeps the whole tool deterministic and offline-capable.

## Connections
- Code concepts: [cluster](../concepts/graphify-cluster.md), [analyze](../concepts/graphify-analyze.md)
- Module catalogs: [cluster](../catalog/graphify/cluster.md), [callflow_html](../catalog/graphify/callflow_html.md)
- Related doc-concepts: [ingest-pipeline](ingest-pipeline.md), [god-nodes-report](god-nodes-report.md)

## Source
Extracted from `docs/how-it-works.md` (kept in place).
