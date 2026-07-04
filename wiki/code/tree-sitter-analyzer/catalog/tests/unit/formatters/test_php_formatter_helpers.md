---
title: 'Module: tests/unit/formatters/test_php_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_php_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_php_formatter_helpers`/Test
symbols:
  TestGetVisibilitySymbol.test_public: GetVisibilitySymbol#test_public().
  TestGetVisibilitySymbol.test_private: GetVisibilitySymbol#test_private().
  TestGetVisibilitySymbol.test_protected: GetVisibilitySymbol#test_protected().
  TestGetVisibilitySymbol.test_unknown: GetVisibilitySymbol#test_unknown().
  TestGetVisibilitySymbol.test_case_insensitive: GetVisibilitySymbol#test_case_insensitive().
  TestGetVisibilitySymbol.test_empty: GetVisibilitySymbol#test_empty().
  TestFormatSignature.test_no_params: FormatSignature#test_no_params().
  TestFormatSignature.test_single_param: FormatSignature#test_single_param().
  TestFormatSignature.test_multiple_params: FormatSignature#test_multiple_params().
  TestFormatSignature.test_dollar_sign_stripped: FormatSignature#test_dollar_sign_stripped().
  TestFormatSignature.test_param_no_name: FormatSignature#test_param_no_name().
  TestFormatSignature.test_string_param: FormatSignature#test_string_param().
  TestFormatSignature.test_empty_return_type: FormatSignature#test_empty_return_type().
  TestFormatSignature.test_missing_return_type_key: FormatSignature#test_missing_return_type_key().
  TestFormatCompactSignature.test_dict_params: FormatCompactSignature#test_dict_params().
  TestFormatCompactSignature.test_string_params: FormatCompactSignature#test_string_params().
  TestFormatCompactSignature.test_no_return_type: FormatCompactSignature#test_no_return_type().
  TestFormatCompactSignature.test_no_params: FormatCompactSignature#test_no_params().
  TestExtractNamespace.test_from_full_qualified_name: ExtractNamespace#test_from_full_qualified_name().
  TestExtractNamespace.test_from_metadata: ExtractNamespace#test_from_metadata().
  TestExtractNamespace.test_no_namespace: ExtractNamespace#test_no_namespace().
  TestExtractNamespace.test_empty_classes: ExtractNamespace#test_empty_classes().
  TestExtractNamespace.test_prefers_fqn_over_metadata: ExtractNamespace#test_prefers_fqn_over_metadata().
  TestFormatFullTable.test_empty_data: FormatFullTable#test_empty_data().
  TestFormatFullTable.test_single_class: FormatFullTable#test_single_class().
  TestFormatFullTable.test_imports_section: FormatFullTable#test_imports_section().
  TestFormatFullTable.test_empty_imports_skipped: FormatFullTable#test_empty_imports_skipped().
  TestFormatFullTable.test_imports_skip_empty_raw_text: FormatFullTable#test_imports_skip_empty_raw_text().
  TestFormatFullTable.test_class_with_fields: FormatFullTable#test_class_with_fields().
  TestFormatFullTable.test_class_with_constructors: FormatFullTable#test_class_with_constructors().
  TestFormatFullTable.test_method_visibility_groups: FormatFullTable#test_method_visibility_groups().
  TestFormatFullTable.test_static_method: FormatFullTable#test_static_method().
  TestFormatFullTable.test_module_level_functions: FormatFullTable#test_module_level_functions().
  TestFormatFullTable.test_qualified_class_name_backslash: FormatFullTable#test_qualified_class_name_backslash().
  TestFormatFullTable.test_top_level_functions_rendered_without_classes: FormatFullTable#test_top_level_functions_rendered_without_classes().
  TestFormatFullTable.test_top_level_functions_exact_row_format: FormatFullTable#test_top_level_functions_exact_row_format().
  TestFormatCompactTable.test_empty_data: FormatCompactTable#test_empty_data().
  TestFormatCompactTable.test_with_methods: FormatCompactTable#test_with_methods().
  TestFormatCompactTable.test_compact_method_with_parent: FormatCompactTable#test_compact_method_with_parent().
  TestFormatCompactTable.test_compact_info_statistics: FormatCompactTable#test_compact_info_statistics().
  TestFormatCompactTable.test_doc_truncation: FormatCompactTable#test_doc_truncation().
  TestGetVisibilitySymbol: GetVisibilitySymbol#
  TestFormatSignature: FormatSignature#
  TestFormatCompactSignature: FormatCompactSignature#
  TestExtractNamespace: ExtractNamespace#
  TestFormatFullTable: FormatFullTable#
  TestFormatCompactTable: FormatCompactTable#
