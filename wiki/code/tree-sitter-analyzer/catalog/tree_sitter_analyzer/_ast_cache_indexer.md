---
title: 'Module: tree_sitter_analyzer/_ast_cache_indexer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_indexer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_indexer`/
symbols:
  parse_and_write: parse_and_write().
  insert_index_row: insert_index_row().
  _AST_CACHE_EXTRACTOR_VERSION: _AST_CACHE_EXTRACTOR_VERSION.
  check_cache_or_read: check_cache_or_read().
  walk_and_partition: walk_and_partition().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/_ast_cache_indexer.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py)

## Functions
- `check_cache_or_read(conn: sqlite3.Connection, rel_path: str, abs_path: str, stat: os.stat_result, content_hash_fn: Any, extractor_version: int)` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L43) — Return cached-response dict or (source_code, content_hash) if stale.
- `insert_index_row(cache: Any, conn: sqlite3.Connection, r: dict[str, Any], indexed_at: str, extractor_version: int, include_activation: bool = True)` — [`L235`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L235) — Write one worker result to SQLite (main table + optional FTS5).
- `parse_and_write(cache: Any, conn: sqlite3.Connection, abs_path: str, rel_path: str, language: str, stat: os.stat_result, source_code: str, content_hash: str, extractor_version: int)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L83) — Parse a file and write all cache rows. Returns result dict.
- `walk_and_partition(cache: Any, conn: sqlite3.Connection, max_files: int, force: bool, activation_enabled: bool, walk_fn: Any, language_fn: Any, extractor_version: int, make_error_entry: Any, language_filter: str | None = None)` — [`L157`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L157) — Walk source files and partition into (stats, candidates, count).

## Module values
- `_AST_CACHE_EXTRACTOR_VERSION` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L40)
- `logger` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_indexer.py#L20)

