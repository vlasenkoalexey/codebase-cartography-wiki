---
title: 'Module: tests/unit/languages/test_typescript_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_plugin`/TestTypeScript
symbols:
  TestTypeScriptElementExtractor.test_extractor_initialization: ElementExtractor#test_extractor_initialization().
  TestTypeScriptPluginIntegration.test_plugin_registration: PluginIntegration#test_plugin_registration().
  TestTypeScriptPluginIntegration.test_language_loader_integration: PluginIntegration#test_language_loader_integration().
  TestTypeScriptPluginIntegration.test_formatter_integration: PluginIntegration#test_formatter_integration().
  TestTypeScriptPluginIntegration.test_language_detection_integration: PluginIntegration#test_language_detection_integration().
  TestTypeScriptPlugin.test_plugin_initialization: Plugin#test_plugin_initialization().
  TestTypeScriptPlugin.test_analyze_file_no_tree_sitter: Plugin#test_analyze_file_no_tree_sitter().
  TestTypeScriptPlugin.test_analyze_file_no_language: Plugin#test_analyze_file_no_language().
  TestTypeScriptPlugin.test_analyze_file_missing_file: Plugin#test_analyze_file_missing_file().
  TestTypeScriptElementExtractor.extractor: ElementExtractor#extractor().
  TestTypeScriptPlugin.plugin: Plugin#plugin().
  TestTypeScriptPlugin.test_get_extractor: Plugin#test_get_extractor().
  TestTypeScriptPluginIntegration.plugin: PluginIntegration#plugin().
  TestTypeScriptElementExtractor: ElementExtractor#
  TestTypeScriptElementExtractor.mock_tree: ElementExtractor#mock_tree().
  TestTypeScriptElementExtractor.sample_typescript_code: ElementExtractor#sample_typescript_code().
  TestTypeScriptElementExtractor.test_detect_file_characteristics_module: ElementExtractor#test_detect_file_characteristics_module().
  TestTypeScriptElementExtractor.test_detect_file_characteristics_tsx: ElementExtractor#test_detect_file_characteristics_tsx().
  TestTypeScriptElementExtractor.test_detect_file_characteristics_angular: ElementExtractor#test_detect_file_characteristics_angular().
  TestTypeScriptElementExtractor.test_detect_file_characteristics_vue: ElementExtractor#test_detect_file_characteristics_vue().
  TestTypeScriptElementExtractor.test_reset_caches: ElementExtractor#test_reset_caches().
  TestTypeScriptElementExtractor.test_infer_type_from_value: ElementExtractor#test_infer_type_from_value().
  TestTypeScriptElementExtractor.test_clean_tsdoc: ElementExtractor#test_clean_tsdoc().
  TestTypeScriptElementExtractor.test_clean_tsdoc_empty: ElementExtractor#test_clean_tsdoc_empty().
  TestTypeScriptElementExtractor.test_extract_functions_empty_tree: ElementExtractor#test_extract_functions_empty_tree().
  TestTypeScriptElementExtractor.test_extract_classes_empty_tree: ElementExtractor#test_extract_classes_empty_tree().
  TestTypeScriptElementExtractor.test_extract_variables_empty_tree: ElementExtractor#test_extract_variables_empty_tree().
  TestTypeScriptElementExtractor.test_extract_imports_empty_tree: ElementExtractor#test_extract_imports_empty_tree().
  TestTypeScriptElementExtractor.test_is_framework_component_react: ElementExtractor#test_is_framework_component_react().
  TestTypeScriptElementExtractor.test_is_framework_component_angular: ElementExtractor#test_is_framework_component_angular().
  TestTypeScriptElementExtractor.test_is_framework_component_vue: ElementExtractor#test_is_framework_component_vue().
  TestTypeScriptElementExtractor.test_is_exported_class: ElementExtractor#test_is_exported_class().
  TestTypeScriptElementExtractor.test_calculate_complexity_optimized: ElementExtractor#test_calculate_complexity_optimized().
  TestTypeScriptPlugin: Plugin#
  TestTypeScriptPlugin.test_supported_queries: Plugin#test_supported_queries().
  TestTypeScriptPlugin.test_get_tree_sitter_language_caching: Plugin#test_get_tree_sitter_language_caching().
  TestTypeScriptPluginIntegration: PluginIntegration#
---
# Module: [`tests/unit/languages/test_typescript_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py)

