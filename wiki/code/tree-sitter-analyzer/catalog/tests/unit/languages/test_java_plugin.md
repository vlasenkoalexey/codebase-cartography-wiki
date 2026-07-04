---
title: 'Module: tests/unit/languages/test_java_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_plugin`/TestJava
symbols:
  TestJavaElementExtractor.test_extract_core_elements_success: ElementExtractor#test_extract_core_elements_success().
  TestJavaPluginIntegration.test_full_extraction_workflow: PluginIntegration#test_full_extraction_workflow().
  TestJavaPluginIntegration.test_plugin_consistency: PluginIntegration#test_plugin_consistency().
  TestJavaElementExtractor.test_extract_method_optimized: ElementExtractor#test_extract_method_optimized().
  TestJavaElementExtractor.test_extract_class_optimized: ElementExtractor#test_extract_class_optimized().
  TestJavaElementExtractor.test_extract_import_info: ElementExtractor#test_extract_import_info().
  TestJavaPlugin.test_analyze_file_nonexistent: Plugin#test_analyze_file_nonexistent().
  TestJavaPluginErrorHandling.test_analyze_file_with_exception: PluginErrorHandling#test_analyze_file_with_exception().
  TestJavaPluginIntegration.test_extractor_consistency: PluginIntegration#test_extractor_consistency().
  TestJavaElementExtractor.test_extractor_initialization: ElementExtractor#test_extractor_initialization().
  TestJavaElementExtractor.test_extract_functions_no_language: ElementExtractor#test_extract_functions_no_language().
  TestJavaElementExtractor.test_extract_field_optimized: ElementExtractor#test_extract_field_optimized().
  TestJavaElementExtractor.test_extract_class_name: ElementExtractor#test_extract_class_name().
  TestJavaElementExtractor.test_extract_class_name_no_identifier: ElementExtractor#test_extract_class_name_no_identifier().
  TestJavaElementExtractor.test_calculate_complexity_optimized: ElementExtractor#test_calculate_complexity_optimized().
  TestJavaPlugin.test_plugin_initialization: Plugin#test_plugin_initialization().
  TestJavaPlugin.test_get_tree_sitter_language: Plugin#test_get_tree_sitter_language().
  TestJavaPlugin.test_get_tree_sitter_language_caching: Plugin#test_get_tree_sitter_language_caching().
  TestJavaPlugin.test_analyze_file_success: Plugin#test_analyze_file_success().
  TestJavaPluginErrorHandling.test_extract_functions_with_exception: PluginErrorHandling#test_extract_functions_with_exception().
  TestJavaPluginErrorHandling.test_extract_classes_with_exception: PluginErrorHandling#test_extract_classes_with_exception().
  TestJavaPluginErrorHandling.test_extract_method_optimized_with_exception: PluginErrorHandling#test_extract_method_optimized_with_exception().
  TestJavaPluginErrorHandling.test_get_tree_sitter_language_failure: PluginErrorHandling#test_get_tree_sitter_language_failure().
  TestJavaPluginIntegration.test_plugin_with_various_java_files: PluginIntegration#test_plugin_with_various_java_files().
  TestJavaElementExtractor.extractor: ElementExtractor#extractor().
  TestJavaPlugin.plugin: Plugin#plugin().
  TestJavaPluginErrorHandling.plugin: PluginErrorHandling#plugin().
  TestJavaPluginErrorHandling.extractor: PluginErrorHandling#extractor().
  TestJavaPluginIntegration.plugin: PluginIntegration#plugin().
  TestJavaElementExtractor: ElementExtractor#
  TestJavaElementExtractor.mock_tree: ElementExtractor#mock_tree().
  TestJavaElementExtractor.sample_java_code: ElementExtractor#sample_java_code().
  TestJavaPlugin: Plugin#
  TestJavaPluginErrorHandling: PluginErrorHandling#
  TestJavaPluginIntegration: PluginIntegration#
---
# Module: [`tests/unit/languages/test_java_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py)

