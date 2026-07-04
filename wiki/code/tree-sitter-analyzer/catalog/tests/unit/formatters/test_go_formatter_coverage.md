---
title: 'Module: tests/unit/formatters/test_go_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_go_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_go_formatter_coverage`/TestGoTableFormatter
symbols:
  TestGoTableFormatterFormatMethods.test_format_table_json: FormatMethods#test_format_table_json().
  TestGoTableFormatterFormatMethods.test_format_table_full: FormatMethods#test_format_table_full().
  TestGoTableFormatterFormatMethods.test_format_summary: FormatMethods#test_format_summary().
  TestGoTableFormatterFormatMethods.test_format_advanced_json: FormatMethods#test_format_advanced_json().
  TestGoTableFormatterFormatMethods.test_format_advanced_csv: FormatMethods#test_format_advanced_csv().
  TestGoTableFormatterFormatMethods.test_format_advanced_full: FormatMethods#test_format_advanced_full().
  TestGoTableFormatterFormatMethods._base_data: FormatMethods#_base_data().
  TestGoTableFormatterFullTable.test_basic_package: FullTable#test_basic_package().
  TestGoTableFormatterFullTable.test_package_with_functions: FullTable#test_package_with_functions().
  TestGoTableFormatterFullTable.test_package_with_structs: FullTable#test_package_with_structs().
  TestGoTableFormatterFullTable.test_package_with_interfaces: FullTable#test_package_with_interfaces().
  TestGoTableFormatterFullTable.test_package_with_type_aliases: FullTable#test_package_with_type_aliases().
  TestGoTableFormatterFullTable.test_package_with_methods_receivers: FullTable#test_package_with_methods_receivers().
  TestGoTableFormatterFullTable.test_package_with_variables: FullTable#test_package_with_variables().
  TestGoTableFormatterFullTable.test_package_no_name: FullTable#test_package_no_name().
  TestGoTableFormatterCompactTable.test_compact_with_functions: CompactTable#test_compact_with_functions().
  TestGoTableFormatterCompactTable.test_compact_empty_data: CompactTable#test_compact_empty_data().
  TestGoTableFormatterCompactTable.test_compact_with_structs: CompactTable#test_compact_with_structs().
  TestGoTableFormatterCSV.test_csv_format_basic: CSV#test_csv_format_basic().
  TestGoTableFormatterCSV.test_csv_format_empty: CSV#test_csv_format_empty().
  TestGoTableFormatterHelperMethods.test_get_package_name: HelperMethods#test_get_package_name().
  TestGoTableFormatterHelperMethods.test_get_package_name_empty: HelperMethods#test_get_package_name_empty().
  TestGoTableFormatterHelperMethods.test_get_package_name_no_key: HelperMethods#test_get_package_name_no_key().
  TestGoTableFormatterHelperMethods.test_go_visibility_exported: HelperMethods#test_go_visibility_exported().
  TestGoTableFormatterHelperMethods.test_go_visibility_unexported: HelperMethods#test_go_visibility_unexported().
  TestGoTableFormatterHelperMethods.test_go_visibility_empty: HelperMethods#test_go_visibility_empty().
  TestGoTableFormatterHelperMethods.test_extract_doc_summary: HelperMethods#test_extract_doc_summary().
  TestGoTableFormatterHelperMethods.test_extract_doc_summary_empty: HelperMethods#test_extract_doc_summary_empty().
  TestGoTableFormatterHelperMethods.test_get_platform_newline: HelperMethods#test_get_platform_newline().
  TestGoTableFormatterEdgeCases.test_invalid_format_type: EdgeCases#test_invalid_format_type().
  TestGoTableFormatterEdgeCases.test_function_with_multiple_returns: EdgeCases#test_function_with_multiple_returns().
  TestGoTableFormatterEdgeCases.test_method_with_pointer_receiver: EdgeCases#test_method_with_pointer_receiver().
  TestGoTableFormatterEdgeCases.test_import_with_alias: EdgeCases#test_import_with_alias().
  TestGoTableFormatterEdgeCases.test_empty_struct: EdgeCases#test_empty_struct().
  TestGoTableFormatterFormatTypeInit.test_full_format_type: FormatTypeInit#test_full_format_type().
  TestGoTableFormatterFormatTypeInit.test_compact_format_type: FormatTypeInit#test_compact_format_type().
  TestGoTableFormatterFormatTypeInit.test_csv_format_type: FormatTypeInit#test_csv_format_type().
  TestGoTableFormatterFormatTypeInit.test_default_format_type: FormatTypeInit#test_default_format_type().
  TestGoTableFormatterMethods.test_methods_with_is_method_flag: Methods#test_methods_with_is_method_flag().
  TestGoTableFormatterMethods.test_mixed_funcs_and_methods: Methods#test_mixed_funcs_and_methods().
  TestGoTableFormatterSignatures.test_create_go_signature_string_params: Signatures#test_create_go_signature_string_params().
  TestGoTableFormatterSignatures.test_create_go_signature_no_return: Signatures#test_create_go_signature_no_return().
  TestGoTableFormatterSignatures.test_shorten_go_type_pointer: Signatures#test_shorten_go_type_pointer().
  TestGoTableFormatterSignatures.test_shorten_go_type_slice: Signatures#test_shorten_go_type_slice().
  TestGoTableFormatterSignatures.test_shorten_go_type_basic: Signatures#test_shorten_go_type_basic().
  TestGoTableFormatterSignatures.test_shorten_go_type_long_custom: Signatures#test_shorten_go_type_long_custom().
  TestGoTableFormatterSignatures.test_shorten_go_type_short_custom: Signatures#test_shorten_go_type_short_custom().
  TestGoTableFormatterSignatures.test_shorten_go_type_empty: Signatures#test_shorten_go_type_empty().
  TestGoTableFormatterPackageName.test_get_package_name_dict: PackageName#test_get_package_name_dict().
  TestGoTableFormatterFormatMethods.test_format_json_serialization_error: FormatMethods#test_format_json_serialization_error().
  TestGoTableFormatterFormatMethods.test_format_json_valid_data: FormatMethods#test_format_json_valid_data().
  TestGoTableFormatterFullTable: FullTable#
  TestGoTableFormatterCompactTable: CompactTable#
  TestGoTableFormatterCSV: CSV#
  TestGoTableFormatterHelperMethods: HelperMethods#
  TestGoTableFormatterEdgeCases: EdgeCases#
  TestGoTableFormatterFormatTypeInit: FormatTypeInit#
  TestGoTableFormatterMethods: Methods#
  TestGoTableFormatterSignatures: Signatures#
  TestGoTableFormatterPackageName: PackageName#
  TestGoTableFormatterFormatMethods: FormatMethods#
