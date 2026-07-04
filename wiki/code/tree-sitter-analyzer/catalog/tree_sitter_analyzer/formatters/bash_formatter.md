---
title: 'Module: tree_sitter_analyzer/formatters/bash_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/bash_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.bash_formatter`/
symbols:
  BashTableFormatter: BashTableFormatter#
  BashTableFormatter.format_structure: BashTableFormatter#format_structure().
  BashTableFormatter.format_type: BashTableFormatter#format_type.
  BashTableFormatter._format_full_table: BashTableFormatter#_format_full_table().
  BashTableFormatter._format_func_row: BashTableFormatter#_format_func_row().
  BashTableFormatter.format_advanced: BashTableFormatter#format_advanced().
  BashTableFormatter._format_compact_table: BashTableFormatter#_format_compact_table().
  BashTableFormatter._format_compact_func_row: BashTableFormatter#_format_compact_func_row().
  BashTableFormatter._format_field_row: BashTableFormatter#_format_field_row().
  BashTableFormatter._bash_visibility: BashTableFormatter#_bash_visibility().
  BashTableFormatter.format_table: BashTableFormatter#format_table().
  BashTableFormatter.format_summary: BashTableFormatter#format_summary().
  BashTableFormatter._format_json: BashTableFormatter#_format_json().
  _file_stem: _file_stem().
  BashTableFormatter._create_bash_signature: BashTableFormatter#_create_bash_signature().
---
# Module: [`tree_sitter_analyzer/formatters/bash_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py)

## Classes
### `BashTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/bash_formatter.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L15)
- doc: Table formatter specialised for Bash / shell scripts.
- signature: `class BashTableFormatter(BaseTableFormatter):`
- members:
  - `_bash_visibility(name: str)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L199) — Bash functions starting with '_' are conventionally private.
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L43) — Advanced output for Bash.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L39) — Dispatch to the correct sub-formatter.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L35) — Compact table (summary) for Bash.
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L22) — Format table output for Bash.
  - `format_type` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L27)
- protocol/private: `_create_bash_signature`[`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L186), `_format_compact_func_row`[`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L161), `_format_compact_table`[`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L116), `_format_field_row`[`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L174), `_format_full_table`[`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L57), `_format_func_row`[`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L149), `_format_json`[`L207`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L207)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_extract_doc_summary`](base_formatter.md#BaseTableFormatter._extract_doc_summary), [`_file_stem`](bash_formatter.md#_file_stem)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced)  (9 test-only)

## Functions
- `_file_stem(file_path: str)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/bash_formatter.py#L216) — Return just the filename (no directory) from a path.

