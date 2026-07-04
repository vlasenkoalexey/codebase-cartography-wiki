---
title: 'Module: tests/unit/formatters/test_ruby_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_ruby_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_ruby_formatter_helpers`/Test
symbols:
  TestGetVisibilitySymbol.test_public: GetVisibilitySymbol#test_public().
  TestGetVisibilitySymbol.test_private: GetVisibilitySymbol#test_private().
  TestGetVisibilitySymbol.test_protected: GetVisibilitySymbol#test_protected().
  TestGetVisibilitySymbol.test_module: GetVisibilitySymbol#test_module().
  TestGetVisibilitySymbol.test_unknown_defaults_to_public: GetVisibilitySymbol#test_unknown_defaults_to_public().
  TestGetVisibilitySymbol.test_case_insensitive: GetVisibilitySymbol#test_case_insensitive().
  TestGetVisibilitySymbol.test_empty_string: GetVisibilitySymbol#test_empty_string().
  TestFormatSignature.test_no_params_no_return: FormatSignature#test_no_params_no_return().
  TestFormatSignature.test_single_param: FormatSignature#test_single_param().
  TestFormatSignature.test_multiple_params: FormatSignature#test_multiple_params().
  TestFormatSignature.test_return_type: FormatSignature#test_return_type().
  TestFormatSignature.test_dict_param_no_name: FormatSignature#test_dict_param_no_name().
  TestFormatSignature.test_string_param: FormatSignature#test_string_param().
  TestFormatSignature.test_missing_parameters_key: FormatSignature#test_missing_parameters_key().
  TestFormatCompactSignature.test_no_params: FormatCompactSignature#test_no_params().
  TestFormatCompactSignature.test_dict_params: FormatCompactSignature#test_dict_params().
  TestFormatCompactSignature.test_string_params: FormatCompactSignature#test_string_params().
  TestFormatCompactSignature.test_no_return_type: FormatCompactSignature#test_no_return_type().
  TestFormatCompactSignature.test_missing_parameters: FormatCompactSignature#test_missing_parameters().
  TestFormatFullTable.test_empty_data: FormatFullTable#test_empty_data().
  TestFormatFullTable.test_single_class: FormatFullTable#test_single_class().
  TestFormatFullTable.test_multiple_classes: FormatFullTable#test_multiple_classes().
  TestFormatFullTable.test_imports_section: FormatFullTable#test_imports_section().
  TestFormatFullTable.test_imports_skipped_when_empty: FormatFullTable#test_imports_skipped_when_empty().
  TestFormatFullTable.test_imports_skips_empty_raw_text: FormatFullTable#test_imports_skips_empty_raw_text().
  TestFormatFullTable.test_class_with_methods_and_fields: FormatFullTable#test_class_with_methods_and_fields().
  TestFormatFullTable.test_constructor_initialize: FormatFullTable#test_constructor_initialize().
  TestFormatFullTable.test_module_level_methods: FormatFullTable#test_module_level_methods().
  TestFormatFullTable.test_static_method_annotation: FormatFullTable#test_static_method_annotation().
  TestFormatFullTable.test_class_method_separator: FormatFullTable#test_class_method_separator().
  TestFormatFullTable.test_instance_method_separator: FormatFullTable#test_instance_method_separator().
  TestFormatFullTable.test_doc_truncation: FormatFullTable#test_doc_truncation().
  TestFormatFullTable.test_doc_none_treated_as_dash: FormatFullTable#test_doc_none_treated_as_dash().
  TestFormatCompactTable.test_empty_data: FormatCompactTable#test_empty_data().
  TestFormatCompactTable.test_with_methods: FormatCompactTable#test_with_methods().
  TestFormatCompactTable.test_compact_info_with_statistics: FormatCompactTable#test_compact_info_with_statistics().
  TestFormatCompactTable.test_compact_info_without_statistics: FormatCompactTable#test_compact_info_without_statistics().
  TestFormatCompactTable.test_compact_method_with_parent_class: FormatCompactTable#test_compact_method_with_parent_class().
  TestFormatCsv.test_header_row: FormatCsv#test_header_row().
  TestFormatCsv.test_fields: FormatCsv#test_fields().
  TestFormatCsv.test_methods: FormatCsv#test_methods().
  TestFormatCsv.test_constructor_in_csv: FormatCsv#test_constructor_in_csv().
  TestFormatCsv.test_csv_static_method: FormatCsv#test_csv_static_method().
  TestFormatCsv.test_csv_field_without_parent: FormatCsv#test_csv_field_without_parent().
  TestFormatCsv.test_csv_method_with_parent_class: FormatCsv#test_csv_method_with_parent_class().
  TestFormatCsv.test_csv_class_method_prefix: FormatCsv#test_csv_class_method_prefix().
  TestGetVisibilitySymbol: GetVisibilitySymbol#
  TestFormatSignature: FormatSignature#
  TestFormatCompactSignature: FormatCompactSignature#
  TestFormatFullTable: FormatFullTable#
  TestFormatCompactTable: FormatCompactTable#
  TestFormatCsv: FormatCsv#
