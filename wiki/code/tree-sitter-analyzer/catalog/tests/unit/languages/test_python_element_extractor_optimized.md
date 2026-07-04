---
title: 'Module: tests/unit/languages/test_python_element_extractor_optimized.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_element_extractor_optimized.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_element_extractor_optimized`/TestPythonElementExtractor#
symbols:
  TestPythonElementExtractor.test_extract_function_optimized_complete: test_extract_function_optimized_complete().
  TestPythonElementExtractor.test_extract_class_optimized_complete: test_extract_class_optimized_complete().
  TestPythonElementExtractor.test_extract_class_attributes: test_extract_class_attributes().
  TestPythonElementExtractor.test_extract_imports_basic: test_extract_imports_basic().
  TestPythonElementExtractor.test_extract_class_attribute_info: test_extract_class_attribute_info().
  TestPythonElementExtractor.extractor: extractor().
  TestPythonElementExtractor: ''
  TestPythonElementExtractor.mock_tree: mock_tree().
  TestPythonElementExtractor.sample_python_code: sample_python_code().
  TestPythonElementExtractor.test_extract_function_optimized_private: test_extract_function_optimized_private().
  TestPythonElementExtractor.test_extract_function_optimized_magic: test_extract_function_optimized_magic().
  TestPythonElementExtractor.test_extract_class_optimized_with_decorators: test_extract_class_optimized_with_decorators().
  TestPythonElementExtractor.test_extract_class_optimized_exception_class: test_extract_class_optimized_exception_class().
  TestPythonElementExtractor.test_is_framework_class: test_is_framework_class().
---
# Module: [`tests/unit/languages/test_python_element_extractor_optimized.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py)

## Classes
### `TestPythonElementExtractor`
- def: [`tests/unit/languages/test_python_element_extractor_optimized.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L11)
- doc: Test Python element extractor functionality
- signature: `class TestPythonElementExtractor:`
- members:
  - `extractor(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L15) — Create a Python element extractor instance
  - `mock_tree(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L20) — Create a mock tree-sitter tree
  - `sample_python_code(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L28) — Sample Python code for testing
  - `test_extract_class_attribute_info(self, extractor)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L420) — Test class attribute info extraction
  - `test_extract_class_attributes(self, extractor)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L384) — Test class attribute extraction
  - `test_extract_class_optimized_complete(self, extractor)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L212) — Test complete class extraction
  - `test_extract_class_optimized_exception_class(self, extractor)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L314) — Test exception class extraction
  - `test_extract_class_optimized_with_decorators(self, extractor)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L272) — Test class extraction with decorators
  - `test_extract_function_optimized_complete(self, extractor)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L90) — Test complete function extraction
  - `test_extract_function_optimized_magic(self, extractor)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L181) — Test magic method extraction
  - `test_extract_function_optimized_private(self, extractor)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L152) — Test private function extraction
  - `test_extract_imports_basic(self, extractor, mock_tree)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L448) — Test basic import extraction
  - `test_is_framework_class(self, extractor)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_optimized.py#L355) — Test framework class detection
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.interfaces), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`superclass`](../../../tree_sitter_analyzer/models/base.md#Class.superclass), [`full_qualified_name`](../../../tree_sitter_analyzer/models/base.md#Class.full_qualified_name), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Class.modifiers), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Function.modifiers), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Function.is_static), [`framework_type`](../../../tree_sitter_analyzer/models/base.md#Function.framework_type), [`package_name`](../../../tree_sitter_analyzer/models/base.md#Class.package_name), [`is_generator`](../../../tree_sitter_analyzer/models/base.md#Function.is_generator), [`is_public`](../../../tree_sitter_analyzer/models/base.md#Function.is_public), [`is_private`](../../../tree_sitter_analyzer/models/base.md#Function.is_private), [`framework_type`](../../../tree_sitter_analyzer/models/base.md#Class.framework_type), [`is_abstract`](../../../tree_sitter_analyzer/models/base.md#Class.is_abstract), [`is_property`](../../../tree_sitter_analyzer/models/base.md#Function.is_property), [`is_classmethod`](../../../tree_sitter_analyzer/models/base.md#Function.is_classmethod), [`is_dataclass`](../../../tree_sitter_analyzer/models/base.md#Class.is_dataclass), [`is_exception`](../../../tree_sitter_analyzer/models/base.md#Class.is_exception), [`is_staticmethod`](../../../tree_sitter_analyzer/models/base.md#Function.is_staticmethod)

