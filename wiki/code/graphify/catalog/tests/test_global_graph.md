---
title: 'Module: tests/test_global_graph.py'
type: catalog
provenance: extracted
module: tests/test_global_graph.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_global_graph`/
symbols:
  _make_graph: _make_graph().
  test_global_remove: test_global_remove().
  _graph_to_json: _graph_to_json().
  test_global_add_two_repos_no_collision: test_global_add_two_repos_no_collision().
  test_global_add_rewires_edges_to_deduplicated_externals: test_global_add_rewires_edges_to_deduplicated_externals().
  test_global_add_creates_global_graph: test_global_add_creates_global_graph().
  test_global_add_skip_on_unchanged_hash: test_global_add_skip_on_unchanged_hash().
  test_global_add_collision_warning: test_global_add_collision_warning().
  test_merge_graphs_prefixes_ids: test_merge_graphs_prefixes_ids().
  test_global_add_rejects_oversized_source_graph: test_global_add_rejects_oversized_source_graph().
  test_prefix_graph_preserves_label: test_prefix_graph_preserves_label().
  test_prefix_graph_sets_repo_and_local_id: test_prefix_graph_sets_repo_and_local_id().
  test_prefix_graph_rewrites_edges: test_prefix_graph_rewrites_edges().
  test_prune_repo_removes_correct_nodes: test_prune_repo_removes_correct_nodes().
  test_prune_repo_returns_zero_if_not_present: test_prune_repo_returns_zero_if_not_present().
  test_global_remove_unknown_tag_raises: test_global_remove_unknown_tag_raises().
  test_dedup_raises_on_cross_repo_nodes: test_dedup_raises_on_cross_repo_nodes().
  test_dedup_ok_with_single_repo: test_dedup_ok_with_single_repo().
  test_dedup_ok_with_no_repo_attr: test_dedup_ok_with_no_repo_attr().
---
# Module: [`tests/test_global_graph.py`](../../../../../raw/code/graphify/tests/test_global_graph.py)

## Functions
- `_graph_to_json(G, path)` — [`L29`](../../../../../raw/code/graphify/tests/test_global_graph.py#L29)
- `_make_graph(nodes, edges=None)` — [`L14`](../../../../../raw/code/graphify/tests/test_global_graph.py#L14) — Build a simple nx.Graph from node dicts.
- `test_dedup_ok_with_no_repo_attr()` — [`L228`](../../../../../raw/code/graphify/tests/test_global_graph.py#L228)
- `test_dedup_ok_with_single_repo()` — [`L218`](../../../../../raw/code/graphify/tests/test_global_graph.py#L218)
- `test_dedup_raises_on_cross_repo_nodes()` — [`L208`](../../../../../raw/code/graphify/tests/test_global_graph.py#L208)
- `test_global_add_collision_warning(tmp_path, capsys)` — [`L187`](../../../../../raw/code/graphify/tests/test_global_graph.py#L187)
- `test_global_add_creates_global_graph(tmp_path)` — [`L93`](../../../../../raw/code/graphify/tests/test_global_graph.py#L93)
- `test_global_add_rejects_oversized_source_graph(monkeypatch, tmp_path)` — [`L323`](../../../../../raw/code/graphify/tests/test_global_graph.py#L323) — #F4: global_add must refuse to read a source graph.json that
- `test_global_add_rewires_edges_to_deduplicated_externals(tmp_path)` — [`L282`](../../../../../raw/code/graphify/tests/test_global_graph.py#L282) — Edges incident to an external node that gets deduplicated against an
- `test_global_add_skip_on_unchanged_hash(tmp_path)` — [`L113`](../../../../../raw/code/graphify/tests/test_global_graph.py#L113)
- `test_global_add_two_repos_no_collision(tmp_path)` — [`L129`](../../../../../raw/code/graphify/tests/test_global_graph.py#L129)
- `test_global_remove(tmp_path)` — [`L153`](../../../../../raw/code/graphify/tests/test_global_graph.py#L153)
- `test_global_remove_unknown_tag_raises(tmp_path)` — [`L177`](../../../../../raw/code/graphify/tests/test_global_graph.py#L177)
- `test_merge_graphs_prefixes_ids(tmp_path)` — [`L240`](../../../../../raw/code/graphify/tests/test_global_graph.py#L240) — merge-graphs should prefix node IDs with repo name to avoid silent collision.
- `test_prefix_graph_preserves_label()` — [`L40`](../../../../../raw/code/graphify/tests/test_global_graph.py#L40)
- `test_prefix_graph_rewrites_edges()` — [`L58`](../../../../../raw/code/graphify/tests/test_global_graph.py#L58)
- `test_prefix_graph_sets_repo_and_local_id()` — [`L49`](../../../../../raw/code/graphify/tests/test_global_graph.py#L49)
- `test_prune_repo_removes_correct_nodes()` — [`L69`](../../../../../raw/code/graphify/tests/test_global_graph.py#L69)
- `test_prune_repo_returns_zero_if_not_present()` — [`L82`](../../../../../raw/code/graphify/tests/test_global_graph.py#L82)

