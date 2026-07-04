---
title: 'Module: tree_sitter_analyzer/mcp/tools/ast_cache_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/ast_cache_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.ast_cache_tool`/
symbols:
  ASTCacheTool: ASTCacheTool#
  ASTCacheTool.execute: ASTCacheTool#execute().
  ASTCacheTool._watcher: ASTCacheTool#_watcher.
  ASTCacheTool._handle_watch_start: ASTCacheTool#_handle_watch_start().
  _build_ast_cache_envelope: _build_ast_cache_envelope().
  ASTCacheTool._on_project_root_changed: ASTCacheTool#_on_project_root_changed().
  ASTCacheTool.validate_arguments: ASTCacheTool#validate_arguments().
  ASTCacheTool._handle_watch_stop: ASTCacheTool#_handle_watch_stop().
  ASTCacheTool._cache: ASTCacheTool#_cache.
  ASTCacheTool._get_cache: ASTCacheTool#_get_cache().
  ASTCacheTool._handle_sync: ASTCacheTool#_handle_sync().
  ASTCacheTool._handle_watch_status: ASTCacheTool#_handle_watch_status().
  ASTCacheTool.get_cache: ASTCacheTool#get_cache().
  ASTCacheTool._get_sync: ASTCacheTool#_get_sync().
  _split_legacy_import_row: _split_legacy_import_row().
  ASTCacheTool._handle_changes: ASTCacheTool#_handle_changes().
  ASTCacheTool._sync: ASTCacheTool#_sync.
  ASTCacheTool._handle_index: ASTCacheTool#_handle_index().
  ASTCacheTool._handle_lookup: ASTCacheTool#_handle_lookup().
  ASTCacheTool._handle_search: ASTCacheTool#_handle_search().
  ASTCacheTool._handle_invalidate: ASTCacheTool#_handle_invalidate().
  ASTCacheTool.cache_initialized: ASTCacheTool#cache_initialized().
  ASTCacheTool._resolve_mode: ASTCacheTool#_resolve_mode().
  ASTCacheTool.get_tool_schema: ASTCacheTool#get_tool_schema().
  logger: logger.
  _apply_legacy_import_split: _apply_legacy_import_split().
  _build_unknown_mode_response: _build_unknown_mode_response().
  ASTCacheTool.get_tool_definition: ASTCacheTool#get_tool_definition().
  ASTCacheTool._handle_stats: ASTCacheTool#_handle_stats().
  _IMPORT_NAME_LIMIT: _IMPORT_NAME_LIMIT.
  _BOUND_NAME_PATTERN: _BOUND_NAME_PATTERN.
  _IMPORT_KEYWORDS: _IMPORT_KEYWORDS.
  ASTCacheTool.__init__: ASTCacheTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/ast_cache_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py)

## Classes
### `ASTCacheTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/ast_cache_tool.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L173)
- doc: MCP Tool for pre-indexed AST cache operations.
- signature: `class ASTCacheTool(BaseMCPTool):`
- members:
  - `_handle_changes(self)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L616) — ``mode=changes``: pending new/modified/deleted file list.
  - `_handle_index(self, arguments: dict[str, Any], cache: Any)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L422) — ``mode=index``: per-file or whole-project AST cache build.
  - `_handle_invalidate(self, arguments: dict[str, Any], cache: Any)` — [`L644`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L644) — ``mode=invalidate``: drop a single file's cached AST entry.
  - `_handle_lookup(self, arguments: dict[str, Any], cache: Any)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L460) — ``mode=lookup``: read a single file's cached AST entry.
  - `_handle_search(arguments: dict[str, Any], cache: Any, mode: str)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L484) — ``mode=search`` / ``fts_search``: J1 unified FTS lookup with K7 split.
  - `_handle_stats(cache: Any)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L546) — ``mode=stats``: aggregate row counts + FTS5 capability flag.
  - `_handle_sync(self, arguments: dict[str, Any])` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L595) — ``mode=sync``: drift-detect + reconcile + M15 considered alias.
  - `_handle_watch_start(self, arguments: dict[str, Any])` — [`L664`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L664) — ``mode=watch_start``: spawn (or reuse) the FileWatcherDaemon.
  - `_handle_watch_status(self)` — [`L759`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L759) — ``mode=watch_status``: report watcher liveness and stats.
  - `_handle_watch_stop(self)` — [`L727`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L727) — ``mode=watch_stop``: stop the running watcher and return stats.
  - `_resolve_mode(arguments: dict[str, Any])` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L336) — Effective mode.
  - `cache_initialized(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L207) — True if the AST cache has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L377) — Dispatch ast_cache by ``mode``.
  - `get_cache(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L202) — Public alias for _get_cache() — use this instead of accessing _cache directly.
  - `get_tool_definition(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L216)
  - `get_tool_schema(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L244)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L348)
- protocol/private: `__init__`[`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L176), `_cache`[`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L177), `_get_cache`[`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L195), `_get_sync`[`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L211), `_on_project_root_changed`[`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L182), `_sync`[`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L178), `_watcher`[`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L179)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`sync`](../../incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../incremental_sync.md#IncrementalSync), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`get_stats`](../../file_watcher.md#FileWatcherDaemon.get_stats), [`to_dict`](../../incremental_sync.md#SyncResult.to_dict), [`_build_ast_cache_envelope`](ast_cache_tool.md#_build_ast_cache_envelope), [`start`](../../file_watcher.md#FileWatcherDaemon.start), [`stop`](../../file_watcher.md#FileWatcherDaemon.stop), [`get_changes`](../../incremental_sync.md#IncrementalSync.get_changes), [`FileWatcherDaemon`](../../file_watcher.md#FileWatcherDaemon), [`is_running`](../../file_watcher.md#FileWatcherDaemon.is_running), [`backend`](../../file_watcher.md#FileWatcherDaemon.backend), [`make_on_sync_callback`](../watch_push_bridge.md#make_on_sync_callback), [`poll_interval`](../../file_watcher.md#FileWatcherDaemon.poll_interval), [`_apply_legacy_import_split`](ast_cache_tool.md#_apply_legacy_import_split), [`_build_unknown_mode_response`](ast_cache_tool.md#_build_unknown_mode_response), [`logger`](ast_cache_tool.md#logger), [`_project_root`](base_tool.md#BaseMCPTool._project_root)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_index_facade`](index_facade.md#build_index_facade)  (33 test-only)

## Functions
- `_apply_legacy_import_split(results: list[dict[str, Any]])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L106) — Apply ``_split_legacy_import_row`` across an FTS result list.
- `_build_ast_cache_envelope(mode: str, payload: dict[str, Any], summary_line: str, next_step: str)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L136) — Wrap an ast_cache mode's raw payload in the canonical envelope.
- `_build_unknown_mode_response(mode: str)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L116) — Canonical INVALID_INPUT envelope for unknown ``mode=`` values.
- `_split_legacy_import_row(row: dict[str, Any])` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L51) — Return one row per bound identifier when ``row['name']`` holds a

## Module values
- `_BOUND_NAME_PATTERN` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L32)
- `_IMPORT_KEYWORDS` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L33)
- `_IMPORT_NAME_LIMIT` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L31)
- `logger` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_cache_tool.py#L23)

