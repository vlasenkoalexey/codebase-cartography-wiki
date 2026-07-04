---
title: 'Module: graphify/cluster.py'
type: catalog
provenance: extracted
module: graphify/cluster.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.cluster`/
symbols:
  cluster: cluster().
  score_all: score_all().
  label_communities_by_hub: label_communities_by_hub().
  community_member_sigs: community_member_sigs().
  cohesion_score: cohesion_score().
  remap_communities_to_previous: remap_communities_to_previous().
  _partition: _partition().
  _split_community: _split_community().
  _suppress_output: _suppress_output().
  _MAX_COMMUNITY_FRACTION: _MAX_COMMUNITY_FRACTION.
  _MIN_SPLIT_SIZE: _MIN_SPLIT_SIZE.
  _COHESION_SPLIT_THRESHOLD: _COHESION_SPLIT_THRESHOLD.
  _COHESION_SPLIT_MIN_SIZE: _COHESION_SPLIT_MIN_SIZE.
---
# Module: [`graphify/cluster.py`](../../../../../raw/code/graphify/graphify/cluster.py)

## Functions
- `_partition(G: nx.Graph, resolution: float = 1)` — [`L22`](../../../../../raw/code/graphify/graphify/cluster.py#L22) — Run community detection. Returns {node_id: community_id}. — documented in [graphify-cluster](../../concepts/graphify-cluster.md)
- `_split_community(G: nx.Graph, nodes: list[str])` — [`L239`](../../../../../raw/code/graphify/graphify/cluster.py#L239) — Run a second Leiden pass on a community subgraph to split it further. — documented in [graphify-cluster](../../concepts/graphify-cluster.md)
- `_suppress_output()` — [`L11`](../../../../../raw/code/graphify/graphify/cluster.py#L11) — Context manager to suppress stdout/stderr during library calls.
- `cluster(G: nx.Graph, resolution: float = 1, exclude_hubs_percentile: float | None = None)` — [`L134`](../../../../../raw/code/graphify/graphify/cluster.py#L134) — Run Leiden community detection. Returns {community_id: [node_ids]}. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `cohesion_score(G: nx.Graph, community_nodes: list[str])` — [`L257`](../../../../../raw/code/graphify/graphify/cluster.py#L257) — Ratio of actual intra-community edges to maximum possible. — documented in [graphify-cluster](../../concepts/graphify-cluster.md)
- `community_member_sigs(communities: dict[int, list[str]])` — [`L113`](../../../../../raw/code/graphify/graphify/cluster.py#L113) — Per-community membership fingerprints: ``{cid: sha256(sorted member ids)}``. — documented in [graphify-cluster](../../concepts/graphify-cluster.md)
- `label_communities_by_hub(G: nx.Graph, communities: dict[int, list[str]])` — [`L86`](../../../../../raw/code/graphify/graphify/cluster.py#L86) — Deterministic, LLM-free community labels: name each community after its — documented in [graphify-cluster](../../concepts/graphify-cluster.md)
- `remap_communities_to_previous(communities: dict[int, list[str]], previous_node_community: dict[str, int])` — [`L272`](../../../../../raw/code/graphify/graphify/cluster.py#L272) — Remap community IDs to maximize overlap with a previous assignment.
- `score_all(G: nx.Graph, communities: dict[int, list[str]])` — [`L268`](../../../../../raw/code/graphify/graphify/cluster.py#L268) — documented in [graphify-cluster](../../concepts/graphify-cluster.md)

## Module values
- `_COHESION_SPLIT_MIN_SIZE` — [`L83`](../../../../../raw/code/graphify/graphify/cluster.py#L83)
- `_COHESION_SPLIT_THRESHOLD` — [`L82`](../../../../../raw/code/graphify/graphify/cluster.py#L82)
- `_MAX_COMMUNITY_FRACTION` — [`L80`](../../../../../raw/code/graphify/graphify/cluster.py#L80)
- `_MIN_SPLIT_SIZE` — [`L81`](../../../../../raw/code/graphify/graphify/cluster.py#L81)

