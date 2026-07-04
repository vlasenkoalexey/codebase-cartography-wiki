---
title: 'Module: tree_sitter_analyzer/mcp/tools/constraint_check_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/constraint_check_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.constraint_check_tool`/
symbols:
  ConstraintCheckTool._run_and_persist: ConstraintCheckTool#_run_and_persist().
  ConstraintCheckTool.execute: ConstraintCheckTool#execute().
  ConstraintCheckTool: ConstraintCheckTool#
  ConstraintCheckTool._read_filtered_violations: ConstraintCheckTool#_read_filtered_violations().
  ConstraintCheckTool._compute_verdict: ConstraintCheckTool#_compute_verdict().
  _SEVERITY_ORDER._SEVERITY_ORDER: _SEVERITY_ORDER._SEVERITY_ORDER.
  ConstraintCheckTool.get_tool_schema: ConstraintCheckTool#get_tool_schema().
  ConstraintCheckTool.validate_arguments: ConstraintCheckTool#validate_arguments().
  ConstraintCheckTool.get_tool_definition: ConstraintCheckTool#get_tool_definition().
  ConstraintCheckTool._violations_ddl: ConstraintCheckTool#_violations_ddl().
  logger: logger.
  ConstraintCheckTool._count_edges: ConstraintCheckTool#_count_edges().
  _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES: _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES.
  _WARNING_SEVERITIES._WARNING_SEVERITIES: _WARNING_SEVERITIES._WARNING_SEVERITIES.
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/constraint_check_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py)

## Classes
### `ConstraintCheckTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/constraint_check_tool.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L76)
- doc: MCP tool `check_constraints` — architectural rule evaluator.
- signature: `class ConstraintCheckTool(BaseMCPTool):`
- members:
  - `_compute_verdict(rows: list[dict[str, Any]])` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L325) — Map (filtered) violations to the canonical verdict.
  - `_count_edges(conn: sqlite3.Connection)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L253) — Return the CALLS row count of the unified ``edges`` table, or 0.
  - `_read_filtered_violations(self, db_path: Path, *, path_filter: str, min_severity_rank: int)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L265) — Read violations from the table with severity + path filters applied.
  - `_run_and_persist(self, db_path: Path, constraints: list[Any])` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L187) — Run the evaluator and write-through into ``ast_constraint_violations``.
  - `_violations_ddl()` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L336) — Self-healing DDL — keeps the tool usable even if the global
  - `execute(self, arguments: dict[str, Any])` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L109)
  - `get_tool_definition(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L79)
  - `get_tool_schema(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L97)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L100)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`load_constraints`](../../constraints/parser.md#load_constraints), [`evaluate`](../../constraints/evaluator.md#evaluate), [`ConstraintParseError`](../../constraints/parser.md#ConstraintParseError), [`_compile_glob`](../../constraints/parser.md#_compile_glob), [`Violation`](../../constraints/schema.md#Violation), [`caller_file`](../../constraints/schema.md#Violation.caller_file), [`rule_id`](../../constraints/schema.md#Violation.rule_id), [`callee_file`](../../constraints/schema.md#Violation.callee_file), [`caller_line`](../../constraints/schema.md#Violation.caller_line), [`callee_name`](../../constraints/schema.md#Violation.callee_name), [`_SEVERITY_ORDER`](constraint_check_tool.md#_SEVERITY_ORDER._SEVERITY_ORDER), [`caller_name`](../../constraints/schema.md#Violation.caller_name), [`severity`](../../constraints/schema.md#Violation.severity), [`detected_at`](../../constraints/schema.md#Violation.detected_at), [`TOOL_SCHEMA`](constraint_check_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_BLOCKING_SEVERITIES`](constraint_check_tool.md#_BLOCKING_SEVERITIES._BLOCKING_SEVERITIES), [`_WARNING_SEVERITIES`](constraint_check_tool.md#_WARNING_SEVERITIES._WARNING_SEVERITIES), [`logger`](constraint_check_tool.md#logger)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_edit_facade`](edit_facade.md#build_edit_facade), [`_run_tool`](../../cli/commands/constraint_check_command.md#_run_tool)  (6 test-only)

## Module values
- `TOOL_SCHEMA` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L42)
- `_BLOCKING_SEVERITIES` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L39)
- `_SEVERITY_ORDER` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L73)
- `_WARNING_SEVERITIES` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L40)
- `logger` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/constraint_check_tool.py#L34)

