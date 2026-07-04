---
title: 'Module: run_regression_tests.py'
type: catalog
provenance: extracted
module: run_regression_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 run_regression_tests/
symbols:
  RegressionTestRunner.run_all_tests: RegressionTestRunner#run_all_tests().
  RegressionTestRunner.run_command: RegressionTestRunner#run_command().
  RegressionTestRunner.generate_report: RegressionTestRunner#generate_report().
  RegressionTestRunner.failed: RegressionTestRunner#failed.
  RegressionTestRunner.passed: RegressionTestRunner#passed.
  RegressionTestRunner.skipped: RegressionTestRunner#skipped.
  RegressionTestRunner.run_new_async_tests: RegressionTestRunner#run_new_async_tests().
  RegressionTestRunner.run_existing_core_tests: RegressionTestRunner#run_existing_core_tests().
  RegressionTestRunner.run_integration_tests: RegressionTestRunner#run_integration_tests().
  RegressionTestRunner.run_emergency_fix_verification: RegressionTestRunner#run_emergency_fix_verification().
  RegressionTestRunner.run_sample_queries: RegressionTestRunner#run_sample_queries().
  main: main().
  RegressionTestRunner.run_pytest_test: RegressionTestRunner#run_pytest_test().
  RegressionTestRunner.results: RegressionTestRunner#results.
  RegressionTestRunner.check_dependencies: RegressionTestRunner#check_dependencies().
  RegressionTestRunner.run_comprehensive_test_suite: RegressionTestRunner#run_comprehensive_test_suite().
  RegressionTestRunner: RegressionTestRunner#
  RegressionTestRunner.__init__: RegressionTestRunner#__init__().
---
# Module: [`run_regression_tests.py`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py)

## Classes
### `RegressionTestRunner`
- def: [`run_regression_tests.py:11`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L11)
- doc: 回帰テスト実行クラス
- signature: `class RegressionTestRunner:`
- members:
  - `check_dependencies(self)` — [`L90`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L90) — 依存関係の確認
  - `generate_report(self)` — [`L268`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L268) — テスト結果レポートの生成
  - `run_all_tests(self)` — [`L305`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L305) — 全ての回帰テストを実行
  - `run_command(self, cmd, description, timeout=60)` — [`L20`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L20) — コマンド実行とログ出力
  - `run_comprehensive_test_suite(self)` — [`L257`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L257) — 包括的テストスイートの実行
  - `run_emergency_fix_verification(self)` — [`L196`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L196) — 緊急修正の検証
  - `run_existing_core_tests(self)` — [`L149`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L149) — 既存のコアテストの実行
  - `run_integration_tests(self)` — [`L176`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L176) — 統合テストの実行
  - `run_new_async_tests(self)` — [`L127`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L127) — 新規非同期テストの実行
  - `run_pytest_test(self, test_path, description, markers="", timeout=120)` — [`L82`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L82) — pytestテストの実行
  - `run_sample_queries(self)` — [`L211`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L211) — サンプルクエリの実行テスト
  - `failed` — [`L16`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L16)
  - `passed` — [`L15`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L15)
  - `results` — [`L18`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L18)
  - `skipped` — [`L17`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L17)
- protocol/private: `__init__`[`L14`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L14)
- used by: [`main`](run_regression_tests.md#main)

## Functions
- `main()` — [`L349`](../../../../raw/code/tree-sitter-analyzer/run_regression_tests.py#L349) — メイン実行関数

