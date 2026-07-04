---
title: 'Module: tree_sitter_analyzer/formatters/_typescript_formatter_full.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_typescript_formatter_full.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._typescript_formatter_full`/
symbols:
  format_typescript_full_table: format_typescript_full_table().
  _append_class_section: _append_class_section().
  _class_overview_row: _class_overview_row().
  _field_row: _field_row().
  _append_method_group: _append_method_group().
  _append_method_sections: _append_method_sections().
  _append_global_functions: _append_global_functions().
  _append_classes_overview: _append_classes_overview().
  _append_fields_section: _append_fields_section().
  _class_type: _class_type().
---
# Module: [`tree_sitter_analyzer/formatters/_typescript_formatter_full.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py)

## Functions
- `_append_class_section(formatter: Any, lines: list[str], class_info: dict[str, Any], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L91)
- `_append_classes_overview(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L57)
- `_append_fields_section(formatter: Any, lines: list[str], class_fields: list[dict[str, Any]])` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L108)
- `_append_global_functions(formatter: Any, lines: list[str], functions: list[dict[str, Any]])` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L42) — Render module-level (non-class) functions in their own section.
- `_append_method_group(formatter: Any, lines: list[str], title: str, label: str, methods: list[dict[str, Any]])` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L150)
- `_append_method_sections(formatter: Any, lines: list[str], class_methods: list[dict[str, Any]])` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L132)
- `_class_overview_row(class_info: dict[str, Any], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L74)
- `_class_type(class_info: dict[str, Any])` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L172)
- `_field_row(formatter: Any, field: dict[str, Any])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L122)
- `format_typescript_full_table(formatter: Any, data: dict[str, Any])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_full.py#L20) — Full table format for TypeScript.

