---
title: 'Module: tree_sitter_analyzer/_legacy_table_formatter_csv.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_legacy_table_formatter_csv.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._legacy_table_formatter_csv`/
symbols:
  format_csv: format_csv().
  _write_csv_method_row: _write_csv_method_row().
  _csv_safe_row: _csv_safe_row().
  _write_csv_field_row: _write_csv_field_row().
  _csv_parameters: _csv_parameters().
  _csv_parameter: _csv_parameter().
---
# Module: [`tree_sitter_analyzer/_legacy_table_formatter_csv.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py)

## Functions
- `_csv_parameter(param: Any)` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L118) — Format one legacy CSV parameter.
- `_csv_parameters(params: list[Any])` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L113) — Format legacy CSV parameter strings.
- `_csv_safe_row(row: list[Any])` — [`L10`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L10) — Sanitize a CSV row, importing the shared helper lazily.
- `_write_csv_field_row(writer: Any, field: dict[str, Any])` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L91) — Write one legacy CSV field row.
- `_write_csv_method_row(writer: Any, method: dict[str, Any])` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L69) — Write one legacy CSV method row.
- `format_csv(data: dict[str, Any])` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_csv.py#L22) — Format structure data as legacy CSV output. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)

