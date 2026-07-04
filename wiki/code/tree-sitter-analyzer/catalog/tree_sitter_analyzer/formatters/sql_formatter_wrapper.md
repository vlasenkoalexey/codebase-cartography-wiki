---
title: 'Module: tree_sitter_analyzer/formatters/sql_formatter_wrapper.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/sql_formatter_wrapper.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.sql_formatter_wrapper`/SQLFormatterWrapper#
symbols:
  SQLFormatterWrapper._convert_analysis_result_to_sql_elements: _convert_analysis_result_to_sql_elements().
  SQLFormatterWrapper._formatters: _formatters.
  SQLFormatterWrapper: ''
  SQLFormatterWrapper.format_elements: format_elements().
  SQLFormatterWrapper._convert_to_sql_elements: _convert_to_sql_elements().
  SQLFormatterWrapper.format_table: format_table().
  SQLFormatterWrapper._create_sql_element_from_dict: _create_sql_element_from_dict().
  SQLFormatterWrapper.format_analysis_result: format_analysis_result().
  SQLFormatterWrapper._element_to_dict: _element_to_dict().
  SQLFormatterWrapper._extract_table_columns: _extract_table_columns().
  SQLFormatterWrapper._extract_view_info: _extract_view_info().
  SQLFormatterWrapper._extract_procedure_info: _extract_procedure_info().
  SQLFormatterWrapper._extract_function_info: _extract_function_info().
  SQLFormatterWrapper._extract_trigger_info: _extract_trigger_info().
  SQLFormatterWrapper._extract_index_info: _extract_index_info().
  SQLFormatterWrapper.__init__: __init__().
  SQLFormatterWrapper.format_summary: format_summary().
  SQLFormatterWrapper.format_structure: format_structure().
  SQLFormatterWrapper.format_advanced: format_advanced().
  SQLFormatterWrapper.supports_language: supports_language().
---
# Module: [`tree_sitter_analyzer/formatters/sql_formatter_wrapper.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py)

## Classes
### `SQLFormatterWrapper`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/sql_formatter_wrapper.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L29)
- doc: Wrapper for SQL-specific formatters to conform to BaseFormatter interface.
- signature: `class SQLFormatterWrapper(BaseFormatter):`
- members:
  - `__init__(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L38) — Initialize the SQL formatter wrapper.
  - `_convert_analysis_result_to_sql_elements(self, analysis_result: Any)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L93) — Convert AnalysisResult directly to SQL elements
  - `_convert_to_sql_elements(self, data: dict[str, Any])` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L108) — Convert generic analysis data to SQL elements.
  - `_create_sql_element_from_dict(self, element_dict: dict[str, Any])` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L155) — Create SQL element from dictionary data.
  - `_element_to_dict(self, element: Any)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L143) — Convert element object to dictionary.
  - `_extract_function_info(self, raw_text: str, func_name: str)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L281) — Extract function information from CREATE FUNCTION statement
  - `_extract_index_info(self, raw_text: str, index_name: str)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L291) — Extract index information from CREATE INDEX statement
  - `_extract_procedure_info(self, raw_text: str, proc_name: str)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L276) — Extract procedure information from CREATE PROCEDURE statement
  - `_extract_table_columns(self, raw_text: str, table_name: str)` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L266) — Extract column information from CREATE TABLE statement
  - `_extract_trigger_info(self, raw_text: str, trigger_name: str)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L286) — Extract trigger information from CREATE TRIGGER statement
  - `_extract_view_info(self, raw_text: str, view_name: str)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L271) — Extract view information from CREATE VIEW statement
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L244) — Format advanced analysis output for SQL.
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L78) — Format AnalysisResult directly for SQL files - prevents degradation
  - `format_elements(self, elements: list[Any], format_type: str = "full")` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L170) — Format elements using SQL-specific formatters.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L230) — Format structure analysis output for SQL.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L216) — Format summary output for SQL analysis.
  - `format_table(self, data: dict[str, Any], table_type: str = "full")` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L48) — Format analysis data as table using SQL-specific formatters.
  - `supports_language(self, language: str)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L203) — Check if this formatter supports the given language.
- protocol/private: `_formatters`[`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatter_wrapper.py#L41)
- uses (calls/refs, reference-scoped): [`SQLElement`](../models/sql_models.md#SQLElement), [`BaseFormatter`](base_formatter.md#BaseFormatter), [`create_sql_element_from_dict`](_sql_formatter_wrapper_helpers.md#create_sql_element_from_dict), [`SQLFullFormatter`](sql_formatters.md#SQLFullFormatter), [`convert_analysis_result_to_sql_elements`](_sql_formatter_wrapper_helpers.md#convert_analysis_result_to_sql_elements), [`SQLCSVFormatter`](sql_formatters.md#SQLCSVFormatter), [`SQLCompactFormatter`](sql_formatters.md#SQLCompactFormatter), [`extract_function_info`](_sql_formatter_wrapper_extractors.md#extract_function_info), [`extract_procedure_info`](_sql_formatter_wrapper_extractors.md#extract_procedure_info), [`extract_trigger_info`](_sql_formatter_wrapper_extractors.md#extract_trigger_info), [`element_to_dict`](_sql_formatter_wrapper_helpers.md#element_to_dict), [`extract_table_columns`](_sql_formatter_wrapper_extractors.md#extract_table_columns), [`__init__`](base_formatter.md#BaseFormatter.__init__), [`extract_index_info`](_sql_formatter_wrapper_extractors.md#extract_index_info), [`extract_view_info`](_sql_formatter_wrapper_extractors.md#extract_view_info)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (3 test-only)

