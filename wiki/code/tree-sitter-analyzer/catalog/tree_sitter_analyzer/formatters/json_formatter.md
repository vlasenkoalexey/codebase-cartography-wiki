---
title: 'Module: tree_sitter_analyzer/formatters/json_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/json_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.json_formatter`/JSONFormatter#
symbols:
  JSONFormatter: ''
  JSONFormatter.format_structure: format_structure().
  JSONFormatter._format_prop_row: _format_prop_row().
  JSONFormatter.format_advanced: format_advanced().
  JSONFormatter.format_summary: format_summary().
  JSONFormatter._format_json_output: _format_json_output().
  JSONFormatter.format_table: format_table().
  JSONFormatter.language: language.
  JSONFormatter.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/formatters/json_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py)

## Classes
### `JSONFormatter`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/json_formatter.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L15)
- doc: Formatter for JSON files.
- signature: `class JSONFormatter(BaseFormatter):`
- members:
  - `_format_json_output(self, title: str, data: dict[str, Any])` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L158) — Format data as a titled JSON block (matches BaseFormatter convention).
  - `_format_prop_row(self, p: dict[str, Any])` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L139) — Format one property as a markdown table row.
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L99) — Advanced analysis: nesting distribution + value-type breakdown.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L44) — Main structure table used by analyze_code_structure.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L25) — Short summary: root type + top-level key count.
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L130)
  - `language` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L19)
- protocol/private: `__init__`[`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/json_formatter.py#L18)
- uses (calls/refs, reference-scoped): [`BaseFormatter`](base_formatter.md#BaseFormatter)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (33 test-only)

