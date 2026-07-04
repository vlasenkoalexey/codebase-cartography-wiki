---
title: 'Module: tests/unit/core/test_models_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_models_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_models_properties`/
symbols:
  TestAnalysisResultProperties.test_analysis_result_with_elements: TestAnalysisResultProperties#test_analysis_result_with_elements().
  TestFunctionProperties.test_function_creation: TestFunctionProperties#test_function_creation().
  TestClassProperties.test_class_creation: TestClassProperties#test_class_creation().
  TestElementSerializationProperties.test_class_summary_serialization: TestElementSerializationProperties#test_class_summary_serialization().
  TestElementEqualityProperties.test_element_attributes_preserved: TestElementEqualityProperties#test_element_attributes_preserved().
  TestFunctionProperties.test_function_default_visibility: TestFunctionProperties#test_function_default_visibility().
  TestClassProperties.test_class_with_methods: TestClassProperties#test_class_with_methods().
  TestVariableProperties.test_variable_creation: TestVariableProperties#test_variable_creation().
  TestImportProperties.test_import_creation: TestImportProperties#test_import_creation().
  TestElementSerializationProperties.test_function_summary_serialization: TestElementSerializationProperties#test_function_summary_serialization().
  TestFunctionProperties.test_function_line_span: TestFunctionProperties#test_function_line_span().
  TestFunctionProperties.test_function_to_summary_item_contains_required_keys: TestFunctionProperties#test_function_to_summary_item_contains_required_keys().
  TestClassProperties.test_class_to_summary_item: TestClassProperties#test_class_to_summary_item().
  TestVariableProperties.test_variable_to_summary_item: TestVariableProperties#test_variable_to_summary_item().
  TestImportProperties.test_import_to_summary_item: TestImportProperties#test_import_to_summary_item().
  TestElementEqualityProperties.test_same_name_elements_can_differ: TestElementEqualityProperties#test_same_name_elements_can_differ().
  valid_name_strategy: valid_name_strategy.
  TestAnalysisResultProperties.test_analysis_result_creation: TestAnalysisResultProperties#test_analysis_result_creation().
  line_number_strategy: line_number_strategy.
  TestAnalysisResultProperties.test_analysis_result_to_dict: TestAnalysisResultProperties#test_analysis_result_to_dict().
  language_strategy: language_strategy.
  TestFunctionProperties: TestFunctionProperties#
  TestClassProperties: TestClassProperties#
  TestVariableProperties: TestVariableProperties#
  TestImportProperties: TestImportProperties#
  TestAnalysisResultProperties: TestAnalysisResultProperties#
  TestElementSerializationProperties: TestElementSerializationProperties#
  TestElementEqualityProperties: TestElementEqualityProperties#
---
# Module: [`tests/unit/core/test_models_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py)

## Classes
### `TestAnalysisResultProperties`
- def: [`tests/unit/core/test_models_properties.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L232)
- doc: Property tests for AnalysisResult model.
- signature: `class TestAnalysisResultProperties:`
- members:
  - `test_analysis_result_creation(self, file_path: str, language: str)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L244) — AnalysisResult should be created with valid parameters.
  - `test_analysis_result_to_dict(self, file_path: str)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L293) — AnalysisResult.to_dict should contain required keys.
  - `test_analysis_result_with_elements(self, file_path: str, num_functions: int, num_classes: int)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L261) — AnalysisResult can hold multiple elements.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict)  (1 test-only)

### `TestClassProperties`
- def: [`tests/unit/core/test_models_properties.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L115)
- doc: Property tests for Class model.
- signature: `class TestClassProperties:`
- members:
  - `test_class_creation(self, name: str, start_line: int, end_line: int, language: str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L125) — Class should be created with valid parameters.
  - `test_class_to_summary_item(self, name: str)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L160) — Class.to_summary_item should work correctly.
  - `test_class_with_methods(self, name: str)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L143) — Class can have methods added.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`to_summary_item`](../../../tree_sitter_analyzer/models/base.md#CodeElement.to_summary_item), [`methods`](../../../tree_sitter_analyzer/models/base.md#Class.methods), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Class.element_type)  (3 test-only)

### `TestElementEqualityProperties`
- def: [`tests/unit/core/test_models_properties.py:347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L347)
- doc: Property tests for element equality and hashing.
- signature: `class TestElementEqualityProperties:`
- members:
  - `test_element_attributes_preserved(self, name: str)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L377) — Element attributes should be preserved after creation.
  - `test_same_name_elements_can_differ(self, name: str, start_line: int)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L355) — Elements with same name but different lines are different.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async)  (2 test-only)

### `TestElementSerializationProperties`
- def: [`tests/unit/core/test_models_properties.py:303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L303)
- doc: Property tests for element serialization.
- signature: `class TestElementSerializationProperties:`
- members:
  - `test_class_summary_serialization(self, name: str)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L335) — Class summary serialization should work correctly.
  - `test_function_summary_serialization(self, name: str, start_line: int, end_line: int)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L312) — Function summary serialization should preserve data.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`to_summary_item`](../../../tree_sitter_analyzer/models/base.md#CodeElement.to_summary_item), [`methods`](../../../tree_sitter_analyzer/models/base.md#Class.methods)  (2 test-only)

### `TestFunctionProperties`
- def: [`tests/unit/core/test_models_properties.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L46)
- doc: Property tests for Function model.
- signature: `class TestFunctionProperties:`
- members:
  - `test_function_creation(self, name: str, start_line: int, end_line: int, language: str)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L56) — Function should be created with valid parameters.
  - `test_function_default_visibility(self, name: str)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L108) — Function should have default public visibility.
  - `test_function_line_span(self, name: str, start_line: int, end_line: int)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L82) — Function line span should be non-negative.
  - `test_function_to_summary_item_contains_required_keys(self, name: str)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L97) — Function.to_summary_item should contain required keys.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`to_summary_item`](../../../tree_sitter_analyzer/models/base.md#CodeElement.to_summary_item), [`is_public`](../../../tree_sitter_analyzer/models/base.md#Function.is_public), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Function.element_type)  (3 test-only)

### `TestImportProperties`
- def: [`tests/unit/core/test_models_properties.py:201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L201)
- doc: Property tests for Import model.
- signature: `class TestImportProperties:`
- members:
  - `test_import_creation(self, module_name: str, start_line: int)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L209) — Import should be created with valid parameters.
  - `test_import_to_summary_item(self, name: str)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L223) — Import.to_summary_item should work correctly.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`to_summary_item`](../../../tree_sitter_analyzer/models/base.md#CodeElement.to_summary_item), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Import.element_type)  (2 test-only)

### `TestVariableProperties`
- def: [`tests/unit/core/test_models_properties.py:169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L169)
- doc: Property tests for Variable model.
- signature: `class TestVariableProperties:`
- members:
  - `test_variable_creation(self, name: str, start_line: int)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L177) — Variable should be created with valid parameters.
  - `test_variable_to_summary_item(self, name: str)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L192) — Variable.to_summary_item should work correctly.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`to_summary_item`](../../../tree_sitter_analyzer/models/base.md#CodeElement.to_summary_item), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Variable.element_type)  (2 test-only)

## Module values
- `language_strategy` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L29)
- `line_number_strategy` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L27)
- `valid_name_strategy` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_properties.py#L19)

