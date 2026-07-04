---
title: 'Module: tests/unit/core/test_async_query_service.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_async_query_service.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_async_query_service`/TestAsyncQueryService#
symbols:
  TestAsyncQueryService.test_execute_query_is_async_method: test_execute_query_is_async_method().
  TestAsyncQueryService.test_execute_query_returns_coroutine: test_execute_query_returns_coroutine().
  TestAsyncQueryService.test_query_key_execution: test_query_key_execution().
  TestAsyncQueryService.test_class_query_execution: test_class_query_execution().
  TestAsyncQueryService.test_custom_query_string: test_custom_query_string().
  TestAsyncQueryService.test_concurrent_execution: test_concurrent_execution().
  TestAsyncQueryService.test_multiple_languages_concurrent: test_multiple_languages_concurrent().
  TestAsyncQueryService.test_error_handling_nonexistent_file: test_error_handling_nonexistent_file().
  TestAsyncQueryService.test_error_handling_invalid_language: test_error_handling_invalid_language().
  TestAsyncQueryService.test_error_handling_invalid_query_key: test_error_handling_invalid_query_key().
  TestAsyncQueryService.test_timeout_behavior: test_timeout_behavior().
  TestAsyncQueryService.test_filter_expression: test_filter_expression().
  TestAsyncQueryService.test_async_file_reading_method: test_async_file_reading_method().
  TestAsyncQueryService.test_large_file_handling: test_large_file_handling().
  TestAsyncQueryService.test_stress_concurrent_execution: test_stress_concurrent_execution().
  TestAsyncQueryService: ''
  TestAsyncQueryService.sample_python_file: sample_python_file().
  TestAsyncQueryService.sample_javascript_file: sample_javascript_file().
---
# Module: [`tests/unit/core/test_async_query_service.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py)

## Classes
### `TestAsyncQueryService`
- def: [`tests/unit/core/test_async_query_service.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L14)
- doc: 非同期QueryServiceのテスト
- signature: `class TestAsyncQueryService:`
- members:
  - `sample_javascript_file(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L44) — テスト用JavaScriptファイル
  - `sample_python_file(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L18) — テスト用Pythonファイル
  - `test_async_file_reading_method(self, sample_python_file)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L274) — 非同期ファイル読み込みメソッドのテスト
  - `test_class_query_execution(self, sample_python_file)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L115) — クラスクエリの実行テスト
  - `test_concurrent_execution(self, sample_python_file)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L146) — 並行実行テスト
  - `test_custom_query_string(self, sample_python_file)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L129) — カスタムクエリ文字列の実行テスト
  - `test_error_handling_invalid_language(self, sample_python_file)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L211) — 無効な言語のエラーハンドリングテスト
  - `test_error_handling_invalid_query_key(self, sample_python_file)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L223) — 無効なクエリキーのエラーハンドリングテスト
  - `test_error_handling_nonexistent_file(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L201) — 存在しないファイルのエラーハンドリングテスト
  - `test_execute_query_is_async_method(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L68) — execute_queryが非同期メソッドであることを確認
  - `test_execute_query_returns_coroutine(self, sample_python_file)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L77) — execute_queryがコルーチンオブジェクトを返すことを確認
  - `test_filter_expression(self, sample_python_file)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L256) — フィルター式のテスト
  - `test_large_file_handling(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L290) — 大きなファイルの処理テスト
  - `test_multiple_languages_concurrent(self, sample_python_file, sample_javascript_file)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L174) — 複数言語の並行処理テスト
  - `test_query_key_execution(self, sample_python_file)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L95) — クエリキーによる実行テスト
  - `test_stress_concurrent_execution(self, sample_python_file)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L320) — ストレステスト: 大量の並行実行
  - `test_timeout_behavior(self, sample_python_file)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_async_query_service.py#L236) — タイムアウト動作テスト
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`_read_file_async`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._read_file_async)

