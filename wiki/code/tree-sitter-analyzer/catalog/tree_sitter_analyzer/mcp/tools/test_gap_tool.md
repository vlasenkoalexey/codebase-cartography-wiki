---
title: 'Module: tree_sitter_analyzer/mcp/tools/test_gap_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/test_gap_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.test_gap_tool`/
symbols:
  CodeGraphTestGapTool.execute: CodeGraphTestGapTool#execute().
  CodeGraphTestGapTool: CodeGraphTestGapTool#
  CodeGraphTestGapTool.validate_arguments: CodeGraphTestGapTool#validate_arguments().
  logger: logger.
  CodeGraphTestGapTool.get_tool_schema: CodeGraphTestGapTool#get_tool_schema().
  CodeGraphTestGapTool.get_tool_definition: CodeGraphTestGapTool#get_tool_definition().
  CodeGraphTestGapTool._build_response: CodeGraphTestGapTool#_build_response().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/test_gap_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py)

## Classes
### `CodeGraphTestGapTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/test_gap_tool.py:89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L89)
- doc: MCP Tool for test coverage gap analysis.
- signature: `class CodeGraphTestGapTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L115)
  - `get_tool_definition(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L92)
  - `get_tool_schema(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L103)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L106)
- protocol/private: `_build_response`[`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L155)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`build_error`](_response_builder.md#build_error), [`invalid_enum_error`](_validators.md#invalid_enum_error)  (4 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_health_facade`](health_facade.md#build_health_facade)  (6 test-only)

## Module values
- `TOOL_SCHEMA` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L26)
- `logger` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/test_gap_tool.py#L24)

