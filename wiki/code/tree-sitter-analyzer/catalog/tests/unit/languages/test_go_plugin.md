---
title: 'Module: tests/unit/languages/test_go_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_plugin`/
symbols:
  test_full_flow_go: test_full_flow_go().
  TestGoElementExtractor.test_reset_caches: TestGoElementExtractor#test_reset_caches().
  TestGoElementExtractorEdgeCases.test_empty_source_code: TestGoElementExtractorEdgeCases#test_empty_source_code().
  TestGoPluginIntegration.test_plugin_consistency: TestGoPluginIntegration#test_plugin_consistency().
  TestGoElementExtractor.test_extractor_has_go_specific_fields: TestGoElementExtractor#test_extractor_has_go_specific_fields().
  TestGoPluginIntegration.test_full_extraction_workflow: TestGoPluginIntegration#test_full_extraction_workflow().
  TestGoPlugin.test_get_tree_sitter_language_import_error: TestGoPlugin#test_get_tree_sitter_language_import_error().
  TestGoPlugin.test_analyze_file_success: TestGoPlugin#test_analyze_file_success().
  TestGoPlugin.test_analyze_file_nonexistent: TestGoPlugin#test_analyze_file_nonexistent().
  TestGoPlugin.test_analyze_file_integration: TestGoPlugin#test_analyze_file_integration().
  TestGoPluginIntegration.test_extractor_independence: TestGoPluginIntegration#test_extractor_independence().
  TestGoPlugin.test_plugin_initialization: TestGoPlugin#test_plugin_initialization().
  TestGoPlugin.test_get_supported_element_types: TestGoPlugin#test_get_supported_element_types().
  TestGoPlugin.test_get_queries: TestGoPlugin#test_get_queries().
  TestGoPlugin.test_get_tree_sitter_language_caching: TestGoPlugin#test_get_tree_sitter_language_caching().
  TestGoElementExtractor.test_extractor_initialization: TestGoElementExtractor#test_extractor_initialization().
  TestGoElementExtractor.test_extract_functions_returns_list: TestGoElementExtractor#test_extract_functions_returns_list().
  TestGoElementExtractor.test_extract_classes_returns_list: TestGoElementExtractor#test_extract_classes_returns_list().
  TestGoElementExtractor.test_extract_variables_returns_list: TestGoElementExtractor#test_extract_variables_returns_list().
  TestGoElementExtractor.test_extract_imports_returns_list: TestGoElementExtractor#test_extract_imports_returns_list().
  TestGoElementExtractor.test_extract_packages_returns_list: TestGoElementExtractor#test_extract_packages_returns_list().
  TestGoElementExtractorEdgeCases.test_unicode_source_code: TestGoElementExtractorEdgeCases#test_unicode_source_code().
  go_plugin: go_plugin().
  go_extractor: go_extractor().
  TestGoPluginIntegration.plugin: TestGoPluginIntegration#plugin().
  mock_tree: mock_tree().
  sample_go_code: sample_go_code().
  TestGoPlugin: TestGoPlugin#
  TestGoElementExtractor: TestGoElementExtractor#
  TestGoElementExtractorEdgeCases: TestGoElementExtractorEdgeCases#
  TestGoPluginIntegration: TestGoPluginIntegration#
---
# Module: [`tests/unit/languages/test_go_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py)

