---
title: 'Module: tests/unit/languages/test_javascript_plugin_extended.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_javascript_plugin_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_javascript_plugin_extended`/
symbols:
  TestJavaScriptElementExtractorExtended.test_extract_function_optimized_with_valid_node: TestJavaScriptElementExtractorExtended#test_extract_function_optimized_with_valid_node().
  TestJavaScriptElementExtractorExtended.test_extract_class_optimized_with_valid_node: TestJavaScriptElementExtractorExtended#test_extract_class_optimized_with_valid_node().
  TestJavaScriptElementExtractorExtended.test_extract_import_info_with_valid_node: TestJavaScriptElementExtractorExtended#test_extract_import_info_with_valid_node().
  TestJavaScriptElementExtractorExtended.test_extract_variable_info_with_valid_node: TestJavaScriptElementExtractorExtended#test_extract_variable_info_with_valid_node().
  TestJavaScriptPluginExtended.test_plugin_properties: TestJavaScriptPluginExtended#test_plugin_properties().
  TestJavaScriptPluginExtended.test_get_extractor: TestJavaScriptPluginExtended#test_get_extractor().
  TestJavaScriptElementExtractorExtended.test_extract_import_info_with_no_source: TestJavaScriptElementExtractorExtended#test_extract_import_info_with_no_source().
  TestJavaScriptPluginExtended.test_tree_sitter_language_caching: TestJavaScriptPluginExtended#test_tree_sitter_language_caching().
  TestJavaScriptPluginExtended.test_tree_sitter_language_loading: TestJavaScriptPluginExtended#test_tree_sitter_language_loading().
  TestJavaScriptPluginErrorHandling.test_extract_functions_without_language: TestJavaScriptPluginErrorHandling#test_extract_functions_without_language().
  TestJavaScriptPluginErrorHandling.test_extract_classes_without_language: TestJavaScriptPluginErrorHandling#test_extract_classes_without_language().
  TestJavaScriptPluginErrorHandling.test_extract_variables_without_language: TestJavaScriptPluginErrorHandling#test_extract_variables_without_language().
  TestJavaScriptPluginErrorHandling.test_extract_imports_without_language: TestJavaScriptPluginErrorHandling#test_extract_imports_without_language().
  extractor: extractor().
  TestJavaScriptElementExtractorExtended.mock_get_text: TestJavaScriptElementExtractorExtended#mock_get_text().
  TestJavaScriptElementExtractorExtended: TestJavaScriptElementExtractorExtended#
  TestJavaScriptElementExtractorExtended.test_extract_function_optimized_with_arrow_function: TestJavaScriptElementExtractorExtended#test_extract_function_optimized_with_arrow_function().
  TestJavaScriptElementExtractorExtended.test_extract_function_optimized_with_no_name: TestJavaScriptElementExtractorExtended#test_extract_function_optimized_with_no_name().
  TestJavaScriptElementExtractorExtended.test_extract_function_optimized_with_exception: TestJavaScriptElementExtractorExtended#test_extract_function_optimized_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_class_optimized_with_no_name: TestJavaScriptElementExtractorExtended#test_extract_class_optimized_with_no_name().
  TestJavaScriptElementExtractorExtended.test_extract_class_optimized_with_exception: TestJavaScriptElementExtractorExtended#test_extract_class_optimized_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_variable_info_with_no_name: TestJavaScriptElementExtractorExtended#test_extract_variable_info_with_no_name().
  TestJavaScriptElementExtractorExtended.test_extract_variable_info_with_exception: TestJavaScriptElementExtractorExtended#test_extract_variable_info_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_import_info_with_double_quotes: TestJavaScriptElementExtractorExtended#test_extract_import_info_with_double_quotes().
  TestJavaScriptElementExtractorExtended.test_extract_import_info_with_exception: TestJavaScriptElementExtractorExtended#test_extract_import_info_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_functions_with_language_available: TestJavaScriptElementExtractorExtended#test_extract_functions_with_language_available().
  TestJavaScriptElementExtractorExtended.test_extract_functions_with_exception: TestJavaScriptElementExtractorExtended#test_extract_functions_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_classes_with_exception: TestJavaScriptElementExtractorExtended#test_extract_classes_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_variables_with_exception: TestJavaScriptElementExtractorExtended#test_extract_variables_with_exception().
  TestJavaScriptElementExtractorExtended.test_extract_imports_with_exception: TestJavaScriptElementExtractorExtended#test_extract_imports_with_exception().
  TestJavaScriptPluginExtended: TestJavaScriptPluginExtended#
  TestJavaScriptPluginErrorHandling: TestJavaScriptPluginErrorHandling#
