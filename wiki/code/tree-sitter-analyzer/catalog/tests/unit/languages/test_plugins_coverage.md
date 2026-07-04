---
title: 'Module: tests/unit/languages/test_plugins_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugins_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugins_coverage`/
symbols:
  default_extractor: default_extractor().
  plugin_manager_instance: plugin_manager_instance().
  TestDefaultExtractor: TestDefaultExtractor#
  TestDefaultExtractor.test_extract_functions_with_valid_tree: TestDefaultExtractor#test_extract_functions_with_valid_tree().
  TestDefaultExtractor.test_extract_functions_with_exception: TestDefaultExtractor#test_extract_functions_with_exception().
  TestDefaultExtractor.test_extract_classes_with_valid_tree: TestDefaultExtractor#test_extract_classes_with_valid_tree().
  TestDefaultExtractor.test_extract_classes_with_exception: TestDefaultExtractor#test_extract_classes_with_exception().
  TestDefaultExtractor.test_extract_variables_with_valid_tree: TestDefaultExtractor#test_extract_variables_with_valid_tree().
  TestDefaultExtractor.test_extract_variables_with_exception: TestDefaultExtractor#test_extract_variables_with_exception().
  TestDefaultExtractor.test_extract_imports_with_valid_tree: TestDefaultExtractor#test_extract_imports_with_valid_tree().
  TestDefaultExtractor.test_extract_imports_with_exception: TestDefaultExtractor#test_extract_imports_with_exception().
  TestDefaultExtractor.test_traverse_for_functions_with_nested_nodes: TestDefaultExtractor#test_traverse_for_functions_with_nested_nodes().
  TestDefaultExtractor.test_traverse_for_classes_with_nested_nodes: TestDefaultExtractor#test_traverse_for_classes_with_nested_nodes().
  TestDefaultExtractor.test_traverse_for_variables_with_nested_nodes: TestDefaultExtractor#test_traverse_for_variables_with_nested_nodes().
  TestDefaultExtractor.test_traverse_for_imports_with_nested_nodes: TestDefaultExtractor#test_traverse_for_imports_with_nested_nodes().
  TestDefaultExtractor.test_extract_node_name_with_identifier: TestDefaultExtractor#test_extract_node_name_with_identifier().
  TestDefaultExtractor.test_extract_node_name_without_identifier: TestDefaultExtractor#test_extract_node_name_without_identifier().
  TestDefaultExtractor.test_extract_node_name_with_exception: TestDefaultExtractor#test_extract_node_name_with_exception().
  TestPluginManagerAdvanced: TestPluginManagerAdvanced#
  TestPluginManagerAdvanced.test_register_plugin_with_exception: TestPluginManagerAdvanced#test_register_plugin_with_exception().
  TestPluginManagerAdvanced.test_get_plugin_for_file_with_applicable_plugin: TestPluginManagerAdvanced#test_get_plugin_for_file_with_applicable_plugin().
  TestPluginManagerAdvanced.test_list_supported_languages_empty: TestPluginManagerAdvanced#test_list_supported_languages_empty().
---
# Module: [`tests/unit/languages/test_plugins_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py)

## Classes
### `TestDefaultExtractor`
- def: [`tests/unit/languages/test_plugins_coverage.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L31)
- doc: Test DefaultExtractor functionality
- signature: `class TestDefaultExtractor:`
- members:
  - `test_extract_classes_with_exception(self, mocker, default_extractor)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L77) — Test class extraction with exception
  - `test_extract_classes_with_valid_tree(self, mocker, default_extractor)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L61) — Test class extraction with valid tree
  - `test_extract_functions_with_exception(self, mocker, default_extractor)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L50) — Test function extraction with exception
  - `test_extract_functions_with_valid_tree(self, mocker, default_extractor)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L34) — Test function extraction with valid tree
  - `test_extract_imports_with_exception(self, mocker, default_extractor)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L131) — Test import extraction with exception
  - `test_extract_imports_with_valid_tree(self, mocker, default_extractor)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L115) — Test import extraction with valid tree
  - `test_extract_node_name_with_exception(self, mocker, default_extractor)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L246) — Test node name extraction with exception
  - `test_extract_node_name_with_identifier(self, mocker, default_extractor)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L223) — Test node name extraction with identifier
  - `test_extract_node_name_without_identifier(self, mocker, default_extractor)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L237) — Test node name extraction without identifier
  - `test_extract_variables_with_exception(self, mocker, default_extractor)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L104) — Test variable extraction with exception
  - `test_extract_variables_with_valid_tree(self, mocker, default_extractor)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L88) — Test variable extraction with valid tree
  - `test_traverse_for_classes_with_nested_nodes(self, mocker, default_extractor)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L163) — Test class traversal with nested nodes
  - `test_traverse_for_functions_with_nested_nodes(self, mocker, default_extractor)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L142) — Test function traversal with nested nodes
  - `test_traverse_for_imports_with_nested_nodes(self, mocker, default_extractor)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L203) — Test import traversal with nested nodes
  - `test_traverse_for_variables_with_nested_nodes(self, mocker, default_extractor)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L183) — Test variable traversal with nested nodes

### `TestPluginManagerAdvanced`
- def: [`tests/unit/languages/test_plugins_coverage.py:256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L256)
- doc: Test advanced PluginManager functionality
- signature: `class TestPluginManagerAdvanced:`
- members:
  - `test_get_plugin_for_file_with_applicable_plugin(self, mocker, plugin_manager_instance)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L267) — Test getting plugin for file with applicable plugin
  - `test_list_supported_languages_empty(self, plugin_manager_instance)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L281) — Test listing supported languages when empty
  - `test_register_plugin_with_exception(self, mocker, plugin_manager_instance)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L259) — Test plugin registration with exception

## Functions
- `default_extractor()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L20) — Fixture for DefaultExtractor
- `plugin_manager_instance()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_coverage.py#L26) — Fixture for PluginManager

