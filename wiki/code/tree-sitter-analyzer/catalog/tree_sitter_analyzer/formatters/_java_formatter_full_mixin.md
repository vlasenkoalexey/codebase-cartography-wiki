---
title: 'Module: tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._java_formatter_full_mixin`/
symbols:
  JavaTableFormatterFullMixin._format_full_table: JavaTableFormatterFullMixin#_format_full_table().
  _java_title: _java_title().
  _class_overview_row: _class_overview_row().
  _exclude_inner_members: _exclude_inner_members().
  JavaTableFormatterFullMixin: JavaTableFormatterFullMixin#
  _append_multi_class: _append_multi_class().
  _java_file_stem: _java_file_stem().
  _append_package: _append_package().
  _append_imports: _append_imports().
  _append_single_class: _append_single_class().
---
# Module: [`tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py)

## Classes
### `JavaTableFormatterFullMixin`
- def: [`tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L17)
- doc: Full-format rendering helpers.
- signature: `class JavaTableFormatterFullMixin:`
- members:
  - `_format_full_table(self, data: dict[str, Any])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L20) — Full table format for Java - matches golden master format
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`trim_trailing_blank_lines`](../_legacy_table_formatter_common.md#trim_trailing_blank_lines), [`_java_title`](_java_formatter_full_mixin.md#_java_title), [`is_inner_class`](_java_formatter_class_mixin.md#is_inner_class), [`_append_multi_class`](_java_formatter_full_mixin.md#_append_multi_class), [`_append_imports`](_java_formatter_full_mixin.md#_append_imports), [`_append_package`](_java_formatter_full_mixin.md#_append_package), [`_append_single_class`](_java_formatter_full_mixin.md#_append_single_class)
- used by: [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`format_advanced`](java_formatter.md#JavaTableFormatter.format_advanced)  (29 test-only)

## Functions
- `_append_imports(lines: list[str], imports: list[dict[str, Any]])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L77)
- `_append_multi_class(lines: list[str], classes: list[dict[str, Any]], data: dict[str, Any], formatter: Any)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L114)
- `_append_package(lines: list[str], package_name: str)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L68)
- `_append_single_class(lines: list[str], single_class: dict[str, Any], data: dict[str, Any], package_name: str, formatter: Any)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L89)
- `_class_overview_row(class_info: dict[str, Any], data: dict[str, Any], classes: list[dict[str, Any]], formatter: Any)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L132)
- `_exclude_inner_members(formatter: Any, class_info: dict[str, Any], classes: list[dict[str, Any]], class_methods: list[dict[str, Any]], class_fields: list[dict[str, Any]])` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L155)
- `_java_file_stem(file_path: str)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L61)
- `_java_title(formatter: Any, data: dict[str, Any], package_name: str, classes: list[dict[str, Any]])` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_full_mixin.py#L41)

