---
title: 'Module: tree_sitter_analyzer/_legacy_table_formatter_members.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_legacy_table_formatter_members.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._legacy_table_formatter_members`/
symbols:
  get_class_methods: get_class_methods().
  get_class_fields: get_class_fields().
  _elements_in_class_range: _elements_in_class_range().
  _nested_class_ranges: _nested_class_ranges().
  _belongs_to_class: _belongs_to_class().
---
# Module: [`tree_sitter_analyzer/_legacy_table_formatter_members.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py)

## Functions
- `_belongs_to_class(element: dict[str, Any], class_start: int, class_end: int, nested_class_ranges: list[tuple[int, int]])` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py#L65) — Return whether an element belongs directly to a class range.
- `_elements_in_class_range(elements: list[dict[str, Any]], classes: list[dict[str, Any]], class_line_range: dict[str, int])` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py#L32) — Return elements inside a class range and outside nested class ranges.
- `_nested_class_ranges(classes: list[dict[str, Any]], class_start: int, class_end: int)` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py#L49) — Return ranges for classes nested inside the provided class range.
- `get_class_fields(data: dict[str, Any], class_line_range: dict[str, int])` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py#L20) — Get fields for a class line range, excluding nested class members.
- `get_class_methods(data: dict[str, Any], class_line_range: dict[str, int])` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_members.py#L8) — Get methods for a class line range, excluding nested class members.

