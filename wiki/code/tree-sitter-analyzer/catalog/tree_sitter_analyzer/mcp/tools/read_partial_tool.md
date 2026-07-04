---
title: 'Module: tree_sitter_analyzer/mcp/tools/read_partial_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/read_partial_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.read_partial_tool`/
symbols:
  ReadPartialTool: ReadPartialTool#
  ReadPartialTool.execute: ReadPartialTool#execute().
  ReadPartialTool.validate_arguments: ReadPartialTool#validate_arguments().
  ReadPartialTool._execute_batch: ReadPartialTool#_execute_batch().
  ReadPartialTool._read_and_format: ReadPartialTool#_read_and_format().
  ReadPartialTool.file_output_manager: ReadPartialTool#file_output_manager.
  ReadPartialTool._build_result: ReadPartialTool#_build_result().
  ReadPartialTool.get_tool_definition: ReadPartialTool#get_tool_definition().
  ReadPartialTool.get_tool_schema: ReadPartialTool#get_tool_schema().
  ReadPartialTool._validate_resolve: ReadPartialTool#_validate_resolve().
  ReadPartialTool._apply_file_output: ReadPartialTool#_apply_file_output().
  logger: logger.
  ReadPartialTool._read_file_partial: ReadPartialTool#_read_file_partial().
  read_partial_tool: read_partial_tool.
  _exc_dict: _exc_dict().
  _log_read_partial_error: _log_read_partial_error().
  _validate_end_line: _validate_end_line().
  _validate_column_fields: _validate_column_fields().
  ReadPartialTool._format_content: ReadPartialTool#_format_content().
  ReadPartialTool.__init__: ReadPartialTool#__init__().
  ReadPartialTool._format_as_json_lines: ReadPartialTool#_format_as_json_lines().
  ReadPartialTool._prepare_save_content: ReadPartialTool#_prepare_save_content().
  _validate_string_field: _validate_string_field().
  _validate_int_field: _validate_int_field().
  _check_col_value: _check_col_value().
  _count_lines: _count_lines().
  _range_dict: _range_dict().
  _set_clamped_to: _set_clamped_to().
  _check_requests_exclusivity: _check_requests_exclusivity().
  _validate_format: _validate_format().
  _validate_suppress_output: _validate_suppress_output().
  _require_fields: _require_fields().
  _read_failure_envelope: _read_failure_envelope().
  _compute_range_flags: _compute_range_flags().
  _TOOL_DESCRIPTION._TOOL_DESCRIPTION: _TOOL_DESCRIPTION._TOOL_DESCRIPTION.
---
# Module: [`tree_sitter_analyzer/mcp/tools/read_partial_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py)

