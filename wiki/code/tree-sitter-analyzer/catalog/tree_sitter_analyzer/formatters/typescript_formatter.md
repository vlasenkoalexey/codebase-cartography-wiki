---
title: 'Module: tree_sitter_analyzer/formatters/typescript_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/typescript_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.typescript_formatter`/TypeScriptTableFormatter#
symbols:
  TypeScriptTableFormatter: ''
  TypeScriptTableFormatter.format_type: format_type.
  TypeScriptTableFormatter.format_structure: format_structure().
  TypeScriptTableFormatter.format_advanced: format_advanced().
  TypeScriptTableFormatter.format: format().
  TypeScriptTableFormatter._format_full_table: _format_full_table().
  TypeScriptTableFormatter._format_compact_table: _format_compact_table().
  TypeScriptTableFormatter._format_csv: _format_csv().
  TypeScriptTableFormatter._format_signatures_table: _format_signatures_table().
  TypeScriptTableFormatter._get_class_methods: _get_class_methods().
  TypeScriptTableFormatter._get_class_fields: _get_class_fields().
  TypeScriptTableFormatter._format_method_row: _format_method_row().
  TypeScriptTableFormatter._create_full_signature: _create_full_signature().
  TypeScriptTableFormatter._create_compact_signature: _create_compact_signature().
  TypeScriptTableFormatter._create_csv_signature: _create_csv_signature().
  TypeScriptTableFormatter._format_modifiers: _format_modifiers().
  TypeScriptTableFormatter.format_table: format_table().
  TypeScriptTableFormatter.format_summary: format_summary().
  TypeScriptTableFormatter._format_json: _format_json().
---
# Module: [`tree_sitter_analyzer/formatters/typescript_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py)

## Classes
### `TypeScriptTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/typescript_formatter.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L28)
- doc: Table formatter specialized for TypeScript
- signature: `class TypeScriptTableFormatter(BaseTableFormatter):`
- members:
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L76) — Create compact method signature
  - `_create_csv_signature(self, method: dict[str, Any])` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L80) — Create CSV method signature with full parameter details
  - `_create_full_signature(self, method: dict[str, Any])` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L72) — Create full method signature
  - `_format_compact_table(self, data: dict[str, Any])` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L41) — Compact table format for TypeScript - matches golden master format
  - `_format_csv(self, data: dict[str, Any])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L46) — CSV format for TypeScript - matches golden master format
  - `_format_full_table(self, data: dict[str, Any])` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L36) — Full table format for TypeScript - matches golden master format
  - `_format_json(self, data: dict[str, Any])` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L125) — Format data as JSON
  - `_format_method_row(self, method: dict[str, Any])` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L68) — Format a method table row
  - `_format_modifiers(self, element: dict[str, Any])` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L85) — Format element modifiers
  - `_format_signatures_table(self, data: dict[str, Any])` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L51) — Signatures format for TypeScript — lightweight method-directory.
  - `_get_class_fields(self, fields: list[dict[str, Any]], line_range: dict[str, int])` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L61) — Get fields within a class range
  - `_get_class_methods(self, methods: list[dict[str, Any]], line_range: dict[str, int])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L55) — Get methods within a class range
  - `format(self, data: dict[str, Any])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L31) — Format data using the configured format type
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L113) — Format advanced analysis output for TypeScript
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L108) — Format structure analysis output for TypeScript
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L103) — Format summary output for TypeScript
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L90) — Format table output for TypeScript
  - `format_type` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/typescript_formatter.py#L95)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`format_typescript_signatures_table`](_typescript_formatter_signatures_table.md#format_typescript_signatures_table), [`format_typescript_full_table`](_typescript_formatter_full.md#format_typescript_full_table), [`format_method_row`](_typescript_formatter_helpers.md#format_method_row), [`format_typescript_compact_table`](_typescript_formatter_compact.md#format_typescript_compact_table), [`get_class_fields`](_typescript_formatter_helpers.md#get_class_fields), [`get_class_methods`](_typescript_formatter_helpers.md#get_class_methods), [`format_typescript_csv`](_typescript_formatter_csv.md#format_typescript_csv), [`create_csv_signature`](_typescript_formatter_helpers.md#create_csv_signature), [`create_full_signature`](_typescript_formatter_helpers.md#create_full_signature), [`create_compact_signature`](_typescript_formatter_helpers.md#create_compact_signature), [`format_typescript_modifiers`](_typescript_formatter_helpers.md#format_typescript_modifiers)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format`](base_formatter.md#BaseFormatter.format), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`_create_full_signature`](base_formatter.md#BaseTableFormatter._create_full_signature)  (16 test-only)

