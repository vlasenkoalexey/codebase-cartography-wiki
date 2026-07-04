---
title: 'Module: tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._java_formatter_compact_mixin`/
symbols:
  JavaTableFormatterCompactMixin._format_compact_table: JavaTableFormatterCompactMixin#_format_compact_table().
  shorten_type: shorten_type().
  JavaTableFormatterCompactMixin: JavaTableFormatterCompactMixin#
  JavaTableFormatterCompactMixin._create_compact_signature: JavaTableFormatterCompactMixin#_create_compact_signature().
  _append_methods: _append_methods().
  _shorten_array_type: _shorten_array_type().
  JavaTableFormatterCompactMixin.create_compact_signature: JavaTableFormatterCompactMixin#create_compact_signature.
  _TYPE_MAPPING: _TYPE_MAPPING.
  _append_info: _append_info().
  _compact_method_row: _compact_method_row().
---
# Module: [`tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py)

## Classes
### `JavaTableFormatterCompactMixin`
- def: [`tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L11)
- doc: Compact-format and compact signature helpers.
- signature: `class JavaTableFormatterCompactMixin:`
- members:
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L29) — Create compact method signature for Java
  - `_format_compact_table(self, data: dict[str, Any])` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L14) — Compact table format for Java
  - `create_compact_signature` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L44)
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`trim_trailing_blank_lines`](../_legacy_table_formatter_common.md#trim_trailing_blank_lines), [`_java_title`](_java_formatter_full_mixin.md#_java_title), [`shorten_type`](_java_formatter_compact_mixin.md#shorten_type), [`_append_methods`](_java_formatter_compact_mixin.md#_append_methods), [`_append_info`](_java_formatter_compact_mixin.md#_append_info)
- used by: [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`format_summary`](java_formatter.md#JavaTableFormatter.format_summary)  (7 test-only)

## Functions
- `_append_info(lines: list[str], package_name: str, stats: dict[str, Any])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L62)
- `_append_methods(lines: list[str], methods: list[dict[str, Any]], formatter: Any)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L73)
- `_compact_method_row(method: dict[str, Any], formatter: Any)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L87)
- `_shorten_array_type(type_name: str)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L103)
- `shorten_type(type_name: Any)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L110) — Shorten type name for Java tables.

## Module values
- `_TYPE_MAPPING` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.py#L47)

