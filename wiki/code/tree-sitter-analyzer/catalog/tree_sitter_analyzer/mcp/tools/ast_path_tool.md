---
title: 'Module: tree_sitter_analyzer/mcp/tools/ast_path_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/ast_path_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.ast_path_tool`/
symbols:
  CodeGraphASTPathTool.execute: CodeGraphASTPathTool#execute().
  CodeGraphASTPathTool: CodeGraphASTPathTool#
  CodeGraphASTPathTool._get_navigator: CodeGraphASTPathTool#_get_navigator().
  CodeGraphASTPathTool.__init__: CodeGraphASTPathTool#__init__().
  CodeGraphASTPathTool._navigator: CodeGraphASTPathTool#_navigator.
  logger: logger.
  CodeGraphASTPathTool._on_project_root_changed: CodeGraphASTPathTool#_on_project_root_changed().
  CodeGraphASTPathTool.get_tool_definition: CodeGraphASTPathTool#get_tool_definition().
  CodeGraphASTPathTool.get_tool_schema: CodeGraphASTPathTool#get_tool_schema().
  CodeGraphASTPathTool.validate_arguments: CodeGraphASTPathTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/ast_path_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py)

## Classes
### `CodeGraphASTPathTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/ast_path_tool.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L25)
- doc: MCP Tool for AST path/scope navigation (CodeGraph parity).
- signature: `class CodeGraphASTPathTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L107)
  - `get_tool_definition(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L40)
  - `get_tool_schema(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L61)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L99)
- protocol/private: `__init__`[`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L28), `_get_navigator`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L35), `_navigator`[`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L29), `_on_project_root_changed`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L32)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`path_at_line`](../../ast_path.md#ASTPathNavigator.path_at_line), [`outline`](../../ast_path.md#ASTPathNavigator.outline), [`ASTPathNavigator`](../../ast_path.md#ASTPathNavigator), [`to_dict`](../../ast_path.md#ASTPathResult.to_dict), [`scope_at`](../../ast_path.md#ASTPathNavigator.scope_at)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade)  (3 test-only)

## Module values
- `logger` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/ast_path_tool.py#L22)

