---
title: 'Module: tree_sitter_analyzer/_legacy_table_formatter_compact.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_legacy_table_formatter_compact.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._legacy_table_formatter_compact`/
symbols:
  compact_table_header: compact_table_header().
  append_compact_fields_section: append_compact_fields_section().
  append_compact_info_section: append_compact_info_section().
  append_compact_methods_section: append_compact_methods_section().
  format_compact_field_row: format_compact_field_row().
---
# Module: [`tree_sitter_analyzer/_legacy_table_formatter_compact.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py)

## Functions
- `append_compact_fields_section(lines: list[str], fields: list[dict[str, Any]], abbreviate_type: Any)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py#L74) — Append compact-table fields section.
- `append_compact_info_section(lines: list[str], package_name: str, methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py#L43) — Append compact-table info section.
- `append_compact_methods_section(lines: list[str], methods: list[dict[str, Any]], format_method_row: Any)` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py#L60) — Append compact-table methods section.
- `compact_table_header(package_name: str, classes: list[dict[str, Any]], file_path: str = "")` — [`L10`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py#L10) — Build the legacy compact-table header. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
- `format_compact_field_row(field: dict[str, Any], abbreviate_type: Any)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_compact.py#L88) — Format a compact-table field row.

