---
title: 'Module: tests/unit/languages/test_csharp_plugin_interface.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_csharp_plugin_interface.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_csharp_plugin_interface`/
symbols:
  get_tree_for_code: get_tree_for_code().
  TestCSharpPluginInterface.test_get_tree_sitter_language: TestCSharpPluginInterface#test_get_tree_sitter_language().
  TestCSharpPluginInterface.test_language_caching: TestCSharpPluginInterface#test_language_caching().
  TestCSharpPluginInterface.test_get_queries: TestCSharpPluginInterface#test_get_queries().
  TestCSharpPluginInterface.test_get_element_categories: TestCSharpPluginInterface#test_get_element_categories().
  TestCSharpPluginInterface.test_execute_query_strategy_wrong_language: TestCSharpPluginInterface#test_execute_query_strategy_wrong_language().
  TestCSharpPluginInterface.test_execute_query_strategy_csharp: TestCSharpPluginInterface#test_execute_query_strategy_csharp().
  TestCSharpPluginInterface.test_execute_query_strategy_none_key: TestCSharpPluginInterface#test_execute_query_strategy_none_key().
  TestCSharpPluginInterface.test_execute_query_strategy_csharp_classes: TestCSharpPluginInterface#test_execute_query_strategy_csharp_classes().
  TestCSharpPluginInterface.test_plugin_instantiation: TestCSharpPluginInterface#test_plugin_instantiation().
  SIMPLE_CLASS_CODE: SIMPLE_CLASS_CODE.
  INTERFACE_CODE: INTERFACE_CODE.
  ASYNC_METHOD_CODE: ASYNC_METHOD_CODE.
  COMPLEX_CLASS_CODE: COMPLEX_CLASS_CODE.
  PROPERTY_VARIATIONS_CODE: PROPERTY_VARIATIONS_CODE.
  CONTROL_FLOW_CODE: CONTROL_FLOW_CODE.
  TestCSharpPluginInterface: TestCSharpPluginInterface#
---
# Module: [`tests/unit/languages/test_csharp_plugin_interface.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py)

## Classes
### `TestCSharpPluginInterface`
- def: [`tests/unit/languages/test_csharp_plugin_interface.py:262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L262)
- doc: Test CSharp plugin interface implementation.
- signature: `class TestCSharpPluginInterface:`
- members:
  - `test_execute_query_strategy_csharp(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L305) — Test query strategy for C#.
  - `test_execute_query_strategy_csharp_classes(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L318) — Query strategy returns string or None for valid C# keys.
  - `test_execute_query_strategy_none_key(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L312) — Test query strategy with None key.
  - `test_execute_query_strategy_wrong_language(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L299) — Test query strategy with wrong language.
  - `test_get_element_categories(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L289) — Test element categories.
  - `test_get_queries(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L283) — Test query retrieval.
  - `test_get_tree_sitter_language(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L270) — Test tree-sitter language retrieval.
  - `test_language_caching(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L276) — Test that language is cached after first load.
  - `test_plugin_instantiation(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L265) — Test that plugin instantiates successfully.
- uses (calls/refs, reference-scoped): [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.get_tree_sitter_language), [`execute_query_strategy`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.execute_query_strategy), [`get_queries`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.get_element_categories)

## Functions
- `get_tree_for_code(code: str, plugin: CSharpPlugin)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L249) — Helper to parse C# code and return tree.

## Module values
- `ASYNC_METHOD_CODE` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L49)
- `COMPLEX_CLASS_CODE` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L74)
- `CONTROL_FLOW_CODE` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L192)
- `INTERFACE_CODE` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L35)
- `PROPERTY_VARIATIONS_CODE` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L152)
- `SIMPLE_CLASS_CODE` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_interface.py#L10)

