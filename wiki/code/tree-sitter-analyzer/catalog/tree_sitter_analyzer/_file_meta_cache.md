---
title: 'Module: tree_sitter_analyzer/_file_meta_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_file_meta_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._file_meta_cache`/
symbols:
  FileMetaCache._conn: FileMetaCache#_conn.
  FileMetaCache._init_db: FileMetaCache#_init_db().
  FileMetaCache.store_line_count: FileMetaCache#store_line_count().
  FileMetaCache.close: FileMetaCache#close().
  FileMetaCache.get_line_count: FileMetaCache#get_line_count().
  FileMetaCache.count_lines: FileMetaCache#count_lines().
  FileMetaCache.enabled: FileMetaCache#enabled().
  FileMetaCache: FileMetaCache#
  FileMetaCache._db_path: FileMetaCache#_db_path.
  FileMetaCache._enabled: FileMetaCache#_enabled.
  logger: logger.
  _SCHEMA: _SCHEMA.
  FileMetaCache._default_db_path: FileMetaCache#_default_db_path().
  FileMetaCache.__init__: FileMetaCache#__init__().
  FileMetaCache._project_root: FileMetaCache#_project_root.
---
# Module: [`tree_sitter_analyzer/_file_meta_cache.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py)

## Classes
### `FileMetaCache`
- def: [`tree_sitter_analyzer/_file_meta_cache.py:39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L39)
- doc: Small SQLite cache for cheap per-file metadata.
- signature: `class FileMetaCache:`
- members:
  - `close(self)` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L78)
  - `count_lines(self, file_path: str)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L133) — High-level entry point: stat + look up + (read on miss) + store.
  - `enabled(self)` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L75)
  - `get_line_count(self, file_path: str, *, mtime_ns: int, size_bytes: int)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L88) — Return cached line count iff fingerprint matches; otherwise None.
  - `store_line_count(self, file_path: str, *, mtime_ns: int, size_bytes: int, line_count: int)` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L113)
- protocol/private: `__init__`[`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L47), `_conn`[`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L50), `_db_path`[`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L49), `_default_db_path`[`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L54), `_enabled`[`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L51), `_init_db`[`L57`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L57), `_project_root`[`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L48)
- uses (calls/refs, reference-scoped): [`logger`](_file_meta_cache.md#logger), [`_SCHEMA`](_file_meta_cache.md#_SCHEMA)
- used by: (5 test-only callers)

## Module values
- `_SCHEMA` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L28)
- `logger` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_file_meta_cache.py#L26)

