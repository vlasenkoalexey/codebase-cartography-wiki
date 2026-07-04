---
title: 'Module: tests/unit/formatters/test_csharp_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_csharp_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_csharp_formatter_coverage`/TestCSharpTableFormatter
symbols:
  TestCSharpTableFormatterFullTable.test_single_class_with_namespace: FullTable#test_single_class_with_namespace().
  TestCSharpTableFormatterFullTable.test_single_class_without_namespace: FullTable#test_single_class_without_namespace().
  TestCSharpTableFormatterFullTable.test_multiple_classes_with_namespace: FullTable#test_multiple_classes_with_namespace().
  TestCSharpTableFormatterFullTable.test_multiple_classes_without_namespace: FullTable#test_multiple_classes_without_namespace().
  TestCSharpTableFormatterFullTable.test_class_with_methods_having_parameters: FullTable#test_class_with_methods_having_parameters().
  TestCSharpTableFormatterFullTable.test_empty_classes: FullTable#test_empty_classes().
  TestCSharpTableFormatterCompactTable.test_compact_with_classes: CompactTable#test_compact_with_classes().
  TestCSharpTableFormatterCompactTable.test_compact_empty_data: CompactTable#test_compact_empty_data().
  TestCSharpTableFormatterCompactTable.test_compact_multiple_classes: CompactTable#test_compact_multiple_classes().
  TestCSharpTableFormatterCSV.test_csv_format_basic: CSV#test_csv_format_basic().
  TestCSharpTableFormatterCSV.test_csv_format_empty: CSV#test_csv_format_empty().
  TestCSharpTableFormatterHelperMethods.test_extract_namespace_with_full_qualified_name: HelperMethods#test_extract_namespace_with_full_qualified_name().
  TestCSharpTableFormatterHelperMethods.test_extract_namespace_without_dot: HelperMethods#test_extract_namespace_without_dot().
  TestCSharpTableFormatterHelperMethods.test_extract_namespace_empty: HelperMethods#test_extract_namespace_empty().
  TestCSharpTableFormatterHelperMethods.test_get_platform_newline: HelperMethods#test_get_platform_newline().
  TestCSharpTableFormatterHelperMethods.test_convert_to_platform_newlines: HelperMethods#test_convert_to_platform_newlines().
  TestCSharpTableFormatterHelperMethods.test_create_full_signature: HelperMethods#test_create_full_signature().
  TestCSharpTableFormatterHelperMethods.test_create_compact_signature: HelperMethods#test_create_compact_signature().
  TestCSharpTableFormatterHelperMethods.test_format_modifiers: HelperMethods#test_format_modifiers().
  TestCSharpTableFormatterHelperMethods.test_abbreviate_type_simple: HelperMethods#test_abbreviate_type_simple().
  TestCSharpTableFormatterHelperMethods.test_abbreviate_type_with_namespace: HelperMethods#test_abbreviate_type_with_namespace().
  TestCSharpTableFormatterHelperMethods.test_convert_visibility: HelperMethods#test_convert_visibility().
  TestCSharpTableFormatterEdgeCases.test_invalid_format_type: EdgeCases#test_invalid_format_type().
  TestCSharpTableFormatterEdgeCases.test_method_with_no_parameters: EdgeCases#test_method_with_no_parameters().
  TestCSharpTableFormatterEdgeCases.test_class_with_static_methods: EdgeCases#test_class_with_static_methods().
  TestCSharpTableFormatterEdgeCases.test_class_with_constructor: EdgeCases#test_class_with_constructor().
  TestCSharpTableFormatterEdgeCases.test_interface_class_type: EdgeCases#test_interface_class_type().
  TestCSharpTableFormatterEdgeCases.test_struct_class_type: EdgeCases#test_struct_class_type().
  TestCSharpTableFormatterEdgeCases.test_method_with_documentation: EdgeCases#test_method_with_documentation().
  TestCSharpTableFormatterEdgeCases.test_field_with_modifiers: EdgeCases#test_field_with_modifiers().
  TestCSharpTableFormatterFormatTypeInit.test_full_format_type: FormatTypeInit#test_full_format_type().
  TestCSharpTableFormatterFormatTypeInit.test_compact_format_type: FormatTypeInit#test_compact_format_type().
  TestCSharpTableFormatterFormatTypeInit.test_csv_format_type: FormatTypeInit#test_csv_format_type().
  TestCSharpTableFormatterFormatTypeInit.test_default_format_type: FormatTypeInit#test_default_format_type().
  TestCSharpTableFormatterFullTable: FullTable#
  TestCSharpTableFormatterCompactTable: CompactTable#
  TestCSharpTableFormatterCSV: CSV#
  TestCSharpTableFormatterHelperMethods: HelperMethods#
  TestCSharpTableFormatterEdgeCases: EdgeCases#
  TestCSharpTableFormatterFormatTypeInit: FormatTypeInit#
