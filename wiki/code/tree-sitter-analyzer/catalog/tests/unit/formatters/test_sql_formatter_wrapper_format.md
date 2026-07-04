---
title: 'Module: tests/unit/formatters/test_sql_formatter_wrapper_format.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_sql_formatter_wrapper_format.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_sql_formatter_wrapper_format`/
symbols:
  TestFormatAnalysisResult.test_format_analysis_result_basic: TestFormatAnalysisResult#test_format_analysis_result_basic().
  TestFormatAnalysisResult.test_format_analysis_result_invalid_type_fallback: TestFormatAnalysisResult#test_format_analysis_result_invalid_type_fallback().
  TestFormatAnalysisResult.test_format_analysis_result_with_view: TestFormatAnalysisResult#test_format_analysis_result_with_view().
  TestFormatAnalysisResult.test_format_analysis_result_with_procedure: TestFormatAnalysisResult#test_format_analysis_result_with_procedure().
  TestFormatAnalysisResult.test_format_analysis_result_with_function: TestFormatAnalysisResult#test_format_analysis_result_with_function().
  TestFormatAnalysisResult.test_format_analysis_result_with_trigger: TestFormatAnalysisResult#test_format_analysis_result_with_trigger().
  TestFormatAnalysisResult.test_format_analysis_result_with_index: TestFormatAnalysisResult#test_format_analysis_result_with_index().
  TestFormatElements.test_format_elements_with_sql_elements: TestFormatElements#test_format_elements_with_sql_elements().
  TestFormatTable.test_format_table_full: TestFormatTable#test_format_table_full().
  TestFormatTable.test_format_table_csv: TestFormatTable#test_format_table_csv().
  TestFormatElements.test_format_elements_invalid_type_fallback: TestFormatElements#test_format_elements_invalid_type_fallback().
  TestFormatElements.test_format_elements_compact: TestFormatElements#test_format_elements_compact().
  TestFormatElements.test_format_elements_csv: TestFormatElements#test_format_elements_csv().
  TestFormatStructure.test_format_structure: TestFormatStructure#test_format_structure().
  TestFormatAdvanced.test_format_advanced_table: TestFormatAdvanced#test_format_advanced_table().
  formatter: formatter().
  TestSQLFormatterWrapperInit: TestSQLFormatterWrapperInit#
  TestSQLFormatterWrapperInit.test_init_creates_formatters: TestSQLFormatterWrapperInit#test_init_creates_formatters().
  TestFormatTable: TestFormatTable#
  TestFormatTable.test_format_table_unsupported_type: TestFormatTable#test_format_table_unsupported_type().
  TestFormatTable.test_format_table_default_file_path: TestFormatTable#test_format_table_default_file_path().
  TestFormatAnalysisResult: TestFormatAnalysisResult#
  TestFormatElements: TestFormatElements#
  TestFormatElements.test_format_elements_with_dict_elements: TestFormatElements#test_format_elements_with_dict_elements().
  TestSupportsLanguage: TestSupportsLanguage#
  TestSupportsLanguage.test_supports_sql: TestSupportsLanguage#test_supports_sql().
  TestSupportsLanguage.test_does_not_support_other_languages: TestSupportsLanguage#test_does_not_support_other_languages().
  TestFormatStructure: TestFormatStructure#
  TestFormatAdvanced: TestFormatAdvanced#
  TestFormatAdvanced.test_format_advanced_json: TestFormatAdvanced#test_format_advanced_json().
---
# Module: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py)

## Classes
### `TestFormatAdvanced`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L302)
- doc: Test format_advanced method.
- signature: `class TestFormatAdvanced:`
- members:
  - `test_format_advanced_json(self, formatter)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L305) — Test format_advanced with json output.
  - `test_format_advanced_table(self, formatter)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L312) — Test format_advanced with table output.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable)

### `TestFormatAnalysisResult`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L87)
- doc: Test format_analysis_result method.
- signature: `class TestFormatAnalysisResult:`
- members:
  - `test_format_analysis_result_basic(self, formatter)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L90) — Test basic format_analysis_result.
  - `test_format_analysis_result_invalid_type_fallback(self, formatter)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L103) — Test format_analysis_result falls back to full for invalid type.
  - `test_format_analysis_result_with_function(self, formatter)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L142) — Test format_analysis_result with function element.
  - `test_format_analysis_result_with_index(self, formatter)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L168) — Test format_analysis_result with index element.
  - `test_format_analysis_result_with_procedure(self, formatter)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L129) — Test format_analysis_result with procedure element.
  - `test_format_analysis_result_with_trigger(self, formatter)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L155) — Test format_analysis_result with trigger element.
  - `test_format_analysis_result_with_view(self, formatter)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L116) — Test format_analysis_result with view element.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`SQLElementType`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType), [`SQLElement`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`SQLIndex`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex), [`SQLProcedure`](../../../tree_sitter_analyzer/models/sql_models.md#SQLProcedure), [`TABLE`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.TABLE), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.sql_element_type)

### `TestFormatElements`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L182)
- doc: Test format_elements method.
- signature: `class TestFormatElements:`
- members:
  - `test_format_elements_compact(self, formatter)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L236) — Test format_elements with compact format.
  - `test_format_elements_csv(self, formatter)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L250) — Test format_elements with csv format.
  - `test_format_elements_invalid_type_fallback(self, formatter)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L222) — Test format_elements falls back to full for invalid type.
  - `test_format_elements_with_dict_elements(self, formatter)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L207) — Test format_elements with dictionary elements.
  - `test_format_elements_with_sql_elements(self, formatter)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L185) — Test format_elements with SQL elements.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView)

### `TestFormatStructure`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L281)
- doc: Test format_structure method.
- signature: `class TestFormatStructure:`
- members:
  - `test_format_structure(self, formatter)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L284) — Test format_structure uses full formatter.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L36)
- doc: Test format_table method.
- signature: `class TestFormatTable:`
- members:
  - `test_format_table_csv(self, formatter)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L56) — Test format_table with csv type.
  - `test_format_table_default_file_path(self, formatter)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L80) — Test format_table with missing file_path uses default.
  - `test_format_table_full(self, formatter)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L39) — Test format_table with full type.
  - `test_format_table_unsupported_type(self, formatter)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L73) — Test format_table with unsupported type raises ValueError.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable)

### `TestSQLFormatterWrapperInit`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L26)
- doc: Test initialization of SQLFormatterWrapper.
- signature: `class TestSQLFormatterWrapperInit:`
- members:
  - `test_init_creates_formatters(self, formatter)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L29) — Test that init creates all required formatters.

### `TestSupportsLanguage`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_format.py:265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L265)
- doc: Test supports_language method.
- signature: `class TestSupportsLanguage:`
- members:
  - `test_does_not_support_other_languages(self, formatter)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L274) — Test that other languages are not supported.
  - `test_supports_sql(self, formatter)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L268) — Test that SQL is supported.

## Functions
- `formatter()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_format.py#L22)

