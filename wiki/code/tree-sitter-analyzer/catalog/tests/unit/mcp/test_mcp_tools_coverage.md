---
title: 'Module: tests/unit/mcp/test_mcp_tools_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_tools_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_tools_coverage`/Test
symbols:
  TestOutputManagerCoverage.test_init_default: OutputManagerCoverage#test_init_default().
  TestOutputManagerCoverage.test_init_with_toon_format: OutputManagerCoverage#test_init_with_toon_format().
  TestOutputManagerCoverage.test_unsupported_format_fallback: OutputManagerCoverage#test_unsupported_format_fallback().
  TestOutputManagerCoverage.test_init_with_json_output: OutputManagerCoverage#test_init_with_json_output().
  TestOutputManagerCoverage.test_info_quiet: OutputManagerCoverage#test_info_quiet().
  TestOutputManagerCoverage.test_info_not_quiet: OutputManagerCoverage#test_info_not_quiet().
  TestOutputManagerCoverage.test_data_json: OutputManagerCoverage#test_data_json().
  TestOutputManagerCoverage.test_data_toon: OutputManagerCoverage#test_data_toon().
  TestOutputManagerCoverage.test_data_string: OutputManagerCoverage#test_data_string().
  TestOutputManagerCoverage.test_format_override: OutputManagerCoverage#test_format_override().
  TestOutputManagerCoverage.test_error_output: OutputManagerCoverage#test_error_output().
  TestOutputManagerCoverage.test_warning_output: OutputManagerCoverage#test_warning_output().
  TestMCPUtilsInit.test_format_helper_import: MCPUtilsInit#test_format_helper_import().
  TestQueryToolCoverage.query_tool: QueryToolCoverage#query_tool().
  TestQueryToolCoverage.test_execute_no_query_params_error: QueryToolCoverage#test_execute_no_query_params_error().
  TestAnalyzeScaleToolCoverage.analyze_scale_tool: AnalyzeScaleToolCoverage#analyze_scale_tool().
  TestReadPartialToolCoverage.read_partial_tool: ReadPartialToolCoverage#read_partial_tool().
  TestAnalyzeCodeStructureToolCoverage.analyze_code_structure_tool: AnalyzeCodeStructureToolCoverage#analyze_code_structure_tool().
  TestMCPUtilsInit.test_file_output_manager_import: MCPUtilsInit#test_file_output_manager_import().
  TestMCPUtilsInit.test_error_handler_import: MCPUtilsInit#test_error_handler_import().
  TestQueryToolCoverage: QueryToolCoverage#
  TestQueryToolCoverage.temp_python_file: QueryToolCoverage#temp_python_file().
  TestQueryToolCoverage.test_get_tool_definition: QueryToolCoverage#test_get_tool_definition().
  TestQueryToolCoverage.test_get_available_queries: QueryToolCoverage#test_get_available_queries().
  TestQueryToolCoverage.test_execute_with_query_key: QueryToolCoverage#test_execute_with_query_key().
  TestQueryToolCoverage.test_execute_with_custom_query: QueryToolCoverage#test_execute_with_custom_query().
  TestQueryToolCoverage.test_execute_both_query_params_error: QueryToolCoverage#test_execute_both_query_params_error().
  TestQueryToolCoverage.test_execute_with_filter: QueryToolCoverage#test_execute_with_filter().
  TestQueryToolCoverage.test_execute_with_output_format_toon: QueryToolCoverage#test_execute_with_output_format_toon().
  TestQueryToolCoverage.test_execute_with_suppress_output: QueryToolCoverage#test_execute_with_suppress_output().
  TestQueryToolCoverage.test_execute_with_summary_format: QueryToolCoverage#test_execute_with_summary_format().
  TestQueryToolCoverage.test_execute_invalid_file: QueryToolCoverage#test_execute_invalid_file().
  TestQueryToolCoverage.test_validate_arguments_invalid_output_format: QueryToolCoverage#test_validate_arguments_invalid_output_format().
  TestQueryToolCoverage.test_validate_arguments_invalid_result_format: QueryToolCoverage#test_validate_arguments_invalid_result_format().
  TestAnalyzeScaleToolCoverage: AnalyzeScaleToolCoverage#
  TestAnalyzeScaleToolCoverage.temp_python_file: AnalyzeScaleToolCoverage#temp_python_file().
  TestAnalyzeScaleToolCoverage.test_execute_basic: AnalyzeScaleToolCoverage#test_execute_basic().
  TestAnalyzeScaleToolCoverage.test_execute_with_threshold: AnalyzeScaleToolCoverage#test_execute_with_threshold().
  TestAnalyzeScaleToolCoverage.test_execute_nonexistent_file: AnalyzeScaleToolCoverage#test_execute_nonexistent_file().
  TestAnalyzeScaleToolCoverage.test_execute_with_output_format_toon: AnalyzeScaleToolCoverage#test_execute_with_output_format_toon().
  TestReadPartialToolCoverage: ReadPartialToolCoverage#
  TestReadPartialToolCoverage.temp_python_file: ReadPartialToolCoverage#temp_python_file().
  TestReadPartialToolCoverage.test_execute_by_line_range: ReadPartialToolCoverage#test_execute_by_line_range().
  TestReadPartialToolCoverage.test_execute_by_element_name: ReadPartialToolCoverage#test_execute_by_element_name().
  TestReadPartialToolCoverage.test_execute_with_context: ReadPartialToolCoverage#test_execute_with_context().
  TestReadPartialToolCoverage.test_execute_nonexistent_file: ReadPartialToolCoverage#test_execute_nonexistent_file().
  TestAnalyzeCodeStructureToolCoverage: AnalyzeCodeStructureToolCoverage#
  TestAnalyzeCodeStructureToolCoverage.temp_python_file: AnalyzeCodeStructureToolCoverage#temp_python_file().
  TestAnalyzeCodeStructureToolCoverage.test_execute_full_format: AnalyzeCodeStructureToolCoverage#test_execute_full_format().
  TestAnalyzeCodeStructureToolCoverage.test_execute_compact_format: AnalyzeCodeStructureToolCoverage#test_execute_compact_format().
  TestAnalyzeCodeStructureToolCoverage.test_execute_csv_format: AnalyzeCodeStructureToolCoverage#test_execute_csv_format().
  TestAnalyzeCodeStructureToolCoverage.test_execute_toon_format: AnalyzeCodeStructureToolCoverage#test_execute_toon_format().
  TestAnalyzeCodeStructureToolCoverage.test_execute_nonexistent_file: AnalyzeCodeStructureToolCoverage#test_execute_nonexistent_file().
  TestOutputManagerCoverage: OutputManagerCoverage#
  TestMCPUtilsInit: MCPUtilsInit#
