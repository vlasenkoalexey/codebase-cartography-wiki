---
title: 'Module: tree_sitter_analyzer/formatters/go_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/go_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.go_formatter`/GoTableFormatter#
symbols:
  GoTableFormatter: ''
  GoTableFormatter.format_structure: format_structure().
  GoTableFormatter._format_full_table: _format_full_table().
  GoTableFormatter.format_type: format_type.
  GoTableFormatter._create_go_signature: _create_go_signature().
  GoTableFormatter._format_compact_table: _format_compact_table().
  GoTableFormatter._shorten_go_type: _shorten_go_type().
  GoTableFormatter.format_advanced: format_advanced().
  GoTableFormatter._go_visibility: _go_visibility().
  GoTableFormatter._format_func_row: _format_func_row().
  GoTableFormatter._format_method_row: _format_method_row().
  GoTableFormatter.format_table: format_table().
  GoTableFormatter._get_package_name: _get_package_name().
  GoTableFormatter.format_summary: format_summary().
  GoTableFormatter._format_json: _format_json().
  GoTableFormatter._create_go_compact_signature: _create_go_compact_signature().
  GoTableFormatter._format_go_param: _format_go_param().
---
# Module: [`tree_sitter_analyzer/formatters/go_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py)

## Classes
### `GoTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/go_formatter.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L20)
- doc: Table formatter specialized for Go
- signature: `class GoTableFormatter(BaseTableFormatter):`
- members:
  - `_create_go_compact_signature(self, func: dict[str, Any])` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L131) — Create compact Go function signature
  - `_create_go_signature(self, func: dict[str, Any])` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L107) — Create Go function signature
  - `_format_compact_table(self, data: dict[str, Any])` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L34) — Compact table format for Go
  - `_format_full_table(self, data: dict[str, Any])` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L23) — Full table format for Go
  - `_format_func_row(self, func: dict[str, Any])` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L80) — Format a function table row for Go
  - `_format_go_param(param: Any)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L121) — Render one Go parameter as 'name type' (never a raw dict repr).
  - `_format_json(self, data: dict[str, Any])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L230) — Format data as JSON
  - `_format_method_row(self, method: dict[str, Any])` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L92) — Format a method table row for Go (with receiver)
  - `_get_package_name(self, data: dict[str, Any])` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L183) — Extract package name from data
  - `_go_visibility(self, name: str)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L177) — Determine Go visibility based on name capitalization
  - `_shorten_go_type(self, type_name: str)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L141) — Shorten Go type name for compact display
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L219) — Format advanced analysis output for Go
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L215) — Format structure analysis output for Go
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L211) — Format summary output for Go
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L197) — Format table output for Go
  - `format_type` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/go_formatter.py#L202)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`format_go_full_table`](_go_formatter_helpers.md#format_go_full_table), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_extract_doc_summary`](base_formatter.md#BaseTableFormatter._extract_doc_summary)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced)  (68 test-only)

