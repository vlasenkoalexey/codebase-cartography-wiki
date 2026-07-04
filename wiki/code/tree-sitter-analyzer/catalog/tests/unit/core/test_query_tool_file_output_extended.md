---
title: 'Module: tests/unit/core/test_query_tool_file_output_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_tool_file_output_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_tool_file_output_extended`/TestQueryToolFileOutputExtended#
symbols:
  TestQueryToolFileOutputExtended.create_mock_query_results: create_mock_query_results().
  TestQueryToolFileOutputExtended.query_tool: query_tool().
  TestQueryToolFileOutputExtended.test_error_handling_file_save_failure: test_error_handling_file_save_failure().
  TestQueryToolFileOutputExtended.test_language_auto_detection: test_language_auto_detection().
  TestQueryToolFileOutputExtended.test_comprehensive_workflow: test_comprehensive_workflow().
  TestQueryToolFileOutputExtended: ''
  TestQueryToolFileOutputExtended.temp_project_dir: temp_project_dir().
  TestQueryToolFileOutputExtended.test_java_file_query: test_java_file_query().
  TestQueryToolFileOutputExtended.test_javascript_file_query: test_javascript_file_query().
  TestQueryToolFileOutputExtended.test_query_execution_failure: test_query_execution_failure().
  TestQueryToolFileOutputExtended.test_invalid_file_path: test_invalid_file_path().
  TestQueryToolFileOutputExtended.test_missing_query_parameters: test_missing_query_parameters().
  TestQueryToolFileOutputExtended.test_both_query_parameters_provided: test_both_query_parameters_provided().
  TestQueryToolFileOutputExtended.test_tool_definition_includes_new_parameters: test_tool_definition_includes_new_parameters().
  TestQueryToolFileOutputExtended.test_filter_parameter: test_filter_parameter().
---
# Module: [`tests/unit/core/test_query_tool_file_output_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py)

## Classes
### `TestQueryToolFileOutputExtended`
- def: [`tests/unit/core/test_query_tool_file_output_extended.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L19)
- doc: Extended tests for file output functionality - multi-language, errors, integration
- signature: `class TestQueryToolFileOutputExtended:`
- members:
  - `create_mock_query_results(self, query_type="functions")` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L158) — Create mock query results for different query types
  - `query_tool(self, temp_project_dir)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L154) — Create QueryTool instance
  - `temp_project_dir(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L23) — Create a temporary project directory with test files
  - `test_both_query_parameters_provided(self, query_tool, temp_project_dir)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L404) — Test handling when both query_key and query_string are provided
  - `test_comprehensive_workflow(self, query_tool, temp_project_dir)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L526) — Test comprehensive workflow with all features
  - `test_error_handling_file_save_failure(self, query_tool, temp_project_dir)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L308) — Test error handling when file save fails
  - `test_filter_parameter(self, query_tool, temp_project_dir)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L489) — Test filter parameter functionality
  - `test_invalid_file_path(self, query_tool, temp_project_dir)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L361) — Test handling of invalid file path
  - `test_java_file_query(self, query_tool, temp_project_dir)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L219) — Test querying Java file
  - `test_javascript_file_query(self, query_tool, temp_project_dir)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L264) — Test querying JavaScript file
  - `test_language_auto_detection(self, query_tool, temp_project_dir)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L467) — Test automatic language detection
  - `test_missing_query_parameters(self, query_tool, temp_project_dir)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L381) — Test handling of missing query parameters
  - `test_query_execution_failure(self, query_tool, temp_project_dir)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L340) — Test handling of query execution failure
  - `test_tool_definition_includes_new_parameters(self, query_tool)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_tool_file_output_extended.py#L433) — Test that tool definition includes new parameters
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

