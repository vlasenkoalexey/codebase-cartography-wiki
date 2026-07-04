---
title: 'Module: tests/unit/core/test_query_tool_file_output.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_tool_file_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_tool_file_output`/TestQueryToolFileOutput#
symbols:
  TestQueryToolFileOutput.create_mock_query_results: create_mock_query_results().
  TestQueryToolFileOutput.query_tool: query_tool().
  TestQueryToolFileOutput.test_basic_file_output_json_format: test_basic_file_output_json_format().
  TestQueryToolFileOutput.test_summary_format_output: test_summary_format_output().
  TestQueryToolFileOutput.test_suppress_output_functionality: test_suppress_output_functionality().
  TestQueryToolFileOutput.test_custom_query_string: test_custom_query_string().
  TestQueryToolFileOutput.test_automatic_base_name_generation: test_automatic_base_name_generation().
  TestQueryToolFileOutput: ''
  TestQueryToolFileOutput.temp_project_dir: temp_project_dir().
  TestQueryToolFileOutput.test_no_results_found: test_no_results_found().
---
# Module: [`tests/unit/core/test_query_tool_file_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py)

## Classes
### `TestQueryToolFileOutput`
- def: [`tests/unit/core/test_query_tool_file_output.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L19)
- doc: Test file output functionality for QueryTool
- signature: `class TestQueryToolFileOutput:`
- members:
  - `create_mock_query_results(self, query_type="functions")` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L158) — Create mock query results for different query types
  - `query_tool(self, temp_project_dir)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L154) — Create QueryTool instance
  - `temp_project_dir(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L23) — Create a temporary project directory with test files
  - `test_automatic_base_name_generation(self, query_tool, temp_project_dir)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L392) — Test automatic base name generation
  - `test_basic_file_output_json_format(self, query_tool, temp_project_dir)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L215) — Test basic file output with JSON format
  - `test_custom_query_string(self, query_tool, temp_project_dir)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L345) — Test custom query string with file output
  - `test_no_results_found(self, query_tool, temp_project_dir)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L368) — Test behavior when no results are found
  - `test_summary_format_output(self, query_tool, temp_project_dir)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L261) — Test file output with summary format
  - `test_suppress_output_functionality(self, query_tool, temp_project_dir)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output.py#L303) — Test suppress_output functionality
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

