---
title: 'Module: tests/unit/tools/test_cross_lang_call_resolution_patterns.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_cross_lang_call_resolution_patterns.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_cross_lang_call_resolution_patterns`/
symbols:
  FIXTURES: FIXTURES.
  _parser: _parser().
  TestCrossLangCallResolutionPatterns.test_dart_main_perform_action_and_part_of: TestCrossLangCallResolutionPatterns#test_dart_main_perform_action_and_part_of().
  TestCrossLangCallResolutionPatterns.test_c_xmacro_enum_members: TestCrossLangCallResolutionPatterns#test_c_xmacro_enum_members().
  TestCrossLangCallResolutionPatterns.test_c_define_handler_macro_functions: TestCrossLangCallResolutionPatterns#test_c_define_handler_macro_functions().
  TestCrossLangCallResolutionPatterns.test_c_function_pointer_callback: TestCrossLangCallResolutionPatterns#test_c_function_pointer_callback().
  TestCrossLangCallResolutionPatterns.test_cpp_template_overload_disambiguation: TestCrossLangCallResolutionPatterns#test_cpp_template_overload_disambiguation().
  TestCrossLangCallResolutionPatterns.test_lua_require_alias_method_call: TestCrossLangCallResolutionPatterns#test_lua_require_alias_method_call().
  TestCrossLangCallResolutionPatterns.test_swift_protocol_extension_calls: TestCrossLangCallResolutionPatterns#test_swift_protocol_extension_calls().
  TestCrossLangCallResolutionPatterns.test_go_struct_implements_shape: TestCrossLangCallResolutionPatterns#test_go_struct_implements_shape().
  TestCrossLangCallResolutionPatterns.test_elixir_alias_and_use_macro_calls: TestCrossLangCallResolutionPatterns#test_elixir_alias_and_use_macro_calls().
  TestCrossLangCallResolutionPatterns.test_java_static_import_method_and_proxy_dispatch: TestCrossLangCallResolutionPatterns#test_java_static_import_method_and_proxy_dispatch().
  TestCrossLangCallResolutionPatterns.test_haskell_typeclass_instances_and_constructor_call: TestCrossLangCallResolutionPatterns#test_haskell_typeclass_instances_and_constructor_call().
  TestCrossLangCallResolutionPatterns.test_perl_isa_inheritance_super_and_file_new: TestCrossLangCallResolutionPatterns#test_perl_isa_inheritance_super_and_file_new().
  TestCrossLangCallResolutionPatterns.test_ruby_new_resolves_to_initialize: TestCrossLangCallResolutionPatterns#test_ruby_new_resolves_to_initialize().
  TestCrossLangCallResolutionPatterns.test_php_trait_conflict_resolution: TestCrossLangCallResolutionPatterns#test_php_trait_conflict_resolution().
  TestCrossLangCallResolutionPatterns.test_rust_module_super_and_trait_specialization: TestCrossLangCallResolutionPatterns#test_rust_module_super_and_trait_specialization().
  TestCrossLangCallResolutionPatterns.test_scala_case_class_apply: TestCrossLangCallResolutionPatterns#test_scala_case_class_apply().
  TestCrossLangCallResolutionPatterns.test_csharp_partial_of_and_cross_file_call: TestCrossLangCallResolutionPatterns#test_csharp_partial_of_and_cross_file_call().
  TestCrossLangCallResolutionPatterns.test_typescript_dynamic_import_calls_static_import_file: TestCrossLangCallResolutionPatterns#test_typescript_dynamic_import_calls_static_import_file().
  TestCrossLangCallResolutionPatterns.test_typescript_decorated_by_validate_on_update_age: TestCrossLangCallResolutionPatterns#test_typescript_decorated_by_validate_on_update_age().
  TestCrossLangCallResolutionPatterns.test_python_metaclass_links: TestCrossLangCallResolutionPatterns#test_python_metaclass_links().
  TestCrossLangCallResolutionPatterns.test_kotlin_companion_of_links: TestCrossLangCallResolutionPatterns#test_kotlin_companion_of_links().
  TestCrossLangCallResolutionPatterns.test_go_struct_embeds_base: TestCrossLangCallResolutionPatterns#test_go_struct_embeds_base().
  TestCrossLangCallResolutionPatterns.test_elixir_defimpl_implements_protocol: TestCrossLangCallResolutionPatterns#test_elixir_defimpl_implements_protocol().
  TestCrossLangCallResolutionPatterns.test_lua_metatable_variable_inherits: TestCrossLangCallResolutionPatterns#test_lua_metatable_variable_inherits().
  TestCrossLangCallResolutionPatterns.test_php_dynamic_member_resolves_sibling_method: TestCrossLangCallResolutionPatterns#test_php_dynamic_member_resolves_sibling_method().
  TestCrossLangCallResolutionPatterns.test_python_universal_module_node: TestCrossLangCallResolutionPatterns#test_python_universal_module_node().
  TestCrossLangCallResolutionPatterns.get_parser: TestCrossLangCallResolutionPatterns#get_parser().
  manager: manager().
  TestCrossLangCallResolutionPatterns: TestCrossLangCallResolutionPatterns#
