---
title: 'Module: tree_sitter_analyzer/formatters/rust_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/rust_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.rust_formatter`/
symbols:
  RustTableFormatter: RustTableFormatter#
  RustTableFormatter._format_fn_row: RustTableFormatter#_format_fn_row().
  RustTableFormatter._format_compact_table: RustTableFormatter#_format_compact_table().
  RustTableFormatter._format_full_table: RustTableFormatter#_format_full_table().
  RustTableFormatter.format_type: RustTableFormatter#format_type.
  RustTableFormatter.format_advanced: RustTableFormatter#format_advanced().
  RustTableFormatter.format_structure: RustTableFormatter#format_structure().
  RustTableFormatter._format_rust_param: RustTableFormatter#_format_rust_param().
  RustTableFormatter._create_full_signature: RustTableFormatter#_create_full_signature().
  RustTableFormatter.format_table: RustTableFormatter#format_table().
  RustTableFormatter._convert_visibility: RustTableFormatter#_convert_visibility().
  RustTableFormatter.format_summary: RustTableFormatter#format_summary().
  RustTableFormatter._format_json: RustTableFormatter#_format_json().
  RustTableFormatter._create_compact_signature: RustTableFormatter#_create_compact_signature().
  _count_items_in_line_range: _count_items_in_line_range().
---
# Module: [`tree_sitter_analyzer/formatters/rust_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py)

## Classes
### `RustTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/rust_formatter.py:30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L30)
- doc: Table formatter specialized for Rust
- signature: `class RustTableFormatter(BaseTableFormatter):`
- members:
  - `_convert_visibility(self, visibility: str)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L211) — Convert visibility to short symbol
  - `_create_compact_signature(self, fn: dict[str, Any])` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L201) — Create compact function signature for Rust
  - `_create_full_signature(self, fn: dict[str, Any])` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L192) — Create full function signature for Rust
  - `_format_compact_table(self, data: dict[str, Any])` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L109) — Compact table format for Rust
  - `_format_fn_row(self, fn: dict[str, Any])` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L153) — Format a function table row for Rust
  - `_format_full_table(self, data: dict[str, Any])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L33) — Full table format for Rust
  - `_format_json(self, data: dict[str, Any])` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L265) — Format data as JSON
  - `_format_rust_param(param: Any)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L172) — Render one Rust parameter as proper Rust syntax (never a raw dict repr).
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L254) — Format advanced analysis output for Rust
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L243) — Format structure analysis output for Rust.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L239) — Format summary output for Rust
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L221) — Format table output for Rust
  - `format_type` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L227)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_extract_doc_summary`](base_formatter.md#BaseTableFormatter._extract_doc_summary), [`_clean_csv_text`](base_formatter.md#BaseTableFormatter._clean_csv_text), [`_count_items_in_line_range`](rust_formatter.md#_count_items_in_line_range)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`_create_full_signature`](base_formatter.md#BaseTableFormatter._create_full_signature), [`_convert_visibility`](base_formatter.md#BaseTableFormatter._convert_visibility)  (45 test-only)

## Functions
- `_count_items_in_line_range(items: list[dict[str, Any]], line_range: dict[str, Any])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/rust_formatter.py#L11) — Count items whose ``line_range.start`` falls inside ``line_range``.

