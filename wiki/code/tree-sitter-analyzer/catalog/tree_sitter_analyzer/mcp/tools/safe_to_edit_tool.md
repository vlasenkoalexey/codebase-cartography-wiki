---
title: 'Module: tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.safe_to_edit_tool`/
symbols:
  SafeToEditTool.execute: SafeToEditTool#execute().
  SafeToEditTool: SafeToEditTool#
  _compute_risk: _compute_risk().
  SafeToEditTool._scorer: SafeToEditTool#_scorer.
  SafeToEditTool._get_graph: SafeToEditTool#_get_graph().
  SafeToEditTool._graph: SafeToEditTool#_graph.
  SafeToEditTool._get_scorer: SafeToEditTool#_get_scorer().
  _syntax_error_response: _syntax_error_response().
  _is_init_file: _is_init_file().
  SafeToEditTool._on_project_root_changed: SafeToEditTool#_on_project_root_changed().
  SafeToEditTool.get_tool_schema: SafeToEditTool#get_tool_schema().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  logger: logger.
  SafeToEditTool.get_tool_definition: SafeToEditTool#get_tool_definition().
  SafeToEditTool.validate_arguments: SafeToEditTool#validate_arguments().
  SafeToEditTool.__init__: SafeToEditTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py)

## Classes
### `SafeToEditTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py:66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L66)
- doc: MCP Tool that assesses how safe it is to edit a specific file.
- signature: `class SafeToEditTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L143)
  - `get_tool_definition(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L94)
  - `get_tool_schema(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L128)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L132)
- protocol/private: `__init__`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L69), `_get_graph`[`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L79), `_get_scorer`[`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L87), `_graph`[`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L70), `_on_project_root_changed`[`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L74), `_scorer`[`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L71)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`DependencyGraph`](../../project_graph.md#DependencyGraph), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`HealthScorer`](../../health_scorer.md#HealthScorer), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`build_file_dependency_view`](utils/safe_to_edit_helpers.md#build_file_dependency_view), [`build_safe_to_edit_result`](utils/safe_to_edit_helpers.md#build_safe_to_edit_result), [`project_root`](utils/safe_to_edit_helpers.md#SafeToEditContext.project_root), [`resolved_path`](utils/safe_to_edit_helpers.md#SafeToEditContext.resolved_path), [`file_path`](utils/safe_to_edit_helpers.md#SafeToEditContext.file_path), [`SafeToEditContext`](utils/safe_to_edit_helpers.md#SafeToEditContext), [`_syntax_error_response`](safe_to_edit_tool.md#_syntax_error_response), [`scorer`](utils/safe_to_edit_helpers.md#SafeToEditContext.scorer), [`edit_type`](utils/safe_to_edit_helpers.md#SafeToEditContext.edit_type), [`TOOL_SCHEMA`](safe_to_edit_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`graph`](utils/safe_to_edit_helpers.md#SafeToEditContext.graph)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (8 test-only)

## Functions
- `_compute_risk(*args: Any, **kwargs: Any)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L283) — Compatibility wrapper for tests and internal imports.
- `_is_init_file(file_path: str)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L288) — Compatibility wrapper for tests and internal imports.
- `_syntax_error_response(resolved: str, file_path: str, edit_type: str)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L218) — M3 (round-26): short-circuit when tree-sitter detected syntax errors.

## Module values
- `TOOL_SCHEMA` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L32)
- `logger` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.py#L30)

