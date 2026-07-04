---
title: 'Module: tree_sitter_analyzer/formatters/_csv_safety.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_csv_safety.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._csv_safety`/
symbols:
  csv_safe_row: csv_safe_row().
  csv_safe_cell: csv_safe_cell().
  _REMOVE: _REMOVE.
  _TRANSLATION: _TRANSLATION.
---
# Module: [`tree_sitter_analyzer/formatters/_csv_safety.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csv_safety.py)

## Functions
- `csv_safe_cell(value: Any)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csv_safety.py#L36) — Strip CSV-unrepresentable control characters from a string cell.
- `csv_safe_row(row: list[Any])` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csv_safety.py#L47) — Return a copy of ``row`` with every string cell sanitized. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)

## Module values
- `_REMOVE` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csv_safety.py#L30)
- `_TRANSLATION` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csv_safety.py#L33)

