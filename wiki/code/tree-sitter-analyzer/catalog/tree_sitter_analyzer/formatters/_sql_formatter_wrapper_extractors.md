---
title: 'Module: tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._sql_formatter_wrapper_extractors`/
symbols:
  extract_function_info: extract_function_info().
  extract_procedure_info: extract_procedure_info().
  extract_trigger_info: extract_trigger_info().
  extract_table_columns: extract_table_columns().
  _extract_table_dependencies: _extract_table_dependencies().
  _extract_procedure_parameters: _extract_procedure_parameters().
  extract_view_info: extract_view_info().
  extract_index_info: extract_index_info().
  _extend_unique: _extend_unique().
  _append_column_name: _append_column_name().
  _format_procedure_parameter: _format_procedure_parameter().
  _extract_function_return_type: _extract_function_return_type().
  _extract_function_parameters: _extract_function_parameters().
  _extract_from_dependencies: _extract_from_dependencies().
---
# Module: [`tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py)

## Functions
- `_append_column_name(columns: list[str], line: str)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L38)
- `_extend_unique(items: list[str], candidates: list[str])` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L196)
- `_extract_from_dependencies(raw_text: str)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L192)
- `_extract_function_parameters(raw_text: str)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L120)
- `_extract_function_return_type(raw_text: str)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L115)
- `_extract_procedure_parameters(raw_text: str, proc_name: str)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L70)
- `_extract_table_dependencies(raw_text: str)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L184)
- `_format_procedure_parameter(param: str)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L90)
- `extract_function_info(raw_text: str, func_name: str)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L106) — Extract function information from CREATE FUNCTION statement.
- `extract_index_info(raw_text: str, index_name: str)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L170) — Extract index information from CREATE INDEX statement.
- `extract_procedure_info(raw_text: str, proc_name: str)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L62) — Extract procedure information from CREATE PROCEDURE statement.
- `extract_table_columns(raw_text: str, table_name: str)` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L8) — Extract column information from CREATE TABLE statement.
- `extract_trigger_info(raw_text: str, trigger_name: str)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L146) — Extract trigger information from CREATE TRIGGER statement.
- `extract_view_info(raw_text: str, view_name: str)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatter_wrapper_extractors.py#L55) — Extract view information from CREATE VIEW statement.

