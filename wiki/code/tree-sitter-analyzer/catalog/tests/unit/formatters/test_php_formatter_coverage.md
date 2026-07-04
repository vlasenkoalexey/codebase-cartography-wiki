---
title: 'Module: tests/unit/formatters/test_php_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_php_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_php_formatter_coverage`/TestPHPTableFormatter
symbols:
  TestPHPTableFormatterFullTable.test_single_class_with_namespace: FullTable#test_single_class_with_namespace().
  TestPHPTableFormatterFullTable.test_single_class_without_namespace: FullTable#test_single_class_without_namespace().
  TestPHPTableFormatterFullTable.test_multiple_classes_with_namespace: FullTable#test_multiple_classes_with_namespace().
  TestPHPTableFormatterFullTable.test_multiple_classes_without_namespace: FullTable#test_multiple_classes_without_namespace().
  TestPHPTableFormatterFullTable.test_class_with_trait: FullTable#test_class_with_trait().
  TestPHPTableFormatterFullTable.test_interface: FullTable#test_interface().
  TestPHPTableFormatterFullTable.test_class_with_methods_and_params: FullTable#test_class_with_methods_and_params().
  TestPHPTableFormatterFullTable.test_empty_classes: FullTable#test_empty_classes().
  TestPHPTableFormatterCompactTable.test_compact_with_classes: CompactTable#test_compact_with_classes().
  TestPHPTableFormatterCompactTable.test_compact_empty_data: CompactTable#test_compact_empty_data().
  TestPHPTableFormatterCompactTable.test_compact_multiple_classes: CompactTable#test_compact_multiple_classes().
  TestPHPTableFormatterCSV.test_csv_format_basic: CSV#test_csv_format_basic().
  TestPHPTableFormatterCSV.test_csv_format_empty: CSV#test_csv_format_empty().
  TestPHPTableFormatterHelperMethods.test_extract_namespace_with_metadata: HelperMethods#test_extract_namespace_with_metadata().
  TestPHPTableFormatterHelperMethods.test_extract_namespace_from_method_metadata: HelperMethods#test_extract_namespace_from_method_metadata().
  TestPHPTableFormatterHelperMethods.test_extract_namespace_empty: HelperMethods#test_extract_namespace_empty().
  TestPHPTableFormatterHelperMethods.test_get_platform_newline: HelperMethods#test_get_platform_newline().
  TestPHPTableFormatterEdgeCases.test_invalid_format_type: EdgeCases#test_invalid_format_type().
  TestPHPTableFormatterEdgeCases.test_abstract_class: EdgeCases#test_abstract_class().
  TestPHPTableFormatterEdgeCases.test_static_method: EdgeCases#test_static_method().
  TestPHPTableFormatterFormatTypeInit.test_full_format_type: FormatTypeInit#test_full_format_type().
  TestPHPTableFormatterFormatTypeInit.test_compact_format_type: FormatTypeInit#test_compact_format_type().
  TestPHPTableFormatterFormatTypeInit.test_csv_format_type: FormatTypeInit#test_csv_format_type().
  TestPHPTableFormatterFormatTypeInit.test_default_format_type: FormatTypeInit#test_default_format_type().
  TestPHPTableFormatterFullTable: FullTable#
  TestPHPTableFormatterCompactTable: CompactTable#
  TestPHPTableFormatterCSV: CSV#
  TestPHPTableFormatterHelperMethods: HelperMethods#
  TestPHPTableFormatterEdgeCases: EdgeCases#
  TestPHPTableFormatterFormatTypeInit: FormatTypeInit#
---
# Module: [`tests/unit/formatters/test_php_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py)

## Classes
### `TestPHPTableFormatterCSV`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L344)
- doc: Test CSV format.
- signature: `class TestPHPTableFormatterCSV:`
- members:
  - `test_csv_format_basic(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L347) — Test basic CSV output.
  - `test_csv_format_empty(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L385) — Test CSV with no methods or fields.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter)

### `TestPHPTableFormatterCompactTable`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L253)
- doc: Test _format_compact_table method.
- signature: `class TestPHPTableFormatterCompactTable:`
- members:
  - `test_compact_empty_data(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L292) — Test compact format with empty data.
  - `test_compact_multiple_classes(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L306) — Test compact format with multiple classes.
  - `test_compact_with_classes(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L256) — Test compact format with classes.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter)

### `TestPHPTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L436)
- doc: Test edge cases and error handling.
- signature: `class TestPHPTableFormatterEdgeCases:`
- members:
  - `test_abstract_class(self)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L446) — Test abstract class type.
  - `test_invalid_format_type(self)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L439) — Test with invalid format type.
  - `test_static_method(self)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L475) — Test static method.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter)

### `TestPHPTableFormatterFormatTypeInit`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L506)
- doc: Test format type initialization.
- signature: `class TestPHPTableFormatterFormatTypeInit:`
- members:
  - `test_compact_format_type(self)` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L514) — Test creating formatter with compact format type.
  - `test_csv_format_type(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L519) — Test creating formatter with csv format type.
  - `test_default_format_type(self)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L524) — Test creating formatter with default format type.
  - `test_full_format_type(self)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L509) — Test creating formatter with full format type.
- uses (calls/refs, reference-scoped): [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_type)

### `TestPHPTableFormatterFullTable`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L9)
- doc: Test _format_full_table method.
- signature: `class TestPHPTableFormatterFullTable:`
- members:
  - `test_class_with_methods_and_params(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L198) — Test class with methods having parameters.
  - `test_class_with_trait(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L138) — Test class with trait type.
  - `test_empty_classes(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L237) — Test data with no classes.
  - `test_interface(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L168) — Test interface type.
  - `test_multiple_classes_with_namespace(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L72) — Test multiple classes with namespace.
  - `test_multiple_classes_without_namespace(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L110) — Test multiple classes without namespace.
  - `test_single_class_with_namespace(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L12) — Test single class with namespace via full_qualified_name.
  - `test_single_class_without_namespace(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L51) — Test single class without namespace.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter)

### `TestPHPTableFormatterHelperMethods`
- def: [`tests/unit/formatters/test_php_formatter_coverage.py:400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L400)
- doc: Test helper methods.
- signature: `class TestPHPTableFormatterHelperMethods:`
- members:
  - `test_extract_namespace_empty(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L421) — Test _extract_namespace with no namespace.
  - `test_extract_namespace_from_method_metadata(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L410) — Test _extract_namespace from method metadata (no longer supported).
  - `test_extract_namespace_with_metadata(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L403) — Test _extract_namespace with metadata namespace.
  - `test_get_platform_newline(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_coverage.py#L429) — Test _get_platform_newline returns string.
- uses (calls/refs, reference-scoped): [`PHPTableFormatter`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter), [`_get_platform_newline`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._get_platform_newline), [`_extract_namespace`](../../../tree_sitter_analyzer/formatters/php_formatter.md#PHPTableFormatter._extract_namespace)

