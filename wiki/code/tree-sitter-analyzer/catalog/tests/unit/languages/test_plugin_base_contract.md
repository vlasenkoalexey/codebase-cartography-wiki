---
title: 'Module: tests/unit/languages/test_plugin_base_contract.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugin_base_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugin_base_contract`/
symbols:
  ALL_PLUGINS.ALL_PLUGINS: ALL_PLUGINS.ALL_PLUGINS.
  TestBasePluginContract.test_get_plugin_info_has_required_keys: TestBasePluginContract#test_get_plugin_info_has_required_keys().
  TestBasePluginContract.test_create_extractor_returns_element_extractor: TestBasePluginContract#test_create_extractor_returns_element_extractor().
  TestBasePluginContract.test_is_applicable_true_for_own_extensions: TestBasePluginContract#test_is_applicable_true_for_own_extensions().
  _PLUGIN_IDS: _PLUGIN_IDS.
  TestBasePluginContract.test_get_language_name_returns_nonempty_string: TestBasePluginContract#test_get_language_name_returns_nonempty_string().
  TestBasePluginContract.test_get_file_extensions_returns_nonempty_list: TestBasePluginContract#test_get_file_extensions_returns_nonempty_list().
  TestBasePluginContract.test_get_supported_element_types_returns_list_of_strings: TestBasePluginContract#test_get_supported_element_types_returns_list_of_strings().
  TestBasePluginContract.test_get_queries_returns_string_dict: TestBasePluginContract#test_get_queries_returns_string_dict().
  TestBasePluginContract.test_get_formatter_map_returns_string_dict: TestBasePluginContract#test_get_formatter_map_returns_string_dict().
  TestBasePluginContract.test_get_element_categories_returns_dict_of_lists: TestBasePluginContract#test_get_element_categories_returns_dict_of_lists().
  TestBasePluginContract.test_is_applicable_false_for_unknown_extension: TestBasePluginContract#test_is_applicable_false_for_unknown_extension().
  TestBasePluginContract: TestBasePluginContract#
---
# Module: [`tests/unit/languages/test_plugin_base_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py)

## Classes
### `TestBasePluginContract`
- def: [`tests/unit/languages/test_plugin_base_contract.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L61)
- doc: Every LanguagePlugin must satisfy these 10 invariants.
- signature: `class TestBasePluginContract:`
- members:
  - `test_create_extractor_returns_element_extractor(self, plugin: LanguagePlugin)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L83)
  - `test_get_element_categories_returns_dict_of_lists(self, plugin: LanguagePlugin)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L113)
  - `test_get_file_extensions_returns_nonempty_list(self, plugin: LanguagePlugin)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L73)
  - `test_get_formatter_map_returns_string_dict(self, plugin: LanguagePlugin)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L104)
  - `test_get_language_name_returns_nonempty_string(self, plugin: LanguagePlugin)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L64)
  - `test_get_plugin_info_has_required_keys(self, plugin: LanguagePlugin)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L135)
  - `test_get_queries_returns_string_dict(self, plugin: LanguagePlugin)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L97)
  - `test_get_supported_element_types_returns_list_of_strings(self, plugin: LanguagePlugin)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L89)
  - `test_is_applicable_false_for_unknown_extension(self, plugin: LanguagePlugin)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L130)
  - `test_is_applicable_true_for_own_extensions(self, plugin: LanguagePlugin)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L122)
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.create_extractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`get_queries`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_supported_element_types), [`get_formatter_map`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_formatter_map)

## Module values
- `ALL_PLUGINS` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L33) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)
- `_PLUGIN_IDS` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_base_contract.py#L57)

