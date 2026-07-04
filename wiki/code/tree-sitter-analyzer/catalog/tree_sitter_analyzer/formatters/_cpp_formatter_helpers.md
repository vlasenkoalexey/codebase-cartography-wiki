---
title: 'Module: tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._cpp_formatter_helpers`/
symbols:
  format_cpp_full_table: format_cpp_full_table().
  shorten_cpp_type: shorten_cpp_type().
  format_cpp_compact_table: format_cpp_compact_table().
  format_cpp_class_details: format_cpp_class_details().
  create_cpp_compact_signature: create_cpp_compact_signature().
  _format_class_overview_row: _format_class_overview_row().
  _append_global_functions: _append_global_functions().
  _append_global_variables: _append_global_variables().
  _compact_param_type: _compact_param_type().
  _members_outside_classes: _members_outside_classes().
  _members_in_range: _members_in_range().
  _line_range_text: _line_range_text().
  _append_namespace_section: _append_namespace_section().
  _append_classes_section: _append_classes_section().
  _append_class_fields: _append_class_fields().
  _append_class_methods: _append_class_methods().
  _append_compact_methods: _append_compact_methods().
  _format_compact_method_row: _format_compact_method_row().
  _append_method_group: _append_method_group().
  _format_field_row: _format_field_row().
  _file_name: _file_name().
  _append_imports_section: _append_imports_section().
  _owner_qualified: _owner_qualified().
  _append_compact_info: _append_compact_info().
  _is_inside_class: _is_inside_class().
  _compact_param_type_from_dict: _compact_param_type_from_dict().
  _compact_param_type_from_string: _compact_param_type_from_string().
---
# Module: [`tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py)

## Functions
- `_append_class_fields(formatter: Any, lines: list[str], class_fields: list[dict[str, Any]])` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L216)
- `_append_class_methods(formatter: Any, lines: list[str], class_methods: list[dict[str, Any]])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L230)
- `_append_classes_section(formatter: Any, lines: list[str], data: dict[str, Any], classes: list[dict[str, Any]])` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L137)
- `_append_compact_info(lines: list[str], data: dict[str, Any])` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L276)
- `_append_compact_methods(formatter: Any, lines: list[str], methods: list[dict[str, Any]])` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L291)
- `_append_global_functions(formatter: Any, lines: list[str], data: dict[str, Any], classes: list[dict[str, Any]])` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L168)
- `_append_global_variables(formatter: Any, lines: list[str], data: dict[str, Any], classes: list[dict[str, Any]])` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L198)
- `_append_imports_section(lines: list[str], data: dict[str, Any])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L122)
- `_append_method_group(formatter: Any, lines: list[str], title: str, methods: list[dict[str, Any]])` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L259)
- `_append_namespace_section(lines: list[str], data: dict[str, Any], package_name: Any)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L105)
- `_compact_param_type(param: Any)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L360)
- `_compact_param_type_from_dict(param: dict[str, Any])` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L368)
- `_compact_param_type_from_string(param: str)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L378)
- `_file_name(file_path: Any)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L399)
- `_format_class_overview_row(data: dict[str, Any], class_info: dict[str, Any])` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L155)
- `_format_compact_method_row(formatter: Any, method: dict[str, Any])` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L305)
- `_format_field_row(formatter: Any, field: dict[str, Any], *, escape_doc: bool)` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L318)
- `_is_inside_class(item: dict[str, Any], classes: list[dict[str, Any]])` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L350)
- `_line_range_text(line_range: dict[str, Any])` — [`L395`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L395)
- `_members_in_range(items: list[dict[str, Any]], line_range: dict[str, Any])` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L332)
- `_members_outside_classes(items: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L344`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L344)
- `_owner_qualified(method: dict[str, Any])` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L186) — Display copy with the owner prefixed (#590): ``math`` + ``max`` → ``math::max``.
- `create_cpp_compact_signature(shorten_type: Callable[[Any], str], method: dict[str, Any])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L62) — Create compact C/C++ method signature.
- `format_cpp_class_details(formatter: Any, class_info: dict[str, Any], data: dict[str, Any])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L33) — Format details for a single C/C++ class.
- `format_cpp_compact_table(formatter: Any, data: dict[str, Any])` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L49) — Compact table format for C/C++.
- `format_cpp_full_table(formatter: Any, data: dict[str, Any])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L11) — Full table format for C/C++.
- `shorten_cpp_type(type_name: Any)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_helpers.py#L75) — Shorten type name for C/C++ compact display.

