---
title: 'Module: tree_sitter_analyzer/_ast_cache_maintenance.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_maintenance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_maintenance`/
symbols:
  reclaim_storage_after_full_rebuild: reclaim_storage_after_full_rebuild().
  get_db_storage_stats: get_db_storage_stats().
  _pragma_int: _pragma_int().
  SQLITE_AUTO_VACUUM_NONE: SQLITE_AUTO_VACUUM_NONE.
  SQLITE_AUTO_VACUUM_INCREMENTAL: SQLITE_AUTO_VACUUM_INCREMENTAL.
  DEFAULT_VACUUM_MIN_FREE_PAGES: DEFAULT_VACUUM_MIN_FREE_PAGES.
---
# Module: [`tree_sitter_analyzer/_ast_cache_maintenance.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py)

## Functions
- `_pragma_int(conn: sqlite3.Connection, pragma_name: str)` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L16)
- `get_db_storage_stats(conn: sqlite3.Connection, db_path: str)` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L21) — Return exact SQLite file/page/free-list storage counters.
- `reclaim_storage_after_full_rebuild(conn: sqlite3.Connection, db_path: str, *, min_free_pages: int = DEFAULT_VACUUM_MIN_FREE_PAGES)` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L45) — Reclaim freelist pages after a force rebuild when the waste is material.

## Module values
- `DEFAULT_VACUUM_MIN_FREE_PAGES` — [`L13`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L13)
- `SQLITE_AUTO_VACUUM_INCREMENTAL` — [`L10`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L10)
- `SQLITE_AUTO_VACUUM_NONE` — [`L9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_maintenance.py#L9)

