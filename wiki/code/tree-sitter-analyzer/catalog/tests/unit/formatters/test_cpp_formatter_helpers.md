---
title: 'Module: tests/unit/formatters/test_cpp_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_cpp_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_cpp_formatter_helpers`/
symbols:
  _make_formatter: _make_formatter().
  TestCreateCppCompactSignature.test_no_params: TestCreateCppCompactSignature#test_no_params().
  TestCreateCppCompactSignature.test_single_param: TestCreateCppCompactSignature#test_single_param().
  TestCreateCppCompactSignature.test_multiple_params: TestCreateCppCompactSignature#test_multiple_params().
  TestCreateCppCompactSignature.test_with_shorten: TestCreateCppCompactSignature#test_with_shorten().
  TestCreateCppCompactSignature.test_default_return_type: TestCreateCppCompactSignature#test_default_return_type().
  TestFormatCppFullTable.test_file_header: TestFormatCppFullTable#test_file_header().
  TestFormatCppFullTable.test_namespace_from_packages: TestFormatCppFullTable#test_namespace_from_packages().
  TestFormatCppFullTable.test_namespace_from_package_name: TestFormatCppFullTable#test_namespace_from_package_name().
  TestFormatCppFullTable.test_imports_section: TestFormatCppFullTable#test_imports_section().
  TestFormatCppFullTable.test_imports_skipped_when_empty: TestFormatCppFullTable#test_imports_skipped_when_empty().
  TestFormatCppFullTable.test_classes_overview: TestFormatCppFullTable#test_classes_overview().
  TestFormatCppFullTable.test_global_functions: TestFormatCppFullTable#test_global_functions().
  TestFormatCppFullTable.test_global_variables: TestFormatCppFullTable#test_global_variables().
  TestFormatCppFullTable.test_no_trailing_blank_lines: TestFormatCppFullTable#test_no_trailing_blank_lines().
  TestFormatCppClassDetails.test_basic_class: TestFormatCppClassDetails#test_basic_class().
  TestFormatCppClassDetails.test_class_with_no_members: TestFormatCppClassDetails#test_class_with_no_members().
  TestFormatCppCompactTable.test_basic: TestFormatCppCompactTable#test_basic().
  TestFormatCppCompactTable.test_compact_info_cpp_package: TestFormatCppCompactTable#test_compact_info_cpp_package().
  TestFormatCppCompactTable.test_compact_info_stats: TestFormatCppCompactTable#test_compact_info_stats().
  TestFormatCppCompactTable.test_no_methods_section_when_empty: TestFormatCppCompactTable#test_no_methods_section_when_empty().
  TestFormatCppCompactTable.test_no_trailing_blank_lines: TestFormatCppCompactTable#test_no_trailing_blank_lines().
  _identity_shorten: _identity_shorten().
  TestShortenCppType.test_none_returns_void: TestShortenCppType#test_none_returns_void().
  TestShortenCppType.test_int: TestShortenCppType#test_int().
  TestShortenCppType.test_double: TestShortenCppType#test_double().
  TestShortenCppType.test_float: TestShortenCppType#test_float().
  TestShortenCppType.test_char: TestShortenCppType#test_char().
  TestShortenCppType.test_long: TestShortenCppType#test_long().
  TestShortenCppType.test_short: TestShortenCppType#test_short().
  TestShortenCppType.test_bool: TestShortenCppType#test_bool().
  TestShortenCppType.test_void: TestShortenCppType#test_void().
  TestShortenCppType.test_size_t: TestShortenCppType#test_size_t().
  TestShortenCppType.test_string: TestShortenCppType#test_string().
  TestShortenCppType.test_unknown_type: TestShortenCppType#test_unknown_type().
  TestShortenCppType.test_pointer_preserved: TestShortenCppType#test_pointer_preserved().
  TestShortenCppType.test_reference_preserved: TestShortenCppType#test_reference_preserved().
  TestShortenCppType.test_array_preserved: TestShortenCppType#test_array_preserved().
  TestShortenCppType.test_const_stripped: TestShortenCppType#test_const_stripped().
  TestShortenCppType.test_volatile_stripped: TestShortenCppType#test_volatile_stripped().
  TestShortenCppType.test_static_stripped: TestShortenCppType#test_static_stripped().
  TestShortenCppType.test_whitespace_trimmed: TestShortenCppType#test_whitespace_trimmed().
  TestShortenCppType: TestShortenCppType#
  TestCreateCppCompactSignature: TestCreateCppCompactSignature#
  TestFormatCppFullTable: TestFormatCppFullTable#
  TestFormatCppClassDetails: TestFormatCppClassDetails#
  TestFormatCppCompactTable: TestFormatCppCompactTable#
