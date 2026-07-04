---
title: 'Module: tree_sitter_analyzer/mcp/tools/code_similarity_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/code_similarity_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.code_similarity_tool`/
symbols:
  CodeGraphSimilarityTool.execute: CodeGraphSimilarityTool#execute().
  CodeGraphSimilarityTool: CodeGraphSimilarityTool#
  logger: logger.
  CodeGraphSimilarityTool.validate_arguments: CodeGraphSimilarityTool#validate_arguments().
  CodeGraphSimilarityTool.get_tool_definition: CodeGraphSimilarityTool#get_tool_definition().
  CodeGraphSimilarityTool.get_tool_schema: CodeGraphSimilarityTool#get_tool_schema().
  CodeGraphSimilarityTool._group_to_dict: CodeGraphSimilarityTool#_group_to_dict().
---
# Module: [`tree_sitter_analyzer/mcp/tools/code_similarity_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py)

## Classes
### `CodeGraphSimilarityTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/code_similarity_tool.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L23)
- doc: MCP Tool for AST-structural clone detection (CodeGraph parity).
- signature: `class CodeGraphSimilarityTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L116)
  - `get_tool_definition(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L26)
  - `get_tool_schema(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L47)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L109)
- protocol/private: `_group_to_dict`[`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L166)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`analyze_code_similarity`](../../code_similarity.md#analyze_code_similarity), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`groups`](../../code_similarity.md#SimilarityResult.groups), [`stats`](../../code_similarity.md#SimilarityResult.stats), [`logger`](code_similarity_tool.md#logger)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_viz_facade`](viz_facade.md#build_viz_facade)  (6 test-only)

## Module values
- `logger` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_similarity_tool.py#L20)

