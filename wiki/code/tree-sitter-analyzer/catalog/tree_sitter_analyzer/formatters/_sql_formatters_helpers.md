---
title: 'Module: tree_sitter_analyzer/formatters/_sql_formatters_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_sql_formatters_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._sql_formatters_helpers`/
symbols:
  format_sql_compact_details: format_sql_compact_details().
  format_sql_overview_details: format_sql_overview_details().
  format_sql_table_foreign_keys: format_sql_table_foreign_keys().
  format_sql_csv_details: format_sql_csv_details().
  _format_compact_trigger_details: _format_compact_trigger_details().
  _format_compact_index_details: _format_compact_index_details().
  iter_sql_elements_by_line: iter_sql_elements_by_line().
  _format_compact_table_details: _format_compact_table_details().
  _format_compact_function_details: _format_compact_function_details().
  format_sql_csv_dependencies: format_sql_csv_dependencies().
  _format_compact_view_details: _format_compact_view_details().
  _format_compact_procedure_details: _format_compact_procedure_details().
  _valid_parameter_names: _valid_parameter_names().
  format_sql_parameter_details: format_sql_parameter_details().
  SQL_PARAMETER_KEYWORDS: SQL_PARAMETER_KEYWORDS.
---
# Module: [`tree_sitter_analyzer/formatters/_sql_formatters_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py)

## Functions
- `_format_compact_function_details(function: SQLFunction)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L166)
- `_format_compact_index_details(index: SQLIndex)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L184)
- `_format_compact_procedure_details(procedure: SQLProcedure)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L160)
- `_format_compact_table_details(table: SQLTable)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L144)
- `_format_compact_trigger_details(trigger: SQLTrigger)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L175)
- `_format_compact_view_details(view: SQLView)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L154)
- `_valid_parameter_names(parameters: Iterable[Any])` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L135)
- `format_sql_compact_details(element: SQLElement)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L64) — Format compact details for a SQL element. — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- `format_sql_csv_dependencies(element: SQLElement)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L121) — Format dependencies for a single-line CSV field.
- `format_sql_csv_details(element: SQLElement)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L104) — Format the columns/parameters field for CSV output.
- `format_sql_overview_details(element: SQLElement)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L41) — Format details for the full formatter overview table.
- `format_sql_parameter_details(parameters: Iterable[Any])` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L93) — Format SQL routine parameters for detail sections.
- `format_sql_table_foreign_keys(table: SQLTable)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L81) — Format table foreign-key details when present.
- `iter_sql_elements_by_line(grouped_elements: dict[SQLElementType, list[SQLElement]])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L31) — Return grouped SQL elements sorted by source line.

## Module values
- `SQL_PARAMETER_KEYWORDS` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_sql_formatters_helpers.py#L17)

