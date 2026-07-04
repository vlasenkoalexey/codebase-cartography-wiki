---
title: 'Module: tests/unit/languages/test_scala_expression_body_return.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_scala_expression_body_return.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_scala_expression_body_return`/
symbols:
  _functions: _functions().
  _FUNCS: _FUNCS.
  _Stub.parent: _Stub#parent.
  test_malformed_expression_body_returns_unknown._Stub: test_malformed_expression_body_returns_unknown()._Stub#
  test_expression_body_string_literal_is_string: test_expression_body_string_literal_is_string().
  test_expression_body_integer_literal_is_int: test_expression_body_integer_literal_is_int().
  test_expression_body_true_is_boolean: test_expression_body_true_is_boolean().
  test_expression_body_false_is_boolean: test_expression_body_false_is_boolean().
  test_expression_body_float_literal_is_double: test_expression_body_float_literal_is_double().
  test_expression_body_raw_string_is_string: test_expression_body_raw_string_is_string().
  test_expression_body_call_is_unknown_not_unit: test_expression_body_call_is_unknown_not_unit().
  test_expression_body_long_suffix_is_unknown: test_expression_body_long_suffix_is_unknown().
  test_expression_body_hex_literal_is_unknown: test_expression_body_hex_literal_is_unknown().
  test_expression_body_null_is_unknown: test_expression_body_null_is_unknown().
  test_expression_body_block_expr_is_unknown: test_expression_body_block_expr_is_unknown().
  test_explicit_return_type_unchanged: test_explicit_return_type_unchanged().
  test_block_body_without_type_stays_unit: test_block_body_without_type_stays_unit().
  test_block_body_with_explicit_type_unchanged: test_block_body_with_explicit_type_unchanged().
  test_abstract_def_without_body_stays_unit: test_abstract_def_without_body_stays_unit().
  test_issue_594_reproducer_class_method: test_issue_594_reproducer_class_method().
  test_indented_block_single_literal_infers_type: test_indented_block_single_literal_infers_type().
  test_indented_block_multi_statement_is_unknown: test_indented_block_multi_statement_is_unknown().
  test_negative_int_literal_is_int: test_negative_int_literal_is_int().
  test_negative_suffixed_literal_is_unknown: test_negative_suffixed_literal_is_unknown().
  _parse: _parse().
  _SRC: _SRC.
  test_malformed_expression_body_returns_unknown: test_malformed_expression_body_returns_unknown().
  test_malformed_expression_body_returns_unknown._Stub.__init__: test_malformed_expression_body_returns_unknown()._Stub#__init__().
  _Stub.children: _Stub#children.
  _Stub.child_count: _Stub#child_count.
---
# Module: [`tests/unit/languages/test_scala_expression_body_return.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py)

## Classes
### `_Stub`
- def: [`tests/unit/languages/test_scala_expression_body_return.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L170)
- signature: `class _Stub:`
- members:
  - `child_count` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L174)
  - `children` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L173)
  - `parent` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L175)
- protocol/private: `__init__`[`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L171)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`_scala_expression_body_type`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_expression_body_type)

## Functions
- `_functions(source: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L41) — Return a name→Function dict parsed from *source*.
- `_parse(source: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L35)
- `test_abstract_def_without_body_stays_unit()` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L144)
- `test_block_body_with_explicit_type_unchanged()` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L140)
- `test_block_body_without_type_stays_unit()` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L135)
- `test_explicit_return_type_unchanged()` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L131)
- `test_expression_body_block_expr_is_unknown()` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L120)
- `test_expression_body_call_is_unknown_not_unit()` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L103)
- `test_expression_body_false_is_boolean()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L83)
- `test_expression_body_float_literal_is_double()` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L87)
- `test_expression_body_hex_literal_is_unknown()` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L112)
- `test_expression_body_integer_literal_is_int()` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L75)
- `test_expression_body_long_suffix_is_unknown()` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L107)
- `test_expression_body_null_is_unknown()` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L116)
- `test_expression_body_raw_string_is_string()` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L91)
- `test_expression_body_string_literal_is_string()` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L71)
- `test_expression_body_true_is_boolean()` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L79)
- `test_indented_block_multi_statement_is_unknown()` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L191)
- `test_indented_block_single_literal_infers_type()` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L183) — Codex P2 on #597: `def f =` followed by an indented literal wraps the
- `test_issue_594_reproducer_class_method()` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L155)
- `test_malformed_expression_body_returns_unknown()` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L166)
- `test_negative_int_literal_is_int()` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L197) — Codex P2 on #597: `-1` is a single integer_literal node; Scala infers Int.
- `test_negative_suffixed_literal_is_unknown()` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L203)

## Module values
- `_FUNCS` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L63)
- `_SRC` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_expression_body_return.py#L47)

