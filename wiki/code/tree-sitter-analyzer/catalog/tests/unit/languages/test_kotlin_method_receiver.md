---
title: 'Module: tests/unit/languages/test_kotlin_method_receiver.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_method_receiver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_method_receiver`/
symbols:
  _functions: _functions().
  _functions._visit: _functions()._visit().
  test_receiver_survives_api_serialization: test_receiver_survives_api_serialization().
  _CLASS_SRC: _CLASS_SRC.
  test_class_method_gets_receiver_type: test_class_method_gets_receiver_type().
  test_class_method_bark_gets_receiver_type: test_class_method_bark_gets_receiver_type().
  test_companion_object_fun_is_not_instance_method: test_companion_object_fun_is_not_instance_method().
  test_object_declaration_member_gets_receiver_type: test_object_declaration_member_gets_receiver_type().
  test_top_level_fun_is_unowned: test_top_level_fun_is_unowned().
  test_extension_fun_receiver_type_and_is_method: test_extension_fun_receiver_type_and_is_method().
  test_local_fun_inside_method_is_unowned: test_local_fun_inside_method_is_unowned().
  test_anon_object_override_inside_method_is_unowned: test_anon_object_override_inside_method_is_unowned().
  test_nullable_extension_receiver_type: test_nullable_extension_receiver_type().
  test_companion_fun_is_static: test_companion_fun_is_static().
  test_nested_class_member_gets_inner_owner: test_nested_class_member_gets_inner_owner().
  test_enum_class_member_gets_enum_owner: test_enum_class_member_gets_enum_owner().
  test_extension_receiver_with_nullable_type_and_dot: test_extension_receiver_with_nullable_type_and_dot().
  test_extension_receiver_with_user_type_and_dot: test_extension_receiver_with_user_type_and_dot().
  _parse: _parse().
  test_kotlin_owning_type_parent_none_depth_zero: test_kotlin_owning_type_parent_none_depth_zero().
  test_kotlin_owning_type_source_file_boundary: test_kotlin_owning_type_source_file_boundary().
  test_kotlin_owning_type_local_function_boundary: test_kotlin_owning_type_local_function_boundary().
  test_kotlin_owning_type_object_literal_boundary: test_kotlin_owning_type_object_literal_boundary().
  test_kotlin_owning_type_class_declaration_with_name_field: test_kotlin_owning_type_class_declaration_with_name_field().
  test_kotlin_owning_type_class_declaration_name_via_identifier_scan: test_kotlin_owning_type_class_declaration_name_via_identifier_scan().
  test_kotlin_owning_type_class_declaration_no_name_found: test_kotlin_owning_type_class_declaration_no_name_found().
  test_kotlin_owning_type_object_declaration_owner: test_kotlin_owning_type_object_declaration_owner().
  test_kotlin_owning_type_companion_object_walks_further: test_kotlin_owning_type_companion_object_walks_further().
  test_kotlin_owning_type_depth_cap: test_kotlin_owning_type_depth_cap().
  test_kotlin_owning_type_unicode_name_handling: test_kotlin_owning_type_unicode_name_handling().
  test_kotlin_owning_type_decode_attribute_error: test_kotlin_owning_type_decode_attribute_error().
  test_kotlin_owning_type_decode_unicode_error: test_kotlin_owning_type_decode_unicode_error().
  _build_language: _build_language().
  _functions._node_text: _functions()._node_text().
  _LOCAL_FUN_SRC: _LOCAL_FUN_SRC.
  _ANON_OBJECT_SRC: _ANON_OBJECT_SRC.
  _NULLABLE_EXT_SRC: _NULLABLE_EXT_SRC.
  _COMPANION_STATIC_SRC: _COMPANION_STATIC_SRC.
  _NESTED_CLASS_OWNER_SRC: _NESTED_CLASS_OWNER_SRC.
  _ENUM_CLASS_WITH_MEMBER_SRC: _ENUM_CLASS_WITH_MEMBER_SRC.
  _EXT_REC_NULLABLE_FOLLOWED_BY_DOT: _EXT_REC_NULLABLE_FOLLOWED_BY_DOT.
  _EXT_REC_USER_TYPE_FOLLOWED_BY_DOT: _EXT_REC_USER_TYPE_FOLLOWED_BY_DOT.
---
# Module: [`tests/unit/languages/test_kotlin_method_receiver.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py)

