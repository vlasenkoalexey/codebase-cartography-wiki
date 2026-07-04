---
title: 'Module: tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.unreachable_code_tool`/
symbols:
  UnreachableCodeTool: UnreachableCodeTool#
  UnreachableCodeTool._build_file_response: UnreachableCodeTool#_build_file_response().
  UnreachableCodeTool._format_file_blocks_toon: UnreachableCodeTool#_format_file_blocks_toon().
  UnreachableCodeTool._build_project_response: UnreachableCodeTool#_build_project_response().
  UnreachableCodeTool.execute: UnreachableCodeTool#execute().
  UnreachableCodeTool._execute_file_mode: UnreachableCodeTool#_execute_file_mode().
  UnreachableCodeTool._execute_project_mode: UnreachableCodeTool#_execute_project_mode().
  UnreachableCodeTool._resolve_path: UnreachableCodeTool#_resolve_path().
  UnreachableCodeTool.validate_arguments: UnreachableCodeTool#validate_arguments().
  logger: logger.
  UnreachableCodeTool.get_tool_definition: UnreachableCodeTool#get_tool_definition().
  UnreachableCodeTool.get_tool_schema: UnreachableCodeTool#get_tool_schema().
  UnreachableCodeTool._format_block_line: UnreachableCodeTool#_format_block_line().
  UnreachableCodeTool.get_tool_name: UnreachableCodeTool#get_tool_name().
---
# Module: [`tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py)

## Classes
### `UnreachableCodeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L35)
- doc: MCP Tool for statement-level unreachable code detection.
- signature: `class UnreachableCodeTool(BaseMCPTool):`
- members:
  - `_format_block_line(block: Any)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L154) — Format a single unreachable block as a TOON line.
  - `_format_file_blocks_toon(self, r: UnreachableCodeResult)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L191) — Format a single file's unreachable blocks as TOON lines.
  - `execute(self, arguments: dict[str, Any])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L101)
  - `get_tool_definition(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L38)
  - `get_tool_name(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L90)
  - `get_tool_schema(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L52)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L93)
- protocol/private: `_build_file_response`[`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L162), `_build_project_response`[`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L203), `_execute_file_mode`[`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L111), `_execute_project_mode`[`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L131), `_resolve_path`[`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L234)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`analyze_file_unreachable`](../../unreachable_code.md#analyze_file_unreachable), [`unreachable_blocks`](../../unreachable_code.md#UnreachableCodeResult.unreachable_blocks), [`analyze_project_unreachable`](../../unreachable_code.md#analyze_project_unreachable), [`to_dict`](../../unreachable_code.md#UnreachableCodeResult.to_dict), [`UnreachableCodeResult`](../../unreachable_code.md#UnreachableCodeResult), [`errors`](../../unreachable_code.md#UnreachableCodeResult.errors), [`reason`](../../unreachable_code.md#UnreachableBlock.reason), [`language`](../../unreachable_code.md#UnreachableCodeResult.language), [`file_path`](../../unreachable_code.md#UnreachableCodeResult.file_path), [`functions_analyzed`](../../unreachable_code.md#UnreachableCodeResult.functions_analyzed), [`end_line`](../../unreachable_code.md#UnreachableBlock.end_line), [`function_name`](../../unreachable_code.md#UnreachableBlock.function_name), [`start_line`](../../unreachable_code.md#UnreachableBlock.start_line), [`logger`](unreachable_code_tool.md#logger)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments)  (30 test-only)

## Module values
- `logger` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/unreachable_code_tool.py#L32)

