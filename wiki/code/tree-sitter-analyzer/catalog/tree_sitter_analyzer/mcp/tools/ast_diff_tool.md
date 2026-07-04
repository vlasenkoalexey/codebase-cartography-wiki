---
title: 'Module: tree_sitter_analyzer/mcp/tools/ast_diff_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/ast_diff_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.ast_diff_tool`/
symbols:
  ASTDiffTool.execute: ASTDiffTool#execute().
  ASTDiffTool: ASTDiffTool#
  ASTDiffTool._diff_git: ASTDiffTool#_diff_git().
  ASTDiffTool._get_differ: ASTDiffTool#_get_differ().
  ASTDiffTool.__init__: ASTDiffTool#__init__().
  ASTDiffTool._differ: ASTDiffTool#_differ.
  ASTDiffTool.validate_arguments: ASTDiffTool#validate_arguments().
  logger: logger.
  ASTDiffTool._on_project_root_changed: ASTDiffTool#_on_project_root_changed().
  ASTDiffTool.get_tool_definition: ASTDiffTool#get_tool_definition().
  ASTDiffTool._resolve_mode: ASTDiffTool#_resolve_mode().
  ASTDiffTool.get_tool_schema: ASTDiffTool#get_tool_schema().
  NODE_BODIES_BUDGET.NODE_BODIES_BUDGET: NODE_BODIES_BUDGET.NODE_BODIES_BUDGET.
---
# Module: [`tree_sitter_analyzer/mcp/tools/ast_diff_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py)

## Classes
### `ASTDiffTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/ast_diff_tool.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L34)
- doc: MCP Tool for structural AST diffing.
- signature: `class ASTDiffTool(BaseMCPTool):`
- members:
  - `_resolve_mode(arguments: dict[str, Any])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L149) — Effective mode — inferred from argument shape when omitted.
  - `execute(self, arguments: dict[str, Any])` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L213) — documented in [tree_sitter_analyzer-ast_diff](../../../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `get_tool_definition(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L49)
  - `get_tool_schema(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L69)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L182)
- protocol/private: `__init__`[`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L37), `_diff_git`[`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L307), `_differ`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L38), `_get_differ`[`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L44), `_on_project_root_changed`[`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L41)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`diff_strings`](../../ast_diff.md#ASTDiffer.diff_strings), [`_language_from_ext`](../../project_graph.md#_language_from_ext), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`diff_files`](../../ast_diff.md#ASTDiffer.diff_files), [`ASTDiffer`](../../ast_diff.md#ASTDiffer), [`to_dict`](../../ast_diff.md#ASTDiffResult.to_dict), [`NODE_BODIES_BUDGET`](ast_diff_tool.md#NODE_BODIES_BUDGET.NODE_BODIES_BUDGET)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (5 test-only)

## Module values
- `NODE_BODIES_BUDGET` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L31)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_diff_tool.py#L18)