## Classes
### `ReadPartialTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/read_partial_tool.py:242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L242) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Tool for reading partial content from code files.
- signature: `class ReadPartialTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L249) — Initialize with optional project root for path resolution.
  - `_apply_file_output(self, result: dict[str, Any], file_path: str, content: str, content_format: str, output_format: str, output_file: str | None)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L562) — Write extracted content to a file (delegates to module helper).
  - `_build_result(self, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, content: str, lines_extracted: int, content_format: str, suppress_output: bool, output_file: str | None, *, file_lines: int | None = None, out_of_range: bool = False, partial_range: bool = False, clamped_to: list | None = None)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L441) — Build the result dict with range metadata and optional formatted content.
  - `_execute_batch(self, arguments: dict[str, Any])` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L597) — Batch mode for extracting multiple ranges from multiple files. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `_format_as_json_lines(self, content: str, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, lines_extracted: int)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L541) — Format content as a JSON line array with metadata (delegates).
  - `_format_content(self, content: str, content_format: str, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, lines_extracted: int)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L513) — Format extracted content as json or text with metadata header.
  - `_prepare_save_content(self, content_format: str, content: str, result: dict[str, Any], file_path: str, output_format: str)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L583) — Prepare content for saving to file (delegates to module helper).
  - `_read_and_format(self, file_path: str, resolved_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, content_format: str, output_format: str, output_file: str | None, suppress_output: bool)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L311) — Read partial content and format the response. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `_read_file_partial(self, file_path: str, start_line: int, end_line: int | None = None, start_column: int | None = None, end_column: int | None = None)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L604) — Delegate to file_handler for the actual partial read.
  - `_validate_resolve(self, file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L386) — Validate and resolve file path and range parameters.
  - `execute(self, arguments: dict[str, Any])` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L261) — Execute single or batch partial read based on arguments. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `get_tool_definition(self)` — [`L646`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L646) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L256) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L620`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L620) — Validate tool arguments: batch vs single mode, types, ranges. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `file_output_manager` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L252)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`FileOutputManager`](../utils/file_output_manager.md#FileOutputManager), [`read_file_partial`](../../file_handler.md#read_file_partial), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`execute_batch`](batch_executor.md#execute_batch), [`TOOL_SCHEMA`](read_partial_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`logger`](read_partial_tool.md#logger), [`build_agent_summary_for_result`](read_partial_helpers.md#build_agent_summary_for_result), [`prepare_partial_save_content`](read_partial_helpers.md#prepare_partial_save_content), [`_exc_dict`](read_partial_tool.md#_exc_dict), [`apply_partial_file_output`](read_partial_helpers.md#apply_partial_file_output), [`format_partial_content`](read_partial_helpers.md#format_partial_content), [`count_file_lines`](read_partial_helpers.md#count_file_lines), [`_log_read_partial_error`](read_partial_tool.md#_log_read_partial_error), [`_validate_column_fields`](read_partial_tool.md#_validate_column_fields), [`_validate_end_line`](read_partial_tool.md#_validate_end_line), [`format_partial_content_as_json_lines`](read_partial_helpers.md#format_partial_content_as_json_lines), [`_validate_int_field`](read_partial_tool.md#_validate_int_field), [`_validate_string_field`](read_partial_tool.md#_validate_string_field), [`_TOOL_DESCRIPTION`](read_partial_tool.md#_TOOL_DESCRIPTION._TOOL_DESCRIPTION), [`_check_requests_exclusivity`](read_partial_tool.md#_check_requests_exclusivity), [`_compute_range_flags`](read_partial_tool.md#_compute_range_flags), [`_count_lines`](read_partial_tool.md#_count_lines), [`_range_dict`](read_partial_tool.md#_range_dict), [`_read_failure_envelope`](read_partial_tool.md#_read_failure_envelope), [`_require_fields`](read_partial_tool.md#_require_fields), [`_set_clamped_to`](read_partial_tool.md#_set_clamped_to), [`_validate_format`](read_partial_tool.md#_validate_format), [`_validate_suppress_output`](read_partial_tool.md#_validate_suppress_output)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_structure_facade`](structure_facade.md#build_structure_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_handle_batch_partial_read`](../../cli/special_commands.md#_handle_batch_partial_read), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class), [`_read_route`](structure_facade.md#build_structure_facade._read_route), [`read_partial_tool`](read_partial_tool.md#read_partial_tool)  (162 test-only)

## Functions
- `_check_col_value(col_value: Any, col_field: str)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L63) — Raise ValueError if *col_value* is not a valid column index.
- `_check_requests_exclusivity(arguments: dict[str, Any], single_keys: list[str])` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L110) — Raise if batch ``requests`` and single-read keys are mixed.
- `_compute_range_flags(content: str, file_lines: int | None, start_line: int, end_line: int | None)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L209) — K8: classify the range as ``out_of_range`` / ``partial_range``.
- `_count_lines(text: str)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L84) — Count lines in *text*; returns 0 for falsy input.
- `_exc_dict(exc: Exception, project_root: str | None, file_path: str)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L73) — Build a canonical error envelope for an unexpected exception.
- `_log_read_partial_error(file_path: str, exc: Exception)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L123) — Emit an error-level log for an unexpected read failure.
- `_range_dict(start_line: int, end_line: int | None, start_column: int | None, end_column: int | None)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L89) — Build the nested ``range`` sub-dict for the response envelope.
- `_read_failure_envelope(file_path: str)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L196) — Build the canonical error envelope when ``file_handler`` returned None.
- `_require_fields(arguments: dict[str, Any], fields: list[str])` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L165)
- `_set_clamped_to(result: dict[str, Any], clamped_to: list | None)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L104) — Write ``clamped_to`` into *result* only when it is not None.
- `_validate_column_fields(arguments: dict[str, Any])` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L158) — Validate start_column and end_column fields.
- `_validate_end_line(arguments: dict[str, Any])` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L128) — Validate ``end_line`` when present: type + range check.
- `_validate_format(arguments: dict[str, Any])` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L139) — Validate the ``format`` field when present.
- `_validate_int_field(arguments: dict[str, Any], field: str, min_val: int = 0)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L183)
- `_validate_string_field(arguments: dict[str, Any], field: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L172)
- `_validate_suppress_output(arguments: dict[str, Any])` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L150) — Validate ``suppress_output`` is a bool when present.

## Module values
- `_TOOL_DESCRIPTION` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L33)
- `logger` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L29)
- `read_partial_tool` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/read_partial_tool.py#L662)

