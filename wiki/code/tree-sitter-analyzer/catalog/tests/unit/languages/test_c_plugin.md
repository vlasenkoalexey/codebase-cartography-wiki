---
title: 'Module: tests/unit/languages/test_c_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_c_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_c_plugin`/
symbols:
  TestCPluginLegacyTests.test_extractor_covers_elements_legacy: TestCPluginLegacyTests#test_extractor_covers_elements_legacy().
  TestCPluginLegacyTests.FakeNode: TestCPluginLegacyTests#FakeNode#
  TestCMacroDeduplication.test_macro_not_duplicated_across_ifdef_else: TestCMacroDeduplication#test_macro_not_duplicated_across_ifdef_else().
  TestCElementExtractor.test_extract_core_elements_success: TestCElementExtractor#test_extract_core_elements_success().
  TestCPluginIntegration.test_full_extraction_workflow: TestCPluginIntegration#test_full_extraction_workflow().
  TestCPluginIntegration.test_plugin_consistency: TestCPluginIntegration#test_plugin_consistency().
  TestMacroRedefinitionSurvives.test_both_definitions_extracted: TestMacroRedefinitionSurvives#test_both_definitions_extracted().
  TestCElementExtractor.test_extract_function_optimized: TestCElementExtractor#test_extract_function_optimized().
  TestCElementExtractor.test_extract_struct_optimized: TestCElementExtractor#test_extract_struct_optimized().
  TestCElementExtractor.test_extract_union_optimized: TestCElementExtractor#test_extract_union_optimized().
  TestCElementExtractor.test_extract_enum_optimized: TestCElementExtractor#test_extract_enum_optimized().
  TestCPlugin.test_analyze_file_nonexistent: TestCPlugin#test_analyze_file_nonexistent().
  TestCPluginErrorHandling.test_analyze_file_with_exception: TestCPluginErrorHandling#test_analyze_file_with_exception().
  TestCPluginIntegration.test_extractor_consistency: TestCPluginIntegration#test_extractor_consistency().
  TestCElementExtractor.test_extractor_initialization: TestCElementExtractor#test_extractor_initialization().
  TestCElementExtractor.test_extract_functions_no_language: TestCElementExtractor#test_extract_functions_no_language().
  TestCElementExtractor.test_extract_field_optimized: TestCElementExtractor#test_extract_field_optimized().
  TestCElementExtractor.test_calculate_complexity_optimized: TestCElementExtractor#test_calculate_complexity_optimized().
  TestCPlugin.test_plugin_initialization: TestCPlugin#test_plugin_initialization().
  TestCPlugin.test_get_tree_sitter_language: TestCPlugin#test_get_tree_sitter_language().
  TestCPlugin.test_get_tree_sitter_language_caching: TestCPlugin#test_get_tree_sitter_language_caching().
  TestCPlugin.test_analyze_file_success: TestCPlugin#test_analyze_file_success().
  TestCPluginErrorHandling.test_extract_functions_with_exception: TestCPluginErrorHandling#test_extract_functions_with_exception().
  TestCPluginErrorHandling.test_extract_classes_with_exception: TestCPluginErrorHandling#test_extract_classes_with_exception().
  TestCPluginErrorHandling.test_get_tree_sitter_language_failure: TestCPluginErrorHandling#test_get_tree_sitter_language_failure().
  TestCPluginIntegration.test_plugin_with_various_c_files: TestCPluginIntegration#test_plugin_with_various_c_files().
  TestCPluginLegacyTests.test_analyze_file_runs_legacy: TestCPluginLegacyTests#test_analyze_file_runs_legacy().
  TestCElementExtractor.extractor: TestCElementExtractor#extractor().
  TestCPlugin.plugin: TestCPlugin#plugin().
  TestCPluginErrorHandling.plugin: TestCPluginErrorHandling#plugin().
  TestCPluginErrorHandling.extractor: TestCPluginErrorHandling#extractor().
  TestCPluginIntegration.plugin: TestCPluginIntegration#plugin().
  FakeNode.end_byte: FakeNode#end_byte.
  TestCPluginLegacyTests.FakeNode.child_by_field_name: TestCPluginLegacyTests#FakeNode#child_by_field_name().
  TestMacroRedefinitionSurvives.CODE: TestMacroRedefinitionSurvives#CODE.
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode._fields: FakeNode#_fields.
  TestCPluginLegacyTests.make_tree: TestCPluginLegacyTests#make_tree().
  TestCElementExtractor: TestCElementExtractor#
  TestCElementExtractor.mock_tree: TestCElementExtractor#mock_tree().
  TestCElementExtractor.sample_c_code: TestCElementExtractor#sample_c_code().
  TestCPlugin: TestCPlugin#
  TestCPluginErrorHandling: TestCPluginErrorHandling#
  TestCPluginIntegration: TestCPluginIntegration#
  TestCPluginLegacyTests: TestCPluginLegacyTests#
  TestCPluginLegacyTests.FakeNode.__init__: TestCPluginLegacyTests#FakeNode#__init__().
  FakeNode._text: FakeNode#_text.
  FakeNode.children: FakeNode#children.
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.parent: FakeNode#parent.
  TestCMacroDeduplication: TestCMacroDeduplication#
  TestMacroRedefinitionSurvives: TestMacroRedefinitionSurvives#