---
# Module: [`tests/unit/formatters/test_php_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py)

## Classes
### `TestExtractNamespace`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L106)
- signature: `class TestExtractNamespace:`
- members:
  - `test_empty_classes(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L126)
  - `test_from_full_qualified_name(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L107)
  - `test_from_metadata(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L111)
  - `test_no_namespace(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L122)
  - `test_prefers_fqn_over_metadata(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L129)
- uses (calls/refs, reference-scoped): [`extract_namespace`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#extract_namespace)

### `TestFormatCompactSignature`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L82)
- signature: `class TestFormatCompactSignature:`
- members:
  - `test_dict_params(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L83)
  - `test_no_params(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L101)
  - `test_no_return_type(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L94)
  - `test_string_params(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L90)
- uses (calls/refs, reference-scoped): [`format_compact_signature`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#format_compact_signature)

### `TestFormatCompactTable`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L450)
- signature: `class TestFormatCompactTable:`
- members:
  - `test_compact_info_statistics(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L499)
  - `test_compact_method_with_parent(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L481)
  - `test_doc_truncation(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L511)
  - `test_empty_data(self)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L451)
  - `test_with_methods(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L456)
- uses (calls/refs, reference-scoped): [`format_compact_table`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#format_compact_table)

### `TestFormatFullTable`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L141)
- signature: `class TestFormatFullTable:`
- members:
  - `test_class_with_constructors(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L234)
  - `test_class_with_fields(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L205)
  - `test_empty_data(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L142)
  - `test_empty_imports_skipped(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L183)
  - `test_imports_section(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L167)
  - `test_imports_skip_empty_raw_text(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L194)
  - `test_method_visibility_groups(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L262)
  - `test_module_level_functions(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L331)
  - `test_qualified_class_name_backslash(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L358)
  - `test_single_class(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L147)
  - `test_static_method(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L304)
  - `test_top_level_functions_exact_row_format(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L407)
  - `test_top_level_functions_rendered_without_classes(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L384)
- uses (calls/refs, reference-scoped): [`format_full_table`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#format_full_table)

### `TestFormatSignature`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L31)
- signature: `class TestFormatSignature:`
- members:
  - `test_dollar_sign_stripped(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L53)
  - `test_empty_return_type(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L72)
  - `test_missing_return_type_key(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L76)
  - `test_multiple_params(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L43)
  - `test_no_params(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L32)
  - `test_param_no_name(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L61)
  - `test_single_param(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L36)
  - `test_string_param(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L68)
- uses (calls/refs, reference-scoped): [`format_signature`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#format_signature)

### `TestGetVisibilitySymbol`
- def: [`tests/unit/formatters/test_php_formatter_helpers.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L11)
- signature: `class TestGetVisibilitySymbol:`
- members:
  - `test_case_insensitive(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L24)
  - `test_empty(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L27)
  - `test_private(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L15)
  - `test_protected(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L18)
  - `test_public(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L12)
  - `test_unknown(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_php_formatter_helpers.py#L21)
- uses (calls/refs, reference-scoped): [`get_visibility_symbol`](../../../tree_sitter_analyzer/formatters/_php_formatter_helpers.md#get_visibility_symbol)

