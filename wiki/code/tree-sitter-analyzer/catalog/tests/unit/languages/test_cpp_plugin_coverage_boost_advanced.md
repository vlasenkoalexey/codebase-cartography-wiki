---
title: 'Module: tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_plugin_coverage_boost_advanced`/
symbols:
  _parse: _parse().
  test_extract_elements_with_bad_extractor: test_extract_elements_with_bad_extractor().
  test_extract_function_optimized_error: test_extract_function_optimized_error().
  test_field_declaration_error_handling: test_field_declaration_error_handling().
  test_function_declaration_error_handling: test_function_declaration_error_handling().
  test_field_declaration_error_handling.find_field_decl: test_field_declaration_error_handling().find_field_decl().
  test_function_declaration_error_handling.find_func_decl: test_function_declaration_error_handling().find_func_decl().
  test_extract_elements_with_bad_extractor.bad_extractor_factory: test_extract_elements_with_bad_extractor().bad_extractor_factory().
  plugin: plugin().
  extractor: extractor().
  test_function_multiple_parameters: test_function_multiple_parameters().
  test_variadic_function: test_variadic_function().
  test_qualified_name_with_namespace: test_qualified_name_with_namespace().
  test_deleted_method: test_deleted_method().
  test_defaulted_method: test_defaulted_method().
  test_protected_access_specifier: test_protected_access_specifier().
  test_field_init_declarator_identifier: test_field_init_declarator_identifier().
  test_include_fallback_local_only: test_include_fallback_local_only().
  test_virtual_const_function: test_virtual_const_function().
  test_for_range_complexity: test_for_range_complexity().
  test_switch_complexity: test_switch_complexity().
  test_try_catch_complexity: test_try_catch_complexity().
  test_get_access_specifier_not_in_class: test_get_access_specifier_not_in_class().
  test_is_global_scope_root: test_is_global_scope_root().
  test_multiple_global_variables_init_declarator: test_multiple_global_variables_init_declarator().
  test_count_tree_nodes_with_children: test_count_tree_nodes_with_children().
  test_doxygen_comment_on_class: test_doxygen_comment_on_class().
  test_namespace_identifier_node: test_namespace_identifier_node().
  test_deeply_nested_blocks: test_deeply_nested_blocks().
  test_static_field_declaration: test_static_field_declaration().
  test_lambda_expression: test_lambda_expression().
  test_extract_imports_fallback_path: test_extract_imports_fallback_path().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#
  test_extract_function_optimized_error.bad_parse: test_extract_function_optimized_error().bad_parse().
  test_protected_explicit_modifier_determine_visibility: test_protected_explicit_modifier_determine_visibility().
  test_private_explicit_modifier_determine_visibility: test_private_explicit_modifier_determine_visibility().
  test_public_explicit_modifier_determine_visibility: test_public_explicit_modifier_determine_visibility().
  test_static_global_determine_visibility: test_static_global_determine_visibility().
  test_default_visibility: test_default_visibility().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor.extract_functions: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#extract_functions().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor.extract_classes: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#extract_classes().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor.extract_variables: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#extract_variables().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor.extract_imports: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#extract_imports().
  test_extract_elements_with_bad_extractor.bad_extractor_factory.BadExtractor.extract_packages: test_extract_elements_with_bad_extractor().bad_extractor_factory().BadExtractor#extract_packages().
  test_include_fallback_regex_direct: test_include_fallback_regex_direct().
  test_include_fallback_system_only: test_include_fallback_system_only().
  test_analyze_file_cpp: test_analyze_file_cpp().
---
# Module: [`tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py)

## Classes
### `BadExtractor`
- def: [`tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L200)
- signature: `class BadExtractor:`
- members:
  - `extract_classes(self, tree, src)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L204)
  - `extract_functions(self, tree, src)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L201)
  - `extract_imports(self, tree, src)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L210)
  - `extract_packages(self, tree, src)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L213)
  - `extract_variables(self, tree, src)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L207)
- used by: (1 test-only callers)

## Functions
- `_parse(code: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L18)
- `bad_extractor_factory(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L199)
- `bad_parse(*args, **kwargs)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L369)
- `extractor()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L14)
- `find_field_decl(node)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L387)
- `find_func_decl(node)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L418)
- `plugin()` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L9)
- `test_analyze_file_cpp(plugin, tmp_path)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L326) — Test analyze_file on a real temporary C++ file.
- `test_count_tree_nodes_with_children(plugin)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L237)
- `test_deeply_nested_blocks(extractor)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L265)
- `test_default_visibility(extractor)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L115)
- `test_defaulted_method(extractor)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L70)
- `test_deleted_method(extractor)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L61)
- `test_doxygen_comment_on_class(extractor)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L245)
- `test_extract_elements_with_bad_extractor(plugin, monkeypatch)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L198)
- `test_extract_function_optimized_error(extractor, monkeypatch)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L360) — Test error handling in _extract_function_optimized.
- `test_extract_imports_fallback_path(extractor)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L348) — Trigger the fallback regex path when tree-sitter finds no includes.
- `test_field_declaration_error_handling(extractor, monkeypatch)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L378) — Test error handling in _extract_function_from_field_declaration.
- `test_field_init_declarator_identifier(extractor)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L121)
- `test_for_range_complexity(extractor)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L151)
- `test_function_declaration_error_handling(extractor, monkeypatch)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L409) — Test error handling in _extract_function_declaration.
- `test_function_multiple_parameters(extractor)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L25)
- `test_get_access_specifier_not_in_class(extractor)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L184)
- `test_include_fallback_local_only(extractor)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L131)
- `test_include_fallback_regex_direct(extractor)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L304) — Test _extract_includes_fallback with system and local includes.
- `test_include_fallback_system_only(extractor)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L315)
- `test_is_global_scope_root(extractor)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L191)
- `test_lambda_expression(extractor)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L291)
- `test_multiple_global_variables_init_declarator(extractor)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L228)
- `test_namespace_identifier_node(extractor)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L256)
- `test_private_explicit_modifier_determine_visibility(extractor)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L97)
- `test_protected_access_specifier(extractor)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L81)
- `test_protected_explicit_modifier_determine_visibility(extractor)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L91)
- `test_public_explicit_modifier_determine_visibility(extractor)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L103)
- `test_qualified_name_with_namespace(extractor)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L44)
- `test_static_field_declaration(extractor)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L281)
- `test_static_global_determine_visibility(extractor)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L109)
- `test_switch_complexity(extractor)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L161)
- `test_try_catch_complexity(extractor)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L172)
- `test_variadic_function(extractor)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L35)
- `test_virtual_const_function(extractor)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_coverage_boost_advanced.py#L140)

