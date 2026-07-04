---
title: 'Module: tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._ruby_formatter_helpers`/
symbols:
  format_full_table: format_full_table().
  format_csv: format_csv().
  format_signature: format_signature().
  get_visibility_symbol: get_visibility_symbol().
  format_compact_table: format_compact_table().
  format_compact_signature: format_compact_signature().
  _method_row: _method_row().
  _compact_method_row: _compact_method_row().
  _csv_method_row: _csv_method_row().
  _field_row: _field_row().
  _append_class_methods: _append_class_methods().
  _module_method_row: _module_method_row().
  _class_member_counts: _class_member_counts().
  _append_class_details: _append_class_details().
  _append_class_fields: _append_class_fields().
  _append_module_level_methods: _append_module_level_methods().
  _increment_member_counts: _increment_member_counts().
  _get_parent_class: _get_parent_class().
  _trim_doc: _trim_doc().
  _append_classes_overview: _append_classes_overview().
  _append_compact_methods: _append_compact_methods().
  _append_csv_methods: _append_csv_methods().
  _csv_signature: _csv_signature().
  _header_lines: _header_lines().
  _empty_class_counts: _empty_class_counts().
  _full_param: _full_param().
  _compact_param: _compact_param().
  _append_imports: _append_imports().
  _class_overview_row: _class_overview_row().
  _modifiers_text: _modifiers_text().
  _ordered_class_methods: _ordered_class_methods().
  _method_display_name: _method_display_name().
  _compact_method_name: _compact_method_name().
  _append_csv_fields: _append_csv_fields().
  _csv_entry_type: _csv_entry_type().
  _csv_method_name: _csv_method_name().
  _line_span: _line_span().
---
# Module: [`tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py)

## Functions
- `_append_class_details(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L199)
- `_append_class_fields(lines: list[str], class_name: str, classes: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L216)
- `_append_class_methods(lines: list[str], class_name: str, classes: list[dict[str, Any]], methods: list[dict[str, Any]])` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L257)
- `_append_classes_overview(lines: list[str], classes: list[dict[str, Any]], method_counts: dict[str, int], field_counts: dict[str, int])` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L166)
- `_append_compact_methods(lines: list[str], methods: list[dict[str, Any]])` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L354)
- `_append_csv_fields(lines: list[str], fields: list[dict[str, Any]])` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L392)
- `_append_csv_methods(lines: list[str], methods: list[dict[str, Any]])` — [`L406`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L406)
- `_append_imports(lines: list[str], imports: list[dict[str, Any]])` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L106)
- `_append_module_level_methods(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]])` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L318)
- `_class_member_counts(classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L120)
- `_class_overview_row(class_info: dict[str, Any], method_counts: dict[str, int], field_counts: dict[str, int])` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L183)
- `_compact_method_name(method: dict[str, Any])` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L379)
- `_compact_method_row(method: dict[str, Any])` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L365)
- `_compact_param(param: Any)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L90)
- `_csv_entry_type(method: dict[str, Any], method_name: str)` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L430)
- `_csv_method_name(method_name: str, parent: str, method_type: str)` — [`L443`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L443)
- `_csv_method_row(method: dict[str, Any])` — [`L411`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L411)
- `_csv_signature(method: dict[str, Any], method_type: str)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L436)
- `_empty_class_counts(classes: list[dict[str, Any]])` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L132)
- `_field_row(field: dict[str, Any])` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L239)
- `_full_param(param: Any)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L82)
- `_get_parent_class(item_start: int, classes: list[dict[str, Any]])` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L149)
- `_header_lines(data: dict[str, Any])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L96)
- `_increment_member_counts(counts: dict[str, int], members: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L136)
- `_line_span(item: dict[str, Any])` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L450)
- `_method_display_name(method: dict[str, Any], class_name: str | None)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L308)
- `_method_row(method: dict[str, Any], class_name: str | None = None)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L291)
- `_modifiers_text(modifiers: Any)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L251)
- `_module_method_row(method: dict[str, Any])` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L340)
- `_ordered_class_methods(methods: list[dict[str, Any]])` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L281)
- `_trim_doc(doc: Any, max_length: int)` — [`L455`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L455)
- `format_compact_signature(method: dict[str, Any])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L27) — Format compact method signature.
- `format_compact_table(data: dict[str, Any])` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L53) — Compact table format for Ruby, following Java golden master format.
- `format_csv(data: dict[str, Any])` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L74) — CSV format for Ruby, following Java golden master format.
- `format_full_table(data: dict[str, Any])` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L37) — Full table format for Ruby, following Java golden master format.
- `format_signature(method: dict[str, Any])` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L17) — Format method signature like Java: (param:type):returnType.
- `get_visibility_symbol(visibility: str)` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_ruby_formatter_helpers.py#L6) — Convert visibility to symbol.

