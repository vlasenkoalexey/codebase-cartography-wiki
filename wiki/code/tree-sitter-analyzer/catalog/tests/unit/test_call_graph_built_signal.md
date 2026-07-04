---
title: 'Module: tests/unit/test_call_graph_built_signal.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_built_signal.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_built_signal`/
symbols:
  _seed_call_edges_without_built_marker: _seed_call_edges_without_built_marker().
  test_fully_cached_rerun_stamps_marker_when_index_complete: test_fully_cached_rerun_stamps_marker_when_index_complete().
  _seed_call_edges_with_marker_table_dropped: _seed_call_edges_with_marker_table_dropped().
  test_single_file_reindex_refreshes_existing_call_graph_built_marker: test_single_file_reindex_refreshes_existing_call_graph_built_marker().
  test_mixed_incremental_rerun_keeps_marker_true: test_mixed_incremental_rerun_keeps_marker_true().
  test_errored_file_does_not_stamp_marker_when_incomplete: test_errored_file_does_not_stamp_marker_when_incomplete().
  test_resolve_only_does_not_mark_call_graph_built_for_partial_cache: test_resolve_only_does_not_mark_call_graph_built_for_partial_cache().
  test_truncated_rerun_does_not_stamp_marker_when_incomplete: test_truncated_rerun_does_not_stamp_marker_when_incomplete().
  test_mark_single_file_complete_no_marker_when_index_incomplete: test_mark_single_file_complete_no_marker_when_index_incomplete().
  _seed_partial_ast_cache_without_call_graph: _seed_partial_ast_cache_without_call_graph().
  test_partial_incremental_index_does_not_stamp_call_graph_built_marker: test_partial_incremental_index_does_not_stamp_call_graph_built_marker().
  test_partial_ast_cache_without_call_graph_marker_hints_full_index: test_partial_ast_cache_without_call_graph_marker_hints_full_index().
  test_existing_edges_without_call_graph_marker_no_empty_index_hint: test_existing_edges_without_call_graph_marker_no_empty_index_hint().
  test_missing_marker_table_with_edges_no_empty_index_hint: test_missing_marker_table_with_edges_no_empty_index_hint().
  test_indexed_source_files_complete_true_when_index_matches_source: test_indexed_source_files_complete_true_when_index_matches_source().
  test_indexed_source_files_complete_false_when_source_added_after_index: test_indexed_source_files_complete_false_when_source_added_after_index().
  test_mark_single_file_complete_skips_non_indexed_status: test_mark_single_file_complete_skips_non_indexed_status().
  test_mark_single_file_complete_skips_skipped_status: test_mark_single_file_complete_skips_skipped_status().
  test_call_graph_state_marker_round_trip: test_call_graph_state_marker_round_trip().
  test_call_graph_state_write_failures_do_not_raise: test_call_graph_state_write_failures_do_not_raise().
  test_call_graph_built_recovers_when_marker_zero_but_edges_exist: test_call_graph_built_recovers_when_marker_zero_but_edges_exist().
  test_cache_call_graph_built_degrades_false_on_reader_error: test_cache_call_graph_built_degrades_false_on_reader_error().
  test_indexed_source_files_complete_false_on_empty_source_set: test_indexed_source_files_complete_false_on_empty_source_set().
  test_stale_walk_agrees_with_indexer_file_selection: test_stale_walk_agrees_with_indexer_file_selection().
  _call_graph_built_at: _call_graph_built_at().
  test_call_graph_built_supports_tuple_rows: test_call_graph_built_supports_tuple_rows().
  test_call_graph_built_recovers_from_missing_marker_table: test_call_graph_built_recovers_from_missing_marker_table().
  test_call_graph_built_marker_set_takes_fast_path: test_call_graph_built_marker_set_takes_fast_path().
  test_call_graph_built_false_when_no_marker_and_empty_edges: test_call_graph_built_false_when_no_marker_and_empty_edges().
  test_cli_callers_partial_ast_cache_matches_mcp_full_index_hint: test_cli_callers_partial_ast_cache_matches_mcp_full_index_hint().
  test_completed_full_index_sweep_true_when_clean: test_completed_full_index_sweep_true_when_clean().
  test_completed_full_index_sweep_false_when_truncated: test_completed_full_index_sweep_false_when_truncated().
  test_completed_full_index_sweep_false_when_errors: test_completed_full_index_sweep_false_when_errors().
  test_completed_full_index_sweep_false_when_skipped: test_completed_full_index_sweep_false_when_skipped().
  test_completed_full_index_sweep_true_on_empty_stats_defaults: test_completed_full_index_sweep_true_on_empty_stats_defaults().
  _make_edges_table: _make_edges_table().
  test_call_graph_built_false_when_state_table_has_no_row: test_call_graph_built_false_when_state_table_has_no_row().
  PROJECT_ROOT: PROJECT_ROOT.
  test_call_graph_state_write_failures_do_not_raise.BrokenConn: test_call_graph_state_write_failures_do_not_raise().BrokenConn#
  test_cache_call_graph_built_degrades_false_on_reader_error.BrokenCache: test_cache_call_graph_built_degrades_false_on_reader_error().BrokenCache#
  test_errored_file_does_not_stamp_marker_when_incomplete._stat_raising_on_b: test_errored_file_does_not_stamp_marker_when_incomplete()._stat_raising_on_b().
  test_call_graph_state_write_failures_do_not_raise.BrokenConn.execute: test_call_graph_state_write_failures_do_not_raise().BrokenConn#execute().
  test_call_graph_state_write_failures_do_not_raise.BrokenConn.commit: test_call_graph_state_write_failures_do_not_raise().BrokenConn#commit().
  test_cache_call_graph_built_degrades_false_on_reader_error.BrokenCache.call_graph_built: test_cache_call_graph_built_degrades_false_on_reader_error().BrokenCache#call_graph_built().