## Classes
### `TestGoElementExtractor`
- def: [`tests/unit/languages/test_go_plugin.py:222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L222)
- doc: Test cases for GoElementExtractor class.
- signature: `class TestGoElementExtractor:`
- members:
  - `test_extract_classes_returns_list(self, go_extractor: GoElementExtractor, mock_tree: Mock)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L267) — Test extract_classes returns a list.
  - `test_extract_functions_returns_list(self, go_extractor: GoElementExtractor, mock_tree: Mock)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L260) — Test extract_functions returns a list.
  - `test_extract_imports_returns_list(self, go_extractor: GoElementExtractor, mock_tree: Mock)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L281) — Test extract_imports returns a list.
  - `test_extract_packages_returns_list(self, go_extractor: GoElementExtractor, mock_tree: Mock)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L288) — Test extract_packages returns a list.
  - `test_extract_variables_returns_list(self, go_extractor: GoElementExtractor, mock_tree: Mock)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L274) — Test extract_variables returns a list.
  - `test_extractor_has_go_specific_fields(self, go_extractor: GoElementExtractor)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L235) — Test Go-specific extractor fields.
  - `test_extractor_initialization(self, go_extractor: GoElementExtractor)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L225) — Test GoElementExtractor initialization.
  - `test_reset_caches(self, go_extractor: GoElementExtractor)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L246) — Test cache reset.
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`GoElementExtractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_functions), [`extract_variables`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_variables), [`extract_packages`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_packages), [`extract_imports`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_imports), [`extract_classes`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_classes), [`_reset_caches`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._reset_caches), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._node_text_cache), [`channels`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.channels), [`defers`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.defers), [`goroutines`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.goroutines)

### `TestGoElementExtractorEdgeCases`
- def: [`tests/unit/languages/test_go_plugin.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L296)
- doc: Test edge cases for GoElementExtractor.
- signature: `class TestGoElementExtractorEdgeCases:`
- members:
  - `test_empty_source_code(self, go_extractor: GoElementExtractor)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L299) — Test extraction with empty source code.
  - `test_unicode_source_code(self, go_extractor: GoElementExtractor)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L317) — Test extraction with Unicode source code.
- uses (calls/refs, reference-scoped): [`GoElementExtractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_functions), [`extract_variables`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_variables), [`extract_packages`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_packages), [`extract_imports`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_imports), [`extract_classes`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_classes)

### `TestGoPlugin`
- def: [`tests/unit/languages/test_go_plugin.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L91)
- doc: Test cases for GoPlugin class.
- signature: `class TestGoPlugin:`
- members:
  - `test_analyze_file_integration(self, mock_parser_cls: Mock, mock_get_lang: Mock, go_plugin: GoPlugin)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L196) — Test file analysis integration.
  - `test_analyze_file_nonexistent(self, go_plugin: GoPlugin)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L181) — Test analysis of non-existent file.
  - `test_analyze_file_success(self, go_plugin: GoPlugin)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L151) — Test successful file analysis.
  - `test_get_queries(self, go_plugin: GoPlugin)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L118) — Test getting tree-sitter queries.
  - `test_get_supported_element_types(self, go_plugin: GoPlugin)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L102) — Test getting supported element types.
  - `test_get_tree_sitter_language_caching(self, go_plugin: GoPlugin)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L123) — Test tree-sitter language caching.
  - `test_get_tree_sitter_language_import_error(self, go_plugin: GoPlugin)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L141) — Test tree-sitter language loading failure.
  - `test_plugin_initialization(self, go_plugin: GoPlugin)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L94) — Test GoPlugin initialization.
- uses (calls/refs, reference-scoped): [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.analyze_file), [`GoPlugin`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.get_tree_sitter_language), [`_cached_language`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin._cached_language), [`get_queries`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.get_queries), [`get_supported_element_types`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.get_supported_element_types)

### `TestGoPluginIntegration`
- def: [`tests/unit/languages/test_go_plugin.py:335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L335)
- doc: Integration tests for GoPlugin.
- signature: `class TestGoPluginIntegration:`
- members:
  - `plugin(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L339) — Create a GoPlugin instance for testing.
  - `test_extractor_independence(self, plugin: GoPlugin)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L360) — Test that extractors are independent instances.
  - `test_full_extraction_workflow(self, plugin: GoPlugin)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L343) — Test complete extraction workflow.
  - `test_plugin_consistency(self, plugin: GoPlugin)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L353) — Test plugin consistency across multiple calls.
- uses (calls/refs, reference-scoped): [`GoElementExtractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`GoPlugin`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoPlugin.get_language_name)

## Functions
- `go_extractor()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L27) — Create a GoElementExtractor instance for testing.
- `go_plugin()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L21) — Create a GoPlugin instance for testing.
- `mock_tree()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L33) — Create a mock tree-sitter tree.
- `sample_go_code()` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L44) — Sample Go code for testing.
- `test_full_flow_go()` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_plugin.py#L371) — Basic integration test with sample code.

