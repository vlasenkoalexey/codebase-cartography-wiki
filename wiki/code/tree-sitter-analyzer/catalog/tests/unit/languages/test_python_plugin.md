---
title: 'Module: tests/unit/languages/test_python_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_plugin`/TestPython
symbols:
  TestPythonElementExtractor.test_extract_detailed_function_info: ElementExtractor#test_extract_detailed_function_info().
  TestPythonElementExtractor.test_extract_detailed_class_info: ElementExtractor#test_extract_detailed_class_info().
  TestPythonElementExtractor.test_extract_core_elements_success: ElementExtractor#test_extract_core_elements_success().
  TestPythonPluginIntegration.test_full_extraction_workflow: PluginIntegration#test_full_extraction_workflow().
  TestPythonPluginIntegration.test_plugin_consistency: PluginIntegration#test_plugin_consistency().
  TestPythonElementExtractor.test_extract_variable_info: ElementExtractor#test_extract_variable_info().
  TestPythonElementExtractor.test_extract_import_info: ElementExtractor#test_extract_import_info().
  TestPythonPlugin.test_analyze_file_nonexistent: Plugin#test_analyze_file_nonexistent().
  TestPythonPluginErrorHandling.test_analyze_file_with_exception: PluginErrorHandling#test_analyze_file_with_exception().
  TestPythonPluginIntegration.test_extractor_consistency: PluginIntegration#test_extractor_consistency().
  TestPythonElementExtractor.test_extractor_initialization: ElementExtractor#test_extractor_initialization().
  TestPythonElementExtractor.test_extract_functions_no_language: ElementExtractor#test_extract_functions_no_language().
  TestPythonElementExtractor.test_extract_name_from_node: ElementExtractor#test_extract_name_from_node().
  TestPythonElementExtractor.test_extract_name_from_node_no_identifier: ElementExtractor#test_extract_name_from_node_no_identifier().
  TestPythonElementExtractor.test_extract_parameters_from_node: ElementExtractor#test_extract_parameters_from_node().
  TestPythonElementExtractor.test_extract_decorators_from_node: ElementExtractor#test_extract_decorators_from_node().
  TestPythonElementExtractor.test_extract_return_type_from_node: ElementExtractor#test_extract_return_type_from_node().
  TestPythonElementExtractor.test_extract_docstring_from_node: ElementExtractor#test_extract_docstring_from_node().
  TestPythonElementExtractor.test_calculate_complexity: ElementExtractor#test_calculate_complexity().
  TestPythonPlugin.test_plugin_initialization: Plugin#test_plugin_initialization().
  TestPythonPlugin.test_get_tree_sitter_language: Plugin#test_get_tree_sitter_language().
  TestPythonPlugin.test_get_tree_sitter_language_caching: Plugin#test_get_tree_sitter_language_caching().
  TestPythonPlugin.test_analyze_file_success: Plugin#test_analyze_file_success().
  TestPythonPluginErrorHandling.test_extract_functions_with_exception: PluginErrorHandling#test_extract_functions_with_exception().
  TestPythonPluginErrorHandling.test_extract_classes_with_exception: PluginErrorHandling#test_extract_classes_with_exception().
  TestPythonPluginErrorHandling.test_extract_detailed_function_info_with_exception: PluginErrorHandling#test_extract_detailed_function_info_with_exception().
  TestPythonPluginErrorHandling.test_get_tree_sitter_language_failure: PluginErrorHandling#test_get_tree_sitter_language_failure().
  TestPythonPluginIntegration.test_plugin_with_various_python_files: PluginIntegration#test_plugin_with_various_python_files().
  TestPythonPluginIntegration.test_python_specific_features: PluginIntegration#test_python_specific_features().
  TestPythonPluginIntegration.test_python_import_variations: PluginIntegration#test_python_import_variations().
  TestPythonElementExtractor.extractor: ElementExtractor#extractor().
  TestPythonPlugin.plugin: Plugin#plugin().
  TestPythonPluginErrorHandling.plugin: PluginErrorHandling#plugin().
  TestPythonPluginErrorHandling.extractor: PluginErrorHandling#extractor().
  TestPythonPluginIntegration.plugin: PluginIntegration#plugin().
  TestPythonElementExtractor: ElementExtractor#
  TestPythonElementExtractor.mock_tree: ElementExtractor#mock_tree().
  TestPythonElementExtractor.sample_python_code: ElementExtractor#sample_python_code().
  TestPythonPlugin: Plugin#
  TestPythonPluginErrorHandling: PluginErrorHandling#
  TestPythonPluginIntegration: PluginIntegration#
---
# Module: [`tests/unit/languages/test_python_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py)