---
# Module: [`tests/unit/formatters/test_go_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py)

## Classes
### `TestGoTableFormatterCSV`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L307)
- doc: Test CSV format.
- signature: `class TestGoTableFormatterCSV:`
- members:
  - `test_csv_format_basic(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L310) — Test basic CSV output.
  - `test_csv_format_empty(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L342) — Test CSV with no data.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)

### `TestGoTableFormatterCompactTable`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L239)
- doc: Test _format_compact_table method.
- signature: `class TestGoTableFormatterCompactTable:`
- members:
  - `test_compact_empty_data(self)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L266) — Test compact format with empty data.
  - `test_compact_with_functions(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L242) — Test compact format with functions.
  - `test_compact_with_structs(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L282) — Test compact format with structs.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)

### `TestGoTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L423)
- doc: Test edge cases and error handling.
- signature: `class TestGoTableFormatterEdgeCases:`
- members:
  - `test_empty_struct(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L508) — Test empty struct.
  - `test_function_with_multiple_returns(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L433) — Test function with multiple return values.
  - `test_import_with_alias(self)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L489) — Test import with alias.
  - `test_invalid_format_type(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L426) — Test with invalid format type.
  - `test_method_with_pointer_receiver(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L457) — Test method with pointer receiver.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)

### `TestGoTableFormatterFormatMethods`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:697`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L697)
- doc: Test format_table, format_summary, format_advanced.
- signature: `class TestGoTableFormatterFormatMethods:`
- members:
  - `test_format_advanced_csv(self)` — [`L739`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L739) — Test format_advanced with csv output.
  - `test_format_advanced_full(self)` — [`L746`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L746) — Test format_advanced with full output.
  - `test_format_advanced_json(self)` — [`L732`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L732) — Test format_advanced with json output.
  - `test_format_json_serialization_error(self)` — [`L753`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L753) — Test _format_json handles serialization errors.
  - `test_format_json_valid_data(self)` — [`L759`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L759) — Test _format_json with valid data.
  - `test_format_summary(self)` — [`L725`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L725) — Test format_summary returns compact table.
  - `test_format_table_full(self)` — [`L718`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L718) — Test format_table with full type.
  - `test_format_table_json(self)` — [`L711`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L711) — Test format_table with json type.