---
# Module: [`tests/unit/tools/test_cross_lang_call_resolution_patterns.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py)

## Classes
### `TestCrossLangCallResolutionPatterns`
- def: [`tests/unit/tools/test_cross_lang_call_resolution_patterns.py:59`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L59)
- signature: `class TestCrossLangCallResolutionPatterns:`
- members:
  - `get_parser(ext)` — [`L615`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L615)
  - `test_c_define_handler_macro_functions(self, manager)` — [`L67`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L67)
  - `test_c_function_pointer_callback(self, manager)` — [`L82`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L82)
  - `test_c_xmacro_enum_members(self, manager)` — [`L60`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L60)
  - `test_cpp_template_overload_disambiguation(self, manager)` — [`L108`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L108)
  - `test_csharp_partial_of_and_cross_file_call(self, manager, monkeypatch)` — [`L531`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L531)
  - `test_dart_main_perform_action_and_part_of(self, manager, monkeypatch)` — [`L577`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L577)
  - `test_elixir_alias_and_use_macro_calls(self, manager)` — [`L204`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L204)
  - `test_elixir_defimpl_implements_protocol(self, manager)` — [`L736`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L736)
  - `test_go_struct_embeds_base(self, manager)` — [`L720`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L720)
  - `test_go_struct_implements_shape(self, manager)` — [`L180`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L180)
  - `test_haskell_typeclass_instances_and_constructor_call(self, manager)` — [`L295`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L295)
  - `test_java_static_import_method_and_proxy_dispatch(self, manager, monkeypatch)` — [`L248`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L248)
  - `test_kotlin_companion_of_links(self, manager)` — [`L702`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L702)
  - `test_lua_metatable_variable_inherits(self, manager)` — [`L752`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L752)
  - `test_lua_require_alias_method_call(self, manager)` — [`L128`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L128)
  - `test_perl_isa_inheritance_super_and_file_new(self, manager, monkeypatch)` — [`L336`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L336)
  - `test_php_dynamic_member_resolves_sibling_method(self, manager, monkeypatch)` — [`L768`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L768)
  - `test_php_trait_conflict_resolution(self, manager, monkeypatch)` — [`L420`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L420)
  - `test_python_metaclass_links(self, manager)` — [`L681`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L681)
  - `test_python_universal_module_node(self, manager)` — [`L792`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L792)
  - `test_ruby_new_resolves_to_initialize(self, manager, monkeypatch)` — [`L387`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L387)
  - `test_rust_module_super_and_trait_specialization(self, manager, monkeypatch)` — [`L456`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L456)
  - `test_scala_case_class_apply(self, manager, monkeypatch)` — [`L493`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L493)
  - `test_swift_protocol_extension_calls(self, manager)` — [`L156`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L156)
  - `test_typescript_decorated_by_validate_on_update_age(self, manager)` — [`L660`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L660)
  - `test_typescript_dynamic_import_calls_static_import_file(self, manager)` — [`L635`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L635)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_parser(manager, lang: str)` — [`L51`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L51)
- `manager()` — [`L47`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L47)

## Module values
- `FIXTURES` — [`L43`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cross_lang_call_resolution_patterns.py#L43)

