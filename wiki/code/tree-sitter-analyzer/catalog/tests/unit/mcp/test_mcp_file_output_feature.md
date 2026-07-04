---
title: 'Module: tests/unit/mcp/test_mcp_file_output_feature.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_file_output_feature.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_file_output_feature`/
symbols:
  TestFileOutputFeature.test_tool_schema_includes_new_parameters: TestFileOutputFeature#test_tool_schema_includes_new_parameters().
  TestFileOutputFeature.test_cross_tool_file_output_consistency: TestFileOutputFeature#test_cross_tool_file_output_consistency().
  TestFileOutputManagerIntegration.test_file_output_manager_initialization: TestFileOutputManagerIntegration#test_file_output_manager_initialization().
  TestFileOutputManagerIntegration.test_file_output_path_resolution: TestFileOutputManagerIntegration#test_file_output_path_resolution().
  TestFileOutputFeature.search_content_tool: TestFileOutputFeature#search_content_tool().
  TestFileOutputFeature.find_and_grep_tool: TestFileOutputFeature#find_and_grep_tool().
  TestFileOutputFeature.read_partial_tool: TestFileOutputFeature#read_partial_tool().
  TestFileOutputFeature.query_tool: TestFileOutputFeature#query_tool().
  mock_external_commands: mock_external_commands().
  TestFileOutputFeature: TestFileOutputFeature#
  TestFileOutputFeature.temp_project_dir: TestFileOutputFeature#temp_project_dir().
  TestFileOutputFeature.test_search_content_output_file_basic: TestFileOutputFeature#test_search_content_output_file_basic().
  TestFileOutputFeature.test_search_content_suppress_output: TestFileOutputFeature#test_search_content_suppress_output().
  TestFileOutputFeature.test_search_content_summary_only_with_output_file: TestFileOutputFeature#test_search_content_summary_only_with_output_file().
  TestFileOutputFeature.test_find_and_grep_output_file: TestFileOutputFeature#test_find_and_grep_output_file().
  TestFileOutputFeature.test_find_and_grep_suppress_output: TestFileOutputFeature#test_find_and_grep_suppress_output().
  TestFileOutputFeature.test_read_partial_output_file_formats: TestFileOutputFeature#test_read_partial_output_file_formats().
  TestFileOutputFeature.test_read_partial_suppress_output: TestFileOutputFeature#test_read_partial_suppress_output().
  TestFileOutputFeature.test_query_tool_output_file: TestFileOutputFeature#test_query_tool_output_file().
  TestFileOutputFeature.test_query_tool_suppress_output: TestFileOutputFeature#test_query_tool_suppress_output().
  TestFileOutputFeature.test_file_output_error_handling: TestFileOutputFeature#test_file_output_error_handling().
  TestFileOutputManagerIntegration: TestFileOutputManagerIntegration#
  TestFileOutputManagerIntegration.temp_project_dir: TestFileOutputManagerIntegration#temp_project_dir().
---
# Module: [`tests/unit/mcp/test_mcp_file_output_feature.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py)

## Classes
### `TestFileOutputFeature`
- def: [`tests/unit/mcp/test_mcp_file_output_feature.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L31)
- doc: Test file output functionality across MCP tools
- signature: `class TestFileOutputFeature:`
- members:
  - `find_and_grep_tool(self, temp_project_dir)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L82) — Create FindAndGrepTool instance
  - `query_tool(self, temp_project_dir)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L92) — Create QueryTool instance
  - `read_partial_tool(self, temp_project_dir)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L87) — Create ReadPartialTool instance
  - `search_content_tool(self, temp_project_dir)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L77) — Create SearchContentTool instance
  - `temp_project_dir(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L35) — Create a temporary project directory with test files
  - `test_cross_tool_file_output_consistency(self, temp_project_dir)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L467) — Test that file output behavior is consistent across tools
  - `test_file_output_error_handling(self, search_content_tool, temp_project_dir)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L416) — Test error handling for file output
  - `test_find_and_grep_output_file(self, find_and_grep_tool, temp_project_dir)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L195) — Test file output functionality for find_and_grep
  - `test_find_and_grep_suppress_output(self, find_and_grep_tool, temp_project_dir)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L234) — Test suppress_output functionality for find_and_grep
  - `test_query_tool_output_file(self, query_tool, temp_project_dir)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L340) — Test file output functionality for query_tool
  - `test_query_tool_suppress_output(self, query_tool, temp_project_dir)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L383) — Test suppress_output functionality for query_tool
  - `test_read_partial_output_file_formats(self, read_partial_tool, temp_project_dir)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L271) — Test different output formats for read_partial
  - `test_read_partial_suppress_output(self, read_partial_tool, temp_project_dir)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L316) — Test suppress_output functionality for read_partial
  - `test_search_content_output_file_basic(self, search_content_tool, temp_project_dir)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L97) — Test basic file output functionality for search_content
  - `test_search_content_summary_only_with_output_file(self, search_content_tool, temp_project_dir)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L164) — Test summary_only mode with file output (only one format parameter allowed)
  - `test_search_content_suppress_output(self, search_content_tool, temp_project_dir)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L136) — Test suppress_output functionality for search_content
  - `test_tool_schema_includes_new_parameters(self)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L454) — File-output capable tools expose output_file/suppress_output.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

### `TestFileOutputManagerIntegration`
- def: [`tests/unit/mcp/test_mcp_file_output_feature.py:569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L569)
- doc: Test FileOutputManager integration with MCP tools
- signature: `class TestFileOutputManagerIntegration:`
- members:
  - `temp_project_dir(self)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L573) — Create a temporary project directory
  - `test_file_output_manager_initialization(self, temp_project_dir)` — [`L578`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L578) — Test that FileOutputManager is properly initialized in tools
  - `test_file_output_path_resolution(self, temp_project_dir)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L597) — Test that file output paths are properly resolved
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

## Functions
- `mock_external_commands(monkeypatch)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_output_feature.py#L23) — Auto-mock external command availability checks for all tests in this module.

