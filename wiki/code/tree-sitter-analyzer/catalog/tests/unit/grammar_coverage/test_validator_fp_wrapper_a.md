---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_wrapper_a`/TestWrapperNodesFalsePositivesA#
symbols:
  TestWrapperNodesFalsePositivesA.test_python_decorated_function_not_false_positive: test_python_decorated_function_not_false_positive().
  TestWrapperNodesFalsePositivesA.test_typescript_export_class_wrapper: test_typescript_export_class_wrapper().
  TestWrapperNodesFalsePositivesA.test_rust_attribute_function_wrapper: test_rust_attribute_function_wrapper().
  TestWrapperNodesFalsePositivesA.test_ruby_visibility_method_wrapper: test_ruby_visibility_method_wrapper().
  TestWrapperNodesFalsePositivesA.test_single_layer_nesting_python: test_single_layer_nesting_python().
  TestWrapperNodesFalsePositivesA.test_multi_layer_nesting_python: test_multi_layer_nesting_python().
  TestWrapperNodesFalsePositivesA: ''
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py)

## Classes
### `TestWrapperNodesFalsePositivesA`
- def: [`tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L20)
- doc: 测试 wrapper nodes（包装节点）不会造成 false positives — Part A
- signature: `class TestWrapperNodesFalsePositivesA:`
- members:
  - `test_multi_layer_nesting_python(self)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L381) — 测试多层嵌套（Python 多个 decorator）
  - `test_python_decorated_function_not_false_positive(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L32) — 测试 Python decorator 不会导致被包裹的函数被误标记
  - `test_ruby_visibility_method_wrapper(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L247) — 测试 Ruby visibility modifier 包裹的方法不被误标记
  - `test_rust_attribute_function_wrapper(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L179) — 测试 Rust attribute 包裹的函数不被误标记
  - `test_single_layer_nesting_python(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L314) — 测试单层嵌套（Python decorator）
  - `test_typescript_export_class_wrapper(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_wrapper_a.py#L109) — 测试 TypeScript export 语句包裹的 class 不被误标记
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)

