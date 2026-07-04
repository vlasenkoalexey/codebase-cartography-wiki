---
title: 'Module: tests/unit/formatters/test_python_formatter_conversion.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_conversion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_conversion`/
symbols:
  TestConvertAnalysisResultToPythonFormat.test_mixed_element_types: TestConvertAnalysisResultToPythonFormat#test_mixed_element_types().
  _make_element: _make_element().
  TestConvertAnalysisResultToPythonFormat.test_empty_elements: TestConvertAnalysisResultToPythonFormat#test_empty_elements().
  TestConvertFunctionElementForPython.test_basic_function: TestConvertFunctionElementForPython#test_basic_function().
  TestConvertFunctionElementForPython.test_async_function_with_params: TestConvertFunctionElementForPython#test_async_function_with_params().
  TestConvertClassElementForPython.test_basic_class: TestConvertClassElementForPython#test_basic_class().
  TestConvertClassElementForPython.test_class_with_no_name: TestConvertClassElementForPython#test_class_with_no_name().
  TestConvertVariableElementForPython.test_basic_variable: TestConvertVariableElementForPython#test_basic_variable().
  TestConvertVariableElementForPython.test_variable_with_field_type_fallback: TestConvertVariableElementForPython#test_variable_with_field_type_fallback().
  TestConvertImportElementForPython.test_import_with_raw_text: TestConvertImportElementForPython#test_import_with_raw_text().
  TestConvertImportElementForPython.test_import_without_raw_text: TestConvertImportElementForPython#test_import_without_raw_text().
  FakeFormatter: FakeFormatter#
  FakeFormatter._convert_class_element_for_python: FakeFormatter#_convert_class_element_for_python().
  FakeFormatter._convert_function_element_for_python: FakeFormatter#_convert_function_element_for_python().
  FakeFormatter._convert_variable_element_for_python: FakeFormatter#_convert_variable_element_for_python().
  FakeFormatter._convert_import_element_for_python: FakeFormatter#_convert_import_element_for_python().
  FakeFormatter._process_python_parameters: FakeFormatter#_process_python_parameters().
  FakeFormatter.convert_class_element_for_python: FakeFormatter#convert_class_element_for_python.
  FakeFormatter.convert_function_element_for_python: FakeFormatter#convert_function_element_for_python.
  FakeFormatter.convert_variable_element_for_python: FakeFormatter#convert_variable_element_for_python.
  FakeFormatter.convert_import_element_for_python: FakeFormatter#convert_import_element_for_python.
  FakeFormatter.process_python_parameters: FakeFormatter#process_python_parameters.
  TestProcessPythonParameters.test_string_params: TestProcessPythonParameters#test_string_params().
  TestProcessPythonParameters.test_empty_string: TestProcessPythonParameters#test_empty_string().
  TestProcessPythonParameters.test_list_of_strings: TestProcessPythonParameters#test_list_of_strings().
  TestProcessPythonParameters.test_list_of_dicts: TestProcessPythonParameters#test_list_of_dicts().
  TestProcessPythonParameters.test_unknown_type_returns_any: TestProcessPythonParameters#test_unknown_type_returns_any().
  TestProcessPythonParameters.test_non_string_non_list_returns_empty: TestProcessPythonParameters#test_non_string_non_list_returns_empty().
  FakeAnalysisResult: FakeAnalysisResult#
  FakeAnalysisResult.elements: FakeAnalysisResult#elements.
  FakeElement: FakeElement#
  FakeElement.name: FakeElement#name.
  FakeElement.element_type: FakeElement#element_type.
  FakeElement.start_line: FakeElement#start_line.
  FakeElement.end_line: FakeElement#end_line.
  FakeElement.raw_text: FakeElement#raw_text.
  FakeElement.parameters: FakeElement#parameters.
  FakeElement.return_type: FakeElement#return_type.
  FakeElement.visibility: FakeElement#visibility.
  FakeElement.is_constructor: FakeElement#is_constructor.
  FakeElement.is_static: FakeElement#is_static.
  FakeElement.is_async: FakeElement#is_async.
  FakeElement.complexity_score: FakeElement#complexity_score.
  FakeElement.docstring: FakeElement#docstring.
  FakeElement.decorators: FakeElement#decorators.
  FakeElement.modifiers: FakeElement#modifiers.
  FakeElement.variable_type: FakeElement#variable_type.
  FakeElement.field_type: FakeElement#field_type.
  FakeElement.class_type: FakeElement#class_type.
  FakeElement.module_name: FakeElement#module_name.
  FakeAnalysisResult.file_path: FakeAnalysisResult#file_path.
  FakeAnalysisResult.language: FakeAnalysisResult#language.
  FakeAnalysisResult.line_count: FakeAnalysisResult#line_count.
  TestConvertAnalysisResultToPythonFormat: TestConvertAnalysisResultToPythonFormat#
  TestConvertClassElementForPython: TestConvertClassElementForPython#
  TestConvertFunctionElementForPython: TestConvertFunctionElementForPython#
  TestConvertVariableElementForPython: TestConvertVariableElementForPython#
  TestConvertImportElementForPython: TestConvertImportElementForPython#
  TestProcessPythonParameters: TestProcessPythonParameters#
