---
title: 'Module: tests/unit/languages/test_ruby_php_inheritance.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_ruby_php_inheritance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_ruby_php_inheritance`/
symbols:
  _php_classes: _php_classes().
  _ruby_classes: _ruby_classes().
  test_php_interface_multi_extends_all_parents_captured: test_php_interface_multi_extends_all_parents_captured().
  test_php_class_multi_extends_anomaly_preserved: test_php_class_multi_extends_anomaly_preserved().
  test_interfaces_survive_api_serialization: test_interfaces_survive_api_serialization().
  test_ruby_superclass_with_only_operator_returns_none: test_ruby_superclass_with_only_operator_returns_none().
  test_ruby_superclass_is_name_not_operator: test_ruby_superclass_is_name_not_operator().
  test_ruby_scoped_superclass: test_ruby_scoped_superclass().
  test_ruby_no_superclass_stays_none: test_ruby_no_superclass_stays_none().
  test_php_extends_captured: test_php_extends_captured().
  test_php_implements_captured: test_php_implements_captured().
  test_php_no_inheritance_stays_empty: test_php_no_inheritance_stays_empty().
  RUBY_SRC: RUBY_SRC.
  PHP_SRC: PHP_SRC.
---
# Module: [`tests/unit/languages/test_ruby_php_inheritance.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py)

## Functions
- `_php_classes()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L55)
- `_ruby_classes()` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L47)
- `test_interfaces_survive_api_serialization()` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L100) — Theme-C tail: plugins collected interfaces but element_to_dict dropped
- `test_php_class_multi_extends_anomaly_preserved()` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L128) — ``class C extends A, B`` is invalid PHP but parses error-tolerantly
- `test_php_extends_captured()` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L82)
- `test_php_implements_captured()` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L87)
- `test_php_interface_multi_extends_all_parents_captured()` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L112) — Review fix: ``interface I extends A, B`` must keep ALL parents —
- `test_php_no_inheritance_stays_empty()` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L94)
- `test_ruby_no_superclass_stays_none()` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L77)
- `test_ruby_scoped_superclass()` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L70)
- `test_ruby_superclass_is_name_not_operator()` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L63)
- `test_ruby_superclass_with_only_operator_returns_none()` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L143) — Degenerate superclass node containing ONLY the '<' token (malformed

## Module values
- `PHP_SRC` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L36)
- `RUBY_SRC` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_inheritance.py#L22)

