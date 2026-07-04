---
title: 'Module: tests/unit/languages/test_typescript_extraction_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_extraction_fixes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_extraction_fixes`/
symbols:
  _fn_by_name: _fn_by_name().
  test_enum_export_surface_includes_members: test_enum_export_surface_includes_members().
  test_enum_export_surface_no_phantom_member: test_enum_export_surface_no_phantom_member().
  _classes: _classes().
  test_property_decorator_column: test_property_decorator_column().
  _cls_by_name: _cls_by_name().
  test_is_async_true_for_private_async_method: test_is_async_true_for_private_async_method().
  _functions: _functions().
  _DECORATOR_CLASS_CODE: _DECORATOR_CLASS_CODE.
  test_visibility_public_method_with_private_in_body: test_visibility_public_method_with_private_in_body().
  test_visibility_public_method_with_protected_in_body: test_visibility_public_method_with_protected_in_body().
  test_visibility_private_method: test_visibility_private_method().
  test_visibility_protected_method: test_visibility_protected_method().
  test_visibility_public_method: test_visibility_public_method().
  test_is_async_false_for_method_with_async_in_body: test_is_async_false_for_method_with_async_in_body().
  test_is_async_false_for_sync_method_with_async_in_comment: test_is_async_false_for_sync_method_with_async_in_comment().
  test_is_async_true_for_async_method: test_is_async_true_for_async_method().
  test_class_decorator_injectable: test_class_decorator_injectable().
  test_class_decorator_singleton: test_class_decorator_singleton().
  test_class_has_exactly_two_decorators: test_class_has_exactly_two_decorators().
  test_method_decorator_get: test_method_decorator_get().
  test_method_has_exactly_one_decorator: test_method_has_exactly_one_decorator().
  test_method_multiple_decorators: test_method_multiple_decorators().
  test_enum_not_confused_with_class: test_enum_not_confused_with_class().
  test_exported_enum_interface_and_type_are_detected: test_exported_enum_interface_and_type_are_detected().
  test_reexport_no_inner_spaces: test_reexport_no_inner_spaces().
  test_reexport_multi_name: test_reexport_multi_name().
  test_reexport_aliased: test_reexport_aliased().
  _VISIBILITY_CODE: _VISIBILITY_CODE.
  test_method_without_decorator_has_empty_list: test_method_without_decorator_has_empty_list().
  test_class_without_decorator_has_empty_list: test_class_without_decorator_has_empty_list().
  test_enum_class_type_is_enum: test_enum_class_type_is_enum().
  test_const_enum_class_type_is_enum: test_const_enum_class_type_is_enum().
  test_enum_kind_in_ast_extraction: test_enum_kind_in_ast_extraction().
  _parse: _parse().
  _ASYNC_CODE: _ASYNC_CODE.
  test_enum_kind_is_available_in_symbol_search_filters: test_enum_kind_is_available_in_symbol_search_filters().
  test_enum_members_phantom_from_quoted_comma: test_enum_members_phantom_from_quoted_comma().
  test_enum_members_phantom_from_call_expr_comma: test_enum_members_phantom_from_call_expr_comma().
  test_enum_members_plain_string_values_regression: test_enum_members_plain_string_values_regression().
  test_reexport_name_is_substring_does_not_match: test_reexport_name_is_substring_does_not_match().
  test_reexport_alias_lhs_substring_does_not_match: test_reexport_alias_lhs_substring_does_not_match().
  test_reexport_no_export_block_returns_false: test_reexport_no_export_block_returns_false().
  test_reexport_alias_form_direct: test_reexport_alias_form_direct().
  test_is_exported_class_unexported_returns_false: test_is_exported_class_unexported_returns_false().
  test_is_exported_class_interface_prefix: test_is_exported_class_interface_prefix().
  test_is_exported_class_default_export: test_is_exported_class_default_export().
  test_split_single_quote_string_with_comma: test_split_single_quote_string_with_comma().
  test_split_double_quote_string_with_comma: test_split_double_quote_string_with_comma().
  test_split_backtick_template_with_comma: test_split_backtick_template_with_comma().
  test_split_escaped_quote_inside_string: test_split_escaped_quote_inside_string().
  test_split_nested_paren_brackets: test_split_nested_paren_brackets().
  test_split_nested_square_brackets: test_split_nested_square_brackets().
  test_split_nested_curly_brackets: test_split_nested_curly_brackets().
  test_split_empty_body: test_split_empty_body().
  test_split_trailing_comma_yields_empty_segment: test_split_trailing_comma_yields_empty_segment().
  test_split_unbalanced_close_bracket_depth_never_negative: test_split_unbalanced_close_bracket_depth_never_negative().
  test_enum_members_trailing_comma_skips_empty_candidate: test_enum_members_trailing_comma_skips_empty_candidate().
  test_enum_members_segment_without_identifier_skipped: test_enum_members_segment_without_identifier_skipped().
  test_enum_members_no_braces_uses_raw_text: test_enum_members_no_braces_uses_raw_text().
---
# Module: [`tests/unit/languages/test_typescript_extraction_fixes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py)