## Classes
### `TestJavaElementExtractor`
- def: [`tests/unit/languages/test_java_plugin.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L20)
- doc: Test cases for JavaElementExtractor class
- signature: `class TestJavaElementExtractor:`
- members:
  - `extractor(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L24) — Create a JavaElementExtractor instance for testing
  - `mock_tree(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L29) — Create a mock tree-sitter tree
  - `sample_java_code(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L39) — Sample Java code for testing
  - `test_calculate_complexity_optimized(self, extractor: JavaElementExtractor)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L212) — Test complexity calculation
  - `test_extract_class_name(self, extractor: JavaElementExtractor)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L185) — Test class name extraction from node
  - `test_extract_class_name_no_identifier(self, extractor: JavaElementExtractor)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L201) — Test class name extraction when no identifier is found
  - `test_extract_class_optimized(self, extractor: JavaElementExtractor)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L140) — Test optimized class extraction
  - `test_extract_core_elements_success(self, extractor: JavaElementExtractor, mock_tree: Mock)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L90) — Test successful extraction of the core Java element families.
  - `test_extract_field_optimized(self, extractor: JavaElementExtractor)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L155) — Test field information extraction
  - `test_extract_functions_no_language(self, extractor: JavaElementExtractor)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L109) — Test function extraction when language is not available
  - `test_extract_import_info(self, extractor: JavaElementExtractor)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L170) — Test import information extraction
  - `test_extract_method_optimized(self, extractor: JavaElementExtractor)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L125) — Test optimized method extraction
  - `test_extractor_initialization(self, extractor: JavaElementExtractor)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L81) — Test JavaElementExtractor initialization
- uses (calls/refs, reference-scoped): [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_classes), [`_extract_class_optimized`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_class_optimized), [`_extract_method_optimized`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_method_optimized), [`extract_variables`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_variables), [`extract_functions`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_functions), [`_extract_field_optimized`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_field_optimized), [`extract_imports`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_imports), [`_extract_import_info`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_import_info), [`_extract_class_name`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_class_name), [`_calculate_complexity_optimized`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._calculate_complexity_optimized)

### `TestJavaPlugin`
- def: [`tests/unit/languages/test_java_plugin.py:238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L238)
- doc: Test cases for JavaPlugin class
- signature: `class TestJavaPlugin:`
- members:
  - `plugin(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L242) — Create a JavaPlugin instance for testing
  - `test_analyze_file_nonexistent(self, plugin: JavaPlugin)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L322) — Test analysis of non-existent file
  - `test_analyze_file_success(self, plugin: JavaPlugin)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L289) — Test successful file analysis
  - `test_get_tree_sitter_language(self, plugin: JavaPlugin)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L254) — Test getting tree-sitter language
  - `test_get_tree_sitter_language_caching(self, plugin: JavaPlugin)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L268) — Test tree-sitter language caching
  - `test_plugin_initialization(self, plugin: JavaPlugin)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L246) — Test JavaPlugin initialization
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.analyze_file), [`JavaPlugin`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.get_tree_sitter_language)

### `TestJavaPluginErrorHandling`
- def: [`tests/unit/languages/test_java_plugin.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L336)
- doc: Test error handling in JavaPlugin
- signature: `class TestJavaPluginErrorHandling:`
- members:
  - `extractor(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L345) — Create a JavaElementExtractor instance for testing
  - `plugin(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L340) — Create a JavaPlugin instance for testing
  - `test_analyze_file_with_exception(self, plugin: JavaPlugin)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L414) — Test file analysis with exception
  - `test_extract_classes_with_exception(self, extractor: JavaElementExtractor)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L366) — Test class extraction with exception
  - `test_extract_functions_with_exception(self, extractor: JavaElementExtractor)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L349) — Test function extraction with exception
  - `test_extract_method_optimized_with_exception(self, extractor: JavaElementExtractor)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L383) — Test optimized method extraction with exception
  - `test_get_tree_sitter_language_failure(self, plugin: JavaPlugin)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L404) — Test tree-sitter language loading failure
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`analyze_file`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.analyze_file), [`JavaPlugin`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin), [`extract_classes`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_classes), [`_extract_method_optimized`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._extract_method_optimized), [`extract_functions`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_functions), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.get_tree_sitter_language)

### `TestJavaPluginIntegration`
- def: [`tests/unit/languages/test_java_plugin.py:443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L443)
- doc: Integration tests for JavaPlugin
- signature: `class TestJavaPluginIntegration:`
- members:
  - `plugin(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L447) — Create a JavaPlugin instance for testing
  - `test_extractor_consistency(self, plugin: JavaPlugin)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L476) — Test extractor consistency
  - `test_full_extraction_workflow(self, plugin: JavaPlugin)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L451) — Test complete extraction workflow
  - `test_plugin_consistency(self, plugin: JavaPlugin)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L468) — Test plugin consistency across multiple calls
  - `test_plugin_with_various_java_files(self, plugin: JavaPlugin)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_plugin.py#L486) — Test plugin with various Java file types
- uses (calls/refs, reference-scoped): [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`JavaPlugin`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`create_extractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.get_language_name)

