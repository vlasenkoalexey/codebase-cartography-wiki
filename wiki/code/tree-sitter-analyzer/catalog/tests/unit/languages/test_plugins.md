---
title: 'Module: tests/unit/languages/test_plugins.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugins`/test_
symbols:
  test_register_plugin: register_plugin().
  test_java_extractor_initialization: java_extractor_initialization().
  test_javascript_extract_methods_return_lists: javascript_extract_methods_return_lists().
  test_get_plugin: get_plugin().
  test_java_plugin_properties: java_plugin_properties().
  test_java_plugin_extractor: java_plugin_extractor().
  test_javascript_plugin_properties: javascript_plugin_properties().
  test_javascript_plugin_extractor: javascript_plugin_extractor().
  test_get_nonexistent_plugin: get_nonexistent_plugin().
  test_java_plugin_tree_sitter_language: java_plugin_tree_sitter_language().
  test_extract_functions_with_mock_tree: extract_functions_with_mock_tree().
  test_extract_classes_with_mock_tree: extract_classes_with_mock_tree().
  test_extract_variables_with_mock_tree: extract_variables_with_mock_tree().
  test_extract_imports_with_mock_tree: extract_imports_with_mock_tree().
  test_plugin_manager_instance: plugin_manager_instance().
  test_javascript_extractor_methods_exist: javascript_extractor_methods_exist().
---
# Module: [`tests/unit/languages/test_plugins.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py)

## Functions
- `test_extract_classes_with_mock_tree(mocker)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L140) — Test class extraction with mock tree
- `test_extract_functions_with_mock_tree(mocker)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L119) — Test function extraction with mock tree
- `test_extract_imports_with_mock_tree(mocker)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L167) — Test import extraction with mock tree
- `test_extract_variables_with_mock_tree(mocker)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L154) — Test variable extraction with mock tree
- `test_get_nonexistent_plugin()` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L50) — Test getting nonexistent plugin returns None
- `test_get_plugin()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L40) — Test getting plugin by language
- `test_java_extractor_initialization()` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L109) — Test Java element extractor initialization
- `test_java_plugin_extractor()` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L69) — Test Java plugin element extractor
- `test_java_plugin_properties()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L58) — Test Java plugin basic properties
- `test_java_plugin_tree_sitter_language()` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L77) — Test Java plugin tree-sitter language loading
- `test_javascript_extract_methods_return_lists(mocker)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L190) — Test all extract methods return lists
- `test_javascript_extractor_methods_exist()` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L180) — Test JavaScript element extractor has required methods
- `test_javascript_plugin_extractor()` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L101) — Test JavaScript plugin element extractor
- `test_javascript_plugin_properties()` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L90) — Test JavaScript plugin basic properties
- `test_plugin_manager_instance()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L23) — Test plugin manager instance creation
- `test_register_plugin()` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins.py#L29) — Test plugin registration

