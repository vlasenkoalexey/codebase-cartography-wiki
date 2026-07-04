---
title: 'Module: tests/unit/languages/test_c_plugin_coverage_boost.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_c_plugin_coverage_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_c_plugin_coverage_boost`/
symbols:
  _parse: _parse().
  test_extractor_init_state: test_extractor_init_state().
  test_traverse_max_depth: test_traverse_max_depth().
  test_extract_local_include_regex_fallback: test_extract_local_include_regex_fallback().
  test_extract_system_include_regex_fallback: test_extract_system_include_regex_fallback().
  test_analyze_file_with_real_file: test_analyze_file_with_real_file().
  FakeNode.end_byte: FakeNode#end_byte.
  test_traverse_none_root: test_traverse_none_root().
  plugin: plugin().
  test_c_plugin_basic: test_c_plugin_basic().
  test_extract_pointer_return_function: test_extract_pointer_return_function().
  test_extract_static_function: test_extract_static_function().
  test_extract_variadic_parameter: test_extract_variadic_parameter().
  test_extract_union: test_extract_union().
  test_extract_enum: test_extract_enum().
  test_extract_typedef_struct: test_extract_typedef_struct().
  test_extract_typedef_enum: test_extract_typedef_enum().
  test_extract_array_field: test_extract_array_field().
  test_extract_pointer_field: test_extract_pointer_field().
  test_extract_global_pointer_variable: test_extract_global_pointer_variable().
  test_extract_static_variable: test_extract_static_variable().
  test_extract_macro_constant: test_extract_macro_constant().
  test_extract_macro_function: test_extract_macro_function().
  test_extract_system_and_local_includes: test_extract_system_and_local_includes().
  test_extract_const_field: test_extract_const_field().
  test_extract_doxygen_comment: test_extract_doxygen_comment().
  test_extract_block_comment: test_extract_block_comment().
  FakeNode.children: FakeNode#children.
  test_extract_variable_in_struct_body_skipped: test_extract_variable_in_struct_body_skipped().
  test_extract_macro_function_with_variadic: test_extract_macro_function_with_variadic().
  test_extract_macros_inside_ifdef_branches: test_extract_macros_inside_ifdef_branches().
  test_extract_anonymous_struct: test_extract_anonymous_struct().
  test_extract_anonymous_union: test_extract_anonymous_union().
  test_extract_anonymous_enum: test_extract_anonymous_enum().
  test_extract_const_function_qualifier: test_extract_const_function_qualifier().
  test_count_tree_nodes: test_count_tree_nodes().
  test_extract_function_with_for_loop: test_extract_function_with_for_loop().
  test_extract_field_with_init_declarator: test_extract_field_with_init_declarator().
  test_plugin_properties: test_plugin_properties().
  test_extract_function_with_switch: test_extract_function_with_switch().
  test_traverse_max_depth.FakeNode: test_traverse_max_depth().FakeNode#
  test_extract_elements_with_none_tree: test_extract_elements_with_none_tree().
  test_traverse_max_depth.FakeNode.__init__: test_traverse_max_depth().FakeNode#__init__().
  FakeNode.start_byte: FakeNode#start_byte.
  test_count_tree_nodes_none: test_count_tree_nodes_none().
  test_get_tree_sitter_language_cached: test_get_tree_sitter_language_cached().
---
# Module: [`tests/unit/languages/test_c_plugin_coverage_boost.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_c_plugin_coverage_boost.py:254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L254)
- signature: `class FakeNode:`
- members:
  - `children` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L257)
  - `end_byte` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L259)
  - `start_byte` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L258)
- protocol/private: `__init__`[`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L255)
- uses (calls/refs, reference-scoped): [`_traverse_and_extract_iterative`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._traverse_and_extract_iterative)

## Functions
- `_parse(plugin, code)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L12)
- `plugin()` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L8)
- `test_analyze_file_with_real_file(plugin, tmp_path)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L229)
- `test_c_plugin_basic(plugin)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L18)
- `test_count_tree_nodes(plugin)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L385)
- `test_count_tree_nodes_none(plugin)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L394)
- `test_extract_anonymous_enum(plugin)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L365)
- `test_extract_anonymous_struct(plugin)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L345)
- `test_extract_anonymous_union(plugin)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L355)
- `test_extract_array_field(plugin)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L110)
- `test_extract_block_comment(plugin)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L218)
- `test_extract_const_field(plugin)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L194)
- `test_extract_const_function_qualifier(plugin)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L375)
- `test_extract_doxygen_comment(plugin)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L206)
- `test_extract_elements_with_none_tree(plugin)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L244)
- `test_extract_enum(plugin)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L80)
- `test_extract_field_with_init_declarator(plugin)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L420)
- `test_extract_function_with_for_loop(plugin)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L405)
- `test_extract_function_with_switch(plugin)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L463)
- `test_extract_global_pointer_variable(plugin)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L137)
- `test_extract_local_include_regex_fallback()` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L446)
- `test_extract_macro_constant(plugin)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L158)
- `test_extract_macro_function(plugin)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L170)
- `test_extract_macro_function_with_variadic(plugin)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L285)
- `test_extract_macros_inside_ifdef_branches(plugin)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L296) — Regression: macros defined inside ``#ifdef`` / ``#else`` / ``#elif``
- `test_extract_pointer_field(plugin)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L124)
- `test_extract_pointer_return_function(plugin)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L36)
- `test_extract_static_function(plugin)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L45)
- `test_extract_static_variable(plugin)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L147)
- `test_extract_system_and_local_includes(plugin)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L181)
- `test_extract_system_include_regex_fallback()` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L455)
- `test_extract_typedef_enum(plugin)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L100)
- `test_extract_typedef_struct(plugin)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L91)
- `test_extract_union(plugin)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L66)
- `test_extract_variable_in_struct_body_skipped(plugin)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L275)
- `test_extract_variadic_parameter(plugin)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L56)
- `test_extractor_init_state()` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L432)
- `test_get_tree_sitter_language_cached(plugin)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L398)
- `test_plugin_properties(plugin)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L439)
- `test_traverse_max_depth(plugin)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L249)
- `test_traverse_none_root(plugin)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin_coverage_boost.py#L268)