## Functions
- `_classes(code: str)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L45)
- `_cls_by_name(code: str, name: str)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L61)
- `_fn_by_name(code: str, name: str)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L51)
- `_functions(code: str)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L39)
- `_parse(code: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L33)
- `test_class_decorator_injectable()` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L186) — @Injectable() on a class must be captured in decorators.
- `test_class_decorator_singleton()` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L193) — @Singleton (no parens) on a class must be captured in decorators.
- `test_class_has_exactly_two_decorators()` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L199)
- `test_class_without_decorator_has_empty_list()` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L246)
- `test_const_enum_class_type_is_enum()` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L267) — TypeScript const enum must have class_type='enum' in extracted Class object.
- `test_enum_class_type_is_enum()` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L260) — TypeScript enum must have class_type='enum' in extracted Class object.
- `test_enum_export_surface_includes_members()` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L318)
- `test_enum_export_surface_no_phantom_member()` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L379) — End-to-end through get_all_exports: quoted comma must not add a member.
- `test_enum_kind_in_ast_extraction()` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L286) — enum_declaration must produce kind='enum' in the _ast_extraction symbol list.
- `test_enum_kind_is_available_in_symbol_search_filters()` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L336)
- `test_enum_members_no_braces_uses_raw_text()` — [`L607`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L607) — With no `{...}` wrapper the whole raw text is split directly.
- `test_enum_members_phantom_from_call_expr_comma()` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L359) — A comma inside a call-expression value must NOT fabricate a member.
- `test_enum_members_phantom_from_quoted_comma()` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L350) — A comma inside a quoted value must NOT fabricate a phantom member.
- `test_enum_members_plain_string_values_regression()` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L368) — Common string-valued enum still splits correctly.
- `test_enum_members_segment_without_identifier_skipped()` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L597) — A segment whose candidate has no leading identifier is skipped.
- `test_enum_members_trailing_comma_skips_empty_candidate()` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L588) — A trailing comma produces an empty segment that is skipped (continue).
- `test_enum_not_confused_with_class()` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L274) — Enum and class in the same file: enum must be 'enum', class must be 'class'.
- `test_exported_enum_interface_and_type_are_detected()` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L302)
- `test_is_async_false_for_method_with_async_in_body()` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L142) — Sync method whose body text contains 'async' must have is_async=False.
- `test_is_async_false_for_sync_method_with_async_in_comment()` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L148) — Sync method with 'async' only in a comment must have is_async=False.
- `test_is_async_true_for_async_method()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L154)
- `test_is_async_true_for_private_async_method()` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L159)
- `test_is_exported_class_default_export()` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L479) — `export default X` is recognised.
- `test_is_exported_class_interface_prefix()` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L470) — `export interface X` is recognised via the interface prefix.
- `test_is_exported_class_unexported_returns_false()` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L461) — A locally-declared, never-exported class is not reported as exported.
- `test_method_decorator_get()` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L204) — @Get('/users') on a method must be captured in decorators.
- `test_method_has_exactly_one_decorator()` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L211)
- `test_method_multiple_decorators()` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L216) — @Post and @Validate must both appear on createUser.
- `test_method_without_decorator_has_empty_list()` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L224) — Methods without decorators must have an empty decorators list, not None.
- `test_property_decorator_column()` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L236) — @Column() on a class field must be captured in Variable.decorators.
- `test_reexport_alias_form_direct()` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L452) — `{ Local as Foo }` reports the LHS `Local` via the alias pattern.
- `test_reexport_alias_lhs_substring_does_not_match()` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L434) — `{ LocalThing as Foo }` must NOT report `Local` (alias-pattern miss).
- `test_reexport_aliased()` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L412)
- `test_reexport_multi_name()` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L405)
- `test_reexport_name_is_substring_does_not_match()` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L425) — `export { LocalThing }` must NOT report `Local` as re-exported.
- `test_reexport_no_export_block_returns_false()` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L443) — A source with no `export { ... }` block at all returns False.
- `test_reexport_no_inner_spaces()` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L400)
- `test_split_backtick_template_with_comma()` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L514)
- `test_split_double_quote_string_with_comma()` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L506)
- `test_split_empty_body()` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L557)
- `test_split_escaped_quote_inside_string()` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L522) — A backslash-escaped quote does not close the string early.
- `test_split_nested_curly_brackets()` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L549)
- `test_split_nested_paren_brackets()` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L533)
- `test_split_nested_square_brackets()` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L541)
- `test_split_single_quote_string_with_comma()` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L498)
- `test_split_trailing_comma_yields_empty_segment()` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L565)
- `test_split_unbalanced_close_bracket_depth_never_negative()` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L573) — A stray closing bracket must not drive depth below zero, so a following
- `test_visibility_private_method()` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L105)
- `test_visibility_protected_method()` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L110)
- `test_visibility_public_method()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L115)
- `test_visibility_public_method_with_private_in_body()` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L93) — Public method whose body contains 'private' must still report visibility='public'.
- `test_visibility_public_method_with_protected_in_body()` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L99) — Public method whose body contains 'protected' must report visibility='public'.

## Module values
- `_ASYNC_CODE` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L124)
- `_DECORATOR_CLASS_CODE` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L169)
- `_VISIBILITY_CODE` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extraction_fixes.py#L75)

