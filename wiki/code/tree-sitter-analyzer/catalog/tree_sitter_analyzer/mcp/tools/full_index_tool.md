---
title: 'Module: tree_sitter_analyzer/mcp/tools/full_index_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/full_index_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.full_index_tool`/
symbols:
  CodeGraphFullIndexTool.execute: CodeGraphFullIndexTool#execute().
  CodeGraphFullIndexTool._phase_incremental_sync: CodeGraphFullIndexTool#_phase_incremental_sync().
  CodeGraphFullIndexTool: CodeGraphFullIndexTool#
  CodeGraphFullIndexTool._phase_call_edge_stats: CodeGraphFullIndexTool#_phase_call_edge_stats().
  CodeGraphFullIndexTool._phase_ast_cache: CodeGraphFullIndexTool#_phase_ast_cache().
  CodeGraphFullIndexTool._phase_fts5_stats: CodeGraphFullIndexTool#_phase_fts5_stats().
  CodeGraphFullIndexTool._collect_final_stats: CodeGraphFullIndexTool#_collect_final_stats().
  CodeGraphFullIndexTool.validate_arguments: CodeGraphFullIndexTool#validate_arguments().
  CodeGraphFullIndexTool.get_tool_definition: CodeGraphFullIndexTool#get_tool_definition().
  logger: logger.
  CodeGraphFullIndexTool.get_tool_schema: CodeGraphFullIndexTool#get_tool_schema().
  CodeGraphFullIndexTool._phase_synapse: CodeGraphFullIndexTool#_phase_synapse().
---
# Module: [`tree_sitter_analyzer/mcp/tools/full_index_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py)

## Classes
### `CodeGraphFullIndexTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/full_index_tool.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L32)
- doc: MCP Tool for one-shot complete project intelligence indexing.
- signature: `class CodeGraphFullIndexTool(BaseMCPTool):`
- members:
  - `_phase_synapse(self, ast_phase: dict[str, Any])` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L259) — Report cross-file resolution results.
  - `execute(self, arguments: dict[str, Any])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L104)
  - `get_tool_definition(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L35)
  - `get_tool_schema(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L57)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L98)
- protocol/private: `_collect_final_stats`[`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L299), `_phase_ast_cache`[`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L171), `_phase_call_edge_stats`[`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L282), `_phase_fts5_stats`[`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L244), `_phase_incremental_sync`[`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L213)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`index_project`](../../ast_cache.md#ASTCache.index_project), [`sync`](../../incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../incremental_sync.md#IncrementalSync), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`has_call_edges`](../../ast_cache.md#ASTCache.has_call_edges), [`errors`](../../incremental_sync.md#SyncResult.errors), [`mark_dirty`](../utils/auto_index_guard.md#mark_dirty), [`deleted_files`](../../incremental_sync.md#SyncResult.deleted_files), [`new_files`](../../incremental_sync.md#SyncResult.new_files), [`updated_files`](../../incremental_sync.md#SyncResult.updated_files), [`scanned`](../../incremental_sync.md#SyncResult.scanned), [`unchanged_files`](../../incremental_sync.md#SyncResult.unchanged_files)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade), [`run_full_index`](../../cli/commands/codegraph_index_commands.md#run_full_index)  (10 test-only)

## Module values
- `logger` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/full_index_tool.py#L29)

