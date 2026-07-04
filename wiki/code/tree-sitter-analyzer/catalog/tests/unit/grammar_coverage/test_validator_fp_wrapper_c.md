---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_wrapper_c`/
symbols:
  TestWrapperNodesFalsePositivesC.test_wrapper_with_multiple_children: TestWrapperNodesFalsePositivesC#test_wrapper_with_multiple_children().
  TestWrapperNodesFalsePositivesC.test_no_wrapper_direct_extraction: TestWrapperNodesFalsePositivesC#test_no_wrapper_direct_extraction().
  TestWrapperNodesFalsePositivesC.test_adjacent_nodes_no_overlap: TestWrapperNodesFalsePositivesC#test_adjacent_nodes_no_overlap().
  _PM_PATCH: _PM_PATCH.
  _PARSER_PATCH: _PARSER_PATCH.
  _make_plugin_mock: _make_plugin_mock().
  TestWrapperNodesFalsePositivesC: TestWrapperNodesFalsePositivesC#
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py)

## Classes
### `TestWrapperNodesFalsePositivesC`
- def: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L36)
- doc: 测试 wrapper nodes（包装节点）不会造成 false positives — Part C
- signature: `class TestWrapperNodesFalsePositivesC:`
- members:
  - `test_adjacent_nodes_no_overlap(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L149) — 测试相邻节点无重叠（应该正确区分）
  - `test_no_wrapper_direct_extraction(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L111) — 测试没有 wrapper 的直接提取（正常情况，无 false positive）
  - `test_wrapper_with_multiple_children(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L44) — 测试 wrapper 包含多个子节点
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)  (4 test-only)

## Functions
- `_make_plugin_mock(start_line: int, end_line: int)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L22) — Return a mock PluginManager with one element covering start_line..end_line.

## Module values
- `_PARSER_PATCH` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L19)
- `_PM_PATCH` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_c.py#L18)

