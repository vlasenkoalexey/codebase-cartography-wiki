---
title: 'Module: tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.incremental_sync_tool`/
symbols:
  CodeGraphIncrementalSyncTool: CodeGraphIncrementalSyncTool#
  CodeGraphIncrementalSyncTool._sync: CodeGraphIncrementalSyncTool#_sync().
  CodeGraphIncrementalSyncTool.execute: CodeGraphIncrementalSyncTool#execute().
  CodeGraphIncrementalSyncTool._changes: CodeGraphIncrementalSyncTool#_changes().
  CodeGraphIncrementalSyncTool._status: CodeGraphIncrementalSyncTool#_status().
  CodeGraphIncrementalSyncTool._ensure_cache: CodeGraphIncrementalSyncTool#_ensure_cache().
  CodeGraphIncrementalSyncTool.validate_arguments: CodeGraphIncrementalSyncTool#validate_arguments().
  logger: logger.
  CodeGraphIncrementalSyncTool.get_tool_definition: CodeGraphIncrementalSyncTool#get_tool_definition().
  CodeGraphIncrementalSyncTool.get_tool_schema: CodeGraphIncrementalSyncTool#get_tool_schema().
---
# Module: [`tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py)

## Classes
### `CodeGraphIncrementalSyncTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L29)
- doc: MCP Tool for incremental AST cache sync (CodeGraph parity).
- signature: `class CodeGraphIncrementalSyncTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L86)
  - `get_tool_definition(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L32)
  - `get_tool_schema(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L54)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L79)
- protocol/private: `_changes`[`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L138), `_ensure_cache`[`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L104), `_status`[`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L168), `_sync`[`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L114)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`sync`](../../incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../incremental_sync.md#IncrementalSync), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`build_error`](_response_builder.md#build_error), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`ensure_indexed`](../utils/auto_index_guard.md#ensure_indexed), [`to_dict`](../../incremental_sync.md#SyncResult.to_dict), [`get_changes`](../../incremental_sync.md#IncrementalSync.get_changes), [`is_indexed`](../utils/auto_index_guard.md#is_indexed), [`logger`](incremental_sync_tool.md#logger)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade), [`run_incremental_sync`](../../cli/commands/codegraph_index_commands.md#run_incremental_sync)  (11 test-only)

## Module values
- `logger` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/incremental_sync_tool.py#L26)

