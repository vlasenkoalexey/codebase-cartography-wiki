---
title: 'Module: tests/test_affected_cli.py'
type: catalog
provenance: extracted
module: tests/test_affected_cli.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_affected_cli`/
symbols:
  test_affected_cli_reverse_traverses_impact_edges: test_affected_cli_reverse_traverses_impact_edges().
  test_affected_cli_relation_filter_limits_reverse_traversal: test_affected_cli_relation_filter_limits_reverse_traversal().
  test_affected_cli_forces_directed_on_undirected_graph: test_affected_cli_forces_directed_on_undirected_graph().
  test_affected_cli_loads_edges_keyed_graph: test_affected_cli_loads_edges_keyed_graph().
  test_resolve_seed_bare_name_matches_callable_label: test_resolve_seed_bare_name_matches_callable_label().
  test_resolve_seed_decorated_query_matches_bare_label: test_resolve_seed_decorated_query_matches_bare_label().
  test_resolve_seed_matches_unicode_normalized_label: test_resolve_seed_matches_unicode_normalized_label().
  test_resolve_seed_preserves_distinct_accents: test_resolve_seed_preserves_distinct_accents().
  test_resolve_seed_bare_name_tie_still_returns_none: test_resolve_seed_bare_name_tie_still_returns_none().
  test_resolve_seed_source_file_path_prefers_file_level_node: test_resolve_seed_source_file_path_prefers_file_level_node().
  test_resolve_seed_source_file_trailing_slash_parity: test_resolve_seed_source_file_trailing_slash_parity().
  test_resolve_seed_source_file_ambiguous_no_file_node_returns_none: test_resolve_seed_source_file_ambiguous_no_file_node_returns_none().
  test_affected_cli_source_file_path_uses_file_level_node: test_affected_cli_source_file_path_uses_file_level_node().
  _write_graph: _write_graph().
---
# Module: [`tests/test_affected_cli.py`](../../../../../raw/code/graphify/tests/test_affected_cli.py)

## Functions
- `_write_graph(tmp_path)` — [`L11`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L11)
- `test_affected_cli_forces_directed_on_undirected_graph(monkeypatch, tmp_path, capsys)` — [`L63`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L63) — A graph persisted with directed=false must still recover caller->callee
- `test_affected_cli_loads_edges_keyed_graph(monkeypatch, tmp_path, capsys)` — [`L97`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L97) — graphify's `extract` writes graph.json with an "edges" key (not networkx's
- `test_affected_cli_relation_filter_limits_reverse_traversal(monkeypatch, tmp_path, capsys)` — [`L46`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L46)
- `test_affected_cli_reverse_traverses_impact_edges(monkeypatch, tmp_path, capsys)` — [`L25`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L25)
- `test_affected_cli_source_file_path_uses_file_level_node(monkeypatch, tmp_path, capsys)` — [`L226`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L226)
- `test_resolve_seed_bare_name_matches_callable_label()` — [`L127`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L127)
- `test_resolve_seed_bare_name_tie_still_returns_none()` — [`L169`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L169)
- `test_resolve_seed_decorated_query_matches_bare_label()` — [`L138`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L138)
- `test_resolve_seed_matches_unicode_normalized_label()` — [`L148`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L148)
- `test_resolve_seed_preserves_distinct_accents()` — [`L159`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L159)
- `test_resolve_seed_source_file_ambiguous_no_file_node_returns_none()` — [`L213`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L213) — Several nodes share a source_file but none is the L1 file node and none's
- `test_resolve_seed_source_file_path_prefers_file_level_node()` — [`L179`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L179)
- `test_resolve_seed_source_file_trailing_slash_parity()` — [`L200`](../../../../../raw/code/graphify/tests/test_affected_cli.py#L200) — A trailing path separator must not change the match (parity with explain's