---
# Module: [`tests/unit/languages/test_c_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_c_plugin.py:455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L455)
- doc: Fake node implementation for legacy tests
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name)` — [`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L485)
  - `children` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L473)
  - `end_byte` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L479)
  - `end_point` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L477)
  - `parent` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L483)
  - `start_byte` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L478)
  - `start_point` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L474)
- protocol/private: `__init__`[`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L458), `_fields`[`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L482), `_text`[`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L472)
- used by: (1 test-only callers)

### `TestCElementExtractor`
- def: [`tests/unit/languages/test_c_plugin.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L20)
- doc: Test cases for CElementExtractor class
- signature: `class TestCElementExtractor:`
- members:
  - `extractor(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L24) — Create a CElementExtractor instance for testing
  - `mock_tree(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L29) — Create a mock tree-sitter tree
  - `sample_c_code(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L39) — Sample C code for testing
  - `test_calculate_complexity_optimized(self, extractor: CElementExtractor)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L198) — Test complexity calculation
  - `test_extract_core_elements_success(self, extractor: CElementExtractor, mock_tree: Mock)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L96) — Test successful extraction of the core C element families.
  - `test_extract_enum_optimized(self, extractor: CElementExtractor)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L170) — Test optimized enum extraction
  - `test_extract_field_optimized(self, extractor: CElementExtractor)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L184) — Test field information extraction
  - `test_extract_function_optimized(self, extractor: CElementExtractor)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L128) — Test optimized function extraction
  - `test_extract_functions_no_language(self, extractor: CElementExtractor)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L115) — Test function extraction when language is not available
  - `test_extract_struct_optimized(self, extractor: CElementExtractor)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L142) — Test optimized struct extraction
  - `test_extract_union_optimized(self, extractor: CElementExtractor)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L156) — Test optimized union extraction
  - `test_extractor_initialization(self, extractor: CElementExtractor)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L87) — Test CElementExtractor initialization
- uses (calls/refs, reference-scoped): [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_classes), [`extract_variables`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_variables), [`_extract_function_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._extract_function_optimized), [`_extract_union_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._extract_union_optimized), [`extract_imports`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_imports), [`_extract_struct_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._extract_struct_optimized), [`_extract_enum_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._extract_enum_optimized), [`_extract_field_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._extract_field_optimized), [`_calculate_complexity_optimized`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._calculate_complexity_optimized)

### `TestCMacroDeduplication`
- def: [`tests/unit/languages/test_c_plugin.py:605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L605)
- doc: Macros defined identically in both #ifdef and #else branches appear once.
- signature: `class TestCMacroDeduplication:`
- members:
  - `test_macro_not_duplicated_across_ifdef_else(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L608) — SQUARE and LOG must appear exactly once even when defined in both
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_functions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_functions), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.get_tree_sitter_language), [`extractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.extractor)