- protocol/private: `_base_data`[`L700`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L700)
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_advanced), [`format_table`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_table), [`format_summary`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_summary), [`_format_json`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._format_json)

### `TestGoTableFormatterFormatTypeInit`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L532)
- doc: Test format type initialization.
- signature: `class TestGoTableFormatterFormatTypeInit:`
- members:
  - `test_compact_format_type(self)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L540) — Test creating formatter with compact format type.
  - `test_csv_format_type(self)` — [`L545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L545) — Test creating formatter with csv format type.
  - `test_default_format_type(self)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L550) — Test creating formatter with default format type.
  - `test_full_format_type(self)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L535) — Test creating formatter with full format type.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_type)

### `TestGoTableFormatterFullTable`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L9)
- doc: Test _format_full_table method.
- signature: `class TestGoTableFormatterFullTable:`
- members:
  - `test_basic_package(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L12) — Test basic package formatting.
  - `test_package_no_name(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L222) — Test package with no name (fallback to main).
  - `test_package_with_functions(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L29) — Test package with functions.
  - `test_package_with_interfaces(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L93) — Test package with interfaces.
  - `test_package_with_methods_receivers(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L151) — Test methods with receivers.
  - `test_package_with_structs(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L61) — Test package with structs.
  - `test_package_with_type_aliases(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L122) — Test package with type aliases.
  - `test_package_with_variables(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L191) — Test package with variables.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)

### `TestGoTableFormatterHelperMethods`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L359)
- doc: Test helper methods.
- signature: `class TestGoTableFormatterHelperMethods:`
- members:
  - `test_extract_doc_summary(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L401) — Test _extract_doc_summary.
  - `test_extract_doc_summary_empty(self)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L409) — Test _extract_doc_summary with empty string.
  - `test_get_package_name(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L362) — Test _get_package_name with packages.
  - `test_get_package_name_empty(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L369) — Test _get_package_name with no packages.
  - `test_get_package_name_no_key(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L376) — Test _get_package_name with missing key.
  - `test_get_platform_newline(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L416) — Test _get_platform_newline returns string.
  - `test_go_visibility_empty(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L395) — Test _go_visibility with empty string.
  - `test_go_visibility_exported(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L383) — Test _go_visibility for exported names.
  - `test_go_visibility_unexported(self)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L389) — Test _go_visibility for unexported names.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`_extract_doc_summary`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._extract_doc_summary), [`_go_visibility`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._go_visibility), [`_get_platform_newline`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._get_platform_newline), [`_get_package_name`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._get_package_name)

### `TestGoTableFormatterMethods`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L556)
- doc: Test methods with is_method flag for ## Methods section.
- signature: `class TestGoTableFormatterMethods:`
- members:
  - `test_methods_with_is_method_flag(self)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L559) — Test that methods with is_method=True appear in Methods section.
  - `test_mixed_funcs_and_methods(self)` — [`L599`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L599) — Test package with both functions and methods.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)

### `TestGoTableFormatterPackageName`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:687`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L687)
- doc: Test _get_package_name variants.
- signature: `class TestGoTableFormatterPackageName:`
- members:
  - `test_get_package_name_dict(self)` — [`L690`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L690) — Test _get_package_name with package dict.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`_get_package_name`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._get_package_name)

### `TestGoTableFormatterSignatures`
- def: [`tests/unit/formatters/test_go_formatter_coverage.py:632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L632)
- doc: Test signature formatting helpers.
- signature: `class TestGoTableFormatterSignatures:`
- members:
  - `test_create_go_signature_no_return(self)` — [`L643`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L643) — Test _create_go_signature with no return type.
  - `test_create_go_signature_string_params(self)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L635) — Test _create_go_signature with string params (not list).
  - `test_shorten_go_type_basic(self)` — [`L663`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L663) — Test _shorten_go_type with basic types.
  - `test_shorten_go_type_empty(self)` — [`L681`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L681) — Test _shorten_go_type with empty string.
  - `test_shorten_go_type_long_custom(self)` — [`L670`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L670) — Test _shorten_go_type truncates long custom types.
  - `test_shorten_go_type_pointer(self)` — [`L651`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L651) — Test _shorten_go_type with pointer type.
  - `test_shorten_go_type_short_custom(self)` — [`L676`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L676) — Test _shorten_go_type keeps short custom types as-is.
  - `test_shorten_go_type_slice(self)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_coverage.py#L657) — Test _shorten_go_type with slice type.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`_create_go_signature`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._create_go_signature), [`_shorten_go_type`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._shorten_go_type)

