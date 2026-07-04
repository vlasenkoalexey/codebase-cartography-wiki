---
title: 'Module: tests/integration/test_phase7_integration_suite.py'
type: catalog
provenance: extracted
module: tests/integration/test_phase7_integration_suite.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_phase7_integration_suite`/
symbols:
  IntegrationTestReporter.test_results: IntegrationTestReporter#test_results.
  IntegrationTestReporter._generate_report: IntegrationTestReporter#_generate_report().
  IntegrationTestReporter._save_report_to_file: IntegrationTestReporter#_save_report_to_file().
  exit_code: exit_code.
  _simulate_integration_step: _simulate_integration_step().
  TestPhase7IntegrationSuite.integration_reporter: TestPhase7IntegrationSuite#integration_reporter().
  IntegrationTestReporter.end_testing: IntegrationTestReporter#end_testing().
  IntegrationTestReporter.start_time: IntegrationTestReporter#start_time.
  IntegrationTestReporter.end_time: IntegrationTestReporter#end_time.
  _simulation_step_seconds: _simulation_step_seconds().
  IntegrationTestReporter.start_testing: IntegrationTestReporter#start_testing().
  IntegrationTestReporter.add_test_result: IntegrationTestReporter#add_test_result().
  TestPhase7IntegrationSuite.test_end_to_end_integration: TestPhase7IntegrationSuite#test_end_to_end_integration().
  TestPhase7IntegrationSuite.test_performance_integration: TestPhase7IntegrationSuite#test_performance_integration().
  TestPhase7IntegrationSuite.test_security_integration: TestPhase7IntegrationSuite#test_security_integration().
  TestPhase7IntegrationSuite.test_integration_compatibility: TestPhase7IntegrationSuite#test_integration_compatibility().
  TestPhase7IntegrationSuite.test_enterprise_readiness_validation: TestPhase7IntegrationSuite#test_enterprise_readiness_validation().
  DEFAULT_PHASE7_SUITE_SIMULATION_SECONDS: DEFAULT_PHASE7_SUITE_SIMULATION_SECONDS.
  IntegrationTestReporter: IntegrationTestReporter#
  run_integration_suite: run_integration_suite().
  IntegrationTestReporter.__init__: IntegrationTestReporter#__init__().
  TestPhase7IntegrationSuite: TestPhase7IntegrationSuite#
---
# Module: [`tests/integration/test_phase7_integration_suite.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py)

## Classes
### `IntegrationTestReporter`
- def: [`tests/integration/test_phase7_integration_suite.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L46)
- doc: 統合テスト結果レポーター
- signature: `class IntegrationTestReporter:`
- members:
  - `_generate_report(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L85) — 統合テスト結果レポート生成
  - `_save_report_to_file(self)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L226) — レポートをファイルに保存
  - `add_test_result(self, test_category: str, test_name: str, success: bool, duration: float, details: dict[str, Any] = None)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L65) — テスト結果追加
  - `end_testing(self)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L60) — テスト終了
  - `start_testing(self)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L54) — テスト開始
  - `end_time` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L52)
  - `start_time` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L51)
  - `test_results` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L50)
- protocol/private: `__init__`[`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L49)
- used by: (1 test-only callers)

### `TestPhase7IntegrationSuite`
- def: [`tests/integration/test_phase7_integration_suite.py:259`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L259)
- doc: Phase 7 統合テストスイート
- signature: `class TestPhase7IntegrationSuite:`
- members:
  - `integration_reporter(self)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L263) — 統合テストレポーター
  - `test_end_to_end_integration(self, integration_reporter)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L271) — エンドツーエンド統合テスト実行
  - `test_enterprise_readiness_validation(self, integration_reporter)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L427) — エンタープライズ準備状況検証
  - `test_integration_compatibility(self, integration_reporter)` — [`L387`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L387) — 統合互換性テスト
  - `test_performance_integration(self, integration_reporter)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L311) — パフォーマンス統合テスト実行
  - `test_security_integration(self, integration_reporter)` — [`L349`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L349) — セキュリティ統合テスト実行
- uses (calls/refs, reference-scoped): (4 test-only callers)

## Functions
- `_simulate_integration_step()` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L39) — Yield to the event loop without making default tests wait on wall-clock time.
- `_simulation_step_seconds()` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L25) — Return the per-case simulation delay for summary-style integration checks.
- `run_integration_suite()` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L464) — 統合テストスイート実行

## Module values
- `DEFAULT_PHASE7_SUITE_SIMULATION_SECONDS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L22)
- `exit_code` — [`L482`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_integration_suite.py#L482)

