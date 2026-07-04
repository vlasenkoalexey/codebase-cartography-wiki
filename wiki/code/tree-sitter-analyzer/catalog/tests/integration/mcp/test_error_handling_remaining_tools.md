---
title: 'Module: tests/integration/mcp/test_error_handling_remaining_tools.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_error_handling_remaining_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_error_handling_remaining_tools`/TestRemainingToolsErrorHandling#
symbols:
  TestRemainingToolsErrorHandling.test_comprehensive_error_scenarios: test_comprehensive_error_scenarios().
  TestRemainingToolsErrorHandling.scale_tool: scale_tool().
  TestRemainingToolsErrorHandling.table_tool: table_tool().
  TestRemainingToolsErrorHandling.query_tool: query_tool().
  TestRemainingToolsErrorHandling.find_grep_tool: find_grep_tool().
  TestRemainingToolsErrorHandling.mcp_server: mcp_server().
  TestRemainingToolsErrorHandling.test_query_code_error_handling: test_query_code_error_handling().
  TestRemainingToolsErrorHandling.test_find_and_grep_error_handling: test_find_and_grep_error_handling().
  TestRemainingToolsErrorHandling: ''
  TestRemainingToolsErrorHandling.temp_project: temp_project().
  TestRemainingToolsErrorHandling.test_check_code_scale_error_handling: test_check_code_scale_error_handling().
  TestRemainingToolsErrorHandling.test_analyze_code_structure_error_handling: test_analyze_code_structure_error_handling().
  TestRemainingToolsErrorHandling.test_set_project_path_error_handling: test_set_project_path_error_handling().
  TestRemainingToolsErrorHandling.test_error_message_quality: test_error_message_quality().
---
# Module: [`tests/integration/mcp/test_error_handling_remaining_tools.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py)

## Classes
### `TestRemainingToolsErrorHandling`
- def: [`tests/integration/mcp/test_error_handling_remaining_tools.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L28)
- doc: 残り5ツールのエラーハンドリングテスト
- signature: `class TestRemainingToolsErrorHandling:`
- members:
  - `find_grep_tool(self, temp_project)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L82) — FindAndGrepTool インスタンス
  - `mcp_server(self, temp_project)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L87) — MCPサーバー インスタンス
  - `query_tool(self, temp_project)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L77) — QueryTool インスタンス
  - `scale_tool(self, temp_project)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L67) — AnalyzeScaleTool インスタンス
  - `table_tool(self, temp_project)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L72) — TableFormatTool インスタンス
  - `temp_project(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L32) — テスト用プロジェクト構造を作成
  - `test_analyze_code_structure_error_handling(self, table_tool)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L117) — analyze_code_structure ツールのエラーハンドリングテスト
  - `test_check_code_scale_error_handling(self, scale_tool)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L92) — check_code_scale ツールのエラーハンドリングテスト
  - `test_comprehensive_error_scenarios(self, temp_project)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L241) — 包括的なエラーシナリオテスト
  - `test_error_message_quality(self, scale_tool, table_tool, query_tool)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L270) — エラーメッセージの品質テスト
  - `test_find_and_grep_error_handling(self, find_grep_tool)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L173) — find_and_grep ツールのエラーハンドリングテスト
  - `test_query_code_error_handling(self, query_tool)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L144) — query_code ツールのエラーハンドリングテスト
  - `test_set_project_path_error_handling(self, mcp_server)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_error_handling_remaining_tools.py#L203) — set_project_path ツールのエラーハンドリングテスト
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

