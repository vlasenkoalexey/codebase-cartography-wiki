---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_multifile.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_multifile.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_multifile`/TestMultiFileScenarios#
symbols:
  TestMultiFileScenarios.test_same_node_type_different_files: test_same_node_type_different_files().
  TestMultiFileScenarios.test_same_position_range_different_files: test_same_position_range_different_files().
  TestMultiFileScenarios.test_cross_file_node_identity_no_conflict: test_cross_file_node_identity_no_conflict().
  TestMultiFileScenarios.test_empty_file_path_boundary: test_empty_file_path_boundary().
  TestMultiFileScenarios.test_relative_vs_absolute_path: test_relative_vs_absolute_path().
  TestMultiFileScenarios: ''
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_multifile.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py)

## Classes
### `TestMultiFileScenarios`
- def: [`tests/unit/grammar_coverage/test_validator_fp_multifile.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L19)
- doc: 测试多文件场景下的节点身份冲突
- signature: `class TestMultiFileScenarios:`
- members:
  - `test_cross_file_node_identity_no_conflict(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L152) — 测试跨文件节点身份不冲突
  - `test_empty_file_path_boundary(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L233) — 测试 file_path 为空的边界情况
  - `test_relative_vs_absolute_path(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L291) — 测试相对路径 vs 绝对路径
  - `test_same_node_type_different_files(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L30) — 测试相同节点类型在不同文件（应正确区分）
  - `test_same_position_range_different_files(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_multifile.py#L93) — 测试相同位置范围但不同文件
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)

