---
title: 'Module: tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._javascript_formatter_compact_mixin`/
symbols:
  JavaScriptTableFormatterCompactMixin._format_compact_table: JavaScriptTableFormatterCompactMixin#_format_compact_table().
  JavaScriptTableFormatterCompactMixin: JavaScriptTableFormatterCompactMixin#
  _append_methods_section: _append_methods_section().
  JavaScriptTableFormatterCompactMixin._create_compact_signature: JavaScriptTableFormatterCompactMixin#_create_compact_signature().
  _append_info_section: _append_info_section().
  _compact_method_row: _compact_method_row().
---
# Module: [`tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py)

## Classes
### `JavaScriptTableFormatterCompactMixin`
- def: [`tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L12)
- doc: Compact-format rendering helpers.
- signature: `class JavaScriptTableFormatterCompactMixin:`
- members:
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L28) — Create compact method signature for JavaScript
  - `_format_compact_table(self, data: dict[str, Any])` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L15) — Compact table format for JavaScript - matches golden master format
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`trim_trailing_blank_lines`](../_legacy_table_formatter_common.md#trim_trailing_blank_lines), [`_list_or_empty`](_javascript_formatter_full_mixin.md#_list_or_empty), [`_append_methods_section`](_javascript_formatter_compact_mixin.md#_append_methods_section), [`_title`](_javascript_formatter_full_mixin.md#_title), [`_append_info_section`](_javascript_formatter_compact_mixin.md#_append_info_section)
- used by: [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`format_summary`](javascript_formatter.md#JavaScriptTableFormatter.format_summary)

## Functions
- `_append_info_section(lines: list[str], methods: list[dict[str, Any]])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L46)
- `_append_methods_section(lines: list[str], methods: list[dict[str, Any]], signature_builder: Any)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L56)
- `_compact_method_row(method: dict[str, Any], signature_builder: Any)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_compact_mixin.py#L71)

