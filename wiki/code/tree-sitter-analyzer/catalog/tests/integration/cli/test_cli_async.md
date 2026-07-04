---
title: 'Module: tests/integration/cli/test_cli_async.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_async.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_async`/TestCLIAsyncIntegration#
symbols:
  TestCLIAsyncIntegration.test_concurrent_cli_execution: test_concurrent_cli_execution().
  TestCLIAsyncIntegration.run_cli_query: run_cli_query().
  TestCLIAsyncIntegration: ''
  TestCLIAsyncIntegration.sample_files: sample_files().
  TestCLIAsyncIntegration.sample_javascript_file: sample_javascript_file().
  TestCLIAsyncIntegration.test_basic_cli_execution_python: test_basic_cli_execution_python().
  TestCLIAsyncIntegration.test_basic_cli_execution_javascript: test_basic_cli_execution_javascript().
  TestCLIAsyncIntegration.test_class_query_execution: test_class_query_execution().
  TestCLIAsyncIntegration.test_multiple_file_processing: test_multiple_file_processing().
  TestCLIAsyncIntegration.test_output_format_json: test_output_format_json().
  TestCLIAsyncIntegration.test_output_format_text: test_output_format_text().
  TestCLIAsyncIntegration.test_custom_query_string: test_custom_query_string().
  TestCLIAsyncIntegration.test_filter_expression: test_filter_expression().
  TestCLIAsyncIntegration.test_language_auto_detection: test_language_auto_detection().
  TestCLIAsyncIntegration.test_explicit_language_specification: test_explicit_language_specification().
  TestCLIAsyncIntegration.test_error_cases_nonexistent_file: test_error_cases_nonexistent_file().
  TestCLIAsyncIntegration.test_error_cases_invalid_language: test_error_cases_invalid_language().
  TestCLIAsyncIntegration.test_error_cases_invalid_query_key: test_error_cases_invalid_query_key().
  TestCLIAsyncIntegration.test_error_cases_malformed_query_string: test_error_cases_malformed_query_string().
  TestCLIAsyncIntegration.test_help_command: test_help_command().
  TestCLIAsyncIntegration.test_version_command: test_version_command().
  TestCLIAsyncIntegration.test_large_file_cli_processing: test_large_file_cli_processing().
  TestCLIAsyncIntegration.test_cli_performance_baseline: test_cli_performance_baseline().
---
# Module: [`tests/integration/cli/test_cli_async.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py)

## Classes
### `TestCLIAsyncIntegration`
- def: [`tests/integration/cli/test_cli_async.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L13)
- doc: CLI非同期統合テスト
- signature: `class TestCLIAsyncIntegration:`
- members:
  - `run_cli_query(file_path)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L540) — CLI クエリを実行する関数
  - `sample_files(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L17) — 複数のテストファイル
  - `sample_javascript_file(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L106) — JavaScriptテストファイル
  - `test_basic_cli_execution_javascript(self, sample_javascript_file)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L193) — 基本的なJavaScript CLIクエリ実行テスト
  - `test_basic_cli_execution_python(self, sample_files)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L170) — 基本的なPython CLIクエリ実行テスト
  - `test_class_query_execution(self, sample_files)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L216) — クラスクエリの実行テスト
  - `test_cli_performance_baseline(self, sample_files)` — [`L634`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L634) — CLIパフォーマンスベースラインテスト
  - `test_concurrent_cli_execution(self, sample_files)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L536) — 並行CLI実行のテスト
  - `test_custom_query_string(self, sample_files)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L313) — カスタムクエリ文字列のテスト
  - `test_error_cases_invalid_language(self, sample_files)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L425) — エラーケース: 無効な言語
  - `test_error_cases_invalid_query_key(self, sample_files)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L451) — エラーケース: 無効なクエリキー
  - `test_error_cases_malformed_query_string(self, sample_files)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L476) — エラーケース: 不正なクエリ文字列
  - `test_error_cases_nonexistent_file(self)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L397) — エラーケース: 存在しないファイル
  - `test_explicit_language_specification(self, sample_files)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L376) — 明示的な言語指定のテスト
  - `test_filter_expression(self, sample_files)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L332) — フィルター式のテスト
  - `test_help_command(self)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L498) — ヘルプコマンドのテスト
  - `test_language_auto_detection(self, sample_files)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L356) — 言語自動検出のテスト
  - `test_large_file_cli_processing(self)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L576) — 大きなファイルのCLI処理テスト
  - `test_multiple_file_processing(self, sample_files)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L239) — 複数ファイルの処理テスト
  - `test_output_format_json(self, sample_files)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L263) — JSON出力フォーマットのテスト
  - `test_output_format_text(self, sample_files)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L292) — テキスト出力フォーマットのテスト
  - `test_version_command(self)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_async.py#L520) — バージョンコマンドのテスト