### `TestCPlugin`
- def: [`tests/unit/languages/test_c_plugin.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L217)
- doc: Test cases for CPlugin class
- signature: `class TestCPlugin:`
- members:
  - `plugin(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L221) — Create a CPlugin instance for testing
  - `test_analyze_file_nonexistent(self, plugin: CPlugin)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L297) — Test analysis of non-existent file
  - `test_analyze_file_success(self, plugin: CPlugin)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L264) — Test successful file analysis
  - `test_get_tree_sitter_language(self, plugin: CPlugin)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L233) — Test getting tree-sitter language
  - `test_get_tree_sitter_language_caching(self, plugin: CPlugin)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L247) — Test tree-sitter language caching
  - `test_plugin_initialization(self, plugin: CPlugin)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L225) — Test CPlugin initialization
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.analyze_file), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.get_tree_sitter_language)

### `TestCPluginErrorHandling`
- def: [`tests/unit/languages/test_c_plugin.py:310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L310)
- doc: Test error handling in CPlugin
- signature: `class TestCPluginErrorHandling:`
- members:
  - `extractor(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L319) — Create a CElementExtractor instance for testing
  - `plugin(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L314) — Create a CPlugin instance for testing
  - `test_analyze_file_with_exception(self, plugin: CPlugin)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L361) — Test file analysis with exception
  - `test_extract_classes_with_exception(self, extractor: CElementExtractor)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L338) — Test class extraction with exception
  - `test_extract_functions_with_exception(self, extractor: CElementExtractor)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L323) — Test function extraction with exception
  - `test_get_tree_sitter_language_failure(self, plugin: CPlugin)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L351) — Test tree-sitter language loading failure
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`analyze_file`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.analyze_file), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_classes), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.get_tree_sitter_language)

### `TestCPluginIntegration`
- def: [`tests/unit/languages/test_c_plugin.py:387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L387)
- doc: Integration tests for CPlugin
- signature: `class TestCPluginIntegration:`
- members:
  - `plugin(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L391) — Create a CPlugin instance for testing
  - `test_extractor_consistency(self, plugin: CPlugin)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L416) — Test extractor consistency
  - `test_full_extraction_workflow(self, plugin: CPlugin)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L395) — Test complete extraction workflow
  - `test_plugin_consistency(self, plugin: CPlugin)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L409) — Test plugin consistency across multiple calls
  - `test_plugin_with_various_c_files(self, plugin: CPlugin)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L425) — Test plugin with various C file types
- uses (calls/refs, reference-scoped): [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`create_extractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.get_language_name)

### `TestCPluginLegacyTests`
- def: [`tests/unit/languages/test_c_plugin.py:452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L452)
- doc: Legacy test cases using FakeNode from original test_c directory
- signature: `class TestCPluginLegacyTests:`
- members:
  - `make_tree(root)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L489) — Create a simple tree with root node
  - `test_analyze_file_runs_legacy(self)` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L588) — Test analyze_file runs successfully on example file (legacy test)
  - `test_extractor_covers_elements_legacy(self)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L495) — Test extractor covers all element types with FakeNode (legacy test)
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.analyze_file), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_classes), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin), [`extract_variables`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_imports), [`import_statement`](../../../tree_sitter_analyzer/models/base.md#Import.import_statement)  (1 test-only)

### `TestMacroRedefinitionSurvives`
- def: [`tests/unit/languages/test_c_plugin.py:637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L637)
- doc: Codex P2 on #566: same-name dedup must NOT swallow a legitimate
- signature: `class TestMacroRedefinitionSurvives:`
- members:
  - `test_both_definitions_extracted(self)` — [`L649`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L649)
  - `CODE` — [`L641`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_plugin.py#L641)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_functions)