---
# Module: [`tests/unit/test_call_graph_built_signal.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py)

## Classes
### `BrokenCache`
- def: [`tests/unit/test_call_graph_built_signal.py:290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L290)
- signature: `class BrokenCache:`
- members:
  - `call_graph_built(self)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L291)
- used by: (1 test-only callers)

### `BrokenConn`
- def: [`tests/unit/test_call_graph_built_signal.py:51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L51)
- signature: `class BrokenConn:`
- members:
  - `commit(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L55)
  - `execute(self, *args: object, **kwargs: object)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L52)
- used by: (1 test-only callers)

## Functions
- `_call_graph_built_at(cache: ASTCache)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L221)
- `_make_edges_table(conn: sqlite3.Connection, *, with_row: bool)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L88) — Create a minimal ``edges`` table; optionally seed one CALLS row.
- `_seed_call_edges_with_marker_table_dropped(root: Path)` — [`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L352) — Real CALLS edges but the marker table is entirely MISSING (#1005).
- `_seed_call_edges_without_built_marker(root: Path)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L193) — Create real CALLS edges with the marker row cleared (built = 0).
- `_seed_partial_ast_cache_without_call_graph(root: Path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L151) — Create an AST-cache row that predates the call-graph-built marker.
- `_stat_raising_on_b(path: object, *args: object, **kwargs: object)` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L599)
- `test_cache_call_graph_built_degrades_false_on_reader_error()` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L289)
- `test_call_graph_built_false_when_no_marker_and_empty_edges()` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L141)
- `test_call_graph_built_false_when_state_table_has_no_row()` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L64)
- `test_call_graph_built_marker_set_takes_fast_path()` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L118)
- `test_call_graph_built_recovers_from_missing_marker_table()` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L105)
- `test_call_graph_built_recovers_when_marker_zero_but_edges_exist()` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L128)
- `test_call_graph_built_supports_tuple_rows()` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L78)
- `test_call_graph_state_marker_round_trip()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L35)
- `test_call_graph_state_write_failures_do_not_raise()` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L50)
- `test_cli_callers_partial_ast_cache_matches_mcp_full_index_hint(tmp_path: Path)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L409)
- `test_completed_full_index_sweep_false_when_errors()` — [`L455`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L455)
- `test_completed_full_index_sweep_false_when_skipped()` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L460)
- `test_completed_full_index_sweep_false_when_truncated()` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L450)
- `test_completed_full_index_sweep_true_on_empty_stats_defaults()` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L465)
- `test_completed_full_index_sweep_true_when_clean()` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L445)
- `test_errored_file_does_not_stamp_marker_when_incomplete(tmp_path: Path)` — [`L587`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L587)
- `test_existing_edges_without_call_graph_marker_no_empty_index_hint(tmp_path: Path, tool_cls: type[CodeGraphCallersTool] | type[CodeGraphCalleesTool], count_key: str)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L329)
- `test_fully_cached_rerun_stamps_marker_when_index_complete(tmp_path: Path)` — [`L515`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L515)
- `test_indexed_source_files_complete_false_on_empty_source_set(tmp_path: Path)` — [`L473`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L473)
- `test_indexed_source_files_complete_false_when_source_added_after_index(tmp_path: Path)` — [`L497`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L497)
- `test_indexed_source_files_complete_true_when_index_matches_source(tmp_path: Path)` — [`L484`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L484)
- `test_mark_single_file_complete_no_marker_when_index_incomplete(tmp_path: Path)` — [`L681`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L681)
- `test_mark_single_file_complete_skips_non_indexed_status(tmp_path: Path)` — [`L652`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L652)
- `test_mark_single_file_complete_skips_skipped_status(tmp_path: Path)` — [`L667`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L667)
- `test_missing_marker_table_with_edges_no_empty_index_hint(tmp_path: Path, tool_cls: type[CodeGraphCallersTool] | type[CodeGraphCalleesTool], count_key: str)` — [`L387`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L387)
- `test_mixed_incremental_rerun_keeps_marker_true(tmp_path: Path)` — [`L542`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L542)
- `test_partial_ast_cache_without_call_graph_marker_hints_full_index(tmp_path: Path, tool_cls: type[CodeGraphCallersTool] | type[CodeGraphCalleesTool], count_key: str)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L305)
- `test_partial_incremental_index_does_not_stamp_call_graph_built_marker(tmp_path: Path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L248)
- `test_resolve_only_does_not_mark_call_graph_built_for_partial_cache(tmp_path: Path)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L231)
- `test_single_file_reindex_refreshes_existing_call_graph_built_marker(tmp_path: Path)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L265)
- `test_stale_walk_agrees_with_indexer_file_selection(tmp_path: Path)` — [`L622`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L622)
- `test_truncated_rerun_does_not_stamp_marker_when_incomplete(tmp_path: Path)` — [`L568`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L568)

## Module values
- `PROJECT_ROOT` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_built_signal.py#L32)

