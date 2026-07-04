---
title: 'Module: tests/unit/languages/test_cpp_qualified_names.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_qualified_names.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_qualified_names`/
symbols:
  _functions: _functions().
  _one: _one().
  _Result.line_count: _Result#line_count.
  test_outline_method_entry_omits_receiver_when_unbound: test_outline_method_entry_omits_receiver_when_unbound().
  test_in_namespace_function_gets_namespace_receiver: test_in_namespace_function_gets_namespace_receiver().
  test_in_namespace_template_function_gets_namespace_receiver: test_in_namespace_template_function_gets_namespace_receiver().
  test_definition_styles_converge_to_same_representation: test_definition_styles_converge_to_same_representation().
  test_out_of_class_method_inside_enclosing_namespace_composes: test_out_of_class_method_inside_enclosing_namespace_composes().
  test_in_class_method_keeps_bare_name_and_no_receiver: test_in_class_method_keeps_bare_name_and_no_receiver().
  test_global_function_has_no_receiver: test_global_function_has_no_receiver().
  test_conversion_operator_name_is_not_split: test_conversion_operator_name_is_not_split().
  test_anonymous_namespace_contributes_no_receiver: test_anonymous_namespace_contributes_no_receiver().
  test_nested_namespaces_join_outer_to_inner: test_nested_namespaces_join_outer_to_inner().
  test_cpp17_nested_namespace_specifier: test_cpp17_nested_namespace_specifier().
  test_namespace_name_accepts_str_text_nodes._NsNode.parent: test_namespace_name_accepts_str_text_nodes()._NsNode#parent.
  test_outline_method_entry_carries_receiver_type: test_outline_method_entry_carries_receiver_type().
  extractor: extractor().
  test_out_of_namespace_qualified_function_splits_qualifier: test_out_of_namespace_qualified_function_splits_qualifier().
  test_out_of_class_qualified_method_splits_qualifier: test_out_of_class_qualified_method_splits_qualifier().
  test_out_of_class_constructor_is_flagged: test_out_of_class_constructor_is_flagged().
  test_out_of_class_destructor_is_not_constructor: test_out_of_class_destructor_is_not_constructor().
  test_namespace_name_accepts_str_text_nodes: test_namespace_name_accepts_str_text_nodes().
  test_namespace_name_accepts_str_text_nodes._NsNode.children: test_namespace_name_accepts_str_text_nodes()._NsNode#children.
  test_typed_namespace_same_name_fn_not_constructor: test_typed_namespace_same_name_fn_not_constructor().
  _parse: _parse().
  test_namespace_name_accepts_str_text_nodes._NameNode: test_namespace_name_accepts_str_text_nodes()._NameNode#
  test_namespace_name_accepts_str_text_nodes._NsNode: test_namespace_name_accepts_str_text_nodes()._NsNode#
  test_full_table_global_functions_show_qualified_name._Result: test_full_table_global_functions_show_qualified_name()._Result#
  test_namespace_name_accepts_str_text_nodes._NameNode.type: test_namespace_name_accepts_str_text_nodes()._NameNode#type.
  test_namespace_name_accepts_str_text_nodes._NameNode.text: test_namespace_name_accepts_str_text_nodes()._NameNode#text.
  test_namespace_name_accepts_str_text_nodes._NameNode.parent: test_namespace_name_accepts_str_text_nodes()._NameNode#parent.
  test_full_table_global_functions_show_qualified_name: test_full_table_global_functions_show_qualified_name().
  test_full_table_global_functions_show_qualified_name._Result.__init__: test_full_table_global_functions_show_qualified_name()._Result#__init__().
  _Result.elements: _Result#elements.
  _Result.file_path: _Result#file_path.
  _Result.language: _Result#language.
---
# Module: [`tests/unit/languages/test_cpp_qualified_names.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py)

## Classes
### `_NameNode`
- def: [`tests/unit/languages/test_cpp_qualified_names.py:169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L169)
- signature: `class _NameNode:`
- members:
  - `parent` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L172)
  - `text` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L171)
  - `type` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L170)
- used by: (1 test-only callers)

### `_NsNode`
- def: [`tests/unit/languages/test_cpp_qualified_names.py:174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L174)
- signature: `class _NsNode:`
- members:
  - `children` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L175)
  - `parent` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L176)
- uses (calls/refs, reference-scoped): [`_cpp_namespace_name`](../../../tree_sitter_analyzer/languages/_cpp_element_helpers.md#_cpp_namespace_name)  (1 test-only)

### `_Result`
- def: [`tests/unit/languages/test_cpp_qualified_names.py:192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L192)
- signature: `class _Result:`
- members:
  - `elements` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L194)
  - `file_path` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L195)
  - `language` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L196)
  - `line_count` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L197)
- protocol/private: `__init__`[`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L193)
- uses (calls/refs, reference-scoped): [`CppTableFormatter`](../../../tree_sitter_analyzer/formatters/cpp_formatter.md#CppTableFormatter), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/cpp_formatter.md#CppTableFormatter.format_analysis_result)  (1 test-only)

## Functions
- `_functions(extractor, code)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L29)
- `_one(funcs, name)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L33)
- `_parse(code: str)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L23)
- `extractor()` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L19)
- `test_anonymous_namespace_contributes_no_receiver(extractor)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L147)
- `test_conversion_operator_name_is_not_split(extractor)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L139)
- `test_cpp17_nested_namespace_specifier(extractor)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L158)
- `test_definition_styles_converge_to_same_representation(extractor)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L74)
- `test_full_table_global_functions_show_qualified_name(extractor)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L184)
- `test_global_function_has_no_receiver(extractor)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L132)
- `test_in_class_method_keeps_bare_name_and_no_receiver(extractor)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L126)
- `test_in_namespace_function_gets_namespace_receiver(extractor)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L42)
- `test_in_namespace_template_function_gets_namespace_receiver(extractor)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L48)
- `test_namespace_name_accepts_str_text_nodes()` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L164)
- `test_nested_namespaces_join_outer_to_inner(extractor)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L152)
- `test_out_of_class_constructor_is_flagged(extractor)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L99)
- `test_out_of_class_destructor_is_not_constructor(extractor)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L108)
- `test_out_of_class_method_inside_enclosing_namespace_composes(extractor)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L117)
- `test_out_of_class_qualified_method_splits_qualifier(extractor)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L91)
- `test_out_of_namespace_qualified_function_splits_qualifier(extractor)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L63)
- `test_outline_method_entry_carries_receiver_type(extractor)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L228) — The outline surface must not orphan out-of-class definitions: a
- `test_outline_method_entry_omits_receiver_when_unbound(extractor)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L242)
- `test_typed_namespace_same_name_fn_not_constructor(extractor)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_qualified_names.py#L211) — int math::math() has a return type (a `type` field child) — a

