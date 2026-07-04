---
title: 'Module: tree_sitter_analyzer/mcp/tools/dead_code_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/dead_code_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.dead_code_tool`/
symbols:
  CodeGraphDeadCodeTool.execute: CodeGraphDeadCodeTool#execute().
  CodeGraphDeadCodeTool: CodeGraphDeadCodeTool#
  _serialize_unused_import: _serialize_unused_import().
  _serialize_unref_var: _serialize_unref_var().
  _serialize_dead_function: _serialize_dead_function().
  CodeGraphDeadCodeTool.validate_arguments: CodeGraphDeadCodeTool#validate_arguments().
  logger: logger.
  CodeGraphDeadCodeTool.get_tool_definition: CodeGraphDeadCodeTool#get_tool_definition().
  CodeGraphDeadCodeTool.get_tool_schema: CodeGraphDeadCodeTool#get_tool_schema().
  _under_path: _under_path().
---
# Module: [`tree_sitter_analyzer/mcp/tools/dead_code_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py)

## Classes
### `CodeGraphDeadCodeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/dead_code_tool.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L30)
- doc: MCP Tool for comprehensive dead code analysis (CodeGraph parity).
- signature: `class CodeGraphDeadCodeTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L114) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_definition(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L33)
  - `get_tool_schema(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L51)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L107)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`FunctionRef`](../../call_graph.md#FunctionRef), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`analyze_dead_code`](../../dead_code_analyzer.md#analyze_dead_code), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`_serialize_unref_var`](dead_code_tool.md#_serialize_unref_var), [`_serialize_unused_import`](dead_code_tool.md#_serialize_unused_import), [`dead_functions`](../../dead_code_analyzer.md#DeadCodeResult.dead_functions), [`stats`](../../dead_code_analyzer.md#DeadCodeResult.stats), [`unreferenced_variables`](../../dead_code_analyzer.md#DeadCodeResult.unreferenced_variables), [`unused_imports`](../../dead_code_analyzer.md#DeadCodeResult.unused_imports), [`_serialize_dead_function`](dead_code_tool.md#_serialize_dead_function), [`file`](../../dead_code_analyzer.md#UnusedImport.file), [`file`](../../dead_code_analyzer.md#UnreferencedVariable.file), [`logger`](dead_code_tool.md#logger), [`_under_path`](dead_code_tool.md#_under_path)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_health_facade`](health_facade.md#build_health_facade)  (35 test-only)

## Functions
- `_serialize_dead_function(df: DeadFunction)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L300)
- `_serialize_unref_var(uv: UnreferencedVariable)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L322)
- `_serialize_unused_import(ui: UnusedImport)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L313)
- `_under_path(file_path: str, path: str)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L280) — True if ``file_path`` is the ``path`` itself or lives under it, matched

## Module values
- `logger` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dead_code_tool.py#L27)

