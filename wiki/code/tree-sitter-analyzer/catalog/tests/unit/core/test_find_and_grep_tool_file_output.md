---
title: 'Module: tests/unit/core/test_find_and_grep_tool_file_output.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_find_and_grep_tool_file_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_find_and_grep_tool_file_output`/TestFindAndGrepToolFileOutput#
symbols:
  TestFindAndGrepToolFileOutput.find_and_grep_tool: find_and_grep_tool().
  TestFindAndGrepToolFileOutput: ''
  TestFindAndGrepToolFileOutput.temp_project_dir: temp_project_dir().
  TestFindAndGrepToolFileOutput.test_basic_file_output: test_basic_file_output().
  TestFindAndGrepToolFileOutput.test_suppress_output_functionality: test_suppress_output_functionality().
  TestFindAndGrepToolFileOutput.test_group_by_file_with_output: test_group_by_file_with_output().
  TestFindAndGrepToolFileOutput.test_summary_only_with_output: test_summary_only_with_output().
  TestFindAndGrepToolFileOutput.test_count_only_mode: test_count_only_mode().
  TestFindAndGrepToolFileOutput.test_total_only_mode: test_total_only_mode().
  TestFindAndGrepToolFileOutput.test_file_filtering_options: test_file_filtering_options().
  TestFindAndGrepToolFileOutput.test_error_handling_with_output: test_error_handling_with_output().
  TestFindAndGrepToolFileOutput.test_fd_failure_handling: test_fd_failure_handling().
  TestFindAndGrepToolFileOutput.test_rg_failure_handling: test_rg_failure_handling().
  TestFindAndGrepToolFileOutput.test_no_files_found: test_no_files_found().
  TestFindAndGrepToolFileOutput.test_sorting_options: test_sorting_options().
  TestFindAndGrepToolFileOutput.test_tool_definition_includes_new_parameters: test_tool_definition_includes_new_parameters().
  TestFindAndGrepToolFileOutput.test_complex_workflow_with_output: test_complex_workflow_with_output().
---
# Module: [`tests/unit/core/test_find_and_grep_tool_file_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py)

## Classes
### `TestFindAndGrepToolFileOutput`
- def: [`tests/unit/core/test_find_and_grep_tool_file_output.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L19)
- doc: Test file output functionality for FindAndGrepTool
- signature: `class TestFindAndGrepToolFileOutput:`
- members:
  - `find_and_grep_tool(self, temp_project_dir)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L77) — Create FindAndGrepTool instance
  - `temp_project_dir(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L23) — Create a temporary project directory with test files
  - `test_basic_file_output(self, find_and_grep_tool, temp_project_dir)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L82) — Test basic file output functionality
  - `test_complex_workflow_with_output(self, find_and_grep_tool, temp_project_dir)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L594) — Test complex workflow combining multiple features with file output
  - `test_count_only_mode(self, find_and_grep_tool, temp_project_dir)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L297) — Test count_only_matches mode
  - `test_error_handling_with_output(self, find_and_grep_tool, temp_project_dir)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L406) — Test error handling when file output fails
  - `test_fd_failure_handling(self, find_and_grep_tool, temp_project_dir)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L448) — Test handling of fd command failure
  - `test_file_filtering_options(self, find_and_grep_tool, temp_project_dir)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L369) — Test various file filtering options with output
  - `test_group_by_file_with_output(self, find_and_grep_tool, temp_project_dir)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L198) — Test group_by_file mode with file output
  - `test_no_files_found(self, find_and_grep_tool, temp_project_dir)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L508) — Test behavior when no files are found by fd
  - `test_rg_failure_handling(self, find_and_grep_tool, temp_project_dir)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L476) — Test handling of ripgrep command failure
  - `test_sorting_options(self, find_and_grep_tool, temp_project_dir)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L539) — Test file sorting options
  - `test_summary_only_with_output(self, find_and_grep_tool, temp_project_dir)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L250) — Test summary_only mode with file output
  - `test_suppress_output_functionality(self, find_and_grep_tool, temp_project_dir)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L147) — Test suppress_output functionality
  - `test_tool_definition_includes_new_parameters(self, find_and_grep_tool)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L571) — Test that tool definition includes new parameters
  - `test_total_only_mode(self, find_and_grep_tool, temp_project_dir)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_find_and_grep_tool_file_output.py#L335) — Test total_only mode
- uses (calls/refs, reference-scoped): [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool)