---
# Module: [`tests/unit/formatters/test_cpp_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py)

## Classes
### `TestCreateCppCompactSignature`
- def: [`tests/unit/formatters/test_cpp_formatter_helpers.py:92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L92)
- signature: `class TestCreateCppCompactSignature:`
- members:
  - `test_default_return_type(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L125)
  - `test_multiple_params(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L106)
  - `test_no_params(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L93)
  - `test_single_param(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L98)
  - `test_with_shorten(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L117)
- uses (calls/refs, reference-scoped): [`shorten_cpp_type`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#shorten_cpp_type), [`create_cpp_compact_signature`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#create_cpp_compact_signature)  (1 test-only)

### `TestFormatCppClassDetails`
- def: [`tests/unit/formatters/test_cpp_formatter_helpers.py:279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L279)
- signature: `class TestFormatCppClassDetails:`
- members:
  - `test_basic_class(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L280)
  - `test_class_with_no_members(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L297)
- uses (calls/refs, reference-scoped): [`format_cpp_class_details`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#format_cpp_class_details)  (1 test-only)

### `TestFormatCppCompactTable`
- def: [`tests/unit/formatters/test_cpp_formatter_helpers.py:309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L309)
- signature: `class TestFormatCppCompactTable:`
- members:
  - `test_basic(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L310)
  - `test_compact_info_cpp_package(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L330)
  - `test_compact_info_stats(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L341)
  - `test_no_methods_section_when_empty(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L352)
  - `test_no_trailing_blank_lines(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L361)
- uses (calls/refs, reference-scoped): [`format_cpp_compact_table`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#format_cpp_compact_table)  (1 test-only)

### `TestFormatCppFullTable`
- def: [`tests/unit/formatters/test_cpp_formatter_helpers.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L131)
- signature: `class TestFormatCppFullTable:`
- members:
  - `test_classes_overview(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L199)
  - `test_file_header(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L132)
  - `test_global_functions(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L218)
  - `test_global_variables(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L241)
  - `test_imports_section(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L169)
  - `test_imports_skipped_when_empty(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L187)
  - `test_namespace_from_package_name(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L156)
  - `test_namespace_from_packages(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L143)
  - `test_no_trailing_blank_lines(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L267)
- uses (calls/refs, reference-scoped): [`format_cpp_full_table`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#format_cpp_full_table)  (1 test-only)

### `TestShortenCppType`
- def: [`tests/unit/formatters/test_cpp_formatter_helpers.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L33)
- signature: `class TestShortenCppType:`
- members:
  - `test_array_preserved(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L76)
  - `test_bool(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L55)
  - `test_char(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L46)
  - `test_const_stripped(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L79)
  - `test_double(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L40)
  - `test_float(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L43)
  - `test_int(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L37)
  - `test_long(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L49)
  - `test_none_returns_void(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L34)
  - `test_pointer_preserved(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L70)
  - `test_reference_preserved(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L73)
  - `test_short(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L52)
  - `test_size_t(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L61)
  - `test_static_stripped(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L85)
  - `test_string(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L64)
  - `test_unknown_type(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L67)
  - `test_void(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L58)
  - `test_volatile_stripped(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L82)
  - `test_whitespace_trimmed(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L88)
- uses (calls/refs, reference-scoped): [`shorten_cpp_type`](../../../tree_sitter_analyzer/formatters/_cpp_formatter_helpers.md#shorten_cpp_type)

## Functions
- `_identity_shorten(t)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L29)
- `_make_formatter()` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_helpers.py#L12)

