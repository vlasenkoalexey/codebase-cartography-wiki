---
title: 'Module: tree_sitter_analyzer/formatters/javascript_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/javascript_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.javascript_formatter`/
symbols:
  JavaScriptTableFormatter: JavaScriptTableFormatter#
  JavaScriptTableFormatter.format_type: JavaScriptTableFormatter#format_type.
  JavaScriptTableFormatter.format: JavaScriptTableFormatter#format().
  JavaScriptTableFormatter.format_advanced: JavaScriptTableFormatter#format_advanced().
  JavaScriptTableFormatter.format_table: JavaScriptTableFormatter#format_table().
  JavaScriptTableFormatter._format_json: JavaScriptTableFormatter#_format_json.
  JavaScriptTableFormatter.format_summary: JavaScriptTableFormatter#format_summary().
  _format_json: _format_json().
---
# Module: [`tree_sitter_analyzer/formatters/javascript_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py)

## Classes
### `JavaScriptTableFormatter`  ·  implements/extends BaseTableFormatter, JavaScriptTableFormatterCompactMixin, JavaScriptTableFormatterFullMixin, JavaScriptTableFormatterRowsMixin, JavaScriptTableFormatterTypeMixin
- def: [`tree_sitter_analyzer/formatters/javascript_formatter.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L29)
- doc: Table formatter specialized for JavaScript
- signature: `class JavaScriptTableFormatter(JavaScriptTableFormatterFullMixin, JavaScriptTableFormatterCompactMixin, JavaScriptTableFormatterRowsMixin, JavaScriptTableFormatterTypeMixin, BaseTableFormatter):`
- members:
  - `format(self, data: dict[str, Any] | None, format_type: str = "full")` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L40) — Format data using the configured format type
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L82) — Format advanced analysis output for JavaScript
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L78) — Format summary output for JavaScript
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L67) — Format table output for JavaScript
  - `format_type` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L61)
- protocol/private: `_format_json`[`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L38)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_full_table`](_javascript_formatter_full_mixin.md#JavaScriptTableFormatterFullMixin._format_full_table), [`_format_compact_table`](_javascript_formatter_compact_mixin.md#JavaScriptTableFormatterCompactMixin._format_compact_table), [`JavaScriptTableFormatterCompactMixin`](_javascript_formatter_compact_mixin.md#JavaScriptTableFormatterCompactMixin), [`JavaScriptTableFormatterFullMixin`](_javascript_formatter_full_mixin.md#JavaScriptTableFormatterFullMixin), [`JavaScriptTableFormatterRowsMixin`](_javascript_formatter_rows_mixin.md#JavaScriptTableFormatterRowsMixin), [`JavaScriptTableFormatterTypeMixin`](_javascript_formatter_type_mixin.md#JavaScriptTableFormatterTypeMixin), [`_format_json`](javascript_formatter.md#_format_json)
- used by: [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format`](base_formatter.md#BaseFormatter.format), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`JavaScriptTableFormatterCompactMixin`](_javascript_formatter_compact_mixin.md#JavaScriptTableFormatterCompactMixin), [`JavaScriptTableFormatterFullMixin`](_javascript_formatter_full_mixin.md#JavaScriptTableFormatterFullMixin), [`JavaScriptTableFormatterRowsMixin`](_javascript_formatter_rows_mixin.md#JavaScriptTableFormatterRowsMixin), [`JavaScriptTableFormatterTypeMixin`](_javascript_formatter_type_mixin.md#JavaScriptTableFormatterTypeMixin)  (19 test-only)

## Functions
- `_format_json(data: dict[str, Any])` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/javascript_formatter.py#L19) — Format data as JSON.

