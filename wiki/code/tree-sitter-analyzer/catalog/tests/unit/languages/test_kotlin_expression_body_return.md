---
title: 'Module: tests/unit/languages/test_kotlin_expression_body_return.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_expression_body_return.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_expression_body_return`/
symbols:
  _FUNCS: _FUNCS.
  _functions._visit: _functions()._visit().
  _functions: _functions().
  _Stub.parent: _Stub#parent.
  _parse: _parse().
  test_malformed_expression_body_returns_unknown._Stub: test_malformed_expression_body_returns_unknown()._Stub#
  test_expression_body_string_literal_is_string: test_expression_body_string_literal_is_string().
  test_expression_body_integer_literal_is_int: test_expression_body_integer_literal_is_int().
  test_expression_body_true_is_boolean: test_expression_body_true_is_boolean().
  test_expression_body_false_is_boolean: test_expression_body_false_is_boolean().
  test_expression_body_float_literal_is_double: test_expression_body_float_literal_is_double().
  test_expression_body_call_is_unknown_not_unit: test_expression_body_call_is_unknown_not_unit().
  test_expression_body_long_suffix_is_unknown: test_expression_body_long_suffix_is_unknown().
  test_expression_body_null_is_unknown: test_expression_body_null_is_unknown().
  test_explicit_return_type_unchanged: test_explicit_return_type_unchanged().
  test_block_body_without_type_stays_unit: test_block_body_without_type_stays_unit().
  test_block_body_with_explicit_type_unchanged: test_block_body_with_explicit_type_unchanged().
  test_abstract_fun_without_body_stays_unit: test_abstract_fun_without_body_stays_unit().
  test_malformed_expression_body_returns_unknown: test_malformed_expression_body_returns_unknown().
  test_issue_591_reproducer_class_method: test_issue_591_reproducer_class_method().
  test_expression_body_raw_string_is_string: test_expression_body_raw_string_is_string().
  _build_language: _build_language().
  _functions._node_text: _functions()._node_text().
  _SRC: _SRC.
  test_malformed_expression_body_returns_unknown._Stub.__init__: test_malformed_expression_body_returns_unknown()._Stub#__init__().
  _Stub.children: _Stub#children.
  _Stub.child_count: _Stub#child_count.
---
# Module: [`tests/unit/languages/test_kotlin_expression_body_return.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py)

## Classes
### `_Stub`
- def: [`tests/unit/languages/test_kotlin_expression_body_return.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L164)
- signature: `class _Stub:`
- members:
  - `child_count` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L168)
  - `children` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L167)
  - `parent` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L169)
- protocol/private: `__init__`[`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L165)
- uses (calls/refs, reference-scoped): [`_kotlin_expression_body_type`](../../../tree_sitter_analyzer/languages/kotlin_helpers.md#_kotlin_expression_body_type)

## Functions
- `_build_language()` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L30)
- `_functions(source: str)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L47) — Return a name→Function dict parsed from *source*.
- `_node_text(n: tree_sitter.Node)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L53)
- `_parse(source: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L37)
- `_visit(node: tree_sitter.Node)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L56)
- `test_abstract_fun_without_body_stays_unit()` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L150)
- `test_block_body_with_explicit_type_unchanged()` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L141)
- `test_block_body_without_type_stays_unit()` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L137)
- `test_explicit_return_type_unchanged()` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L133)
- `test_expression_body_call_is_unknown_not_unit()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L115)
- `test_expression_body_false_is_boolean()` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L102)
- `test_expression_body_float_literal_is_double()` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L106)
- `test_expression_body_integer_literal_is_int()` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L94)
- `test_expression_body_long_suffix_is_unknown()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L119)
- `test_expression_body_null_is_unknown()` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L124)
- `test_expression_body_raw_string_is_string()` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L188) — Codex P2 on #593: multiline_string_literal ("raw strings") are the
- `test_expression_body_string_literal_is_string()` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L90)
- `test_expression_body_true_is_boolean()` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L98)
- `test_issue_591_reproducer_class_method()` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L177)
- `test_malformed_expression_body_returns_unknown()` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L156)

## Module values
- `_FUNCS` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L82)
- `_SRC` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_expression_body_return.py#L68)

