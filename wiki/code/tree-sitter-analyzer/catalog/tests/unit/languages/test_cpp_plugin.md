---
title: 'Module: tests/unit/languages/test_cpp_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_plugin`/
symbols:
  TestCppPluginLegacyTests.test_extractor_covers_elements_legacy: TestCppPluginLegacyTests#test_extractor_covers_elements_legacy().
  TestCppPluginLegacyTests.FakeNode: TestCppPluginLegacyTests#FakeNode#
  TestCppElementExtractor.test_extract_core_elements_success: TestCppElementExtractor#test_extract_core_elements_success().
  TestCppPluginIntegration.test_full_extraction_workflow: TestCppPluginIntegration#test_full_extraction_workflow().
  TestCppPluginIntegration.test_plugin_consistency: TestCppPluginIntegration#test_plugin_consistency().
  TestCppElementExtractor.test_extract_function_optimized: TestCppElementExtractor#test_extract_function_optimized().
  TestCppElementExtractor.test_extract_class_optimized: TestCppElementExtractor#test_extract_class_optimized().
  TestCppPlugin.test_analyze_file_nonexistent: TestCppPlugin#test_analyze_file_nonexistent().
  TestCppPluginErrorHandling.test_analyze_file_with_exception: TestCppPluginErrorHandling#test_analyze_file_with_exception().
  TestCppPluginIntegration.test_extractor_consistency: TestCppPluginIntegration#test_extractor_consistency().
  TestCppElementExtractor.test_extractor_initialization: TestCppElementExtractor#test_extractor_initialization().
  TestCppElementExtractor.test_extract_functions_no_language: TestCppElementExtractor#test_extract_functions_no_language().
  TestCppElementExtractor.test_extract_field_optimized: TestCppElementExtractor#test_extract_field_optimized().
  TestCppElementExtractor.test_calculate_complexity_optimized: TestCppElementExtractor#test_calculate_complexity_optimized().
  TestCppPlugin.test_plugin_initialization: TestCppPlugin#test_plugin_initialization().
  TestCppPlugin.test_get_tree_sitter_language: TestCppPlugin#test_get_tree_sitter_language().
  TestCppPlugin.test_get_tree_sitter_language_caching: TestCppPlugin#test_get_tree_sitter_language_caching().
  TestCppPlugin.test_analyze_file_success: TestCppPlugin#test_analyze_file_success().
  TestCppPluginErrorHandling.test_extract_functions_with_exception: TestCppPluginErrorHandling#test_extract_functions_with_exception().
  TestCppPluginErrorHandling.test_extract_classes_with_exception: TestCppPluginErrorHandling#test_extract_classes_with_exception().
  TestCppPluginErrorHandling.test_get_tree_sitter_language_failure: TestCppPluginErrorHandling#test_get_tree_sitter_language_failure().
  TestCppPluginIntegration.test_plugin_with_various_cpp_files: TestCppPluginIntegration#test_plugin_with_various_cpp_files().
  TestCppPluginLegacyTests.test_analyze_file_runs_legacy: TestCppPluginLegacyTests#test_analyze_file_runs_legacy().
  TestCppElementExtractor.extractor: TestCppElementExtractor#extractor().
  TestCppPlugin.plugin: TestCppPlugin#plugin().
  TestCppPluginErrorHandling.plugin: TestCppPluginErrorHandling#plugin().
  TestCppPluginErrorHandling.extractor: TestCppPluginErrorHandling#extractor().
  TestCppPluginIntegration.plugin: TestCppPluginIntegration#plugin().
  FakeNode.end_byte: FakeNode#end_byte.
  TestCppPluginLegacyTests.FakeNode.child_by_field_name: TestCppPluginLegacyTests#FakeNode#child_by_field_name().
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode._fields: FakeNode#_fields.
  TestCppPluginLegacyTests.make_tree: TestCppPluginLegacyTests#make_tree().
  TestCppElementExtractor: TestCppElementExtractor#
  TestCppElementExtractor.mock_tree: TestCppElementExtractor#mock_tree().
  TestCppElementExtractor.sample_cpp_code: TestCppElementExtractor#sample_cpp_code().
  TestCppPlugin: TestCppPlugin#
  TestCppPluginErrorHandling: TestCppPluginErrorHandling#
  TestCppPluginIntegration: TestCppPluginIntegration#
  TestCppPluginLegacyTests: TestCppPluginLegacyTests#
  TestCppPluginLegacyTests.FakeNode.__init__: TestCppPluginLegacyTests#FakeNode#__init__().
  FakeNode._text: FakeNode#_text.
  FakeNode.children: FakeNode#children.
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.parent: FakeNode#parent.
---
# Module: [`tests/unit/languages/test_cpp_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_cpp_plugin.py:438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L438)
- doc: Fake node implementation for legacy tests
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L468)
  - `children` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L456)
  - `end_byte` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L462)
  - `end_point` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L460)
  - `parent` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L466)
  - `start_byte` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L461)
  - `start_point` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L457)
