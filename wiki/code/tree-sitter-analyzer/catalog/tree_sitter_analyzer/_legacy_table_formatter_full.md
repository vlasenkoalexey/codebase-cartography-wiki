---
title: 'Module: tree_sitter_analyzer/_legacy_table_formatter_full.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_legacy_table_formatter_full.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._legacy_table_formatter_full`/
symbols:
  append_multi_class_full_sections: append_multi_class_full_sections().
  append_single_class_full_sections: append_single_class_full_sections().
  full_table_header: full_table_header().
  append_full_package_section: append_full_package_section().
  append_full_imports_section: append_full_imports_section().
  append_full_class_info_section: append_full_class_info_section().
  format_simple_method_row: format_simple_method_row().
  _append_simple_methods_table: _append_simple_methods_table().
  _append_simple_fields_table: _append_simple_fields_table().
  _simple_parameters: _simple_parameters().
  _append_simple_methods_section: _append_simple_methods_section().
  _append_simple_fields_section: _append_simple_fields_section().
  format_simple_field_row: format_simple_field_row().
  _simple_parameter: _simple_parameter().
---
# Module: [`tree_sitter_analyzer/_legacy_table_formatter_full.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py)

## Functions
- `_append_simple_fields_section(lines: list[str], fields: list[dict[str, Any]])` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L224) — Append a headed legacy fields subsection.
- `_append_simple_fields_table(lines: list[str], fields: list[dict[str, Any]])` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L234) — Append a legacy fields table.
- `_append_simple_methods_section(lines: list[str], methods: list[dict[str, Any]])` — [`L203`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L203) — Append a headed legacy methods subsection.
- `_append_simple_methods_table(lines: list[str], methods: list[dict[str, Any]])` — [`L213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L213) — Append a legacy methods table.
- `_simple_parameter(param: Any)` — [`L190`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L190) — Format one legacy full-table parameter.
- `_simple_parameters(params: list[Any])` — [`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L185) — Format legacy full-table parameter strings.
- `append_full_class_info_section(lines: list[str], classes: list[dict[str, Any]], display_package: str)` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L94) — Append the legacy full-table class info section.
- `append_full_imports_section(lines: list[str], imports: list[dict[str, Any]], language: str)` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L76) — Append the legacy full-table imports section.
- `append_full_package_section(lines: list[str], package_name: str)` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L68) — Append the legacy full-table package section.
- `append_multi_class_full_sections(lines: list[str], data: dict[str, Any], classes: list[dict[str, Any]], get_class_methods: Any, get_class_fields: Any)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L128) — Append legacy full-table sections for multiple classes. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
- `append_single_class_full_sections(lines: list[str], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L170) — Append legacy full-table sections for one or zero classes. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
- `format_simple_field_row(field: dict[str, Any])` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L20) — Format a legacy full-table field row.
- `format_simple_method_row(method: dict[str, Any])` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L8) — Format a legacy full-table method row.
- `full_table_header(data: dict[str, Any], classes: list[dict[str, Any]])` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_full.py#L40) — Build the legacy full-table header.

