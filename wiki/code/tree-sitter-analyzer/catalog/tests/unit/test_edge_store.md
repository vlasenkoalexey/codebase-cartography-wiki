---
title: 'Module: tests/unit/test_edge_store.py'
type: catalog
provenance: extracted
module: tests/unit/test_edge_store.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_edge_store`/
symbols:
  test_edge_store_query_directions_filters_and_fallbacks: test_edge_store_query_directions_filters_and_fallbacks().
  test_edge_store_call_queries_and_node_parser: test_edge_store_call_queries_and_node_parser().
  test_edge_store_crud_and_neighbors: test_edge_store_crud_and_neighbors().
  test_ast_cache_writes_calls_imports_contains_and_extends_edges: test_ast_cache_writes_calls_imports_contains_and_extends_edges().
  test_edge_store_serializes_edges_and_subgraphs: test_edge_store_serializes_edges_and_subgraphs().
  test_edge_store_inheritance_tree_and_node_helpers: test_edge_store_inheritance_tree_and_node_helpers().
  test_edge_store_call_queries_deduplicate_and_fallback_to_call_site_file: test_edge_store_call_queries_deduplicate_and_fallback_to_call_site_file().
  test_edge_store_neighbors_deduplicates_null_line_edges: test_edge_store_neighbors_deduplicates_null_line_edges().
  test_edge_store_reuses_external_transaction: test_edge_store_reuses_external_transaction().
  test_replace_edges_for_file_deletes_use_indexes_not_full_scan: test_replace_edges_for_file_deletes_use_indexes_not_full_scan().
  test_ast_cache_call_queries_read_from_edge_store_when_legacy_edges_missing: test_ast_cache_call_queries_read_from_edge_store_when_legacy_edges_missing().
  test_replace_edges_for_file_deletes_all_predicate_kinds: test_replace_edges_for_file_deletes_all_predicate_kinds().
  test_replace_edges_for_file_preserve_calls_keeps_calls_rows: test_replace_edges_for_file_preserve_calls_keeps_calls_rows().
  test_ast_cache_call_queries_fall_back_when_edge_store_raises: test_ast_cache_call_queries_fall_back_when_edge_store_raises().
  test_ast_cache_get_call_edges_handles_missing_table: test_ast_cache_get_call_edges_handles_missing_table().
  test_ast_cache_refresh_edges_from_all_cached_rows_counts_json_errors: test_ast_cache_refresh_edges_from_all_cached_rows_counts_json_errors().
  test_ast_cache_call_queries_fall_back_when_edge_store_empty: test_ast_cache_call_queries_fall_back_when_edge_store_empty().
  test_ast_cache_post_index_backfill_swallows_edge_refresh_failure: test_ast_cache_post_index_backfill_swallows_edge_refresh_failure().
  test_project_index_refreshes_edge_store_with_resolved_call_metadata: test_project_index_refreshes_edge_store_with_resolved_call_metadata().
  _insert_raw_edge: _insert_raw_edge().
  test_ast_cache_creates_edges_schema: test_ast_cache_creates_edges_schema().
  test_edge_store_migration_ignores_operational_error: test_edge_store_migration_ignores_operational_error().
  test_ast_cache_resolve_only_refreshes_edge_store: test_ast_cache_resolve_only_refreshes_edge_store().
  test_write_graph_edges_handles_empty_imports_and_missing_parent: test_write_graph_edges_handles_empty_imports_and_missing_parent().
  _SQLCapturingConnection.execute: _SQLCapturingConnection#execute().
  test_write_graph_edges_logs_operational_error: test_write_graph_edges_logs_operational_error().
  test_edge_kind_covers_unified_relationship_surface: test_edge_kind_covers_unified_relationship_surface().
  _SQLCapturingConnection.__getattr__: _SQLCapturingConnection#__getattr__().
  test_write_graph_edges_logs_operational_error.BrokenEdgeStore.replace_edges_for_file: test_write_graph_edges_logs_operational_error().BrokenEdgeStore#replace_edges_for_file().
  _SQLCapturingConnection._conn: _SQLCapturingConnection#_conn.
  _SQLCapturingConnection.calls: _SQLCapturingConnection#calls.
  _SQLCapturingConnection: _SQLCapturingConnection#
  test_edge_store_migration_ignores_operational_error.FailingConn: test_edge_store_migration_ignores_operational_error().FailingConn#
  test_edge_store_migration_ignores_operational_error.record_fn: test_edge_store_migration_ignores_operational_error().record_fn().
  test_ast_cache_call_queries_fall_back_when_edge_store_raises.BrokenStore: test_ast_cache_call_queries_fall_back_when_edge_store_raises().BrokenStore#
  test_ast_cache_call_queries_fall_back_when_edge_store_empty.EmptyStore: test_ast_cache_call_queries_fall_back_when_edge_store_empty().EmptyStore#
  test_ast_cache_post_index_backfill_swallows_edge_refresh_failure.fail_refresh: test_ast_cache_post_index_backfill_swallows_edge_refresh_failure().fail_refresh().
  test_write_graph_edges_logs_operational_error.BrokenEdgeStore: test_write_graph_edges_logs_operational_error().BrokenEdgeStore#
  _SQLCapturingConnection.__init__: _SQLCapturingConnection#__init__().
  test_edge_store_migration_ignores_operational_error.FailingConn.executescript: test_edge_store_migration_ignores_operational_error().FailingConn#executescript().
  test_ast_cache_call_queries_fall_back_when_edge_store_raises.BrokenStore.__init__: test_ast_cache_call_queries_fall_back_when_edge_store_raises().BrokenStore#__init__().
  test_ast_cache_call_queries_fall_back_when_edge_store_raises.BrokenStore.has_edges: test_ast_cache_call_queries_fall_back_when_edge_store_raises().BrokenStore#has_edges().
  test_ast_cache_call_queries_fall_back_when_edge_store_empty.EmptyStore.__init__: test_ast_cache_call_queries_fall_back_when_edge_store_empty().EmptyStore#__init__().
  test_ast_cache_call_queries_fall_back_when_edge_store_empty.EmptyStore.has_edges: test_ast_cache_call_queries_fall_back_when_edge_store_empty().EmptyStore#has_edges().
  test_write_graph_edges_logs_operational_error.BrokenEdgeStore.__init__: test_write_graph_edges_logs_operational_error().BrokenEdgeStore#__init__().
---
# Module: [`tests/unit/test_edge_store.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py)

