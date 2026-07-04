---
title: 'Module: tests/unit/languages/test_ruby_phantom_fields_770.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_ruby_phantom_fields_770.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_ruby_phantom_fields_770`/
symbols:
  _extract_vars: _extract_vars().
  test_local_variable_in_initialize_is_not_a_field: test_local_variable_in_initialize_is_not_a_field().
  test_instance_variable_in_initialize_is_a_field: test_instance_variable_in_initialize_is_a_field().
  test_qualified_assignment_is_not_a_field: test_qualified_assignment_is_not_a_field().
  test_index_assignment_is_not_a_field: test_index_assignment_is_not_a_field().
  test_toplevel_lambda_is_not_a_field: test_toplevel_lambda_is_not_a_field().
  test_real_ivar_still_extracted: test_real_ivar_still_extracted().
  test_real_classvar_still_extracted: test_real_classvar_still_extracted().
  test_real_constant_still_extracted: test_real_constant_still_extracted().
  RUBY_AVAILABLE: RUBY_AVAILABLE.
  pytestmark: pytestmark.
  test_exact_field_count_in_clean_class: test_exact_field_count_in_clean_class().
  _parse: _parse().
---
# Module: [`tests/unit/languages/test_ruby_phantom_fields_770.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py)

## Functions
- `_extract_vars(code: str)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L36)
- `_parse(code: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L30)
- `test_exact_field_count_in_clean_class()` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L186) — A class with exactly 2 @ivars and 1 @@cvar yields exactly 3 fields (#770).
- `test_index_assignment_is_not_a_field()` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L99) — recv[key] = value (element_reference target) must NOT become a field (#770).
- `test_instance_variable_in_initialize_is_a_field()` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L68) — @ivar assignment inside initialize MUST be emitted (#770 complement).
- `test_local_variable_in_initialize_is_not_a_field()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L49) — Local variable assignment inside initialize must NOT become a field (#770).
- `test_qualified_assignment_is_not_a_field()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L83) — recv.attr = value (call target) must NOT become a field (#770).
- `test_real_classvar_still_extracted()` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L156) — @@cvar at class body level must still be a field after the fix.
- `test_real_constant_still_extracted()` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L172) — CONSTANT assignment at class body level must still be a field after the fix.
- `test_real_ivar_still_extracted()` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L140) — @ivar inside initialize must still be a field after the fix.
- `test_toplevel_lambda_is_not_a_field()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L119) — Top-level lambda/proc assignments must NOT appear as fields (#770).

## Module values
- `RUBY_AVAILABLE` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L20)
- `pytestmark` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_phantom_fields_770.py#L24)

