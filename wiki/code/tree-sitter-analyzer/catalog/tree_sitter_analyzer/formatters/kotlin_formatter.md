---
title: 'Module: tree_sitter_analyzer/formatters/kotlin_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/kotlin_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.kotlin_formatter`/
symbols:
  KotlinTableFormatter: KotlinTableFormatter#
  KotlinTableFormatter._format_full_table: KotlinTableFormatter#_format_full_table().
  KotlinTableFormatter._format_fn_row: KotlinTableFormatter#_format_fn_row().
  KotlinTableFormatter._format_compact_table: KotlinTableFormatter#_format_compact_table().
  KotlinTableFormatter.format_type: KotlinTableFormatter#format_type.
  KotlinTableFormatter._format_prop_row: KotlinTableFormatter#_format_prop_row().
  KotlinTableFormatter.format_advanced: KotlinTableFormatter#format_advanced().
  KotlinTableFormatter.format_structure: KotlinTableFormatter#format_structure().
  KotlinTableFormatter._convert_visibility: KotlinTableFormatter#_convert_visibility().
  KotlinTableFormatter.format_table: KotlinTableFormatter#format_table().
  KotlinTableFormatter.format_summary: KotlinTableFormatter#format_summary().
  KotlinTableFormatter._format_json: KotlinTableFormatter#_format_json().
  KotlinTableFormatter._create_full_signature: KotlinTableFormatter#_create_full_signature().
  _count_items_in_line_range: _count_items_in_line_range().
  KotlinTableFormatter._create_compact_signature: KotlinTableFormatter#_create_compact_signature().
---
# Module: [`tree_sitter_analyzer/formatters/kotlin_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py)

## Classes
### `KotlinTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/kotlin_formatter.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L29)
- doc: Table formatter specialized for Kotlin
- signature: `class KotlinTableFormatter(BaseTableFormatter):`
- members:
  - `_convert_visibility(self, visibility: str)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L219) — Convert visibility to short symbol
  - `_create_compact_signature(self, fn: dict[str, Any])` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L210) — Create compact function signature for Kotlin
  - `_create_full_signature(self, fn: dict[str, Any])` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L192) — Create full function signature for Kotlin
  - `_format_compact_table(self, data: dict[str, Any])` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L107) — Compact table format for Kotlin
  - `_format_fn_row(self, fn: dict[str, Any])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L156) — Format a function table row for Kotlin
  - `_format_full_table(self, data: dict[str, Any])` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L32) — Full table format for Kotlin
  - `_format_json(self, data: dict[str, Any])` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L275) — Format data as JSON
  - `_format_prop_row(self, prop: dict[str, Any])` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L174) — Format a property table row for Kotlin
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L264) — Format advanced analysis output for Kotlin
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L253) — Format structure analysis output for Kotlin.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L249) — Format summary output for Kotlin
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L231) — Format table output for Kotlin
  - `format_type` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L237)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_extract_doc_summary`](base_formatter.md#BaseTableFormatter._extract_doc_summary), [`_clean_csv_text`](base_formatter.md#BaseTableFormatter._clean_csv_text), [`_count_items_in_line_range`](kotlin_formatter.md#_count_items_in_line_range)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`_create_full_signature`](base_formatter.md#BaseTableFormatter._create_full_signature), [`_convert_visibility`](base_formatter.md#BaseTableFormatter._convert_visibility)  (41 test-only)

## Functions
- `_count_items_in_line_range(items: list[dict[str, Any]], line_range: dict[str, Any])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/kotlin_formatter.py#L11) — Count items whose ``line_range.start`` falls inside ``line_range``.