## Classes
### `BrokenEdgeStore`
- def: [`tests/unit/test_edge_store.py:799`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L799)
- signature: `class BrokenEdgeStore:`
- members:
  - `replace_edges_for_file(self, _file_path: str, _edges: list[Edge], **_kwargs: Any)` — [`L803`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L803)
- protocol/private: `__init__`[`L800`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L800)
- uses (calls/refs, reference-scoped): [`Edge`](../../tree_sitter_analyzer/graph/edge_store.md#Edge)
- used by: (1 test-only callers)

### `BrokenStore`
- def: [`tests/unit/test_edge_store.py:588`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L588)
- signature: `class BrokenStore:`
- members:
  - `has_edges(self, *_args: Any, **_kwargs: Any)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L592)
- protocol/private: `__init__`[`L589`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L589)
- used by: (1 test-only callers)

### `EmptyStore`
- def: [`tests/unit/test_edge_store.py:608`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L608)
- signature: `class EmptyStore:`
- members:
  - `has_edges(self, *_args: Any, **_kwargs: Any)` — [`L612`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L612)
- protocol/private: `__init__`[`L609`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L609)
- used by: (1 test-only callers)

### `FailingConn`
- def: [`tests/unit/test_edge_store.py:499`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L499)
- signature: `class FailingConn:`
- members:
  - `executescript(self, _schema: str)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L500)
- used by: (1 test-only callers)

