---
title: 'Module: tree_sitter_analyzer/formatters/ruby_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/ruby_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.ruby_formatter`/Ruby
symbols:
  RubyTableFormatter: TableFormatter#
  RubyFullFormatter: FullFormatter#
  RubyCompactFormatter: CompactFormatter#
  RubyCSVFormatter: CSVFormatter#
  RubyTableFormatter._format_full_table: TableFormatter#_format_full_table().
  RubyTableFormatter._format_compact_table: TableFormatter#_format_compact_table().
  RubyTableFormatter._format_csv: TableFormatter#_format_csv().
  RubyTableFormatter._get_visibility_symbol: TableFormatter#_get_visibility_symbol().
  RubyTableFormatter._format_signature: TableFormatter#_format_signature().
  RubyTableFormatter._format_compact_signature: TableFormatter#_format_compact_signature().
  RubyFullFormatter.format: FullFormatter#format().
  RubyCompactFormatter.format: CompactFormatter#format().
  RubyCSVFormatter.format: CSVFormatter#format().
---
# Module: [`tree_sitter_analyzer/formatters/ruby_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py)

## Classes
### `RubyCSVFormatter`  ·  implements/extends RubyTableFormatter
- def: [`tree_sitter_analyzer/formatters/ruby_formatter.py:64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L64)
- doc: CSV formatter for Ruby
- signature: `class RubyCSVFormatter(RubyTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L67) — Format data as CSV
- uses (calls/refs, reference-scoped): [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`_format_csv`](ruby_formatter.md#RubyTableFormatter._format_csv)
- used by: [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `RubyCompactFormatter`  ·  implements/extends RubyTableFormatter
- def: [`tree_sitter_analyzer/formatters/ruby_formatter.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L56)
- doc: Compact table formatter for Ruby
- signature: `class RubyCompactFormatter(RubyTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L59) — Format data as compact table
- uses (calls/refs, reference-scoped): [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`_format_compact_table`](ruby_formatter.md#RubyTableFormatter._format_compact_table)
- used by: [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `RubyFullFormatter`  ·  implements/extends RubyTableFormatter
- def: [`tree_sitter_analyzer/formatters/ruby_formatter.py:48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L48)
- doc: Full table formatter for Ruby
- signature: `class RubyFullFormatter(RubyTableFormatter):`
- members:
  - `format(self, data: dict[str, Any])` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L51) — Format data as full table
- uses (calls/refs, reference-scoped): [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`_format_full_table`](ruby_formatter.md#RubyTableFormatter._format_full_table)
- used by: [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`format`](base_formatter.md#BaseFormatter.format)  (1 test-only)

### `RubyTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/ruby_formatter.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L20)
- doc: Table formatter specialized for Ruby, following Java golden master format.
- signature: `class RubyTableFormatter(BaseTableFormatter):`
- members:
  - `_format_compact_signature(self, method: dict[str, Any])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L31) — Format compact method signature.
  - `_format_compact_table(self, data: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L39) — Compact table format for Ruby, following Java golden master format.
  - `_format_csv(self, data: dict[str, Any])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L43) — CSV format for Ruby, following Java golden master format.
  - `_format_full_table(self, data: dict[str, Any])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L35) — Full table format for Ruby, following Java golden master format.
  - `_format_signature(self, method: dict[str, Any])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L27) — Format method signature like Java: (param:type):returnType.
  - `_get_visibility_symbol(self, visibility: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/ruby_formatter.py#L23) — Convert visibility to symbol.
- uses (calls/refs, reference-scoped): [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`format_full_table`](_ruby_formatter_helpers.md#format_full_table), [`format_csv`](_ruby_formatter_helpers.md#format_csv), [`format_signature`](_ruby_formatter_helpers.md#format_signature), [`get_visibility_symbol`](_ruby_formatter_helpers.md#get_visibility_symbol), [`format_compact_table`](_ruby_formatter_helpers.md#format_compact_table), [`format_compact_signature`](_ruby_formatter_helpers.md#format_compact_signature), [`RubyCSVFormatter`](ruby_formatter.md#RubyCSVFormatter), [`RubyCompactFormatter`](ruby_formatter.md#RubyCompactFormatter), [`RubyFullFormatter`](ruby_formatter.md#RubyFullFormatter)
- used by: [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`RubyCSVFormatter`](ruby_formatter.md#RubyCSVFormatter), [`RubyCompactFormatter`](ruby_formatter.md#RubyCompactFormatter), [`RubyFullFormatter`](ruby_formatter.md#RubyFullFormatter), [`format`](ruby_formatter.md#RubyCSVFormatter.format), [`format`](ruby_formatter.md#RubyCompactFormatter.format), [`format`](ruby_formatter.md#RubyFullFormatter.format)  (23 test-only)

