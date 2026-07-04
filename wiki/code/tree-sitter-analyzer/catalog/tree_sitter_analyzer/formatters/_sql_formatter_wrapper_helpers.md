---
title: 'Module: tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._sql_formatter_wrapper_helpers`/
symbols:
  _sql_trigger_from_analysis: _sql_trigger_from_analysis().
  _sql_index_from_analysis: _sql_index_from_analysis().
  _sql_trigger_from_dict: _sql_trigger_from_dict().
  _sql_index_from_dict: _sql_index_from_dict().
  _convert_analysis_element: _convert_analysis_element().
  _sql_table_from_analysis: _sql_table_from_analysis().
  _sql_view_from_analysis: _sql_view_from_analysis().
  _sql_function_from_analysis: _sql_function_from_analysis().
  _sql_table_from_dict: _sql_table_from_dict().
  _sql_view_from_dict: _sql_view_from_dict().
  _sql_function_from_dict: _sql_function_from_dict().
  _sql_procedure_from_analysis: _sql_procedure_from_analysis().
  _sql_procedure_from_dict: _sql_procedure_from_dict().
  create_sql_element_from_dict: create_sql_element_from_dict().
  _DICT_FACTORIES._DICT_FACTORIES: _DICT_FACTORIES._DICT_FACTORIES.
  convert_analysis_result_to_sql_elements: convert_analysis_result_to_sql_elements().
  _dict_fields: _dict_fields().
  InfoExtractor: InfoExtractor.
  _analysis_fields: _analysis_fields().
  _AnalysisElementFields.name: _AnalysisElementFields#name.
  _AnalysisElementFields.raw_text: _AnalysisElementFields#raw_text.
  _DictElementFields: _DictElementFields#
  _AnalysisElementFields: _AnalysisElementFields#
  _AnalysisElementFields.start_line: _AnalysisElementFields#start_line.
  _AnalysisElementFields.end_line: _AnalysisElementFields#end_line.
  _AnalysisElementFields.language: _AnalysisElementFields#language.
  _DictElementFields.name: _DictElementFields#name.
  _DictElementFields.start_line: _DictElementFields#start_line.
  _DictElementFields.end_line: _DictElementFields#end_line.
  _DictElementFields.raw_text: _DictElementFields#raw_text.
  _DictElementFields.language: _DictElementFields#language.
  element_to_dict: element_to_dict().
  _DictElementFields.element_type: _DictElementFields#element_type.
  _LOGGER: _LOGGER.
---
# Module: [`tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py)

## Classes
### `_AnalysisElementFields`
- def: [`tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L34)
- signature: `class _AnalysisElementFields:`
- members:
  - `end_line` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L37)
  - `language` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L39)
  - `name` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L35)
  - `raw_text` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L38)
  - `start_line` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L36)
- used by: [`_sql_index_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_index_from_analysis), [`_sql_trigger_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_trigger_from_analysis), [`_sql_function_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_function_from_analysis), [`_sql_table_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_table_from_analysis), [`_sql_view_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_view_from_analysis), [`_sql_procedure_from_analysis`](_sql_formatter_wrapper_helpers.md#_sql_procedure_from_analysis), [`_analysis_fields`](_sql_formatter_wrapper_helpers.md#_analysis_fields)

### `_DictElementFields`
- def: [`tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py:43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L43)
- signature: `class _DictElementFields:`
- members:
  - `element_type` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L44)
  - `end_line` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L47)
  - `language` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L49)
  - `name` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L45)
  - `raw_text` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L48)
  - `start_line` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L46)
- used by: [`_sql_index_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_index_from_dict), [`_sql_trigger_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_trigger_from_dict), [`_sql_table_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_table_from_dict), [`_sql_function_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_function_from_dict), [`_sql_view_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_view_from_dict), [`_sql_procedure_from_dict`](_sql_formatter_wrapper_helpers.md#_sql_procedure_from_dict), [`create_sql_element_from_dict`](_sql_formatter_wrapper_helpers.md#create_sql_element_from_dict), [`_DICT_FACTORIES`](_sql_formatter_wrapper_helpers.md#_DICT_FACTORIES._DICT_FACTORIES), [`_dict_fields`](_sql_formatter_wrapper_helpers.md#_dict_fields)

## Functions
- `_analysis_fields(element: Any)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L121)
- `_convert_analysis_element(element: Any, *, extract_table_columns: InfoExtractor, extract_view_info: InfoExtractor, extract_procedure_info: InfoExtractor, extract_function_info: InfoExtractor, extract_trigger_info: InfoExtractor, extract_index_info: InfoExtractor)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L91) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `_dict_fields(element_dict: dict[str, Any])` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L241)
- `_sql_function_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L179) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `_sql_function_from_dict(fields: _DictElementFields)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L290) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `_sql_index_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L212)
- `_sql_index_from_dict(fields: _DictElementFields)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L317)
- `_sql_procedure_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L164)
- `_sql_procedure_from_dict(fields: _DictElementFields)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L278)
- `_sql_table_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L131) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `_sql_table_from_dict(fields: _DictElementFields)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L252) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `_sql_trigger_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L195)
- `_sql_trigger_from_dict(fields: _DictElementFields)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L303)
- `_sql_view_from_analysis(fields: _AnalysisElementFields, extract_info: InfoExtractor)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L147)
- `_sql_view_from_dict(fields: _DictElementFields)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L265)
- `convert_analysis_result_to_sql_elements(analysis_result: Any, *, extract_table_columns: InfoExtractor, extract_view_info: InfoExtractor, extract_procedure_info: InfoExtractor, extract_function_info: InfoExtractor, extract_trigger_info: InfoExtractor, extract_index_info: InfoExtractor)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L64) — Convert AnalysisResult elements to SQL elements with extracted metadata.
- `create_sql_element_from_dict(element_dict: dict[str, Any])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L230) — Create a SQL element from dictionary data, preserving soft-failure behavior. — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `element_to_dict(element: Any)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L52) — Convert element object to the dictionary shape expected by SQL conversion.

## Module values
- `InfoExtractor` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L29)
- `_DICT_FACTORIES` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L331)
- `_LOGGER` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.py#L30)