## Classes
### `TestTypeScriptElementExtractor`
- def: [`tests/unit/languages/test_typescript_plugin.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L21)
- doc: Test cases for TypeScriptElementExtractor class
- signature: `class TestTypeScriptElementExtractor:`
- members:
  - `extractor(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L25) — Create a TypeScriptElementExtractor instance for testing
  - `mock_tree(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L30) — Create a mock tree-sitter tree
  - `sample_typescript_code(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L40) — Sample TypeScript code for testing
  - `test_calculate_complexity_optimized(self, extractor)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L312) — Cache hit returns the cached value; otherwise an AST-node walk.
  - `test_clean_tsdoc(self, extractor)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L237) — Test TSDoc comment cleaning
  - `test_clean_tsdoc_empty(self, extractor)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L249) — Test TSDoc cleaning with empty input
  - `test_detect_file_characteristics_angular(self, extractor)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L186) — Test detection of Angular framework
  - `test_detect_file_characteristics_module(self, extractor)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L170) — Test detection of TypeScript module characteristics
  - `test_detect_file_characteristics_tsx(self, extractor)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L178) — Test detection of TSX characteristics
  - `test_detect_file_characteristics_vue(self, extractor)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L193) — Test detection of Vue framework
  - `test_extract_classes_empty_tree(self, extractor, mock_tree)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L259) — Test class extraction with empty tree
  - `test_extract_functions_empty_tree(self, extractor, mock_tree)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L254) — Test function extraction with empty tree
  - `test_extract_imports_empty_tree(self, extractor, mock_tree)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L269) — Test import extraction with empty tree
  - `test_extract_variables_empty_tree(self, extractor, mock_tree)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L264) — Test variable extraction with empty tree
  - `test_extractor_initialization(self, extractor)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L158) — Test that extractor initializes properly
  - `test_infer_type_from_value(self, extractor)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L219) — Test TypeScript type inference from values
  - `test_is_exported_class(self, extractor)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L301) — Test exported class detection
  - `test_is_framework_component_angular(self, extractor)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L285) — Test Angular component detection
  - `test_is_framework_component_react(self, extractor)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L274) — Test React component detection
  - `test_is_framework_component_vue(self, extractor)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L293) — Test Vue component detection
  - `test_reset_caches(self, extractor)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L200) — Test cache reset functionality
- uses (calls/refs, reference-scoped): [`TypeScriptElementExtractor`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor), [`source_code`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.source_code), [`framework_type`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.framework_type), [`content_lines`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.content_lines), [`current_file`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.current_file), [`is_module`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.is_module), [`is_tsx`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.is_tsx), [`exports`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.exports), [`imports`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.imports)

### `TestTypeScriptPlugin`
- def: [`tests/unit/languages/test_typescript_plugin.py:342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L342)
- doc: Test cases for TypeScriptPlugin class
- signature: `class TestTypeScriptPlugin:`
- members:
  - `plugin(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L346) — Create a TypeScriptPlugin instance for testing
  - `test_analyze_file_missing_file(self, plugin)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L418) — Test file analysis with missing file
  - `test_analyze_file_no_language(self, mock_load_language, plugin)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L406) — Test file analysis when TypeScript language cannot be loaded
  - `test_analyze_file_no_tree_sitter(self, plugin)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L392) — Test file analysis when tree-sitter is not available
  - `test_get_extractor(self, plugin)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L355) — Test extractor getter
  - `test_get_tree_sitter_language_caching(self, plugin)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L428) — Test tree-sitter language caching
  - `test_plugin_initialization(self, plugin)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L350) — Test that plugin initializes properly
  - `test_supported_queries(self, plugin)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L360) — Test supported queries
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`TypeScriptElementExtractor`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor), [`TypeScriptPlugin`](../../../tree_sitter_analyzer/languages/typescript_plugin/plugin.md#TypeScriptPlugin)

### `TestTypeScriptPluginIntegration`
- def: [`tests/unit/languages/test_typescript_plugin.py:447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L447)
- doc: Integration tests for TypeScript plugin
- signature: `class TestTypeScriptPluginIntegration:`
- members:
  - `plugin(self)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L451) — Create a TypeScriptPlugin instance for testing
  - `test_formatter_integration(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L476) — Test TypeScript formatter integration
  - `test_language_detection_integration(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L494) — Test TypeScript language detection integration
  - `test_language_loader_integration(self)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L506) — Test TypeScript language loader integration
  - `test_plugin_registration(self)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin.py#L455) — Test that TypeScript plugin can be discovered by plugin manager
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`detect_from_extension`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension), [`detector`](../../../tree_sitter_analyzer/language_detector.md#detector), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`get_formatter_for_language`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`is_language_available`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.is_language_available), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`TypeScriptPlugin`](../../../tree_sitter_analyzer/languages/typescript_plugin/plugin.md#TypeScriptPlugin), [`get_loader`](../../../tree_sitter_analyzer/language_loader.md#get_loader), [`is_supported`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.is_supported), [`LANGUAGE_MODULES`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.LANGUAGE_MODULES), [`get_supported_languages`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.get_supported_languages), [`get_supported_languages`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_supported_languages)

