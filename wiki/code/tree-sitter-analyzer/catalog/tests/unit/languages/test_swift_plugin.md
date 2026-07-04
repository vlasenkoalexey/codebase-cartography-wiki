---
title: 'Module: tests/unit/languages/test_swift_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_swift_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_swift_plugin`/
symbols:
  TestSwiftExtraction.test_extract_functions: TestSwiftExtraction#test_extract_functions().
  TestSwiftExtraction.test_analyze_file: TestSwiftExtraction#test_analyze_file().
  TestSwiftExtraction.test_extract_types: TestSwiftExtraction#test_extract_types().
  TestSwiftExtraction.test_extract_variables: TestSwiftExtraction#test_extract_variables().
  TestSwiftExtraction.test_function_parameters_keep_types: TestSwiftExtraction#test_function_parameters_keep_types().
  TestSwiftExtraction.test_parameters_with_nested_commas: TestSwiftExtraction#test_parameters_with_nested_commas().
  TestSwiftExtraction.test_return_types_with_brackets_and_closures: TestSwiftExtraction#test_return_types_with_brackets_and_closures().
  TestSwiftExtraction.test_no_return_type_with_closure_param: TestSwiftExtraction#test_no_return_type_with_closure_param().
  TestSwiftExtraction.test_extract_imports: TestSwiftExtraction#test_extract_imports().
  TestSwiftFailurePaths.test_analyze_file_without_language: TestSwiftFailurePaths#test_analyze_file_without_language().
  TestSwiftFailurePaths.test_analyze_file_read_error: TestSwiftFailurePaths#test_analyze_file_read_error().
  TestSwiftPluginBasics.test_tree_sitter_language_is_cached: TestSwiftPluginBasics#test_tree_sitter_language_is_cached().
  TestSwiftExtraction.test_extract_elements: TestSwiftExtraction#test_extract_elements().
  SWIFT_SAMPLE: SWIFT_SAMPLE.
  TREE_SITTER_SWIFT_AVAILABLE: TREE_SITTER_SWIFT_AVAILABLE.
  _swift_parser: _swift_parser().
  TestSwiftPluginBasics.test_tree_sitter_language_missing_package: TestSwiftPluginBasics#test_tree_sitter_language_missing_package().
  TestSwiftExtraction.tree: TestSwiftExtraction#tree().
  TestSwiftFailurePaths.test_extract_elements_with_none_tree: TestSwiftFailurePaths#test_extract_elements_with_none_tree().
  plugin: plugin().
  TestSwiftExtraction: TestSwiftExtraction#
  TestSwiftPluginBasics: TestSwiftPluginBasics#
  TestSwiftFailurePaths: TestSwiftFailurePaths#
---
# Module: [`tests/unit/languages/test_swift_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py)

## Classes
### `TestSwiftExtraction`
- def: [`tests/unit/languages/test_swift_plugin.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L96)
- doc: Swift extraction tests using the real parser.
- signature: `class TestSwiftExtraction:`
- members:
  - `test_analyze_file(self, plugin: SwiftPlugin, tmp_path)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L231)
  - `test_extract_elements(self, plugin: SwiftPlugin, tree)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L223)
  - `test_extract_functions(self, plugin: SwiftPlugin, tree)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L120)
  - `test_extract_imports(self, plugin: SwiftPlugin, tree)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L103)
  - `test_extract_types(self, plugin: SwiftPlugin, tree)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L109)
  - `test_extract_variables(self, plugin: SwiftPlugin, tree)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L215)
  - `test_function_parameters_keep_types(self, plugin: SwiftPlugin)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L133)
  - `test_no_return_type_with_closure_param(self, plugin: SwiftPlugin)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L198)
  - `test_parameters_with_nested_commas(self, plugin: SwiftPlugin)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L154)
  - `test_return_types_with_brackets_and_closures(self, plugin: SwiftPlugin)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L178)
  - `tree(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L100)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_imports), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`SwiftPlugin`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`analyze_file`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.analyze_file), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`create_extractor`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.create_extractor), [`interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.interfaces), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`is_constant`](../../../tree_sitter_analyzer/models/base.md#Variable.is_constant), [`module_name`](../../../tree_sitter_analyzer/models/base.md#Import.module_name), [`extract_elements`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.extract_elements)  (3 test-only)

### `TestSwiftFailurePaths`
- def: [`tests/unit/languages/test_swift_plugin.py:243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L243)
- doc: Swift plugin fallback and error handling tests.
- signature: `class TestSwiftFailurePaths:`
- members:
  - `test_analyze_file_read_error(self, plugin: SwiftPlugin)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L269)
  - `test_analyze_file_without_language(self, plugin: SwiftPlugin, tmp_path)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L255)
  - `test_extract_elements_with_none_tree(self, plugin: SwiftPlugin)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L246)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`SwiftPlugin`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.analyze_file), [`extract_elements`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.extract_elements)

### `TestSwiftPluginBasics`
- def: [`tests/unit/languages/test_swift_plugin.py:74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L74)
- doc: Swift plugin interface tests.
- signature: `class TestSwiftPluginBasics:`
- members:
  - `test_tree_sitter_language_is_cached(self, plugin: SwiftPlugin)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L85)
  - `test_tree_sitter_language_missing_package(self, plugin: SwiftPlugin)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L77)
- uses (calls/refs, reference-scoped): [`SwiftPlugin`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/swift_plugin.md#SwiftPlugin.get_tree_sitter_language)  (1 test-only)

## Functions
- `_swift_parser()` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L62)
- `plugin()` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L70)

## Module values
- `SWIFT_SAMPLE` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L23)
- `TREE_SITTER_SWIFT_AVAILABLE` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin.py#L18)

