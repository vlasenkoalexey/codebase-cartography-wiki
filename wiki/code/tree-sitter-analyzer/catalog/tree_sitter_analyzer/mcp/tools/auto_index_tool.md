---
title: 'Module: tree_sitter_analyzer/mcp/tools/auto_index_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/auto_index_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.auto_index_tool`/
symbols:
  CodeGraphAutoIndexTool: CodeGraphAutoIndexTool#
  CodeGraphAutoIndexTool.execute: CodeGraphAutoIndexTool#execute().
  CodeGraphAutoIndexTool._status: CodeGraphAutoIndexTool#_status().
  CodeGraphAutoIndexTool._warm: CodeGraphAutoIndexTool#_warm().
  CodeGraphAutoIndexTool._reset: CodeGraphAutoIndexTool#_reset().
  CodeGraphAutoIndexTool.validate_arguments: CodeGraphAutoIndexTool#validate_arguments().
  CodeGraphAutoIndexTool.get_tool_definition: CodeGraphAutoIndexTool#get_tool_definition().
  logger: logger.
  CodeGraphAutoIndexTool.get_tool_schema: CodeGraphAutoIndexTool#get_tool_schema().
---
# Module: [`tree_sitter_analyzer/mcp/tools/auto_index_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py)

## Classes
### `CodeGraphAutoIndexTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/auto_index_tool.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L33)
- doc: MCP Tool for transparent AST cache warming (CodeGraph parity).
- signature: `class CodeGraphAutoIndexTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L91)
  - `get_tool_definition(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L36)
  - `get_tool_schema(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L59)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L84)
- protocol/private: `_reset`[`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L182), `_status`[`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L105), `_warm`[`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L144)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`build_error`](_response_builder.md#build_error), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`ensure_indexed`](../utils/auto_index_guard.md#ensure_indexed), [`is_indexed`](../utils/auto_index_guard.md#is_indexed), [`mark_dirty`](../utils/auto_index_guard.md#mark_dirty)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade), [`run_autoindex`](../../cli/commands/codegraph_index_commands.md#run_autoindex)  (14 test-only)

## Module values
- `logger` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/auto_index_tool.py#L30)

