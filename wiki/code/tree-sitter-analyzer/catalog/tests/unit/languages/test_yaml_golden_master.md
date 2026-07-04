---
title: 'Module: tests/unit/languages/test_yaml_golden_master.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_golden_master.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_golden_master`/
symbols:
  run_yaml_analyzer: run_yaml_analyzer().
  compare_with_golden_master: compare_with_golden_master().
  TestYAMLGoldenMasterRegression.test_yaml_golden_master_comparison: TestYAMLGoldenMasterRegression#test_yaml_golden_master_comparison().
  TestYAMLGoldenMasterRegression.test_yaml_elements_extracted: TestYAMLGoldenMasterRegression#test_yaml_elements_extracted().
  TestYAMLGoldenMasterRegression.test_yaml_multi_document_detected: TestYAMLGoldenMasterRegression#test_yaml_multi_document_detected().
  TestYAMLGoldenMasterRegression.test_yaml_value_types_correct: TestYAMLGoldenMasterRegression#test_yaml_value_types_correct().
  TestYAMLGoldenMasterRegression.test_yaml_merge_key_detected: TestYAMLGoldenMasterRegression#test_yaml_merge_key_detected().
  TestYAMLGoldenMasterRegression.test_yaml_block_scalars_detected: TestYAMLGoldenMasterRegression#test_yaml_block_scalars_detected().
  TestYAMLGoldenMasterRegression.test_yaml_flow_style_detected: TestYAMLGoldenMasterRegression#test_yaml_flow_style_detected().
  TestYAMLGoldenMasterRegression.test_yaml_deep_nesting_detected: TestYAMLGoldenMasterRegression#test_yaml_deep_nesting_detected().
  TestYAMLGoldenMasterRegression.test_yaml_comments_extracted: TestYAMLGoldenMasterRegression#test_yaml_comments_extracted().
  normalize_yaml_output: normalize_yaml_output().
  TestYAMLGoldenMasterRegression: TestYAMLGoldenMasterRegression#
---
# Module: [`tests/unit/languages/test_yaml_golden_master.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py)

## Classes
### `TestYAMLGoldenMasterRegression`
- def: [`tests/unit/languages/test_yaml_golden_master.py:135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L135)
- doc: YAMLゴールデンマスターリグレッションテスト
- signature: `class TestYAMLGoldenMasterRegression:`
- members:
  - `test_yaml_block_scalars_detected(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L214) — ブロックスカラー（| と >）が正しく検出されることを確認
  - `test_yaml_comments_extracted(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L248) — コメントが正しく抽出されることを確認
  - `test_yaml_deep_nesting_detected(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L236) — 深いネスト構造が正しく検出されることを確認
  - `test_yaml_elements_extracted(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L160) — YAML要素が正しく抽出されることを確認
  - `test_yaml_flow_style_detected(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L224) — フロースタイル（{} と []）が正しく検出されることを確認
  - `test_yaml_golden_master_comparison(self, input_file: str, golden_name: str, table_format: str)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L145) — YAMLゴールデンマスターとの比較テスト
  - `test_yaml_merge_key_detected(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L201) — マージキー（<<: *anchor）が正しく検出されることを確認
  - `test_yaml_multi_document_detected(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L181) — マルチドキュメントが正しく検出されることを確認
  - `test_yaml_value_types_correct(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L189) — 値の型が正しく識別されることを確認
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `compare_with_golden_master(input_file: str, golden_name: str, table_format: str = "full")` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L57) — 現在の出力とゴールデンマスターを比較
- `normalize_yaml_output(content: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L18) — YAML出力を正規化して、可変部分を除去します
- `run_yaml_analyzer(input_file: str, table_format: str = "full")` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_golden_master.py#L40) — YAMLアナライザーを実行して出力を取得

