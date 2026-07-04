---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_wrapper_b`/TestWrapperNodesFalsePositivesB#
symbols:
  TestWrapperNodesFalsePositivesB.test_wrapper_node_boundary_same_start_line: test_wrapper_node_boundary_same_start_line().
  TestWrapperNodesFalsePositivesB.test_wrapper_node_partial_overlap: test_wrapper_node_partial_overlap().
  TestWrapperNodesFalsePositivesB.test_typescript_decorator_method_wrapper: test_typescript_decorator_method_wrapper().
  TestWrapperNodesFalsePositivesB.test_multiple_wrappers_same_level: test_multiple_wrappers_same_level().
  TestWrapperNodesFalsePositivesB.test_deeply_nested_wrappers_three_levels: test_deeply_nested_wrappers_three_levels().
  TestWrapperNodesFalsePositivesB: ''
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py)

## Classes
### `TestWrapperNodesFalsePositivesB`
- def: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L19)
- doc: 测试 wrapper nodes（包装节点）不会造成 false positives — Part B
- signature: `class TestWrapperNodesFalsePositivesB:`
- members:
  - `test_deeply_nested_wrappers_three_levels(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L316) — 测试三层嵌套 wrapper
  - `test_multiple_wrappers_same_level(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L230) — 测试同级多个 wrapper nodes
  - `test_typescript_decorator_method_wrapper(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L162) — 测试 TypeScript decorator 包裹的方法
  - `test_wrapper_node_boundary_same_start_line(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L27) — 测试边界情况：wrapper 和被包裹节点起始行相同
  - `test_wrapper_node_partial_overlap(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_b.py#L94) — 测试部分重叠：提取的元素只覆盖 wrapper 的一部分
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)

