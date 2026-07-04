---
title: 'Module: tests/unit/test_edge_store_name_columns.py'
type: catalog
provenance: extracted
module: tests/unit/test_edge_store_name_columns.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_edge_store_name_columns`/
symbols:
  test_calls_queries_results_unchanged: test_calls_queries_results_unchanged().
  test_upsert_populates_name_columns_from_metadata: test_upsert_populates_name_columns_from_metadata().
  test_calls_query_uses_index_not_full_scan: test_calls_query_uses_index_not_full_scan().
  test_edges_table_has_name_and_file_columns: test_edges_table_has_name_and_file_columns().
  test_edges_table_indexes_name_columns: test_edges_table_indexes_name_columns().
  test_ast_cache_migration_v10_recorded: test_ast_cache_migration_v10_recorded().
  test_indexed_file_populates_name_columns: test_indexed_file_populates_name_columns().
  test_legacy_v9_db_upgrades_to_v10: test_legacy_v9_db_upgrades_to_v10().
  _edges_columns: _edges_columns().
  _edges_indexes: _edges_indexes().
---
# Module: [`tests/unit/test_edge_store_name_columns.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py)

## Functions
- `_edges_columns(conn: sqlite3.Connection)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L28)
- `_edges_indexes(conn: sqlite3.Connection)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L32)
- `test_ast_cache_migration_v10_recorded(tmp_path: Path)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L59) — A fresh ASTCache stamps schema version 10 and the new edges columns.
- `test_calls_queries_results_unchanged(tmp_path: Path)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L129) — Pushed-down CALLS queries return identical entries to the legacy path.
- `test_calls_query_uses_index_not_full_scan(tmp_path: Path)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L103) — query_callers' direct lookup plans use the callee_name index, not a scan.
- `test_edges_table_has_name_and_file_columns(tmp_path: Path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L36) — edges schema exposes caller_name / callee_name / file_path real columns.
- `test_edges_table_indexes_name_columns(tmp_path: Path)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L48) — Name columns are indexed so CALLS queries can push the filter to SQL.
- `test_indexed_file_populates_name_columns(tmp_path: Path)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L186) — Indexing a real file fills the new columns end-to-end via the write path.
- `test_legacy_v9_db_upgrades_to_v10(tmp_path: Path)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L212) — A pre-existing edges table without name columns is migrated to v10.
- `test_upsert_populates_name_columns_from_metadata(tmp_path: Path)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_edge_store_name_columns.py#L74) — upsert_edges writes caller_name/callee_name/file_path real columns.