- protocol/private: `__init__`[`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L441), `_fields`[`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L465), `_text`[`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L455)
- used by: (1 test-only callers)

### `TestCppElementExtractor`
- def: [`tests/unit/languages/test_cpp_plugin.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L20)
- doc: Test cases for CppElementExtractor class
- signature: `class TestCppElementExtractor:`
- members:
  - `extractor(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L24) — Create a CppElementExtractor instance for testing
  - `mock_tree(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L29) — Create a mock tree-sitter tree
  - `sample_cpp_code(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L39) — Sample C++ code for testing
  - `test_calculate_complexity_optimized(self, extractor: CppElementExtractor)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L173) — Test complexity calculation
  - `test_extract_class_optimized(self, extractor: CppElementExtractor)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L143) — Test optimized class extraction
  - `test_extract_core_elements_success(self, extractor: CppElementExtractor, mock_tree: Mock)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L94) — Test successful extraction of the core C++ element families.
  - `test_extract_field_optimized(self, extractor: CppElementExtractor)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L158) — Test field information extraction
  - `test_extract_function_optimized(self, extractor: CppElementExtractor)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L128) — Test optimized function extraction
  - `test_extract_functions_no_language(self, extractor: CppElementExtractor)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L113) — Test function extraction when language is not available
  - `test_extractor_initialization(self, extractor: CppElementExtractor)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L85) — Test CppElementExtractor initialization
- uses (calls/refs, reference-scoped): [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`_extract_function_optimized`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor._extract_function_optimized), [`extract_classes`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_classes), [`_extract_class_optimized`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor._extract_class_optimized), [`extract_functions`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_functions), [`extract_variables`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_variables), [`_extract_field_optimized`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor._extract_field_optimized), [`extract_imports`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_imports), [`_calculate_complexity_optimized`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor._calculate_complexity_optimized)

### `TestCppPlugin`
- def: [`tests/unit/languages/test_cpp_plugin.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L194)
- doc: Test cases for CppPlugin class
- signature: `class TestCppPlugin:`
- members:
  - `plugin(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L198) — Create a CppPlugin instance for testing
  - `test_analyze_file_nonexistent(self, plugin: CppPlugin)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L277) — Test analysis of non-existent file
  - `test_analyze_file_success(self, plugin: CppPlugin)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L244) — Test successful file analysis
  - `test_get_tree_sitter_language(self, plugin: CppPlugin)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L210) — Test getting tree-sitter language
  - `test_get_tree_sitter_language_caching(self, plugin: CppPlugin)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L224) — Test tree-sitter language caching
  - `test_plugin_initialization(self, plugin: CppPlugin)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L202) — Test CppPlugin initialization
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.analyze_file), [`CppPlugin`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.get_tree_sitter_language)

### `TestCppPluginErrorHandling`
- def: [`tests/unit/languages/test_cpp_plugin.py:290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L290)
- doc: Test error handling in CppPlugin
- signature: `class TestCppPluginErrorHandling:`
- members:
  - `extractor(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L299) — Create a CppElementExtractor instance for testing
  - `plugin(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L294) — Create a CppPlugin instance for testing
  - `test_analyze_file_with_exception(self, plugin: CppPlugin)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L343) — Test file analysis with exception
  - `test_extract_classes_with_exception(self, extractor: CppElementExtractor)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L318) — Test class extraction with exception
  - `test_extract_functions_with_exception(self, extractor: CppElementExtractor)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L303) — Test function extraction with exception
  - `test_get_tree_sitter_language_failure(self, plugin: CppPlugin)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L333) — Test tree-sitter language loading failure
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.analyze_file), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_functions), [`CppPlugin`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.get_tree_sitter_language)

### `TestCppPluginIntegration`
- def: [`tests/unit/languages/test_cpp_plugin.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L369)
- doc: Integration tests for CppPlugin
- signature: `class TestCppPluginIntegration:`
- members:
  - `plugin(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L373) — Create a CppPlugin instance for testing
  - `test_extractor_consistency(self, plugin: CppPlugin)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L398) — Test extractor consistency
  - `test_full_extraction_workflow(self, plugin: CppPlugin)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L377) — Test complete extraction workflow
  - `test_plugin_consistency(self, plugin: CppPlugin)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L391) — Test plugin consistency across multiple calls
  - `test_plugin_with_various_cpp_files(self, plugin: CppPlugin)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L407) — Test plugin with various C++ file types
- uses (calls/refs, reference-scoped): [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`CppPlugin`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`create_extractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.get_language_name)

### `TestCppPluginLegacyTests`
- def: [`tests/unit/languages/test_cpp_plugin.py:435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L435)
- doc: Legacy test cases using FakeNode from original test_cpp directory
- signature: `class TestCppPluginLegacyTests:`
- members:
  - `make_tree(root)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L472) — Create a simple tree with root node
  - `test_analyze_file_runs_legacy(self)` — [`L606`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L606) — Test analyze_file runs successfully on example file (legacy test)
  - `test_extractor_covers_elements_legacy(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin.py#L478) — Test extractor covers all element types with FakeNode (legacy test)
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.analyze_file), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_functions), [`CppPlugin`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin), [`extract_variables`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_imports), [`import_statement`](../../../tree_sitter_analyzer/models/base.md#Import.import_statement)  (1 test-only)

