---
title: 'Module: tests/unit/mcp/test_mcp_async_integration.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_async_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_async_integration`/TestMCPAsyncIntegration#
symbols:
  TestMCPAsyncIntegration.test_mcp_tool_argument_validation: test_mcp_tool_argument_validation().
  TestMCPAsyncIntegration.test_query_tool_basic_execution: test_query_tool_basic_execution().
  TestMCPAsyncIntegration.test_query_tool_class_execution: test_query_tool_class_execution().
  TestMCPAsyncIntegration.test_query_tool_javascript_execution: test_query_tool_javascript_execution().
  TestMCPAsyncIntegration.test_query_tool_output_formats: test_query_tool_output_formats().
  TestMCPAsyncIntegration.test_query_tool_custom_query_string: test_query_tool_custom_query_string().
  TestMCPAsyncIntegration.test_query_tool_filter_expression: test_query_tool_filter_expression().
  TestMCPAsyncIntegration.test_query_tool_language_auto_detection: test_query_tool_language_auto_detection().
  TestMCPAsyncIntegration.test_query_tool_error_handling_nonexistent_file: test_query_tool_error_handling_nonexistent_file().
  TestMCPAsyncIntegration.test_query_tool_error_handling_invalid_language: test_query_tool_error_handling_invalid_language().
  TestMCPAsyncIntegration.test_query_tool_error_handling_invalid_query_key: test_query_tool_error_handling_invalid_query_key().
  TestMCPAsyncIntegration.test_query_tool_error_handling_malformed_query_string: test_query_tool_error_handling_malformed_query_string().
  TestMCPAsyncIntegration.test_concurrent_mcp_execution: test_concurrent_mcp_execution().
  TestMCPAsyncIntegration.test_multiple_languages_concurrent: test_multiple_languages_concurrent().
  TestMCPAsyncIntegration.test_large_file_mcp_processing: test_large_file_mcp_processing().
  TestMCPAsyncIntegration.test_mcp_performance_baseline: test_mcp_performance_baseline().
  TestMCPAsyncIntegration.test_stress_concurrent_mcp_execution: test_stress_concurrent_mcp_execution().
  TestMCPAsyncIntegration.test_mcp_tool_output_file_feature: test_mcp_tool_output_file_feature().
  TestMCPAsyncIntegration.test_mcp_tool_suppress_output_feature: test_mcp_tool_suppress_output_feature().
  TestMCPAsyncIntegration: ''
  TestMCPAsyncIntegration.sample_code_file: sample_code_file().
  TestMCPAsyncIntegration.sample_javascript_file: sample_javascript_file().
  TestMCPAsyncIntegration.large_code_file: large_code_file().
---
# Module: [`tests/unit/mcp/test_mcp_async_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py)

## Classes
### `TestMCPAsyncIntegration`
- def: [`tests/unit/mcp/test_mcp_async_integration.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L14)
- doc: MCP非同期統合テスト
- signature: `class TestMCPAsyncIntegration:`
- members:
  - `large_code_file(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L105) — 大きなコードファイル
  - `sample_code_file(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L18) — テスト用コードファイル
  - `sample_javascript_file(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L64) — テスト用JavaScriptファイル
  - `test_concurrent_mcp_execution(self, sample_code_file)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L396) — 並行MCP実行テスト
  - `test_large_file_mcp_processing(self, large_code_file)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L483) — 大きなファイルのMCP処理テスト
  - `test_mcp_performance_baseline(self, sample_code_file)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L501) — MCPパフォーマンスベースラインテスト
  - `test_mcp_tool_argument_validation(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L560) — MCP引数バリデーションテスト
  - `test_mcp_tool_output_file_feature(self, sample_code_file)` — [`L577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L577) — MCP出力ファイル機能のテスト
  - `test_mcp_tool_suppress_output_feature(self, sample_code_file)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L619) — MCP出力抑制機能のテスト
  - `test_multiple_languages_concurrent(self, sample_code_file, sample_javascript_file)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L443) — 複数言語の並行処理テスト
  - `test_query_tool_basic_execution(self, sample_code_file)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L132) — QueryToolの基本実行テスト
  - `test_query_tool_class_execution(self, sample_code_file)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L159) — QueryToolのクラスクエリ実行テスト
  - `test_query_tool_custom_query_string(self, sample_code_file)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L233) — カスタムクエリ文字列のテスト
  - `test_query_tool_error_handling_invalid_language(self, sample_code_file)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L323) — エラーハンドリング: 無効な言語
  - `test_query_tool_error_handling_invalid_query_key(self, sample_code_file)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L348) — エラーハンドリング: 無効なクエリキー
  - `test_query_tool_error_handling_malformed_query_string(self, sample_code_file)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L369) — エラーハンドリング: 不正なクエリ文字列
  - `test_query_tool_error_handling_nonexistent_file(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L299) — エラーハンドリング: 存在しないファイル
  - `test_query_tool_filter_expression(self, sample_code_file)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L251) — フィルター式のテスト
  - `test_query_tool_javascript_execution(self, sample_javascript_file)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L184) — QueryToolのJavaScript実行テスト
  - `test_query_tool_language_auto_detection(self, sample_code_file)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L281) — 言語自動検出のテスト
  - `test_query_tool_output_formats(self, sample_code_file)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L204) — 出力フォーマットのテスト
  - `test_stress_concurrent_mcp_execution(self, sample_code_file)` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_async_integration.py#L529) — ストレステスト: 大量の並行MCP実行
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)

