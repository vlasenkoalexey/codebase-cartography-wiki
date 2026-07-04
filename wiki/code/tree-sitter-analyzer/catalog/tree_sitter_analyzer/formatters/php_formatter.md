---
title: 'Module: tree_sitter_analyzer/formatters/php_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/php_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.php_formatter`/PHP
symbols:
  PHPTableFormatter: TableFormatter#
  PHPTableFormatter._extract_namespace: TableFormatter#_extract_namespace().
  PHPFullFormatter: FullFormatter#
  PHPCompactFormatter: CompactFormatter#
  PHPCSVFormatter: CSVFormatter#
  PHPTableFormatter._format_signature: TableFormatter#_format_signature().
  PHPTableFormatter._format_full_table: TableFormatter#_format_full_table().
  PHPTableFormatter._format_compact_table: TableFormatter#_format_compact_table().
  PHPTableFormatter._format_csv: TableFormatter#_format_csv().
  PHPTableFormatter._get_visibility_symbol: TableFormatter#_get_visibility_symbol().
  PHPTableFormatter._format_compact_signature: TableFormatter#_format_compact_signature().
  PHPFullFormatter.format: FullFormatter#format().
  PHPCompactFormatter.format: CompactFormatter#format().
  PHPCSVFormatter.format: CSVFormatter#format().
---
# Module: [`tree_sitter_analyzer/formatters/php_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py)

## Classes
### `PHPCSVFormatter`  ·  implements/extends PHPTableFormatter
- def: [`tree_sitter_analyzer/formatters/php_formatter.py:115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L115)
- doc: CSV formatter for PHP
- signature: `class PHPCSVFormatter(PHPTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L118) — Format data as CSV
- uses (calls/refs, reference-scoped): [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`_format_csv`](php_formatter.md#PHPTableFormatter._format_csv)
- used by: [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `PHPCompactFormatter`  ·  implements/extends PHPTableFormatter
- def: [`tree_sitter_analyzer/formatters/php_formatter.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L107)
- doc: Compact table formatter for PHP
- signature: `class PHPCompactFormatter(PHPTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L110) — Format data as compact table
- uses (calls/refs, reference-scoped): [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`_format_compact_table`](php_formatter.md#PHPTableFormatter._format_compact_table)
- used by: [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `PHPFullFormatter`  ·  implements/extends PHPTableFormatter
- def: [`tree_sitter_analyzer/formatters/php_formatter.py:99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L99)
- doc: Full table formatter for PHP
- signature: `class PHPFullFormatter(PHPTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L102) — Format data as full table
- uses (calls/refs, reference-scoped): [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`_format_full_table`](php_formatter.md#PHPTableFormatter._format_full_table)
- used by: [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `PHPTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/php_formatter.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L20)
- doc: Table formatter specialized for PHP, following Java golden master format.
- signature: `class PHPTableFormatter(BaseTableFormatter):`
- members:
  - `_extract_namespace(self, data: dict[str, Any])` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L38) — Extract namespace from data.
  - `_format_compact_signature(self, method: dict[str, Any])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L33) — Format compact method signature.
  - `_format_compact_table(self, data: dict[str, Any])` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L48) — Compact table format for PHP, following Java golden master format.
  - `_format_csv(self, data: dict[str, Any])` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L53) — CSV format for PHP, following Java golden master format.
  - `_format_full_table(self, data: dict[str, Any])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L43) — Full table format for PHP, following Java golden master format.
  - `_format_signature(self, method: dict[str, Any])` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L28) — Format method signature like Java: ($param:type):returnType.
  - `_get_visibility_symbol(self, visibility: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/php_formatter.py#L23) — Convert visibility to symbol.
- uses (calls/refs, reference-scoped): [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`format_full_table`](_php_formatter_helpers.md#format_full_table), [`format_compact_table`](_php_formatter_helpers.md#format_compact_table), [`format_signature`](_php_formatter_helpers.md#format_signature), [`get_visibility_symbol`](_php_formatter_helpers.md#get_visibility_symbol), [`extract_namespace`](_php_formatter_helpers.md#extract_namespace), [`format_compact_signature`](_php_formatter_helpers.md#format_compact_signature), [`PHPCSVFormatter`](php_formatter.md#PHPCSVFormatter), [`PHPCompactFormatter`](php_formatter.md#PHPCompactFormatter), [`PHPFullFormatter`](php_formatter.md#PHPFullFormatter)
- used by: [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`PHPCSVFormatter`](php_formatter.md#PHPCSVFormatter), [`PHPCompactFormatter`](php_formatter.md#PHPCompactFormatter), [`PHPFullFormatter`](php_formatter.md#PHPFullFormatter), [`format`](php_formatter.md#PHPCSVFormatter.format), [`format`](php_formatter.md#PHPCompactFormatter.format), [`format`](php_formatter.md#PHPFullFormatter.format)  (25 test-only)

