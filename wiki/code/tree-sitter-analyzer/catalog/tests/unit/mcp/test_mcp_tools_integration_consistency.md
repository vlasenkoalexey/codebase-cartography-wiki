---
title: 'Module: tests/unit/mcp/test_mcp_tools_integration_consistency.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_tools_integration_consistency.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_tools_integration_consistency`/
symbols:
  all_tools: all_tools().
  TestMCPConsistencyIntegration.test_concurrent_file_output: TestMCPConsistencyIntegration#test_concurrent_file_output().
  TestMCPConsistencyIntegration.test_error_handling_consistency: TestMCPConsistencyIntegration#test_error_handling_consistency().
  TestMCPConsistencyIntegration.read_task: TestMCPConsistencyIntegration#read_task().
  TestMCPConsistencyIntegration.search_task: TestMCPConsistencyIntegration#search_task().
  TestMCPConsistencyIntegration.query_task: TestMCPConsistencyIntegration#query_task().
  mock_external_commands: mock_external_commands().
  comprehensive_project: comprehensive_project().
  TestMCPConsistencyIntegration: TestMCPConsistencyIntegration#
  TestMCPConsistencyIntegration.test_cross_tool_file_output_consistency: TestMCPConsistencyIntegration#test_cross_tool_file_output_consistency().
  TestMCPConsistencyIntegration.test_file_output_path_consistency: TestMCPConsistencyIntegration#test_file_output_path_consistency().
  TestMCPConsistencyIntegration.test_tool_schema_consistency: TestMCPConsistencyIntegration#test_tool_schema_consistency().
  TestMCPConsistencyIntegration.test_performance_with_file_output: TestMCPConsistencyIntegration#test_performance_with_file_output().
---
# Module: [`tests/unit/mcp/test_mcp_tools_integration_consistency.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py)

## Classes
### `TestMCPConsistencyIntegration`
- def: [`tests/unit/mcp/test_mcp_tools_integration_consistency.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L188)
- signature: `class TestMCPConsistencyIntegration:`
- members:
  - `query_task()` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L533)
  - `read_task()` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L503)
  - `search_task()` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L514)
  - `test_concurrent_file_output(self, all_tools, comprehensive_project)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L500)
  - `test_cross_tool_file_output_consistency(self, all_tools, comprehensive_project)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L191)
  - `test_error_handling_consistency(self, all_tools, comprehensive_project)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L367)
  - `test_file_output_path_consistency(self, all_tools, comprehensive_project)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L285)
  - `test_performance_with_file_output(self, all_tools, comprehensive_project)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L473)
  - `test_tool_schema_consistency(self, all_tools)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L455)
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

## Functions
- `all_tools(comprehensive_project)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L178)
- `comprehensive_project()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L33)
- `mock_external_commands(monkeypatch)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_integration_consistency.py#L25)