---
# Module: [`tests/unit/mcp/test_mcp_tools_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py)

## Classes
### `TestAnalyzeCodeStructureToolCoverage`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L380)
- doc: Test AnalyzeCodeStructureTool for coverage boost.
- signature: `class TestAnalyzeCodeStructureToolCoverage:`
- members:
  - `analyze_code_structure_tool(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L384) — Create AnalyzeCodeStructureTool instance.
  - `temp_python_file(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L393) — Create temporary Python file.
  - `test_execute_compact_format(self, analyze_code_structure_tool, temp_python_file)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L424) — Test execute with compact format.
  - `test_execute_csv_format(self, analyze_code_structure_tool, temp_python_file)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L437) — Test execute with CSV format.
  - `test_execute_full_format(self, analyze_code_structure_tool, temp_python_file)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L411) — Test execute with full format.
  - `test_execute_nonexistent_file(self, analyze_code_structure_tool)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L465) — Test execute with nonexistent file raises ValueError.
  - `test_execute_toon_format(self, analyze_code_structure_tool, temp_python_file)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L450) — Test execute with TOON format.
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool)

### `TestAnalyzeScaleToolCoverage`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L199)
- doc: Test AnalyzeScaleTool for coverage boost.
- signature: `class TestAnalyzeScaleToolCoverage:`
- members:
  - `analyze_scale_tool(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L203) — Create AnalyzeScaleTool instance.
  - `temp_python_file(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L210) — Create temporary Python file.
  - `test_execute_basic(self, analyze_scale_tool, temp_python_file)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L239) — Test basic execute.
  - `test_execute_nonexistent_file(self, analyze_scale_tool)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L262) — Test execute with nonexistent file raises ValueError.
  - `test_execute_with_output_format_toon(self, analyze_scale_tool, temp_python_file)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L272) — Test execute with TOON output format.
  - `test_execute_with_threshold(self, analyze_scale_tool, temp_python_file)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L249) — Test execute on a small file (F5: ``threshold`` was a typo'd
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool)

### `TestMCPUtilsInit`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L593)
- doc: Test mcp/utils/__init__.py coverage.
- signature: `class TestMCPUtilsInit:`
- members:
  - `test_error_handler_import(self)` — [`L612`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L612) — Test error_handler can be imported.
  - `test_file_output_manager_import(self)` — [`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L596) — Test FileOutputManager can be imported from submodule.
  - `test_format_helper_import(self)` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L602) — Test format_helper functions can be imported.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`format_for_file_output`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_for_file_output), [`format_output`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_output)

