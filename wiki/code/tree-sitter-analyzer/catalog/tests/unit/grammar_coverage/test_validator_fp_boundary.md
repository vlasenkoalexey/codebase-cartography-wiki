---
title: 'Module: tests/unit/grammar_coverage/test_validator_fp_boundary.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator_fp_boundary.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator_fp_boundary`/
symbols:
  TestBoundaryCases.test_empty_file: TestBoundaryCases#test_empty_file().
  TestBoundaryCases.test_single_node_file: TestBoundaryCases#test_single_node_file().
  TestBoundaryCases.test_no_named_nodes_only_tokens: TestBoundaryCases#test_no_named_nodes_only_tokens().
  TestBoundaryCases.test_plugin_returns_empty_elements: TestBoundaryCases#test_plugin_returns_empty_elements().
  _PM_PATCH: _PM_PATCH.
  TestBoundaryCases.test_plugin_raises_exception: TestBoundaryCases#test_plugin_raises_exception().
  _PARSER_PATCH: _PARSER_PATCH.
  _make_plugin_mock: _make_plugin_mock().
  _make_empty_plugin_mock: _make_empty_plugin_mock().
  TestBoundaryCases: TestBoundaryCases#
---
# Module: [`tests/unit/grammar_coverage/test_validator_fp_boundary.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py)

## Classes
### `TestBoundaryCases`
- def: [`tests/unit/grammar_coverage/test_validator_fp_boundary.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L49)
- doc: 测试边界情况和异常处理
- signature: `class TestBoundaryCases:`
- members:
  - `test_empty_file(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L62) — 测试空文件
  - `test_no_named_nodes_only_tokens(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L136) — 测试无命名节点（只有 token）
  - `test_plugin_raises_exception(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L224) — 测试插件抛出异常
  - `test_plugin_returns_empty_elements(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L187) — 测试插件返回空元素列表
  - `test_single_node_file(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L95) — 测试单节点文件
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)  (5 test-only)

## Functions
- `_make_empty_plugin_mock()` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L38) — Return a mock PluginManager whose plugin returns no elements.
- `_make_plugin_mock(start_line: int, end_line: int)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L24) — Return a mock PluginManager with one element covering start_line..end_line.

## Module values
- `_PARSER_PATCH` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L21)
- `_PM_PATCH` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator_fp_boundary.py#L20)