---
# Module: [`tests/unit/formatters/test_csharp_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py)

## Classes
### `TestCSharpTableFormatterCSV`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L296)
- doc: Test CSV format.
- signature: `class TestCSharpTableFormatterCSV:`
- members:
  - `test_csv_format_basic(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L299) — Test basic CSV output.
  - `test_csv_format_empty(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L338) — Test CSV with no methods or fields.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter)

### `TestCSharpTableFormatterCompactTable`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L205)
- doc: Test _format_compact_table method.
- signature: `class TestCSharpTableFormatterCompactTable:`
- members:
  - `test_compact_empty_data(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L245) — Test compact format with empty data.
  - `test_compact_multiple_classes(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L259) — Test compact format with multiple classes.
  - `test_compact_with_classes(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L208) — Test compact format with classes.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter)

### `TestCSharpTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L438)
- doc: Test edge cases and error handling.
- signature: `class TestCSharpTableFormatterEdgeCases:`
- members:
  - `test_class_with_constructor(self)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L507) — Test class with constructor.
  - `test_class_with_static_methods(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L477) — Test class with static methods.
  - `test_field_with_modifiers(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L626) — Test field with modifiers.
  - `test_interface_class_type(self)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L537) — Test interface as class type.
  - `test_invalid_format_type(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L441) — Test with invalid format type.
  - `test_method_with_documentation(self)` — [`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L596) — Test method with documentation.
  - `test_method_with_no_parameters(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L448) — Test method with empty parameters list.
  - `test_struct_class_type(self)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L567) — Test struct as class type.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter)

### `TestCSharpTableFormatterFormatTypeInit`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:656`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L656)
- doc: Test format type initialization.
- signature: `class TestCSharpTableFormatterFormatTypeInit:`
- members:
  - `test_compact_format_type(self)` — [`L664`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L664) — Test creating formatter with compact format type.
  - `test_csv_format_type(self)` — [`L669`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L669) — Test creating formatter with csv format type.
  - `test_default_format_type(self)` — [`L674`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L674) — Test creating formatter with default format type.
  - `test_full_format_type(self)` — [`L659`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L659) — Test creating formatter with full format type.
- uses (calls/refs, reference-scoped): [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_type)

### `TestCSharpTableFormatterFullTable`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L9)
- doc: Test _format_full_table method.
- signature: `class TestCSharpTableFormatterFullTable:`
- members:
  - `test_class_with_methods_having_parameters(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L148) — Test class with methods having parameters.
  - `test_empty_classes(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L189) — Test data with no classes.
  - `test_multiple_classes_with_namespace(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L75) — Test multiple classes with namespace.
  - `test_multiple_classes_without_namespace(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L120) — Test multiple classes without namespace.
  - `test_single_class_with_namespace(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L12) — Test single class with namespace via full_qualified_name.
  - `test_single_class_without_namespace(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L54) — Test single class without namespace.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter)

### `TestCSharpTableFormatterHelperMethods`
- def: [`tests/unit/formatters/test_csharp_formatter_coverage.py:354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L354)
- doc: Test helper methods.
- signature: `class TestCSharpTableFormatterHelperMethods:`
- members:
  - `test_abbreviate_type_simple(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L416) — Test _abbreviate_type with simple types.
  - `test_abbreviate_type_with_namespace(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L423) — Test _abbreviate_type removes namespace.
  - `test_convert_to_platform_newlines(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L384) — Test _convert_to_platform_newlines.
  - `test_convert_visibility(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L429) — Test _convert_visibility method.
  - `test_create_compact_signature(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L401) — Test _create_compact_signature method.
  - `test_create_full_signature(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L393) — Test _create_full_signature method.
  - `test_extract_namespace_empty(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L371) — Test _extract_namespace with no namespace.
  - `test_extract_namespace_with_full_qualified_name(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L357) — Test _extract_namespace with full_qualified_name.
  - `test_extract_namespace_without_dot(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L364) — Test _extract_namespace with no dot in name.
  - `test_format_modifiers(self)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L408) — Test _format_modifiers method.
  - `test_get_platform_newline(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_coverage.py#L378) — Test _get_platform_newline returns string.
- uses (calls/refs, reference-scoped): [`CSharpTableFormatter`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter), [`_convert_to_platform_newlines`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._convert_to_platform_newlines), [`_get_platform_newline`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._get_platform_newline), [`_convert_visibility`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._convert_visibility), [`_abbreviate_type`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._abbreviate_type), [`_create_compact_signature`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._create_compact_signature), [`_extract_namespace`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._extract_namespace), [`_create_full_signature`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._create_full_signature), [`_format_modifiers`](../../../tree_sitter_analyzer/formatters/csharp_formatter.md#CSharpTableFormatter._format_modifiers)

