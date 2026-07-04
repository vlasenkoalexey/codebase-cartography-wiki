---
title: 'Module: tests/test_build_merge_hyperedges_and_prune.py'
type: catalog
provenance: extracted
module: tests/test_build_merge_hyperedges_and_prune.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_build_merge_hyperedges_and_prune`/
symbols:
  test_update_preserves_hyperedges_of_unchanged_files: test_update_preserves_hyperedges_of_unchanged_files().
  test_update_without_root_still_preserves_hyperedges: test_update_without_root_still_preserves_hyperedges().
  test_deleted_file_hyperedges_are_pruned: test_deleted_file_hyperedges_are_pruned().
  test_prune_without_root_uses_graphify_root_marker: test_prune_without_root_uses_graphify_root_marker().
  _seed_two_file_graph: _seed_two_file_graph().
  test_prune_without_root_removes_ghost_nodes_via_grandparent_fallback: test_prune_without_root_removes_ghost_nodes_via_grandparent_fallback().
  test_prune_matches_across_symlinked_root: test_prune_matches_across_symlinked_root().
  _write_graph: _write_graph().
  _he_ids: _he_ids().
---
# Module: [`tests/test_build_merge_hyperedges_and_prune.py`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py)

## Functions
- `_he_ids(G)` — [`L32`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L32)
- `_seed_two_file_graph(tmp_path)` — [`L38`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L38)
- `_write_graph(graph_path: Path, nodes, edges, hyperedges)` — [`L24`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L24) — Write a graph.json in the shape to_json emits (top-level hyperedges).
- `test_deleted_file_hyperedges_are_pruned(tmp_path)` — [`L85`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L85)
- `test_prune_matches_across_symlinked_root(tmp_path)` — [`L133`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L133) — A symlinked scan root (macOS /var -> /private/var, symlinked home/worktree)
- `test_prune_without_root_removes_ghost_nodes_via_grandparent_fallback(tmp_path)` — [`L99`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L99)
- `test_prune_without_root_uses_graphify_root_marker(tmp_path)` — [`L116`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L116)
- `test_update_preserves_hyperedges_of_unchanged_files(tmp_path)` — [`L55`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L55)
- `test_update_without_root_still_preserves_hyperedges(tmp_path)` — [`L71`](../../../../../raw/code/graphify/tests/test_build_merge_hyperedges_and_prune.py#L71) — The runbook omits root; the fallback root must not break preservation.

