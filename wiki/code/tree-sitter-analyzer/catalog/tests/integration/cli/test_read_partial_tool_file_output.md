---
title: 'Module: tests/integration/cli/test_read_partial_tool_file_output.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_read_partial_tool_file_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_read_partial_tool_file_output`/TestReadPartialToolFileOutput#
symbols:
  TestReadPartialToolFileOutput.read_partial_tool: read_partial_tool().
  TestReadPartialToolFileOutput: ''
  TestReadPartialToolFileOutput.temp_project_dir: temp_project_dir().
  TestReadPartialToolFileOutput.test_basic_file_output_text_format: test_basic_file_output_text_format().
  TestReadPartialToolFileOutput.test_json_format_output: test_json_format_output().
  TestReadPartialToolFileOutput.test_raw_format_output: test_raw_format_output().
  TestReadPartialToolFileOutput.test_suppress_output_functionality: test_suppress_output_functionality().
  TestReadPartialToolFileOutput.test_suppress_output_without_file: test_suppress_output_without_file().
  TestReadPartialToolFileOutput.test_column_range_extraction: test_column_range_extraction().
  TestReadPartialToolFileOutput.test_single_line_extraction: test_single_line_extraction().
  TestReadPartialToolFileOutput.test_large_range_extraction: test_large_range_extraction().
  TestReadPartialToolFileOutput.test_java_file_extraction: test_java_file_extraction().
  TestReadPartialToolFileOutput.test_error_handling_file_save_failure: test_error_handling_file_save_failure().
  TestReadPartialToolFileOutput.test_invalid_line_ranges: test_invalid_line_ranges().
  TestReadPartialToolFileOutput.test_invalid_column_ranges: test_invalid_column_ranges().
  TestReadPartialToolFileOutput.test_nonexistent_file: test_nonexistent_file().
  TestReadPartialToolFileOutput.test_tool_definition_includes_new_parameters: test_tool_definition_includes_new_parameters().
  TestReadPartialToolFileOutput.test_automatic_base_name_generation: test_automatic_base_name_generation().
  TestReadPartialToolFileOutput.test_format_parameter_validation: test_format_parameter_validation().
  TestReadPartialToolFileOutput.test_comprehensive_workflow: test_comprehensive_workflow().
---
# Module: [`tests/integration/cli/test_read_partial_tool_file_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py)

## Classes
### `TestReadPartialToolFileOutput`
- def: [`tests/integration/cli/test_read_partial_tool_file_output.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L18)
- doc: Test file output functionality for ReadPartialTool
- signature: `class TestReadPartialToolFileOutput:`
- members:
  - `read_partial_tool(self, temp_project_dir)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L116) — Create ReadPartialTool instance
  - `temp_project_dir(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L22) — Create a temporary project directory with test files
  - `test_automatic_base_name_generation(self, read_partial_tool, temp_project_dir)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L515) — Test automatic base name generation when output_file is empty
  - `test_basic_file_output_text_format(self, read_partial_tool, temp_project_dir)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L121) — Test basic file output with text format
  - `test_column_range_extraction(self, read_partial_tool, temp_project_dir)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L295) — Test extraction with column ranges
  - `test_comprehensive_workflow(self, read_partial_tool, temp_project_dir)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L576) — Test comprehensive workflow with all features
  - `test_error_handling_file_save_failure(self, read_partial_tool, temp_project_dir)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L411) — Test error handling when file save fails
  - `test_format_parameter_validation(self, read_partial_tool, temp_project_dir)` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L544) — Test format parameter validation
  - `test_invalid_column_ranges(self, read_partial_tool, temp_project_dir)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L463) — Test handling of invalid column ranges
  - `test_invalid_line_ranges(self, read_partial_tool, temp_project_dir)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L444) — Test handling of invalid line ranges
  - `test_java_file_extraction(self, read_partial_tool, temp_project_dir)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L377) — Test extraction from Java file
  - `test_json_format_output(self, read_partial_tool, temp_project_dir)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L164) — Test file output with JSON format
  - `test_large_range_extraction(self, read_partial_tool, temp_project_dir)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L351) — Test extraction of a large range
  - `test_nonexistent_file(self, read_partial_tool, temp_project_dir)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L482) — Test handling of nonexistent file
  - `test_raw_format_output(self, read_partial_tool, temp_project_dir)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L201) — Test file output with raw format
  - `test_single_line_extraction(self, read_partial_tool, temp_project_dir)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L328) — Test extraction of a single line
  - `test_suppress_output_functionality(self, read_partial_tool, temp_project_dir)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L238) — Test suppress_output functionality
  - `test_suppress_output_without_file(self, read_partial_tool, temp_project_dir)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L271) — Test suppress_output without output_file (should include partial_content_result)
  - `test_tool_definition_includes_new_parameters(self, read_partial_tool)` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_file_output.py#L492) — Test that tool definition includes new parameters
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool)

