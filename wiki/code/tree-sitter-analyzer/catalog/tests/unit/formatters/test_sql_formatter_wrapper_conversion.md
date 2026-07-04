---
title: 'Module: tests/unit/formatters/test_sql_formatter_wrapper_conversion.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_sql_formatter_wrapper_conversion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_sql_formatter_wrapper_conversion`/
symbols:
  TestConvertAnalysisResultToSQLElements.test_convert_multiple_sql_elements: TestConvertAnalysisResultToSQLElements#test_convert_multiple_sql_elements().
  TestConvertAnalysisResultToSQLElements.test_convert_sql_element_passthrough: TestConvertAnalysisResultToSQLElements#test_convert_sql_element_passthrough().
  TestConvertToSQLElements.test_convert_sql_element_passthrough: TestConvertToSQLElements#test_convert_sql_element_passthrough().
  TestConvertToSQLElements.test_convert_methods_included: TestConvertToSQLElements#test_convert_methods_included().
  TestElementToDict.test_element_to_dict_with_attributes: TestElementToDict#test_element_to_dict_with_attributes().
  formatter: formatter().
  TestConvertAnalysisResultToSQLElements: TestConvertAnalysisResultToSQLElements#
  TestConvertToSQLElements: TestConvertToSQLElements#
  TestConvertToSQLElements.test_convert_empty_data: TestConvertToSQLElements#test_convert_empty_data().
  TestConvertToSQLElements.test_convert_dict_element: TestConvertToSQLElements#test_convert_dict_element().
  TestElementToDict: TestElementToDict#
  TestCreateSQLElementFromDict: TestCreateSQLElementFromDict#
  TestCreateSQLElementFromDict.test_create_table_element: TestCreateSQLElementFromDict#test_create_table_element().
  TestCreateSQLElementFromDict.test_create_view_element: TestCreateSQLElementFromDict#test_create_view_element().
  TestCreateSQLElementFromDict.test_create_procedure_element: TestCreateSQLElementFromDict#test_create_procedure_element().
  TestCreateSQLElementFromDict.test_create_function_element: TestCreateSQLElementFromDict#test_create_function_element().
  TestCreateSQLElementFromDict.test_create_trigger_element: TestCreateSQLElementFromDict#test_create_trigger_element().
  TestCreateSQLElementFromDict.test_create_index_element: TestCreateSQLElementFromDict#test_create_index_element().
  TestCreateSQLElementFromDict.test_create_unknown_type_fallback: TestCreateSQLElementFromDict#test_create_unknown_type_fallback().
  TestCreateSQLElementFromDict.test_create_with_create_prefix_types: TestCreateSQLElementFromDict#test_create_with_create_prefix_types().
---
# Module: [`tests/unit/formatters/test_sql_formatter_wrapper_conversion.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py)

## Classes
### `TestConvertAnalysisResultToSQLElements`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_conversion.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L24)
- doc: Test _convert_analysis_result_to_sql_elements method.
- signature: `class TestConvertAnalysisResultToSQLElements:`
- members:
  - `test_convert_multiple_sql_elements(self, formatter)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L41) — Test conversion of multiple SQL elements.
  - `test_convert_sql_element_passthrough(self, formatter)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L27) — Test that existing SQL elements pass through unchanged.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`SQLIndex`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex), [`SQLProcedure`](../../../tree_sitter_analyzer/models/sql_models.md#SQLProcedure)

### `TestConvertToSQLElements`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_conversion.py:92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L92)
- doc: Test _convert_to_sql_elements method.
- signature: `class TestConvertToSQLElements:`
- members:
  - `test_convert_dict_element(self, formatter)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L115) — Test conversion of dictionary element.
  - `test_convert_empty_data(self, formatter)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L95) — Test conversion with empty data.
  - `test_convert_methods_included(self, formatter)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L134) — Test that methods are also converted.
  - `test_convert_sql_element_passthrough(self, formatter)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L101) — Test that SQL elements pass through unchanged.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`SQLProcedure`](../../../tree_sitter_analyzer/models/sql_models.md#SQLProcedure)

### `TestCreateSQLElementFromDict`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_conversion.py:172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L172)
- doc: Test _create_sql_element_from_dict method.
- signature: `class TestCreateSQLElementFromDict:`
- members:
  - `test_create_function_element(self, formatter)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L217) — Test creation of function element.
  - `test_create_index_element(self, formatter)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L245) — Test creation of index element.
  - `test_create_procedure_element(self, formatter)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L203) — Test creation of procedure element.
  - `test_create_table_element(self, formatter)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L175) — Test creation of table element.
  - `test_create_trigger_element(self, formatter)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L231) — Test creation of trigger element.
  - `test_create_unknown_type_fallback(self, formatter)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L259) — Test creation with unknown type falls back to SQLTable.
  - `test_create_view_element(self, formatter)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L189) — Test creation of view element.
  - `test_create_with_create_prefix_types(self, formatter)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L273) — Test creation with create_ prefix types.

### `TestElementToDict`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_conversion.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L152)
- doc: Test _element_to_dict method.
- signature: `class TestElementToDict:`
- members:
  - `test_element_to_dict_with_attributes(self, formatter)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L155) — Test conversion of element with all attributes.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable)

## Functions
- `formatter()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_conversion.py#L20)

