---
title: 'Module: tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._javascript_formatter_full_mixin`/
symbols:
  JavaScriptTableFormatterFullMixin._format_full_table: JavaScriptTableFormatterFullMixin#_format_full_table().
  JavaScriptTableFormatterFullMixin._format_class_section: JavaScriptTableFormatterFullMixin#_format_class_section().
  _list_or_empty: _list_or_empty().
  JavaScriptTableFormatterFullMixin._format_method_table_row: JavaScriptTableFormatterFullMixin#_format_method_table_row().
  JavaScriptTableFormatterFullMixin: JavaScriptTableFormatterFullMixin#
  _append_classes_overview: _append_classes_overview().
  _title: _title().
  _append_method_section: _append_method_section().
  _items_in_range: _items_in_range().
  JavaScriptTableFormatterFullMixin._create_full_signature: JavaScriptTableFormatterFullMixin#_create_full_signature().
  _module_level_functions: _module_level_functions().
---
# Module: [`tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py)

## Classes
### `JavaScriptTableFormatterFullMixin`
- def: [`tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L10)
- doc: Full-format rendering helpers.
- signature: `class JavaScriptTableFormatterFullMixin:`
- members:
  - `_create_full_signature(self, method: dict[str, Any])` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L90) — Create full method signature for JavaScript
  - `_format_class_section(self, class_info: dict[str, Any], data: dict[str, Any])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L46) — Format a single class section with its methods
  - `_format_full_table(self, data: dict[str, Any])` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L13) — Full table format for JavaScript - matches golden master format
  - `_format_method_table_row(self, method: dict[str, Any])` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L81) — Format a method table row for JavaScript (golden master format)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`trim_trailing_blank_lines`](../_legacy_table_formatter_common.md#trim_trailing_blank_lines), [`_list_or_empty`](_javascript_formatter_full_mixin.md#_list_or_empty), [`_append_classes_overview`](_javascript_formatter_full_mixin.md#_append_classes_overview), [`_append_method_section`](_javascript_formatter_full_mixin.md#_append_method_section), [`_title`](_javascript_formatter_full_mixin.md#_title), [`_items_in_range`](_javascript_formatter_full_mixin.md#_items_in_range), [`_module_level_functions`](_javascript_formatter_full_mixin.md#_module_level_functions)
- used by: [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`format_advanced`](javascript_formatter.md#JavaScriptTableFormatter.format_advanced)

## Functions
- `_append_classes_overview(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]])` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L125)
- `_append_method_section(lines: list[str], title: str, header: str, separator: str, methods: list[dict[str, Any]], row_formatter: Any)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L174)
- `_items_in_range(items: list[dict[str, Any]], start: int, end: int)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L147)
- `_list_or_empty(value: Any)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L110)
- `_module_level_functions(methods: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L157) — Return methods that don't fall inside any class range.
- `_title(data: dict[str, Any], classes: list[dict[str, Any]])` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_full_mixin.py#L114)

