---
title: 'Module: tests/unit/languages/test_plugins_base_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugins_base_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugins_base_advanced`/Test
symbols:
  TestLanguagePluginIntegration.test_plugin_workflow: LanguagePluginIntegration#test_plugin_workflow().
  TestLanguagePluginIntegration.test_plugin_with_empty_extensions: LanguagePluginIntegration#test_plugin_with_empty_extensions().
  TestEdgeCases.test_extractor_with_malformed_nodes: EdgeCases#test_extractor_with_malformed_nodes().
  TestEdgeCases.test_plugin_with_special_characters_in_filename: EdgeCases#test_plugin_with_special_characters_in_filename().
  TestEdgeCases.test_extractor_with_empty_source_code: EdgeCases#test_extractor_with_empty_source_code().
  TestEdgeCases.test_extractor_with_very_large_source_code: EdgeCases#test_extractor_with_very_large_source_code().
  TestDefaultExtractorTraversal.extractor: DefaultExtractorTraversal#extractor().
  TestDefaultExtractorTraversal.test_traverse_for_classes_creates_element: DefaultExtractorTraversal#test_traverse_for_classes_creates_element().
  TestDefaultExtractorTraversal.test_traverse_for_classes_recursive: DefaultExtractorTraversal#test_traverse_for_classes_recursive().
  TestDefaultExtractorTraversal.test_traverse_for_variables_creates_element: DefaultExtractorTraversal#test_traverse_for_variables_creates_element().
  TestDefaultExtractorTraversal.test_traverse_for_variables_recursive: DefaultExtractorTraversal#test_traverse_for_variables_recursive().
  TestDefaultExtractorTraversal.test_traverse_for_imports_creates_element: DefaultExtractorTraversal#test_traverse_for_imports_creates_element().
  TestDefaultExtractorTraversal.test_traverse_for_imports_recursive: DefaultExtractorTraversal#test_traverse_for_imports_recursive().
  TestDefaultExtractorErrorPaths.extractor: DefaultExtractorErrorPaths#extractor().
  TestLanguagePluginIntegration: LanguagePluginIntegration#
  TestEdgeCases: EdgeCases#
  TestDefaultExtractorTraversal: DefaultExtractorTraversal#
  TestDefaultExtractorTraversal.test_traverse_for_classes_error_handling: DefaultExtractorTraversal#test_traverse_for_classes_error_handling().
  TestDefaultExtractorTraversal.test_traverse_for_classes_skips_non_class_nodes: DefaultExtractorTraversal#test_traverse_for_classes_skips_non_class_nodes().
  TestDefaultExtractorErrorPaths: DefaultExtractorErrorPaths#
  TestDefaultExtractorErrorPaths.test_traverse_for_classes_exception_logged: DefaultExtractorErrorPaths#test_traverse_for_classes_exception_logged().
  TestDefaultExtractorErrorPaths.test_traverse_for_variables_exception_logged: DefaultExtractorErrorPaths#test_traverse_for_variables_exception_logged().
  TestDefaultExtractorErrorPaths.test_traverse_for_imports_exception_logged: DefaultExtractorErrorPaths#test_traverse_for_imports_exception_logged().
  TestDefaultExtractorErrorPaths.test_traverse_for_functions_exception_logged: DefaultExtractorErrorPaths#test_traverse_for_functions_exception_logged().
  TestDefaultExtractorErrorPaths.test_extract_node_text_encoding_error: DefaultExtractorErrorPaths#test_extract_node_text_encoding_error().
  TestDefaultExtractorErrorPaths.test_extract_node_text_missing_attrs: DefaultExtractorErrorPaths#test_extract_node_text_missing_attrs().
---
# Module: [`tests/unit/languages/test_plugins_base_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py)

## Classes
### `TestDefaultExtractorErrorPaths`
- def: [`tests/unit/languages/test_plugins_base_advanced.py:297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L297)
- doc: Coverage for exception-handling branches in extractor methods
- signature: `class TestDefaultExtractorErrorPaths:`
- members:
  - `extractor(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L301)
  - `test_extract_node_text_encoding_error(self, extractor)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L364) — _extract_node_text returns '' on encoding/decoding errors
  - `test_extract_node_text_missing_attrs(self, extractor)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L375) — _extract_node_text returns '' when node lacks start_byte/end_byte
  - `test_traverse_for_classes_exception_logged(self, extractor)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L304) — Exception in _traverse_for_classes body is caught and logged
  - `test_traverse_for_functions_exception_logged(self, extractor)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L349) — Exception in _traverse_for_functions body is caught and logged
  - `test_traverse_for_imports_exception_logged(self, extractor)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L334) — Exception in _traverse_for_imports body is caught and logged
  - `test_traverse_for_variables_exception_logged(self, extractor)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L319) — Exception in _traverse_for_variables body is caught and logged
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor)

### `TestDefaultExtractorTraversal`
- def: [`tests/unit/languages/test_plugins_base_advanced.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L123)
- doc: Direct tests for _traverse_for_* methods in DefaultExtractor
- signature: `class TestDefaultExtractorTraversal:`
- members:
  - `extractor(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L127)
  - `test_traverse_for_classes_creates_element(self, extractor)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L132) — _traverse_for_classes should create and append a Class element
  - `test_traverse_for_classes_error_handling(self, extractor)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L151) — _traverse_for_classes should not raise on extraction errors
  - `test_traverse_for_classes_recursive(self, extractor)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L166) — _traverse_for_classes should recurse into children
  - `test_traverse_for_classes_skips_non_class_nodes(self, extractor)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L191) — _traverse_for_classes should skip nodes that are not class-like
  - `test_traverse_for_imports_creates_element(self, extractor)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L252) — _traverse_for_imports should create and append an Import element
  - `test_traverse_for_imports_recursive(self, extractor)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L271) — _traverse_for_imports should recurse into children
  - `test_traverse_for_variables_creates_element(self, extractor)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L204) — _traverse_for_variables should create and append a Variable element
  - `test_traverse_for_variables_recursive(self, extractor)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L225) — _traverse_for_variables should recurse into children
- uses (calls/refs, reference-scoped): [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor)

### `TestEdgeCases`
- def: [`tests/unit/languages/test_plugins_base_advanced.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L59)
- doc: Test edge cases and error conditions
- signature: `class TestEdgeCases:`
- members:
  - `test_extractor_with_empty_source_code(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L94) — Test extractor with empty source code
  - `test_extractor_with_malformed_nodes(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L62) — Test extractor with malformed tree nodes
  - `test_extractor_with_very_large_source_code(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L107) — Test extractor with large source code
  - `test_plugin_with_special_characters_in_filename(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L83) — Test plugin with special characters in filename
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`DefaultLanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin), [`extract_all_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_all_elements), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_functions)

### `TestLanguagePluginIntegration`
- def: [`tests/unit/languages/test_plugins_base_advanced.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L17)
- doc: Integration tests for LanguagePlugin
- signature: `class TestLanguagePluginIntegration:`
- members:
  - `test_plugin_with_empty_extensions(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L42) — Test plugin behavior with empty extensions
  - `test_plugin_workflow(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_advanced.py#L20) — Test complete plugin workflow
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`DefaultLanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_language_name)

