---
title: 'Module: tests/unit/languages/test_kotlin_target_75.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_target_75.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_target_75`/T
symbols:
  TestKotlinExtractorMissingLines.test_extract_function_name_from_children_fallback: estKotlinExtractorMissingLines#test_extract_function_name_from_children_fallback().
  TestKotlinExtractorMissingLines.test_extract_function_with_parameters_node_mock: estKotlinExtractorMissingLines#test_extract_function_with_parameters_node_mock().
  TestKotlinExtractorMissingLines.test_extract_function_return_type_with_colon: estKotlinExtractorMissingLines#test_extract_function_return_type_with_colon().
  TestKotlinExtractorMissingLines.test_extract_class_name_from_children_fallback: estKotlinExtractorMissingLines#test_extract_class_name_from_children_fallback().
  TestKotlinExtractorMissingLines.test_extract_class_visibility_from_modifiers: estKotlinExtractorMissingLines#test_extract_class_visibility_from_modifiers().
  TestKotlinExtractorMissingLines.test_extract_class_protected_visibility: estKotlinExtractorMissingLines#test_extract_class_protected_visibility().
  TestKotlinExtractorMissingLines.test_extract_class_internal_visibility: estKotlinExtractorMissingLines#test_extract_class_internal_visibility().
  TestKotlinPluginMissingLines.test_analyze_file_without_tree_sitter_language: estKotlinPluginMissingLines#test_analyze_file_without_tree_sitter_language().
  TestKotlinExtractorMissingLines.test_extract_package_with_identifier_type: estKotlinExtractorMissingLines#test_extract_package_with_identifier_type().
  TestKotlinExtractorErrorHandling.test_extract_class_with_exception: estKotlinExtractorErrorHandling#test_extract_class_with_exception().
  TestKotlinExtractorErrorHandling.test_get_node_text_with_exception: estKotlinExtractorErrorHandling#test_get_node_text_with_exception().
  TestKotlinPropertyExtraction.test_extract_property_val: estKotlinPropertyExtraction#test_extract_property_val().
  TestKotlinPropertyExtraction.test_extract_property_var: estKotlinPropertyExtraction#test_extract_property_var().
  TestKotlinPluginParserVariants.test_plugin_with_parser_language_attribute: estKotlinPluginParserVariants#test_plugin_with_parser_language_attribute().
  TestKotlinPluginParserVariants.test_plugin_creates_correct_extractor: estKotlinPluginParserVariants#test_plugin_creates_correct_extractor().
  TestKotlinExtractorErrorHandling.test_extract_function_with_exception: estKotlinExtractorErrorHandling#test_extract_function_with_exception().
  TREE_SITTER_KOTLIN_AVAILABLE: REE_SITTER_KOTLIN_AVAILABLE.
  TestKotlinPluginMissingLines.test_get_tree_sitter_language_import_error: estKotlinPluginMissingLines#test_get_tree_sitter_language_import_error().
  TestKotlinPluginMissingLines.test_extract_elements_exception_handling: estKotlinPluginMissingLines#test_extract_elements_exception_handling().
  TestKotlinTreeSitterSpecificBranches: estKotlinTreeSitterSpecificBranches#
  TestKotlinTreeSitterSpecificBranches.plugin: estKotlinTreeSitterSpecificBranches#plugin().
  TestKotlinExtractorMissingLines: estKotlinExtractorMissingLines#
  TestKotlinPluginMissingLines: estKotlinPluginMissingLines#
  TestKotlinTreeSitterSpecificBranches.parser: estKotlinTreeSitterSpecificBranches#parser().
  TestKotlinTreeSitterSpecificBranches.test_package_with_deeply_nested_identifier: estKotlinTreeSitterSpecificBranches#test_package_with_deeply_nested_identifier().
  TestKotlinTreeSitterSpecificBranches.test_function_with_no_name_field: estKotlinTreeSitterSpecificBranches#test_function_with_no_name_field().
  TestKotlinTreeSitterSpecificBranches.test_function_with_complex_parameters: estKotlinTreeSitterSpecificBranches#test_function_with_complex_parameters().
  TestKotlinTreeSitterSpecificBranches.test_class_without_name_node_field: estKotlinTreeSitterSpecificBranches#test_class_without_name_node_field().
  TestKotlinTreeSitterSpecificBranches.test_class_with_all_visibility_modifiers: estKotlinTreeSitterSpecificBranches#test_class_with_all_visibility_modifiers().
  TestKotlinTreeSitterSpecificBranches.test_interface_vs_class_detection: estKotlinTreeSitterSpecificBranches#test_interface_vs_class_detection().
  TestKotlinPluginParserVariants: estKotlinPluginParserVariants#
  TestKotlinExtractorErrorHandling: estKotlinExtractorErrorHandling#
  TestKotlinPropertyExtraction: estKotlinPropertyExtraction#
---
# Module: [`tests/unit/languages/test_kotlin_target_75.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py)