## Classes
### `TestPythonElementExtractor`
- def: [`tests/unit/languages/test_python_plugin.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L23)
- doc: Test cases for PythonElementExtractor class
- signature: `class TestPythonElementExtractor:`
- members:
  - `extractor(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L27) — Create a PythonElementExtractor instance for testing
  - `mock_tree(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L32) — Create a mock tree-sitter tree
  - `sample_python_code(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L42) — Sample Python code for testing
  - `test_calculate_complexity(self, extractor: PythonElementExtractor)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L366) — Test complexity calculation
  - `test_extract_core_elements_success(self, extractor: PythonElementExtractor, mock_tree: Mock)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L110) — Test successful extraction of the core Python element families.
  - `test_extract_decorators_from_node(self, extractor: PythonElementExtractor)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L314) — Test decorator extraction from node
  - `test_extract_detailed_class_info(self, extractor: PythonElementExtractor)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L187) — Test detailed class information extraction
  - `test_extract_detailed_function_info(self, extractor: PythonElementExtractor)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L143) — Test detailed function information extraction
  - `test_extract_docstring_from_node(self, extractor: PythonElementExtractor)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L340) — Test docstring extraction from node
  - `test_extract_functions_no_language(self, extractor: PythonElementExtractor)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L129) — Test function extraction when language is not available
  - `test_extract_import_info(self, extractor: PythonElementExtractor)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L246) — Test import information extraction
  - `test_extract_name_from_node(self, extractor: PythonElementExtractor)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L265) — Test name extraction from node
  - `test_extract_name_from_node_no_identifier(self, extractor: PythonElementExtractor)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L278) — Test name extraction when no identifier is found
  - `test_extract_parameters_from_node(self, extractor: PythonElementExtractor)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L289) — Test parameter extraction from function node
  - `test_extract_return_type_from_node(self, extractor: PythonElementExtractor)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L325) — Test return type extraction from function node
  - `test_extract_variable_info(self, extractor: PythonElementExtractor)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L225) — Test variable information extraction
  - `test_extractor_initialization(self, extractor: PythonElementExtractor)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L101) — Test PythonElementExtractor initialization
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.interfaces), [`_extract_detailed_function_info`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_detailed_function_info), [`superclass`](../../../tree_sitter_analyzer/models/base.md#Class.superclass), [`_extract_detailed_class_info`](../../../tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin._extract_detailed_class_info), [`extract_imports`](../../../tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin.extract_variables), [`_extract_import_info`](../../../tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin._extract_import_info), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Class.modifiers), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Function.modifiers), [`_extract_variable_info`](../../../tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin._extract_variable_info), [`extract_functions`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin.extract_functions), [`_extract_docstring_from_node`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_docstring_from_node), [`_calculate_complexity`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor._calculate_complexity), [`_extract_name_from_node`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor._extract_name_from_node), [`_extract_return_type_from_node`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_return_type_from_node), [`extract_classes`](../../../tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin.extract_classes), [`_extract_decorators_from_node`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor._extract_decorators_from_node), [`_extract_parameters_from_node`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor._extract_parameters_from_node)

### `TestPythonPlugin`
- def: [`tests/unit/languages/test_python_plugin.py:389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L389)
- doc: Test cases for PythonPlugin class
- signature: `class TestPythonPlugin:`
- members:
  - `plugin(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L393) — Create a PythonPlugin instance for testing
  - `test_analyze_file_nonexistent(self, plugin: PythonPlugin)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L476) — Test analysis of non-existent file
  - `test_analyze_file_success(self, plugin: PythonPlugin)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L445) — Test successful file analysis
  - `test_get_tree_sitter_language(self, plugin: PythonPlugin)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L405) — Test getting tree-sitter language
  - `test_get_tree_sitter_language_caching(self, plugin: PythonPlugin)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L422) — Test tree-sitter language caching
  - `test_plugin_initialization(self, plugin: PythonPlugin)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L397) — Test PythonPlugin initialization
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.analyze_file), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_tree_sitter_language)

### `TestPythonPluginErrorHandling`
- def: [`tests/unit/languages/test_python_plugin.py:490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L490)
- doc: Test error handling in PythonPlugin
- signature: `class TestPythonPluginErrorHandling:`
- members:
  - `extractor(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L499) — Create a PythonElementExtractor instance for testing
  - `plugin(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L494) — Create a PythonPlugin instance for testing
  - `test_analyze_file_with_exception(self, plugin: PythonPlugin)` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L557) — Test file analysis with exception
  - `test_extract_classes_with_exception(self, extractor: PythonElementExtractor)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L518) — Test class extraction with exception
  - `test_extract_detailed_function_info_with_exception(self, extractor: PythonElementExtractor)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L533) — Test detailed function info extraction with exception
  - `test_extract_functions_with_exception(self, extractor: PythonElementExtractor)` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L503) — Test function extraction with exception
  - `test_get_tree_sitter_language_failure(self, plugin: PythonPlugin)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L547) — Test tree-sitter language loading failure
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.analyze_file), [`_extract_detailed_function_info`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_detailed_function_info), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_tree_sitter_language), [`extract_functions`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin.extract_classes)

### `TestPythonPluginIntegration`
- def: [`tests/unit/languages/test_python_plugin.py:586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L586)
- doc: Integration tests for PythonPlugin
- signature: `class TestPythonPluginIntegration:`
- members:
  - `plugin(self)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L590) — Create a PythonPlugin instance for testing
  - `test_extractor_consistency(self, plugin: PythonPlugin)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L619) — Test extractor consistency
  - `test_full_extraction_workflow(self, plugin: PythonPlugin)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L594) — Test complete extraction workflow
  - `test_plugin_consistency(self, plugin: PythonPlugin)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L611) — Test plugin consistency across multiple calls
  - `test_plugin_with_various_python_files(self, plugin: PythonPlugin)` — [`L629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L629) — Test plugin with various Python file types
  - `test_python_import_variations(self, plugin: PythonPlugin)` — [`L682`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L682) — Test Python import statement variations
  - `test_python_specific_features(self, plugin: PythonPlugin)` — [`L655`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin.py#L655) — Test Python-specific features
- uses (calls/refs, reference-scoped): [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.create_extractor), [`get_plugin_info`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_plugin_info), [`get_language_name`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_language_name), [`is_applicable`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.is_applicable), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_file_extensions)

