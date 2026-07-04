---
title: 'Module: tests/unit/core/test_suppress_output_feature.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_suppress_output_feature.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_suppress_output_feature`/
symbols:
  TestSuppressOutputFeature.test_suppress_output_true_with_output_file_excludes_table_output: TestSuppressOutputFeature#test_suppress_output_true_with_output_file_excludes_table_output().
  TestSuppressOutputFeature.test_suppress_output_false_with_output_file_includes_table_output: TestSuppressOutputFeature#test_suppress_output_false_with_output_file_includes_table_output().
  TestSuppressOutputFeature.test_suppress_output_false_includes_table_output: TestSuppressOutputFeature#test_suppress_output_false_includes_table_output().
  TestSuppressOutputFeature.test_suppress_output_true_without_output_file_includes_table_output: TestSuppressOutputFeature#test_suppress_output_true_without_output_file_includes_table_output().
  TestMCPServerSuppressOutputIntegration.test_mcp_server_schema_includes_suppress_output: TestMCPServerSuppressOutputIntegration#test_mcp_server_schema_includes_suppress_output().
  _setup_analysis_mocks: _setup_analysis_mocks().
  TestSuppressOutputFeature.table_format_tool: TestSuppressOutputFeature#table_format_tool().
  TestMCPServerSuppressOutputIntegration.test_mcp_server_passes_suppress_output_parameter: TestMCPServerSuppressOutputIntegration#test_mcp_server_passes_suppress_output_parameter().
  _setup_file_manager_mock: _setup_file_manager_mock().
  TestSuppressOutputFeature: TestSuppressOutputFeature#
  TestSuppressOutputFeature.temp_java_file: TestSuppressOutputFeature#temp_java_file().
  TestSuppressOutputFeature.test_schema_includes_suppress_output: TestSuppressOutputFeature#test_schema_includes_suppress_output().
  TestSuppressOutputFeature.test_validate_arguments_with_suppress_output: TestSuppressOutputFeature#test_validate_arguments_with_suppress_output().
  TestSuppressOutputFeature.test_backward_compatibility_default_behavior: TestSuppressOutputFeature#test_backward_compatibility_default_behavior().
  TestMCPServerSuppressOutputIntegration: TestMCPServerSuppressOutputIntegration#
---
# Module: [`tests/unit/core/test_suppress_output_feature.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py)

## Classes
### `TestMCPServerSuppressOutputIntegration`
- def: [`tests/unit/core/test_suppress_output_feature.py:270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L270)
- doc: Test suppress_output integration with MCP server.
- signature: `class TestMCPServerSuppressOutputIntegration:`
- members:
  - `test_mcp_server_passes_suppress_output_parameter(self, mock_logger, mock_engine)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L297) — Test that MCP server correctly passes suppress_output parameter to tool.
  - `test_mcp_server_schema_includes_suppress_output(self, mock_logger, mock_engine)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L276) — Test that MCP server schema includes suppress_output parameter.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server)

### `TestSuppressOutputFeature`
- def: [`tests/unit/core/test_suppress_output_feature.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L46)
- doc: Test suppress_output functionality in TableFormatTool.
- signature: `class TestSuppressOutputFeature:`
- members:
  - `table_format_tool(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L89) — Create a TableFormatTool instance for testing.
  - `temp_java_file(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L50) — Create a temporary Java file for testing.
  - `test_backward_compatibility_default_behavior(self, table_format_tool)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L257) — Test that default behavior (no suppress_output) maintains backward compatibility.
  - `test_schema_includes_suppress_output(self, table_format_tool)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L97) — Test that the tool schema includes suppress_output parameter.
  - `test_suppress_output_false_includes_table_output(self, mock_detect_lang, mock_engine, temp_java_file)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L133) — Test that suppress_output=False includes table_output in response.
  - `test_suppress_output_false_with_output_file_includes_table_output(self, mock_get_managed_instance, mock_detect_lang, mock_engine, temp_java_file)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L229) — Test that suppress_output=False with output_file still includes table_output.
  - `test_suppress_output_true_with_output_file_excludes_table_output(self, mock_get_managed_instance, mock_detect_lang, mock_engine, temp_java_file)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L191) — Test that suppress_output=True with output_file excludes table_output from response.
  - `test_suppress_output_true_without_output_file_includes_table_output(self, mock_detect_lang, mock_engine, temp_java_file)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L160) — Test that suppress_output=True without output_file still includes table_output.
  - `test_validate_arguments_with_suppress_output(self, table_format_tool)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L111) — Test argument validation with suppress_output parameter.
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)  (2 test-only)

## Functions
- `_setup_analysis_mocks(mock_detect_lang: Mock, mock_engine: Mock, file_path: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L20) — Configure the two standard analysis mocks; returns mock_analysis_result.
- `_setup_file_manager_mock(mock_get_managed_instance: Mock)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_suppress_output_feature.py#L38) — Configure FileOutputManager mock; returns mock_file_manager_instance.