## Classes
### `TestKotlinExtractorErrorHandling`
- def: [`tests/unit/languages/test_kotlin_target_75.py:509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L509)
- doc: Test error handling in extractor methods.
- signature: `class TestKotlinExtractorErrorHandling:`
- members:
  - `test_extract_class_with_exception(self)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L524) — Test _extract_class_or_object handles exceptions (lines 401-403).
  - `test_extract_function_with_exception(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L512) — Test _extract_function handles exceptions (lines 385-386, 388-389).
  - `test_get_node_text_with_exception(self)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L537) — Test _get_node_text handles exceptions (line 468-469).
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`_get_node_text`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._get_node_text), [`content_lines`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.content_lines), [`_extract_class_or_object`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_class_or_object), [`_extract_function`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_function), [`current_package`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.current_package), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._node_text_cache)

### `TestKotlinExtractorMissingLines`
- def: [`tests/unit/languages/test_kotlin_target_75.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L24)
- doc: Test to cover missing lines in KotlinElementExtractor.
- signature: `class TestKotlinExtractorMissingLines:`
- members:
  - `test_extract_class_internal_visibility(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L272) — Test _extract_class_or_object internal visibility.
  - `test_extract_class_name_from_children_fallback(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L163) — Test _extract_class_or_object when name_node is None (lines 311-314).
  - `test_extract_class_protected_visibility(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L232) — Test _extract_class_or_object protected visibility.
  - `test_extract_class_visibility_from_modifiers(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L191) — Test _extract_class_or_object visibility extraction (lines 322-328).
  - `test_extract_function_name_from_children_fallback(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L54) — Test _extract_function when name_node is None (lines 205-208).
  - `test_extract_function_return_type_with_colon(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L128) — Test _extract_function return type extraction (lines 258-267).
  - `test_extract_function_with_parameters_node_mock(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L80) — Test _extract_function tolerates a mocked parameters node.
  - `test_extract_package_with_identifier_type(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L27) — Test _extract_package when grandchild has 'identifier' in type (line 191-192).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`_get_node_text`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._get_node_text), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Class.visibility), [`content_lines`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.content_lines), [`_extract_class_or_object`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_class_or_object), [`_extract_function`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_function), [`current_package`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.current_package), [`_extract_package`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_package)

### `TestKotlinPluginMissingLines`
- def: [`tests/unit/languages/test_kotlin_target_75.py:313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L313)
- doc: Test to cover missing lines in KotlinPlugin.
- signature: `class TestKotlinPluginMissingLines:`
- members:
  - `test_analyze_file_without_tree_sitter_language(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L316) — Test analyze_file when get_tree_sitter_language returns None (lines 515, 529, 533).
  - `test_extract_elements_exception_handling(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L353) — Test extract_elements exception handling (lines 642-644, 654).
  - `test_get_tree_sitter_language_import_error(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L343) — Test get_tree_sitter_language when tree-sitter-kotlin is not available (line 604).
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`analyze_file`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin.analyze_file), [`KotlinPlugin`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin), [`extract_elements`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin.extract_elements), [`_cached_language`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin._cached_language)

### `TestKotlinPluginParserVariants`
- def: [`tests/unit/languages/test_kotlin_target_75.py:477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L477)
- doc: Test parser setup variations.
- signature: `class TestKotlinPluginParserVariants:`
- members:
  - `test_plugin_creates_correct_extractor(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L501) — Test that create_extractor returns KotlinElementExtractor.
  - `test_plugin_with_parser_language_attribute(self)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L480) — Test parser setup when parser has 'language' attribute (line 529).
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`KotlinPlugin`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin.create_extractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin.get_tree_sitter_language)  (1 test-only)

### `TestKotlinPropertyExtraction`
- def: [`tests/unit/languages/test_kotlin_target_75.py:553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L553)
- doc: Test property extraction edge cases.
- signature: `class TestKotlinPropertyExtraction:`
- members:
  - `test_extract_property_val(self)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L556) — Test extracting val property.
  - `test_extract_property_var(self)` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L574) — Test extracting var property.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`_get_node_text`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._get_node_text), [`content_lines`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.content_lines), [`_extract_property`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_property)

### `TestKotlinTreeSitterSpecificBranches`
- def: [`tests/unit/languages/test_kotlin_target_75.py:378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L378)
- doc: Test specific branches that need real tree-sitter parsing.
- signature: `class TestKotlinTreeSitterSpecificBranches:`
- members:
  - `parser(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L386)
  - `plugin(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L382)
  - `test_class_with_all_visibility_modifiers(self, plugin, parser)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L437) — Test class with all visibility modifiers.
  - `test_class_without_name_node_field(self, plugin, parser)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L424) — Test object expression (anonymous class).
  - `test_function_with_complex_parameters(self, plugin, parser)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L412) — Test function with varargs and defaults.
  - `test_function_with_no_name_field(self, plugin, parser)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L402) — Test anonymous function handling.
  - `test_interface_vs_class_detection(self, plugin, parser)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L456) — Test that interface is properly detected vs class.
  - `test_package_with_deeply_nested_identifier(self, plugin, parser)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L390) — Test package extraction with nested structure.
- uses (calls/refs, reference-scoped): [`KotlinPlugin`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin)  (1 test-only)

## Module values
- `TREE_SITTER_KOTLIN_AVAILABLE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_target_75.py#L19)

