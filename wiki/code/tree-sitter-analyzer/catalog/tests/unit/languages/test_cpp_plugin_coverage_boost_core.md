---
title: 'Module: tests/unit/languages/test_cpp_plugin_coverage_boost_core.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_plugin_coverage_boost_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_plugin_coverage_boost_core`/
symbols:
  _parse: _parse().
  plugin: plugin().
  extractor: extractor().
  test_cpp_plugin_basic: test_cpp_plugin_basic().
  test_template_function: test_template_function().
  test_template_class: test_template_class().
  test_union_extraction: test_union_extraction().
  test_namespace_extraction: test_namespace_extraction().
  test_using_declaration_import: test_using_declaration_import().
  test_alias_declaration_import: test_alias_declaration_import().
  test_include_fallback_regex: test_include_fallback_regex().
  test_system_include: test_system_include().
  test_class_inheritance: test_class_inheritance().
  test_pure_virtual_function: test_pure_virtual_function().
  test_static_const_modifiers: test_static_const_modifiers().
  test_global_variable: test_global_variable().
  test_visibility_in_class: test_visibility_in_class().
  test_struct_default_visibility: test_struct_default_visibility().
  test_doxygen_comment_extraction: test_doxygen_comment_extraction().
  test_triple_slash_comment: test_triple_slash_comment().
  test_complexity_with_control_flow: test_complexity_with_control_flow().
  test_qualified_function: test_qualified_function().
  test_count_tree_nodes: test_count_tree_nodes().
  test_variable_with_init_declarator: test_variable_with_init_declarator().
  test_field_with_init_declarator: test_field_with_init_declarator().
  test_destructor_extraction: test_destructor_extraction().
  test_const_method: test_const_method().
  test_static_global_private_visibility: test_static_global_private_visibility().
  test_class_no_name_returns_none: test_class_no_name_returns_none().
  test_function_declaration: test_function_declaration().
  test_method_declaration_in_class: test_method_declaration_in_class().
  test_mixed_includes: test_mixed_includes().
  test_fallback_regex_only: test_fallback_regex_only().
  test_reference_return_function: test_reference_return_function().
  test_pointer_return_function: test_pointer_return_function().
  test_operator_function: test_operator_function().
  test_nested_namespace: test_nested_namespace().
  test_class_default_visibility: test_class_default_visibility().
  test_field_multiple_declarators: test_field_multiple_declarators().
  test_variable_template_type: test_variable_template_type().
  test_function_with_static: test_function_with_static().
  test_template_struct: test_template_struct().
  test_extract_elements_none_tree: test_extract_elements_none_tree().
  test_count_tree_nodes_none: test_count_tree_nodes_none().
  test_extract_elements_exception_handling: test_extract_elements_exception_handling().
---
# Module: [`tests/unit/languages/test_cpp_plugin_coverage_boost_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py)

## Functions
- `_parse(code: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L18)
- `extractor()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L14)
- `plugin()` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L9)
- `test_alias_declaration_import(extractor)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L98)
- `test_class_default_visibility(extractor)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L412)
- `test_class_inheritance(extractor)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L126)
- `test_class_no_name_returns_none(extractor)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L327)
- `test_complexity_with_control_flow(extractor)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L224)
- `test_const_method(extractor)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L308)
- `test_count_tree_nodes(plugin)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L268)
- `test_count_tree_nodes_none(plugin)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L275)
- `test_cpp_plugin_basic(plugin)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L24)
- `test_destructor_extraction(extractor)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L299)
- `test_doxygen_comment_extraction(extractor)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L203)
- `test_extract_elements_exception_handling(plugin)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L450)
- `test_extract_elements_none_tree(plugin)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L258)
- `test_fallback_regex_only(extractor)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L366)
- `test_field_multiple_declarators(extractor)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L422)
- `test_field_with_init_declarator(extractor)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L290)
- `test_function_declaration(extractor)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L338)
- `test_function_with_static(extractor)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L440)
- `test_global_variable(extractor)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L160)
- `test_include_fallback_regex(extractor)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L107)
- `test_method_declaration_in_class(extractor)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L348)
- `test_mixed_includes(extractor)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L358)
- `test_namespace_extraction(extractor)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L80)
- `test_nested_namespace(extractor)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L403)
- `test_operator_function(extractor)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L394)
- `test_pointer_return_function(extractor)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L385)
- `test_pure_virtual_function(extractor)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L139)
- `test_qualified_function(extractor)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L242)
- `test_reference_return_function(extractor)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L376)
- `test_static_const_modifiers(extractor)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L148)
- `test_static_global_private_visibility(extractor)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L317)
- `test_struct_default_visibility(extractor)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L193)
- `test_system_include(extractor)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L116)
- `test_template_class(extractor)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L58)
- `test_template_function(extractor)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L47)
- `test_template_struct(extractor)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L456)
- `test_triple_slash_comment(extractor)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L213)
- `test_union_extraction(extractor)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L69)
- `test_using_declaration_import(extractor)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L89)
- `test_variable_template_type(extractor)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L431)
- `test_variable_with_init_declarator(extractor)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L280)
- `test_visibility_in_class(extractor)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_core.py#L170)

