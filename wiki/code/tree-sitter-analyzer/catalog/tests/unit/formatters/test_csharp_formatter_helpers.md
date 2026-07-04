---
title: 'Module: tests/unit/formatters/test_csharp_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_csharp_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_csharp_formatter_helpers`/
symbols:
  _noop_visibility: _noop_visibility().
  _noop_method_row: _noop_method_row().
  TestFormatCsharpFullTable.test_file_header: TestFormatCsharpFullTable#test_file_header().
  TestFormatCsharpFullTable.test_imports_section: TestFormatCsharpFullTable#test_imports_section().
  TestFormatCsharpFullTable.test_imports_skip_empty: TestFormatCsharpFullTable#test_imports_skip_empty().
  TestFormatCsharpFullTable.test_no_imports_section_when_empty: TestFormatCsharpFullTable#test_no_imports_section_when_empty().
  TestFormatCsharpFullTable.test_classes_overview: TestFormatCsharpFullTable#test_classes_overview().
  TestFormatCsharpFullTable.test_class_fields: TestFormatCsharpFullTable#test_class_fields().
  TestFormatCsharpFullTable.test_method_groups_by_visibility: TestFormatCsharpFullTable#test_method_groups_by_visibility().
  TestFormatCsharpFullTable.test_no_trailing_blank_lines: TestFormatCsharpFullTable#test_no_trailing_blank_lines().
  TestFormatCsharpFullTable.test_multiple_classes: TestFormatCsharpFullTable#test_multiple_classes().
  TestFormatCsharpFullTable.test_field_type_fallback: TestFormatCsharpFullTable#test_field_type_fallback().
  TestFormatCsharpFullTable.test_variable_type_fallback: TestFormatCsharpFullTable#test_variable_type_fallback().
  _noop_signature: _noop_signature().
  _noop_modifiers: _noop_modifiers().
  _noop_class_methods: _noop_class_methods().
  _noop_class_fields: _noop_class_fields().
  TestFormatCsharpCompactTable.test_basic: TestFormatCsharpCompactTable#test_basic().
  TestFormatCsharpCompactTable.test_empty_methods: TestFormatCsharpCompactTable#test_empty_methods().
  TestFormatCsharpCompactTable.test_namespace_in_info: TestFormatCsharpCompactTable#test_namespace_in_info().
  TestFormatCsharpCompactTable.test_no_trailing_blanks: TestFormatCsharpCompactTable#test_no_trailing_blanks().
  TestFormatCsharpCsv.test_header_row: TestFormatCsharpCsv#test_header_row().
  TestFormatCsharpCsv.test_fields: TestFormatCsharpCsv#test_fields().
  TestFormatCsharpCsv.test_methods: TestFormatCsharpCsv#test_methods().
  TestFormatCsharpCsv.test_constructor: TestFormatCsharpCsv#test_constructor().
  TestFormatCsharpCsv.test_static_method: TestFormatCsharpCsv#test_static_method().
  TestFormatCsharpCsv.test_field_type_fallbacks: TestFormatCsharpCsv#test_field_type_fallbacks().
  TestFormatCsharpCsv.test_field_variable_type_fallback: TestFormatCsharpCsv#test_field_variable_type_fallback().
  TestFormatCsharpCsv.test_csv_comma_in_signature_quoted: TestFormatCsharpCsv#test_csv_comma_in_signature_quoted().
  TestFormatCsharpCsv.test_empty_data: TestFormatCsharpCsv#test_empty_data().
  _noop_namespace: _noop_namespace().
  TestFormatCsharpCsv.sig_with_comma: TestFormatCsharpCsv#sig_with_comma().
  TestFormatCsharpFullTable: TestFormatCsharpFullTable#
  TestFormatCsharpCompactTable: TestFormatCsharpCompactTable#
  TestFormatCsharpCsv: TestFormatCsharpCsv#
---
# Module: [`tests/unit/formatters/test_csharp_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py)

## Classes
### `TestFormatCsharpCompactTable`
- def: [`tests/unit/formatters/test_csharp_formatter_helpers.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L353)
- signature: `class TestFormatCsharpCompactTable:`
- members:
  - `test_basic(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L354)
  - `test_empty_methods(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L377)
  - `test_namespace_in_info(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L388)
  - `test_no_trailing_blanks(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L399)
- uses (calls/refs, reference-scoped): [`format_csharp_compact_table`](../../../tree_sitter_analyzer/formatters/_csharp_formatter_helpers.md#format_csharp_compact_table)  (3 test-only)

### `TestFormatCsharpCsv`
- def: [`tests/unit/formatters/test_csharp_formatter_helpers.py:411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L411)
- signature: `class TestFormatCsharpCsv:`
- members:
  - `sig_with_comma(method: dict)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L513)
  - `test_constructor(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L448)
  - `test_csv_comma_in_signature_quoted(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L512)
  - `test_empty_data(self)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L531)
  - `test_field_type_fallbacks(self)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L482)
  - `test_field_variable_type_fallback(self)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L497)
  - `test_fields(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L416)
  - `test_header_row(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L412)
  - `test_methods(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L431)
  - `test_static_method(self)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L465)
- uses (calls/refs, reference-scoped): [`format_csharp_csv`](../../../tree_sitter_analyzer/formatters/_csharp_formatter_helpers.md#format_csharp_csv)  (1 test-only)

### `TestFormatCsharpFullTable`
- def: [`tests/unit/formatters/test_csharp_formatter_helpers.py:50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L50)
- signature: `class TestFormatCsharpFullTable:`
- members:
  - `test_class_fields(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L153)
  - `test_classes_overview(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L127)
  - `test_field_type_fallback(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L286)
  - `test_file_header(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L51)
  - `test_imports_section(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L68)
  - `test_imports_skip_empty(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L91)
  - `test_method_groups_by_visibility(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L187)
  - `test_multiple_classes(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L254)
  - `test_no_imports_section_when_empty(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L109)
  - `test_no_trailing_blank_lines(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L237)
  - `test_variable_type_fallback(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L319)
- uses (calls/refs, reference-scoped): [`format_csharp_full_table`](../../../tree_sitter_analyzer/formatters/_csharp_formatter_helpers.md#format_csharp_full_table)  (5 test-only)

## Functions
- `_noop_class_fields(fields: list, line_range: dict)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L29)
- `_noop_class_methods(methods: list, line_range: dict)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L21)
- `_noop_method_row(method: dict)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L43)
- `_noop_modifiers(field: dict)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L16)
- `_noop_namespace(_data: dict)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L12)
- `_noop_signature(method: dict)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L37)
- `_noop_visibility(v: str)` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csharp_formatter_helpers.py#L8)

