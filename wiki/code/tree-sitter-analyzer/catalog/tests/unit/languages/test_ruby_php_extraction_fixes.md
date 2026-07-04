---
title: 'Module: tests/unit/languages/test_ruby_php_extraction_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_ruby_php_extraction_fixes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_ruby_php_extraction_fixes`/
symbols:
  test_ruby_keyword_param_extracted: test_ruby_keyword_param_extracted().
  test_ruby_function_line_count_nonzero: test_ruby_function_line_count_nonzero().
  test_php_method_line_count_nonzero: test_php_method_line_count_nonzero().
  test_php_enum_method_has_receiver_type: test_php_enum_method_has_receiver_type().
  test_php_enum_static_method_has_receiver_type: test_php_enum_static_method_has_receiver_type().
  test_php_top_level_function_name_consistent_after_extract_classes: test_php_top_level_function_name_consistent_after_extract_classes().
  test_ruby_mixed_params_all_extracted: test_ruby_mixed_params_all_extracted().
  test_ruby_class_level_constant_extracted: test_ruby_class_level_constant_extracted().
  test_ruby_initialize_ivar_extracted: test_ruby_initialize_ivar_extracted().
  test_ruby_non_initialize_ivar_not_extracted: test_ruby_non_initialize_ivar_not_extracted().
  test_php_top_level_function_name_consistent_when_called_standalone: test_php_top_level_function_name_consistent_when_called_standalone().
  test_ruby_single_line_method_line_count_one: test_ruby_single_line_method_line_count_one().
  test_ruby_exact_variable_count: test_ruby_exact_variable_count().
  test_php_enum_method_count: test_php_enum_method_count().
  test_php_no_namespace_function_has_bare_name: test_php_no_namespace_function_has_bare_name().
  _ruby_parser: _ruby_parser().
  RUBY_PHANTOM_FIELD_SRC: RUBY_PHANTOM_FIELD_SRC.
  _php_parser: _php_parser().
  PHP_ENUM_SRC: PHP_ENUM_SRC.
  PHP_NS_FUNC_SRC: PHP_NS_FUNC_SRC.
  RUBY_KEYWORD_PARAM_SRC: RUBY_KEYWORD_PARAM_SRC.
---
# Module: [`tests/unit/languages/test_ruby_php_extraction_fixes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py)

## Functions
- `_php_parser()` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L31)
- `_ruby_parser()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L26)
- `test_php_enum_method_count()` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L257) — Exact count: 2 methods in the Suit enum.
- `test_php_enum_method_has_receiver_type()` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L235) — Methods declared inside a PHP enum must have receiver_type == enum name.
- `test_php_enum_static_method_has_receiver_type()` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L246) — Static methods inside a PHP enum must also carry receiver_type.
- `test_php_method_line_count_nonzero()` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L107) — PHP method line_count must equal end_line - start_line + 1.
- `test_php_no_namespace_function_has_bare_name()` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L315) — A function in a file with no namespace declaration must keep its bare name.
- `test_php_top_level_function_name_consistent_after_extract_classes()` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L300) — #765: order-independence — result must be bare name whether or not
- `test_php_top_level_function_name_consistent_when_called_standalone()` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L285) — #765: top-level functions in namespaced files use bare names (not qualified).
- `test_ruby_class_level_constant_extracted()` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L164) — Constants assigned at class body level must be extracted.
- `test_ruby_exact_variable_count()` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L198) — Exact count: 1 constant (MAX_ITEMS) + 1 ivar (@buyer) = 2.
- `test_ruby_function_line_count_nonzero()` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L85) — getattr(func, 'line_count', 0) must return end_line - start_line + 1.
- `test_ruby_initialize_ivar_extracted()` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L175) — @ivar assigned inside initialize IS a field and must be extracted.
- `test_ruby_keyword_param_extracted()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L49) — Keyword parameters (name: default) must appear in .parameters.
- `test_ruby_mixed_params_all_extracted()` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L61) — All Ruby parameter kinds (positional, optional, keyword, splat, block)
- `test_ruby_non_initialize_ivar_not_extracted()` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L186) — @ivar assigned inside non-initialize methods must NOT be extracted.
- `test_ruby_single_line_method_line_count_one()` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L129) — A one-liner method must have line_count == 1.

## Module values
- `PHP_ENUM_SRC` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L212)
- `PHP_NS_FUNC_SRC` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L271)
- `RUBY_KEYWORD_PARAM_SRC` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L40)
- `RUBY_PHANTOM_FIELD_SRC` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_php_extraction_fixes.py#L145)

