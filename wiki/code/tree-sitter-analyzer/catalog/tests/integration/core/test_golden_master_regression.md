---
title: 'Module: tests/integration/core/test_golden_master_regression.py'
type: catalog
provenance: extracted
module: tests/integration/core/test_golden_master_regression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.core.test_golden_master_regression`/
symbols:
  compare_with_golden_master: compare_with_golden_master().
  TestToonGoldenMasterRegression.compare_toon_golden_master: TestToonGoldenMasterRegression#compare_toon_golden_master().
  run_analyzer: run_analyzer().
  normalize_output: normalize_output().
  TestToonGoldenMasterRegression.normalize_toon_output: TestToonGoldenMasterRegression#normalize_toon_output().
  TestToonGoldenMasterRegression.run_toon_analyzer: TestToonGoldenMasterRegression#run_toon_analyzer().
  TestGoldenMasterRegression.test_golden_master_comparison: TestGoldenMasterRegression#test_golden_master_comparison().
  TestGoldenMasterRegression.test_enum_members_extracted: TestGoldenMasterRegression#test_enum_members_extracted().
  TestGoldenMasterRegression.test_interface_type_correct: TestGoldenMasterRegression#test_interface_type_correct().
  TestGoldenMasterRegression.test_enum_type_correct: TestGoldenMasterRegression#test_enum_type_correct().
  TestGoldenMasterRegression.test_visibility_correct: TestGoldenMasterRegression#test_visibility_correct().
  TestToonGoldenMasterRegression.test_toon_golden_master_comparison: TestToonGoldenMasterRegression#test_toon_golden_master_comparison().
  TestToonGoldenMasterRegression.test_toon_format_consistency: TestToonGoldenMasterRegression#test_toon_format_consistency().
  TestToonGoldenMasterRegression.test_toon_token_reduction: TestToonGoldenMasterRegression#test_toon_token_reduction().
  TestGoldenMasterRegression: TestGoldenMasterRegression#
  TestToonGoldenMasterRegression: TestToonGoldenMasterRegression#
---
# Module: [`tests/integration/core/test_golden_master_regression.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py)

## Classes
### `TestGoldenMasterRegression`
- def: [`tests/integration/core/test_golden_master_regression.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L95)
- doc: ゴールデンマスターリグレッションテスト
- signature: `class TestGoldenMasterRegression:`
- members:
  - `test_enum_members_extracted(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L197) — Enumのメンバーが正しく抽出されることを確認
  - `test_enum_type_correct(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L221) — Enumのtypeが正しく認識されることを確認
  - `test_golden_master_comparison(self, input_file: str, golden_name: str, table_format: str)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L182) — ゴールデンマスターとの比較テスト
  - `test_interface_type_correct(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L213) — Interfaceのtypeが正しく認識されることを確認
  - `test_visibility_correct(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L228) — Visibilityが正しく認識されることを確認
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestToonGoldenMasterRegression`
- def: [`tests/integration/core/test_golden_master_regression.py:240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L240)
- doc: TOON フォーマットゴールデンマスターリグレッションテスト
- signature: `class TestToonGoldenMasterRegression:`
- members:
  - `compare_toon_golden_master(self, input_file: str, golden_name: str)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L270) — TOON ゴールデンマスターとの比較
  - `normalize_toon_output(content: str)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L264) — TOON 出力を正規化して、可変部分を除去
  - `run_toon_analyzer(input_file: str)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L244) — TOON フォーマットでアナライザーを実行 (--table toon)
  - `test_toon_format_consistency(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L347) — TOON フォーマットの一貫性を確認
  - `test_toon_golden_master_comparison(self, input_file: str, golden_name: str)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L336) — TOON ゴールデンマスターとの比較テスト
  - `test_toon_token_reduction(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L359) — TOON フォーマットのトークン削減を確認
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `compare_with_golden_master(input_file: str, golden_name: str, table_format: str = "full")` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L57) — 現在の出力とゴールデンマスターを比較
- `normalize_output(content: str)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L49) — 出力を正規化して、バージョン情報や日時などの
- `run_analyzer(input_file: str, table_format: str = "full")` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_golden_master_regression.py#L26) — アナライザーを実行して出力を取得