---
# Module: [`tests/unit/languages/test_javascript_plugin_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py)

## Classes
### `TestJavaScriptElementExtractorExtended`
- def: [`tests/unit/languages/test_javascript_plugin_extended.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L30)
- doc: Extended tests for JavaScript element extractor
- signature: `class TestJavaScriptElementExtractorExtended:`
- members:
  - `mock_get_text(node)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L68)
  - `test_extract_class_optimized_with_exception(self, extractor, mocker)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L199) — Test class info extraction with exception
  - `test_extract_class_optimized_with_no_name(self, extractor, mocker)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L190) — Test class info extraction with no name node
  - `test_extract_class_optimized_with_valid_node(self, extractor, mocker)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L161) — Test class info extraction with valid node
  - `test_extract_classes_with_exception(self, extractor, mocker)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L408) — Test class extraction with exception during query
  - `test_extract_function_optimized_with_arrow_function(self, extractor, mocker)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L91) — Test function info extraction with arrow function structure
  - `test_extract_function_optimized_with_exception(self, extractor, mocker)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L152) — Test function info extraction with exception
  - `test_extract_function_optimized_with_no_name(self, extractor, mocker)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L143) — Test function info extraction with no name node
  - `test_extract_function_optimized_with_valid_node(self, extractor, mocker)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L33) — Test function info extraction with valid node
  - `test_extract_functions_with_exception(self, extractor, mocker)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L395) — Test function extraction with exception during query
  - `test_extract_functions_with_language_available(self, extractor, mocker)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L374) — Test function extraction with language available
  - `test_extract_import_info_with_double_quotes(self, extractor, mocker)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L320) — Test import info extraction with double quotes
  - `test_extract_import_info_with_exception(self, extractor, mocker)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L361) — Test import info extraction with exception
  - `test_extract_import_info_with_no_source(self, extractor, mocker)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L347) — Test import info extraction with no source node
  - `test_extract_import_info_with_valid_node(self, extractor, mocker)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L289) — Test import info extraction with valid node
  - `test_extract_imports_with_exception(self, extractor, mocker)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L432) — Test import extraction with exception during query
  - `test_extract_variable_info_with_exception(self, extractor, mocker)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L271) — Test variable info extraction with exception
  - `test_extract_variable_info_with_no_name(self, extractor, mocker)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L250) — Test variable info extraction with no name node
  - `test_extract_variable_info_with_valid_node(self, extractor, mocker)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L208) — Test variable info extraction with valid node
  - `test_extract_variables_with_exception(self, extractor, mocker)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L420) — Test variable extraction with exception during query
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`module_path`](../../../tree_sitter_analyzer/models/base.md#Import.module_path)

### `TestJavaScriptPluginErrorHandling`
- def: [`tests/unit/languages/test_javascript_plugin_extended.py:491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L491)
- doc: Test error handling in JavaScript plugin
- signature: `class TestJavaScriptPluginErrorHandling:`
- members:
  - `test_extract_classes_without_language(self, mocker)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L504) — Test class extraction without language
  - `test_extract_functions_without_language(self, mocker)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L494) — Test function extraction without language
  - `test_extract_imports_without_language(self, mocker)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L524) — Test import extraction without language
  - `test_extract_variables_without_language(self, mocker)` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L514) — Test variable extraction without language
- uses (calls/refs, reference-scoped): [`JavaScriptElementExtractor`](../../../tree_sitter_analyzer/languages/javascript_plugin/extractor.md#JavaScriptElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_classes), [`extract_imports`](../../../tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_variables), [`extract_functions`](../../../tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_functions)

### `TestJavaScriptPluginExtended`
- def: [`tests/unit/languages/test_javascript_plugin_extended.py:445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L445)
- doc: Extended tests for JavaScript plugin
- signature: `class TestJavaScriptPluginExtended:`
- members:
  - `test_get_extractor(self)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L462) — Test get extractor method
  - `test_plugin_properties(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L448) — Test JavaScript plugin properties
  - `test_tree_sitter_language_caching(self)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L469) — Test tree-sitter language caching
  - `test_tree_sitter_language_loading(self)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L482) — Test tree-sitter language loading
- uses (calls/refs, reference-scoped): [`JavaScriptElementExtractor`](../../../tree_sitter_analyzer/languages/javascript_plugin/extractor.md#JavaScriptElementExtractor), [`JavaScriptPlugin`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_tree_sitter_language), [`get_extractor`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_extractor), [`get_language_name`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_language_name), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_file_extensions)

## Functions
- `extractor()` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extended.py#L25) — Fixture to provide JavaScriptElementExtractor instance

