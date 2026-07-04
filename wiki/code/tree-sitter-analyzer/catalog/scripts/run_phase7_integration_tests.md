---
title: 'Module: scripts/run_phase7_integration_tests.py'
type: catalog
provenance: extracted
module: scripts/run_phase7_integration_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.run_phase7_integration_tests`/
symbols:
  Phase7TestRunner.test_results: Phase7TestRunner#test_results.
  Phase7TestRunner.run_all_tests: Phase7TestRunner#run_all_tests().
  Phase7TestRunner._generate_final_report: Phase7TestRunner#_generate_final_report().
  Phase7TestRunner._save_report: Phase7TestRunner#_save_report().
  Phase7TestRunner._run_test_category: Phase7TestRunner#_run_test_category().
  main: main().
  Phase7TestRunner.start_time: Phase7TestRunner#start_time.
  Phase7TestRunner.end_time: Phase7TestRunner#end_time.
  Phase7TestRunner.project_root: Phase7TestRunner#project_root.
  Phase7TestRunner: Phase7TestRunner#
  Phase7TestRunner.__init__: Phase7TestRunner#__init__().
---
# Module: [`scripts/run_phase7_integration_tests.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py)

## Classes
### `Phase7TestRunner`
- def: [`scripts/run_phase7_integration_tests.py:16`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L16)
- doc: Phase 7統合テストランナー
- signature: `class Phase7TestRunner:`
- members:
  - `_generate_final_report(self)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L160) — 最終レポート生成
  - `_run_test_category(self, category: dict, verbose: bool, coverage: bool)` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L78) — テストカテゴリを実行
  - `_save_report(self)` — [`L248`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L248) — レポートをファイルに保存
  - `run_all_tests(self, verbose: bool = False, coverage: bool = False)` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L25) — 全統合テストを実行
  - `end_time` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L23)
  - `project_root` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L20)
  - `start_time` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L22)
  - `test_results` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L21)
- protocol/private: `__init__`[`L19`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L19)
- used by: [`main`](run_phase7_integration_tests.md#main)

## Functions
- `main()` — [`L289`](../../../../../raw/code/tree-sitter-analyzer/scripts/run_phase7_integration_tests.py#L289) — メイン関数