### `_SQLCapturingConnection`
- def: [`tests/unit/test_edge_store.py:318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L318)
- doc: Wraps a sqlite3 connection, recording every `execute` SQL/params.
- signature: `class _SQLCapturingConnection:`
- members:
  - `execute(self, sql: str, params: tuple[Any, ...] = ())` — [`L330`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L330)
  - `calls` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L328)
- protocol/private: `__getattr__`[`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L334), `__init__`[`L326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L326), `_conn`[`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L327)
- used by: (1 test-only callers)

## Functions
- `_insert_raw_edge(conn: sqlite3.Connection, source_node_id: str, target_node_id: str, kind: str, file_path: str)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L232) — Insert one edge row with explicit source/file_path columns.
- `fail_refresh(file_paths: list[str] | None = None)` — [`L676`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L676)
- `record_fn(*_args: Any)` — [`L503`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L503)
- `test_ast_cache_call_queries_fall_back_when_edge_store_empty(monkeypatch: pytest.MonkeyPatch, tmp_path: Path)` — [`L604`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L604)
- `test_ast_cache_call_queries_fall_back_when_edge_store_raises(monkeypatch: pytest.MonkeyPatch, tmp_path: Path)` — [`L584`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L584)
- `test_ast_cache_call_queries_read_from_edge_store_when_legacy_edges_missing(tmp_path: Path)` — [`L563`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L563)
- `test_ast_cache_creates_edges_schema(tmp_path: Path)` — [`L473`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L473)
- `test_ast_cache_get_call_edges_handles_missing_table(tmp_path: Path)` — [`L623`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L623)
- `test_ast_cache_post_index_backfill_swallows_edge_refresh_failure(monkeypatch: pytest.MonkeyPatch, tmp_path: Path)` — [`L663`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L663)
- `test_ast_cache_refresh_edges_from_all_cached_rows_counts_json_errors(tmp_path: Path)` — [`L691`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L691)
- `test_ast_cache_resolve_only_refreshes_edge_store(monkeypatch: pytest.MonkeyPatch, tmp_path: Path)` — [`L637`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L637)
- `test_ast_cache_writes_calls_imports_contains_and_extends_edges(tmp_path: Path)` — [`L509`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L509)
- `test_edge_kind_covers_unified_relationship_surface()` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L24)
- `test_edge_store_call_queries_and_node_parser(tmp_path: Path)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L378)
- `test_edge_store_call_queries_deduplicate_and_fallback_to_call_site_file(tmp_path: Path)` — [`L446`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L446)
- `test_edge_store_crud_and_neighbors(tmp_path: Path)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L37)
- `test_edge_store_inheritance_tree_and_node_helpers(tmp_path: Path)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L210)
- `test_edge_store_migration_ignores_operational_error()` — [`L498`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L498)
- `test_edge_store_neighbors_deduplicates_null_line_edges(tmp_path: Path)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L191)
- `test_edge_store_query_directions_filters_and_fallbacks(tmp_path: Path)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L133)
- `test_edge_store_reuses_external_transaction(tmp_path: Path)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L90) — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `test_edge_store_serializes_edges_and_subgraphs(tmp_path: Path)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L64)
- `test_project_index_refreshes_edge_store_with_resolved_call_metadata(tmp_path: Path)` — [`L725`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L725)
- `test_replace_edges_for_file_deletes_all_predicate_kinds(tmp_path: Path)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L253) — ``replace_edges_for_file`` removes file_path / file-node / symbol-prefix
- `test_replace_edges_for_file_deletes_use_indexes_not_full_scan(tmp_path: Path)` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L338) — Every DELETE ``replace_edges_for_file`` issues must be index-driven (#990).
- `test_replace_edges_for_file_preserve_calls_keeps_calls_rows(tmp_path: Path)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L291) — ``preserve_calls=True`` deletes structural edges for the file but keeps
- `test_write_graph_edges_handles_empty_imports_and_missing_parent(tmp_path: Path)` — [`L758`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L758)
- `test_write_graph_edges_logs_operational_error(monkeypatch: pytest.MonkeyPatch, tmp_path: Path)` — [`L795`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store.py#L795)

