---
title: 'Module: tests/test_cluster.py'
type: catalog
provenance: extracted
module: tests/test_cluster.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_cluster`/
symbols:
  make_graph: make_graph().
  test_cohesion_score_range: test_cohesion_score_range().
  test_score_all_keys_match_communities: test_score_all_keys_match_communities().
  test_cluster_returns_dict: test_cluster_returns_dict().
  test_cluster_covers_all_nodes: test_cluster_covers_all_nodes().
  test_cluster_does_not_write_to_stdout: test_cluster_does_not_write_to_stdout().
  test_cluster_does_not_write_to_stderr: test_cluster_does_not_write_to_stderr().
  test_cohesion_score_complete_graph: test_cohesion_score_complete_graph().
  test_cohesion_score_single_node: test_cohesion_score_single_node().
  test_cohesion_score_disconnected: test_cohesion_score_disconnected().
  test_remap_communities_to_previous_reuses_old_ids: test_remap_communities_to_previous_reuses_old_ids().
  test_remap_communities_to_previous_assigns_deterministic_new_ids: test_remap_communities_to_previous_assigns_deterministic_new_ids().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_cluster.py`](../../../../../raw/code/graphify/tests/test_cluster.py)

## Functions
- `make_graph()` — [`L10`](../../../../../raw/code/graphify/tests/test_cluster.py#L10)
- `test_cluster_covers_all_nodes()` — [`L18`](../../../../../raw/code/graphify/tests/test_cluster.py#L18)
- `test_cluster_does_not_write_to_stderr(capsys)` — [`L69`](../../../../../raw/code/graphify/tests/test_cluster.py#L69) — Same as above but for stderr — ANSI codes can go to either stream.
- `test_cluster_does_not_write_to_stdout(capsys)` — [`L56`](../../../../../raw/code/graphify/tests/test_cluster.py#L56) — Clustering should not emit ANSI escape codes or other output.
- `test_cluster_returns_dict()` — [`L13`](../../../../../raw/code/graphify/tests/test_cluster.py#L13)
- `test_cohesion_score_complete_graph()` — [`L24`](../../../../../raw/code/graphify/tests/test_cluster.py#L24)
- `test_cohesion_score_disconnected()` — [`L36`](../../../../../raw/code/graphify/tests/test_cluster.py#L36)
- `test_cohesion_score_range()` — [`L42`](../../../../../raw/code/graphify/tests/test_cluster.py#L42)
- `test_cohesion_score_single_node()` — [`L30`](../../../../../raw/code/graphify/tests/test_cluster.py#L30)
- `test_remap_communities_to_previous_assigns_deterministic_new_ids()` — [`L91`](../../../../../raw/code/graphify/tests/test_cluster.py#L91)
- `test_remap_communities_to_previous_reuses_old_ids()` — [`L79`](../../../../../raw/code/graphify/tests/test_cluster.py#L79)
- `test_score_all_keys_match_communities()` — [`L49`](../../../../../raw/code/graphify/tests/test_cluster.py#L49)

## Module values
- `FIXTURES` — [`L8`](../../../../../raw/code/graphify/tests/test_cluster.py#L8)

