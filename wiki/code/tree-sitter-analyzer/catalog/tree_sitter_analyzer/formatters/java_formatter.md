---
title: 'Module: tree_sitter_analyzer/formatters/java_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/java_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.java_formatter`/
symbols:
  JavaTableFormatter: JavaTableFormatter#
  JavaTableFormatter.format_type: JavaTableFormatter#format_type.
  JavaTableFormatter.format_advanced: JavaTableFormatter#format_advanced().
  JavaTableFormatter._format_json: JavaTableFormatter#_format_json.
  JavaTableFormatter.format_table: JavaTableFormatter#format_table().
  JavaTableFormatter.format_summary: JavaTableFormatter#format_summary().
  _format_json: _format_json().
---
# Module: [`tree_sitter_analyzer/formatters/java_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py)

## Classes
### `JavaTableFormatter`  ·  implements/extends BaseTableFormatter, JavaTableFormatterClassMixin, JavaTableFormatterCompactMixin, JavaTableFormatterFullMixin, JavaTableFormatterSignaturesMixin
- def: [`tree_sitter_analyzer/formatters/java_formatter.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L25)
- doc: Table formatter specialized for Java
- signature: `class JavaTableFormatter(JavaTableFormatterFullMixin, JavaTableFormatterClassMixin, JavaTableFormatterCompactMixin, JavaTableFormatterSignaturesMixin, BaseTableFormatter):`
- members:
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L54) — Format advanced analysis output for Java
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L50) — Format summary output for Java
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L36) — Format table output for Java
  - `format_type` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L41)
- protocol/private: `_format_json`[`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L34)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_full_table`](_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin._format_compact_table), [`JavaTableFormatterClassMixin`](_java_formatter_class_mixin.md#JavaTableFormatterClassMixin), [`JavaTableFormatterCompactMixin`](_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin), [`JavaTableFormatterFullMixin`](_java_formatter_full_mixin.md#JavaTableFormatterFullMixin), [`JavaTableFormatterSignaturesMixin`](_java_formatter_signatures_mixin.md#JavaTableFormatterSignaturesMixin), [`_format_json`](java_formatter.md#_format_json)
- used by: [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`JavaTableFormatterClassMixin`](_java_formatter_class_mixin.md#JavaTableFormatterClassMixin), [`JavaTableFormatterCompactMixin`](_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin), [`JavaTableFormatterFullMixin`](_java_formatter_full_mixin.md#JavaTableFormatterFullMixin), [`JavaTableFormatterSignaturesMixin`](_java_formatter_signatures_mixin.md#JavaTableFormatterSignaturesMixin)  (83 test-only)

## Functions
- `_format_json(data: dict[str, Any])` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/java_formatter.py#L15) — Format data as JSON.

