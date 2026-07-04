---
title: 'Module: tests/unit/formatters/test_ruby_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_ruby_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_ruby_formatter_coverage`/TestRubyTableFormatter
symbols:
  TestRubyTableFormatterFullTable.test_single_class: FullTable#test_single_class().
  TestRubyTableFormatterFullTable.test_multiple_classes: FullTable#test_multiple_classes().
  TestRubyTableFormatterFullTable.test_module: FullTable#test_module().
  TestRubyTableFormatterFullTable.test_class_with_constants: FullTable#test_class_with_constants().
  TestRubyTableFormatterFullTable.test_class_with_methods_and_params: FullTable#test_class_with_methods_and_params().
  TestRubyTableFormatterFullTable.test_empty_classes: FullTable#test_empty_classes().
  TestRubyTableFormatterFullTable.test_singleton_class: FullTable#test_singleton_class().
  TestRubyTableFormatterCompactTable.test_compact_with_classes: CompactTable#test_compact_with_classes().
  TestRubyTableFormatterCompactTable.test_compact_empty_data: CompactTable#test_compact_empty_data().
  TestRubyTableFormatterCompactTable.test_compact_multiple_classes: CompactTable#test_compact_multiple_classes().
  TestRubyTableFormatterCSV.test_csv_format_basic: CSV#test_csv_format_basic().
  TestRubyTableFormatterCSV.test_csv_format_empty: CSV#test_csv_format_empty().
  TestRubyTableFormatterHelperMethods.test_get_platform_newline: HelperMethods#test_get_platform_newline().
  TestRubyTableFormatterHelperMethods.test_convert_to_platform_newlines: HelperMethods#test_convert_to_platform_newlines().
  TestRubyTableFormatterEdgeCases.test_invalid_format_type: EdgeCases#test_invalid_format_type().
  TestRubyTableFormatterEdgeCases.test_method_with_block: EdgeCases#test_method_with_block().
  TestRubyTableFormatterEdgeCases.test_method_with_splat: EdgeCases#test_method_with_splat().
  TestRubyTableFormatterEdgeCases.test_class_with_inheritance: EdgeCases#test_class_with_inheritance().
  TestRubyTableFormatterFormatTypeInit.test_full_format_type: FormatTypeInit#test_full_format_type().
  TestRubyTableFormatterFormatTypeInit.test_compact_format_type: FormatTypeInit#test_compact_format_type().
  TestRubyTableFormatterFormatTypeInit.test_csv_format_type: FormatTypeInit#test_csv_format_type().
  TestRubyTableFormatterFormatTypeInit.test_default_format_type: FormatTypeInit#test_default_format_type().
  TestRubyTableFormatterFullTable: FullTable#
  TestRubyTableFormatterCompactTable: CompactTable#
  TestRubyTableFormatterCSV: CSV#
  TestRubyTableFormatterHelperMethods: HelperMethods#
  TestRubyTableFormatterEdgeCases: EdgeCases#
  TestRubyTableFormatterFormatTypeInit: FormatTypeInit#
---
# Module: [`tests/unit/formatters/test_ruby_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py)

## Classes
### `TestRubyTableFormatterCSV`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L312)
- doc: Test CSV format.
- signature: `class TestRubyTableFormatterCSV:`
- members:
  - `test_csv_format_basic(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L315) — Test basic CSV output.
  - `test_csv_format_empty(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L353) — Test CSV with no methods or fields.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter)

### `TestRubyTableFormatterCompactTable`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L231)
- doc: Test _format_compact_table method.
- signature: `class TestRubyTableFormatterCompactTable:`
- members:
  - `test_compact_empty_data(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L262) — Test compact format with empty data.
  - `test_compact_multiple_classes(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L276) — Test compact format with multiple classes.
  - `test_compact_with_classes(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L234) — Test compact format with classes.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter)

### `TestRubyTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L387)
- doc: Test edge cases and error handling.
- signature: `class TestRubyTableFormatterEdgeCases:`
- members:
  - `test_class_with_inheritance(self)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L453) — Test class with inheritance.
  - `test_invalid_format_type(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L390) — Test with invalid format type.
  - `test_method_with_block(self)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L397) — Test method with block parameter.
  - `test_method_with_splat(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L425) — Test method with splat parameter.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter)

### `TestRubyTableFormatterFormatTypeInit`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L475)
- doc: Test format type initialization.
- signature: `class TestRubyTableFormatterFormatTypeInit:`
- members:
  - `test_compact_format_type(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L483) — Test creating formatter with compact format type.
  - `test_csv_format_type(self)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L488) — Test creating formatter with csv format type.
  - `test_default_format_type(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L493) — Test creating formatter with default format type.
  - `test_full_format_type(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L478) — Test creating formatter with full format type.
- uses (calls/refs, reference-scoped): [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_type)

### `TestRubyTableFormatterFullTable`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L9)
- doc: Test _format_full_table method.
- signature: `class TestRubyTableFormatterFullTable:`
- members:
  - `test_class_with_constants(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L115) — Test class with constants.
  - `test_class_with_methods_and_params(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L150) — Test class with methods having parameters.
  - `test_empty_classes(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L186) — Test data with no classes.
  - `test_module(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L85) — Test module type.
  - `test_multiple_classes(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L50) — Test multiple classes.
  - `test_single_class(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L12) — Test single class.
  - `test_singleton_class(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L201) — Test singleton class.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter)

### `TestRubyTableFormatterHelperMethods`
- def: [`tests/unit/formatters/test_ruby_formatter_coverage.py:368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L368)
- doc: Test helper methods.
- signature: `class TestRubyTableFormatterHelperMethods:`
- members:
  - `test_convert_to_platform_newlines(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L377) — Test _convert_to_platform_newlines.
  - `test_get_platform_newline(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_coverage.py#L371) — Test _get_platform_newline returns string.
- uses (calls/refs, reference-scoped): [`RubyTableFormatter`](../../../tree_sitter_analyzer/formatters/ruby_formatter.md#RubyTableFormatter), [`_convert_to_platform_newlines`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._convert_to_platform_newlines), [`_get_platform_newline`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._get_platform_newline)