---
# Module: [`tests/unit/formatters/test_ruby_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py)

## Classes
### `TestFormatCompactSignature`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L77)
- signature: `class TestFormatCompactSignature:`
- members:
  - `test_dict_params(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L83)
  - `test_missing_parameters(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L104)
  - `test_no_params(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L79)
  - `test_no_return_type(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L97)
  - `test_string_params(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L93)
- uses (calls/refs, reference-scoped): [`format_compact_signature`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#format_compact_signature)

### `TestFormatCompactTable`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L424)
- signature: `class TestFormatCompactTable:`
- members:
  - `test_compact_info_with_statistics(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L450)
  - `test_compact_info_without_statistics(self)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L461)
  - `test_compact_method_with_parent_class(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L473)
  - `test_empty_data(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L426)
  - `test_with_methods(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L431)
- uses (calls/refs, reference-scoped): [`format_compact_table`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#format_compact_table)

### `TestFormatCsv`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L493)
- signature: `class TestFormatCsv:`
- members:
  - `test_constructor_in_csv(self)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L533)
  - `test_csv_class_method_prefix(self)` — [`L600`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L600)
  - `test_csv_field_without_parent(self)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L567)
  - `test_csv_method_with_parent_class(self)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L582)
  - `test_csv_static_method(self)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L550)
  - `test_fields(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L499)
  - `test_header_row(self)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L495)
  - `test_methods(self)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L515)
- uses (calls/refs, reference-scoped): [`format_csv`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#format_csv)

### `TestFormatFullTable`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L109)
- signature: `class TestFormatFullTable:`
- members:
  - `test_class_method_separator(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L329)
  - `test_class_with_methods_and_fields(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L200)
  - `test_constructor_initialize(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L238)
  - `test_doc_none_treated_as_dash(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L403)
  - `test_doc_truncation(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L383)
  - `test_empty_data(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L111)
  - `test_imports_section(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L162)
  - `test_imports_skipped_when_empty(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L178)
  - `test_imports_skips_empty_raw_text(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L189)
  - `test_instance_method_separator(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L356)
  - `test_module_level_methods(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L275)
  - `test_multiple_classes(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L136)
  - `test_single_class(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L116)
  - `test_static_method_annotation(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L302)
- uses (calls/refs, reference-scoped): [`format_full_table`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#format_full_table)

### `TestFormatSignature`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L36)
- signature: `class TestFormatSignature:`
- members:
  - `test_dict_param_no_name(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L64)
  - `test_missing_parameters_key(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L72)
  - `test_multiple_params(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L50)
  - `test_no_params_no_return(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L38)
  - `test_return_type(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L60)
  - `test_single_param(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L43)
  - `test_string_param(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L68)
- uses (calls/refs, reference-scoped): [`format_signature`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#format_signature)

### `TestGetVisibilitySymbol`
- def: [`tests/unit/formatters/test_ruby_formatter_helpers.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L11)
- signature: `class TestGetVisibilitySymbol:`
- members:
  - `test_case_insensitive(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L28)
  - `test_empty_string(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L32)
  - `test_module(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L22)
  - `test_private(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L16)
  - `test_protected(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L19)
  - `test_public(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L13)
  - `test_unknown_defaults_to_public(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_ruby_formatter_helpers.py#L25)
- uses (calls/refs, reference-scoped): [`get_visibility_symbol`](../../../tree_sitter_analyzer/formatters/_ruby_formatter_helpers.md#get_visibility_symbol)

