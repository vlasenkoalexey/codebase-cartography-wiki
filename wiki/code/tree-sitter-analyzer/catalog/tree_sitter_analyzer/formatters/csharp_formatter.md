---
title: 'Module: tree_sitter_analyzer/formatters/csharp_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/csharp_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.csharp_formatter`/CSharpTableFormatter#
symbols:
  CSharpTableFormatter: ''
  CSharpTableFormatter._format_full_table: _format_full_table().
  CSharpTableFormatter._format_compact_table: _format_compact_table().
  CSharpTableFormatter._convert_visibility: _convert_visibility().
  CSharpTableFormatter._format_method_row: _format_method_row().
  CSharpTableFormatter._abbreviate_type: _abbreviate_type().
  CSharpTableFormatter._format_csv: _format_csv().
  CSharpTableFormatter._create_compact_signature: _create_compact_signature().
  CSharpTableFormatter._extract_namespace: _extract_namespace().
  CSharpTableFormatter._create_full_signature: _create_full_signature().
  CSharpTableFormatter._format_modifiers: _format_modifiers().
  CSharpTableFormatter._get_class_methods: _get_class_methods().
  CSharpTableFormatter._get_class_fields: _get_class_fields().
---
# Module: [`tree_sitter_analyzer/formatters/csharp_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py)

## Classes
### `CSharpTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/csharp_formatter.py:16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L16)
- doc: Table formatter specialized for C#
- signature: `class CSharpTableFormatter(BaseTableFormatter):`
- members:
  - `_abbreviate_type(self, type_str: str)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L168) — Abbreviate type name for compact display
  - `_convert_visibility(self, visibility: str)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L194) — Convert visibility to symbol
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L105) — Create compact method signature
  - `_create_full_signature(self, method: dict[str, Any])` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L82) — Create full method signature
  - `_extract_namespace(self, data: dict[str, Any])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L156) — Extract namespace from data
  - `_format_compact_table(self, data: dict[str, Any])` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L30) — Compact table format for C# - matches golden master format
  - `_format_csv(self, data: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L39) — CSV format for C# - matches golden master format
  - `_format_full_table(self, data: dict[str, Any])` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L19) — Full table format for C# - matches golden master format
  - `_format_method_row(self, method: dict[str, Any])` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L67) — Format a method table row
  - `_format_modifiers(self, element: dict[str, Any])` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L128) — Format element modifiers
  - `_get_class_fields(self, fields: list[dict[str, Any]], line_range: dict[str, int])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L55) — Get fields within a class range
  - `_get_class_methods(self, methods: list[dict[str, Any]], line_range: dict[str, int])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/csharp_formatter.py#L43) — Get methods within a class range
- uses (calls/refs, reference-scoped): [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`format_csharp_full_table`](_csharp_formatter_helpers.md#format_csharp_full_table), [`format_csharp_compact_table`](_csharp_formatter_helpers.md#format_csharp_compact_table), [`format_csharp_csv`](_csharp_formatter_helpers.md#format_csharp_csv)
- used by: [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`_create_full_signature`](base_formatter.md#BaseTableFormatter._create_full_signature), [`_convert_visibility`](base_formatter.md#BaseTableFormatter._convert_visibility)  (35 test-only)

