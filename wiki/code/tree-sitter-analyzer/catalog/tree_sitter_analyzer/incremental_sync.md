---
title: 'Module: tree_sitter_analyzer/incremental_sync.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/incremental_sync.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.incremental_sync`/
symbols:
  IncrementalSync.sync: IncrementalSync#sync().
  IncrementalSync: IncrementalSync#
  SyncResult.to_dict: SyncResult#to_dict().
  IncrementalSync._index_or_reindex_files: IncrementalSync#_index_or_reindex_files().
  IncrementalSync._invalidate_deleted_files: IncrementalSync#_invalidate_deleted_files().
  SyncResult.errors: SyncResult#errors.
  IncrementalSync._cache: IncrementalSync#_cache.
  IncrementalSync.get_changes: IncrementalSync#get_changes().
  SyncResult: SyncResult#
  SyncResult.details: SyncResult#details.
  SyncResult.new_files: SyncResult#new_files.
  SyncResult.updated_files: SyncResult#updated_files.
  SyncResult.deleted_files: SyncResult#deleted_files.
  IncrementalSync._scan_disk_files: IncrementalSync#_scan_disk_files().
  IncrementalSync._index_new_file: IncrementalSync#_index_new_file().
  IncrementalSync._reindex_modified: IncrementalSync#_reindex_modified().
  logger: logger.
  SyncResult.scanned: SyncResult#scanned.
  SyncResult.unchanged_files: SyncResult#unchanged_files.
  IncrementalSync._file_changed: IncrementalSync#_file_changed().
  SyncResult.synapse_resolved: SyncResult#synapse_resolved.
  _file_content_hash: _file_content_hash().
  IncrementalSync._load_indexed_rows: IncrementalSync#_load_indexed_rows().
  IncrementalSync.__init__: IncrementalSync#__init__().
---
# Module: [`tree_sitter_analyzer/incremental_sync.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py)

## Classes
### `IncrementalSync`
- def: [`tree_sitter_analyzer/incremental_sync.py:63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L63)
- doc: Incremental sync engine for ASTCache.
- signature: `class IncrementalSync:`
- members:
  - `_index_or_reindex_files(self, disk_files: dict[str, dict[str, Any]], indexed_rows: dict[str, dict[str, Any]], conn: Any, result: SyncResult, callback: Any | None)` — [`L186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L186) — For each disk file: index if new, re-index if changed, skip otherwise.
  - `_invalidate_deleted_files(self, deleted_paths: set[str], result: SyncResult, callback: Any | None)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L160) — Drop AST rows for files that vanished from disk.
  - `_load_indexed_rows(conn: Any)` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L127) — Snapshot the ``ast_index`` table as ``{path: {hash, mtime, size}}``.
  - `_scan_disk_files(self, max_files: int)` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L140) — Walk the project tree; return ``{rel_path: {abs_path, mtime, size}}``.
  - `get_changes(self)` — [`L326`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L326) — Quick scan that returns lists of changed file paths without re-indexing.
  - `sync(self, max_files: int = 20000, callback: Any | None = None)` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L78) — Sync the on-disk source tree with the AST cache.
- protocol/private: `__init__`[`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L75), `_cache`[`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L76), `_file_changed`[`L212`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L212), `_index_new_file`[`L228`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L228), `_reindex_modified`[`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L282)
- uses (calls/refs, reference-scoped): [`EXT_TO_LANG`](_lang_extension_map.md#EXT_TO_LANG.EXT_TO_LANG), [`_walk_source_files`](ast_cache.md#_walk_source_files), [`errors`](incremental_sync.md#SyncResult.errors), [`SyncResult`](incremental_sync.md#SyncResult), [`details`](incremental_sync.md#SyncResult.details), [`deleted_files`](incremental_sync.md#SyncResult.deleted_files), [`new_files`](incremental_sync.md#SyncResult.new_files), [`updated_files`](incremental_sync.md#SyncResult.updated_files), [`logger`](incremental_sync.md#logger), [`scanned`](incremental_sync.md#SyncResult.scanned), [`unchanged_files`](incremental_sync.md#SyncResult.unchanged_files), [`synapse_resolved`](incremental_sync.md#SyncResult.synapse_resolved), [`_file_content_hash`](incremental_sync.md#_file_content_hash)
- used by: [`_phase_incremental_sync`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._phase_incremental_sync), [`_do_sync`](file_watcher.md#FileWatcherDaemon._do_sync), [`_ensure_ast_cache`](mcp/tools/utils/change_impact_analysis.md#_ensure_ast_cache), [`_sync`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._sync), [`_prepare_index`](mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool._prepare_index), [`_changes`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._changes), [`_status`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._status), [`_handle_sync`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_sync), [`_get_sync`](mcp/tools/ast_cache_tool.md#ASTCacheTool._get_sync), [`_handle_changes`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_changes), [`_sync`](mcp/tools/ast_cache_tool.md#ASTCacheTool._sync), [`_sync`](file_watcher.md#FileWatcherDaemon._sync)  (18 test-only)

### `SyncResult`
- def: [`tree_sitter_analyzer/incremental_sync.py:29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L29)
- doc: Result of an incremental sync operation.
- signature: `class SyncResult:`
- members:
  - `to_dict(self)` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L41)
  - `deleted_files` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L35)
  - `details` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L39)
  - `errors` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L37)
  - `new_files` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L33)
  - `scanned` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L32)
  - `synapse_resolved` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L38)
  - `unchanged_files` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L36)
  - `updated_files` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L34)
- used by: [`sync`](incremental_sync.md#IncrementalSync.sync), [`_phase_incremental_sync`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._phase_incremental_sync), [`_do_sync`](file_watcher.md#FileWatcherDaemon._do_sync), [`_index_or_reindex_files`](incremental_sync.md#IncrementalSync._index_or_reindex_files), [`_sync`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._sync), [`_prepare_index`](mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool._prepare_index), [`_invalidate_deleted_files`](incremental_sync.md#IncrementalSync._invalidate_deleted_files), [`_handle_sync`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_sync)  (8 test-only)

## Functions
- `_file_content_hash(path: str)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L55)

## Module values
- `logger` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/incremental_sync.py#L25)

