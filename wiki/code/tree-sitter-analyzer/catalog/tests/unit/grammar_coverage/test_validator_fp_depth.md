---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_depth.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_depth.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_depth`/
symbols:
  TestDepthLimitFalsePositives.test_nesting_99_layers_should_pass: TestDepthLimitFalsePositives#test_nesting_99_layers_should_pass().
  TestDepthLimitFalsePositives.test_nesting_100_layers_should_trigger_limit: TestDepthLimitFalsePositives#test_nesting_100_layers_should_trigger_limit().
  TestDepthLimitFalsePositives.test_nesting_101_layers_extreme: TestDepthLimitFalsePositives#test_nesting_101_layers_extreme().
  TestDepthLimitFalsePositives.test_extreme_nesting_1000_layers: TestDepthLimitFalsePositives#test_extreme_nesting_1000_layers().
  TestDepthLimitFalsePositives.test_circular_reference_detection: TestDepthLimitFalsePositives#test_circular_reference_detection().
  _PM_PATCH: _PM_PATCH.
  _PARSER_PATCH: _PARSER_PATCH.
  _make_plugin_mock: _make_plugin_mock().
  _make_deep_nodes: _make_deep_nodes().
  TestDepthLimitFalsePositives: TestDepthLimitFalsePositives#
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_depth.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py)

## Classes
### `TestDepthLimitFalsePositives`
- def: [`tests/unit/grammar_coverage/test_validator_fp_depth.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L67)
- doc: 测试深度限制防止无限嵌套和递归
- signature: `class TestDepthLimitFalsePositives:`
- members:
  - `test_circular_reference_detection(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L144) — 测试循环引用检测（病态 AST）
  - `test_extreme_nesting_1000_layers(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L190) — 测试极端 1000 层嵌套（断路器测试）
  - `test_nesting_100_layers_should_trigger_limit(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L100) — 测试 100 层嵌套应该触发限制（如果实现了限制）
  - `test_nesting_101_layers_extreme(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L122) — 测试 101 层极端嵌套
  - `test_nesting_99_layers_should_pass(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L78) — 测试 99 层嵌套应该通过
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)  (5 test-only)

## Functions
- `_make_deep_nodes(n: int, *, name_prefix: str = "node_level")` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L24) — Create a linear chain of *n* MagicMock AST nodes.
- `_make_plugin_mock(start_line: int, end_line: int)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L53) — Return a mock PluginManager with one element covering start_line..end_line.

## Module values
- `_PARSER_PATCH` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L21)
- `_PM_PATCH` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_depth.py#L20)

