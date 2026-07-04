---
title: 'Module: tree_sitter_analyzer/mcp/tools/read_partial_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/read_partial_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.read_partial_helpers`/
symbols:
  build_agent_summary: build_agent_summary().
  build_batch_agent_summary: build_batch_agent_summary().
  validate_line_range: validate_line_range().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  build_agent_summary_for_result: build_agent_summary_for_result().
  prepare_partial_save_content: prepare_partial_save_content().
  format_partial_content: format_partial_content().
  apply_partial_file_output: apply_partial_file_output().
  build_read_response: build_read_response().
  count_file_lines: count_file_lines().
  format_partial_content_as_json_lines: format_partial_content_as_json_lines().
  build_validation_error: build_validation_error().
  _summary_risk: _summary_risk().
  _summary_verdict: _summary_verdict().
  _summary_next_step: _summary_next_step().
  _summary_suggested_tool: _summary_suggested_tool().
  _summary_stop_condition: _summary_stop_condition().
  _summary_line: _summary_line().
  _batch_summary_risk: _batch_summary_risk().
  _batch_next_step: _batch_next_step().
  _batch_stop_condition: _batch_stop_condition().
  _SECTION_ITEM_SCHEMA._SECTION_ITEM_SCHEMA: _SECTION_ITEM_SCHEMA._SECTION_ITEM_SCHEMA.
  _resolve_range_state: _resolve_range_state().
---
# Module: [`tree_sitter_analyzer/mcp/tools/read_partial_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py)

## Functions
- `_batch_next_step(risk: str, truncated: bool, error_count: int)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L453)
- `_batch_stop_condition(risk: str)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L463)
- `_batch_summary_risk(count_sections: int, truncated: bool, error_count: int)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L445)
- `_resolve_range_state(start_line: int, end_line: int | None, file_lines: int | None)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L160) — Classify the requested range against the file's true line count.
- `_summary_line(*, start_line: int, end_line: int | None, lines_extracted: int, content_length: int, file_lines: int | None, out_of_range: bool, partial_range: bool)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L417) — One-line human-readable summary for the agent.
- `_summary_next_step(risk: str, content_format: str, start_column: int | None, end_column: int | None, *, out_of_range: bool = False, partial_range: bool = False, start_line: int | None = None, end_line: int | None = None, file_lines: int | None = None)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L347)
- `_summary_risk(lines_extracted: int, content_length: int, *, out_of_range: bool = False)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L315)
- `_summary_stop_condition(risk: str, *, out_of_range: bool = False, partial_range: bool = False)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L407)
- `_summary_suggested_tool(risk: str, lines_extracted: int, *, out_of_range: bool = False)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L394)
- `_summary_verdict(out_of_range: bool, partial_range: bool)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L333)
- `apply_partial_file_output(*, result: dict[str, Any], file_path: str, content: str, content_format: str, output_format: str, output_file: str | None, file_output_manager: Any, logger: Any)` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L598) — Persist extracted content to ``output_file`` when requested.
- `build_agent_summary(*, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, content_length: int, lines_extracted: int, content_format: str, output_file: str | None = None, suppress_output: bool = False, file_lines: int | None = None, out_of_range: bool = False, partial_range: bool = False, clamped_to: list[int] | None = None)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L187) — Summarize a partial read for immediate agent decision-making.
- `build_agent_summary_for_result(result: dict[str, Any], content_format: str, output_file: str | None = None, suppress_output: bool = False)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L267) — Build an agent summary from the standard partial-read result envelope.
- `build_batch_agent_summary(*, count_files: int, count_sections: int, truncated: bool, error_count: int)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L293) — Summarize a batch partial read for immediate agent decision-making.
- `build_read_response(file_path: str, content: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, resolved_path: str, line_count: int, truncated: bool)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L78) — Build the standard response for a partial read result.
- `build_validation_error(field: str, message: str)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L134) — Build a standard error response for input validation failures.
- `count_file_lines(file_path: str)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L143) — Count total newline-delimited lines in ``file_path``.
- `format_partial_content(content: str, content_format: str, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, lines_extracted: int)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L476) — Format extracted content as JSON-lines dict or text header + body.
- `format_partial_content_as_json_lines(content: str, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, lines_extracted: int)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L531) — Format content as a JSON line array with range metadata.
- `prepare_partial_save_content(content_format: str, content: str, result: dict[str, Any], file_path: str, output_format: str)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L568) — Prepare extracted content for file output based on ``content_format``.
- `validate_line_range(start_line: Any, end_line: Any, start_column: Any, end_column: Any)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L108) — Validate line/column ranges. Returns error message or None.

## Module values
- `TOOL_SCHEMA` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L24)
- `_SECTION_ITEM_SCHEMA` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_helpers.py#L12)