---
# Module: [`tests/unit/formatters/test_python_formatter_conversion.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py)

## Classes
### `FakeAnalysisResult`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L46)
- signature: `class FakeAnalysisResult:`
- members:
  - `elements` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L50)
  - `file_path` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L47)
  - `language` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L48)
  - `line_count` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L49)
- used by: (2 test-only callers)

### `FakeElement`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L23)
- signature: `class FakeElement:`
- members:
  - `class_type` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L41)
  - `complexity_score` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L35)
  - `decorators` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L37)
  - `docstring` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L36)
  - `element_type` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L25)
  - `end_line` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L27)
  - `field_type` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L40)
  - `is_async` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L34)
  - `is_constructor` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L32)
  - `is_static` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L33)
  - `modifiers` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L38)
  - `module_name` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L42)
  - `name` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L24)
  - `parameters` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L29)
  - `raw_text` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L28)
  - `return_type` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L30)
  - `start_line` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L26)
  - `variable_type` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L39)
  - `visibility` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L31)
- used by: (1 test-only callers)

### `FakeFormatter`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L53)
- signature: `class FakeFormatter:`
- members:
  - `convert_class_element_for_python` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L70)
  - `convert_function_element_for_python` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L71)
  - `convert_import_element_for_python` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L73)
  - `convert_variable_element_for_python` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L72)
  - `process_python_parameters` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L74)
- protocol/private: `_convert_class_element_for_python`[`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L54), `_convert_function_element_for_python`[`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L57), `_convert_import_element_for_python`[`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L63), `_convert_variable_element_for_python`[`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L60), `_process_python_parameters`[`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L66)
- uses (calls/refs, reference-scoped): [`process_python_parameters`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#process_python_parameters), [`convert_class_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_class_element_for_python), [`convert_function_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_function_element_for_python), [`convert_variable_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_variable_element_for_python), [`convert_import_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_import_element_for_python)
- used by: (4 test-only callers)

### `TestConvertAnalysisResultToPythonFormat`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L81)
- signature: `class TestConvertAnalysisResultToPythonFormat:`
- members:
  - `test_empty_elements(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L82)
  - `test_mixed_element_types(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L91)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT), [`ELEMENT_TYPE_PACKAGE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_PACKAGE), [`convert_analysis_result_to_python_format`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_analysis_result_to_python_format)  (4 test-only)

### `TestConvertClassElementForPython`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L109)
- signature: `class TestConvertClassElementForPython:`
- members:
  - `test_basic_class(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L110)
  - `test_class_with_no_name(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L117)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`convert_class_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_class_element_for_python)  (1 test-only)

### `TestConvertFunctionElementForPython`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L123)
- signature: `class TestConvertFunctionElementForPython:`
- members:
  - `test_async_function_with_params(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L133)
  - `test_basic_function(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L124)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`convert_function_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_function_element_for_python)  (2 test-only)

### `TestConvertImportElementForPython`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L168)
- signature: `class TestConvertImportElementForPython:`
- members:
  - `test_import_with_raw_text(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L169)
  - `test_import_without_raw_text(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L174)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT), [`convert_import_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_import_element_for_python)  (1 test-only)

### `TestConvertVariableElementForPython`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L148)
- signature: `class TestConvertVariableElementForPython:`
- members:
  - `test_basic_variable(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L149)
  - `test_variable_with_field_type_fallback(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L157)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`convert_variable_element_for_python`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#convert_variable_element_for_python)  (1 test-only)

### `TestProcessPythonParameters`
- def: [`tests/unit/formatters/test_python_formatter_conversion.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L180)
- signature: `class TestProcessPythonParameters:`
- members:
  - `test_empty_string(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L186)
  - `test_list_of_dicts(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L195)
  - `test_list_of_strings(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L190)
  - `test_non_string_non_list_returns_empty(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L204)
  - `test_string_params(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L181)
  - `test_unknown_type_returns_any(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L200)
- uses (calls/refs, reference-scoped): [`process_python_parameters`](../../../tree_sitter_analyzer/formatters/_python_formatter_conversion.md#process_python_parameters)

## Functions
- `_make_element(**kwargs)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_conversion.py#L77)