### `TestOutputManagerCoverage`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L475)
- doc: Test OutputManager for coverage boost.
- signature: `class TestOutputManagerCoverage:`
- members:
  - `test_data_json(self, capsys)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L523) — Test data output in JSON format.
  - `test_data_string(self, capsys)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L541) — Test data output with string data.
  - `test_data_toon(self, capsys)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L532) — Test data output in TOON format.
  - `test_error_output(self, capsys)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L559) — Test error output.
  - `test_format_override(self, capsys)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L550) — Test data with format_type override.
  - `test_info_not_quiet(self, capsys)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L511) — Test info message when not quiet — goes to stderr (Q2).
  - `test_info_quiet(self, capsys)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L502) — Test info message when quiet.
  - `test_init_default(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L478) — Test default initialization.
  - `test_init_with_json_output(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L486) — Test initialization with json_output flag.
  - `test_init_with_toon_format(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L494) — Test initialization with toon format.
  - `test_unsupported_format_fallback(self, capsys)` — [`L579`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L579) — Test fallback for unsupported format.
  - `test_warning_output(self, capsys)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L569) — Test warning output.
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.data), [`quiet`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.quiet), [`_formatter_registry`](../../../tree_sitter_analyzer/output_manager.md#OutputManager._formatter_registry), [`warning`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.warning), [`info`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.info), [`output_format`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_format), [`error`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.error)

### `TestQueryToolCoverage`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L15)
- doc: Test QueryTool for coverage boost.
- signature: `class TestQueryToolCoverage:`
- members:
  - `query_tool(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L19) — Create QueryTool instance.
  - `temp_python_file(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L26) — Create temporary Python file.
  - `test_execute_both_query_params_error(self, query_tool, temp_python_file)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L90) — Test error when both query_key and query_string provided.
  - `test_execute_invalid_file(self, query_tool)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L166) — Test execute with nonexistent file.
  - `test_execute_no_query_params_error(self, query_tool, temp_python_file)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L102) — Test error when no query parameters provided.
  - `test_execute_with_custom_query(self, query_tool, temp_python_file)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L79) — Test execute with custom query string.
  - `test_execute_with_filter(self, query_tool, temp_python_file)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L114) — Test execute with filter parameter.
  - `test_execute_with_output_format_toon(self, query_tool, temp_python_file)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L126) — Test execute with TOON output format.
  - `test_execute_with_query_key(self, query_tool, temp_python_file)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L68) — Test execute with query_key.
  - `test_execute_with_summary_format(self, query_tool, temp_python_file)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L154) — Test execute with summary result format.
  - `test_execute_with_suppress_output(self, query_tool, temp_python_file)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L142) — Test execute with suppress_output.
  - `test_get_available_queries(self, query_tool)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L62) — Test get_available_queries returns list.
  - `test_get_tool_definition(self, query_tool)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L51) — Test get_tool_definition returns valid schema.
  - `test_validate_arguments_invalid_output_format(self, query_tool)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L176) — Test validate_arguments with invalid output_format.
  - `test_validate_arguments_invalid_result_format(self, query_tool)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L187) — Test validate_arguments with invalid result_format.
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

### `TestReadPartialToolCoverage`
- def: [`tests/unit/mcp/test_mcp_tools_coverage.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L286)
- doc: Test ReadPartialTool for coverage boost.
- signature: `class TestReadPartialToolCoverage:`
- members:
  - `read_partial_tool(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L290) — Create ReadPartialTool instance.
  - `temp_python_file(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L297) — Create temporary Python file with multiple elements.
  - `test_execute_by_element_name(self, read_partial_tool, temp_python_file)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L341) — Test execute with element name requires start_line, so use line range.
  - `test_execute_by_line_range(self, read_partial_tool, temp_python_file)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L329) — Test execute with line range.
  - `test_execute_nonexistent_file(self, read_partial_tool)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L368) — Test execute with nonexistent file.
  - `test_execute_with_context(self, read_partial_tool, temp_python_file)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_coverage.py#L353) — Test execute with a line range. F5: ``context_lines`` was a
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool)