## Functions
- `_build_language()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L40)
- `_functions(source: str)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L57) — Return a name→Function dict parsed from *source*.
- `_node_text(n: tree_sitter.Node)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L72)
- `_parse(source: str)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L47)
- `_visit(node: tree_sitter.Node)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L62)
- `test_anon_object_override_inside_method_is_unowned()` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L205) — P1: ``run`` inside an anonymous object literal in a method must NOT be
- `test_class_method_bark_gets_receiver_type()` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L113)
- `test_class_method_gets_receiver_type()` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L106) — fun inside a class_declaration → receiver_type = class name, is_method=True.
- `test_companion_fun_is_static()` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L248) — P2b: companion fun -> is_method=False, is_static=True,
- `test_companion_object_fun_is_not_instance_method()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L119) — companion object funs are static-like — receiver_type = enclosing class,
- `test_enum_class_member_gets_enum_owner()` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L299) — fun inside enum class body → receiver_type = enum name, is_method=True.
- `test_extension_fun_receiver_type_and_is_method()` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L142) — ``fun String.shout()`` — receiver_type='String', is_method=True.
- `test_extension_receiver_with_nullable_type_and_dot()` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L310) — _kotlin_extension_receiver identifies nullable_type followed by '.' as
- `test_extension_receiver_with_user_type_and_dot()` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L320) — _kotlin_extension_receiver identifies user_type followed by '.' as
- `test_kotlin_owning_type_class_declaration_name_via_identifier_scan()` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L416) — _kotlin_owning_type falls back to scanning children for 'identifier'
- `test_kotlin_owning_type_class_declaration_no_name_found()` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L439) — _kotlin_owning_type returns (None, False) when class has no name field
- `test_kotlin_owning_type_class_declaration_with_name_field()` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L398) — _kotlin_owning_type finds class owner via child_by_field_name('name').
- `test_kotlin_owning_type_companion_object_walks_further()` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L473) — _kotlin_owning_type marks in_companion=True and continues walking
- `test_kotlin_owning_type_decode_attribute_error()` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L536) — _kotlin_owning_type handles AttributeError when name_node.text
- `test_kotlin_owning_type_decode_unicode_error()` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L556) — _kotlin_owning_type handles UnicodeDecodeError when name_node.text
- `test_kotlin_owning_type_depth_cap()` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L498) — _kotlin_owning_type is capped at 256 iterations to prevent unbounded loops
- `test_kotlin_owning_type_local_function_boundary()` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L358) — _kotlin_owning_type stops at function_declaration → (None, False).
- `test_kotlin_owning_type_object_declaration_owner()` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L456) — _kotlin_owning_type finds object owner.
- `test_kotlin_owning_type_object_literal_boundary()` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L378) — _kotlin_owning_type stops at object_literal → (None, False).
- `test_kotlin_owning_type_parent_none_depth_zero()` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L335) — _kotlin_owning_type with node.parent = None → (None, False).
- `test_kotlin_owning_type_source_file_boundary()` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L345) — _kotlin_owning_type stops at source_file → (None, False).
- `test_kotlin_owning_type_unicode_name_handling()` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L518) — _kotlin_owning_type safely decodes non-UTF8 bytes in name_node.text.
- `test_local_fun_inside_method_is_unowned()` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L192) — P1: ``inner`` declared inside a method body must NOT be attributed to Outer.
- `test_nested_class_member_gets_inner_owner()` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L289) — fun inside nested Inner class → receiver_type = Inner (the immediate owner,
- `test_nullable_extension_receiver_type()` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L225) — P2a: ``fun String?.safe()`` -> receiver_type='String?', is_method=True.
- `test_object_declaration_member_gets_receiver_type()` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L129) — fun inside an object_declaration → receiver_type = object name, is_method=True.
- `test_receiver_survives_api_serialization()` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L158) — End-to-end Theme-A (Kotlin): the serializer allowlist must carry
- `test_top_level_fun_is_unowned()` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L136)

## Module values
- `_ANON_OBJECT_SRC` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L181)
- `_CLASS_SRC` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L83)
- `_COMPANION_STATIC_SRC` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L239)
- `_ENUM_CLASS_WITH_MEMBER_SRC` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L272)
- `_EXT_REC_NULLABLE_FOLLOWED_BY_DOT` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L280)
- `_EXT_REC_USER_TYPE_FOLLOWED_BY_DOT` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L284)
- `_LOCAL_FUN_SRC` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L173)
- `_NESTED_CLASS_OWNER_SRC` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L264)
- `_NULLABLE_EXT_SRC` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_method_receiver.py#L220)

