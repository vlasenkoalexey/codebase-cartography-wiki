---
title: 'Module: tree_sitter_analyzer/formatters/_php_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_php_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._php_formatter_helpers`/
symbols:
  format_full_table: format_full_table().
  format_compact_table: format_compact_table().
  _append_class_details: _append_class_details().
  get_visibility_symbol: get_visibility_symbol().
  format_signature: format_signature().
  _field_row: _field_row().
  _full_method_row: _full_method_row().
  extract_namespace: extract_namespace().
  _method_groups: _method_groups().
  _module_level_methods: _module_level_methods().
  _compact_method_row: _compact_method_row().
  format_compact_signature: format_compact_signature().
  _class_overview_row: _class_overview_row().
  _append_class_methods: _append_class_methods().
  _append_module_level_functions: _append_module_level_functions().
  _range_count: _range_count().
  _append_classes_overview: _append_classes_overview().
  _append_class_fields: _append_class_fields().
  _constructor_methods: _constructor_methods().
  _append_compact_info: _append_compact_info().
  _append_compact_methods: _append_compact_methods().
  _class_line_range: _class_line_range().
  _elements_in_range: _elements_in_range().
  _trim_doc: _trim_doc().
  _header_lines: _header_lines().
  _methods_with_visibility: _methods_with_visibility().
  _append_imports: _append_imports().
  _qualified_field_name: _qualified_field_name().
  _field_modifiers: _field_modifiers().
  _is_constructor: _is_constructor().
  _public_methods: _public_methods().
  _method_start_line: _method_start_line().
  _line_in_any_range: _line_in_any_range().
  _simple_class_name: _simple_class_name().
---
# Module: [`tree_sitter_analyzer/formatters/_php_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py)

## Functions
- `_append_class_details(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L135)
- `_append_class_fields(lines: list[str], simple_class_name: str, fields: list[dict[str, Any]])` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L154)
- `_append_class_methods(lines: list[str], simple_class_name: str, methods: list[dict[str, Any]])` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L195)
- `_append_classes_overview(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L97)
- `_append_compact_info(lines: list[str], data: dict[str, Any])` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L306)
- `_append_compact_methods(lines: list[str], methods: list[dict[str, Any]])` — [`L322`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L322)
- `_append_imports(lines: list[str], imports: list[dict[str, Any]])` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L83)
- `_append_module_level_functions(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]])` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L268)
- `_class_line_range(class_info: dict[str, Any])` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L348)
- `_class_overview_row(class_info: dict[str, Any], methods: list[dict[str, Any]], fields: list[dict[str, Any]])` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L115)
- `_compact_method_row(method: dict[str, Any])` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L333)
- `_constructor_methods(methods: list[dict[str, Any]])` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L223)
- `_elements_in_range(elements: list[dict[str, Any]], start_line: int, end_line: int)` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L353)
- `_field_modifiers(field: dict[str, Any])` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L184)
- `_field_row(field: dict[str, Any], simple_class_name: str)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L168)
- `_full_method_row(method: dict[str, Any], simple_class_name: str | None = None)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L249)
- `_header_lines(data: dict[str, Any])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L77)
- `_is_constructor(method: dict[str, Any])` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L227)
- `_line_in_any_range(line: int, ranges: list[tuple[int, int]])` — [`L363`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L363)
- `_method_groups(methods: list[dict[str, Any]])` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L211)
- `_method_start_line(method: dict[str, Any])` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L294)
- `_methods_with_visibility(methods: list[dict[str, Any]], visibility: str)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L243)
- `_module_level_methods(classes: list[dict[str, Any]], methods: list[dict[str, Any]])` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L283)
- `_public_methods(methods: list[dict[str, Any]], constructors: list[dict[str, Any]])` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L233)
- `_qualified_field_name(field_name: str, simple_class_name: str)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L180)
- `_range_count(elements: list[dict[str, Any]], start_line: int, end_line: int)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L131)
- `_simple_class_name(class_name: str)` — [`L367`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L367)
- `_trim_doc(doc: str, limit: int)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L371)
- `extract_namespace(data: dict[str, Any])` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L50) — Extract namespace from class metadata.
- `format_compact_signature(method: dict[str, Any])` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L36) — Format compact method signature.
- `format_compact_table(data: dict[str, Any])` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L298) — Compact table format for PHP, following Java golden master format.
- `format_full_table(data: dict[str, Any])` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L63) — Full table format for PHP, following Java golden master format.
- `format_signature(method: dict[str, Any])` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L18) — Format method signature like Java: ($param:type):returnType.
- `get_visibility_symbol(visibility: str)` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_php_formatter_helpers.py#L8) — Convert visibility to a compact symbol.

