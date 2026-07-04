---
title: 'Module: tests/unit/formatters/test_go_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_go_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_go_formatter_helpers`/
symbols:
  _noop_func_row: _noop_func_row().
  _noop_method_row: _noop_method_row().
  _noop_visibility: _noop_visibility().
  _noop_package: _noop_package().
  _noop_doc: _noop_doc().
  TestFormatGoFullTable.test_file_header_with_package: TestFormatGoFullTable#test_file_header_with_package().
  TestFormatGoFullTable.test_file_header_without_package: TestFormatGoFullTable#test_file_header_without_package().
  TestFormatGoFullTable.test_package_info_section: TestFormatGoFullTable#test_package_info_section().
  TestFormatGoFullTable.test_imports_section: TestFormatGoFullTable#test_imports_section().
  TestFormatGoFullTable.test_imports_add_import_prefix: TestFormatGoFullTable#test_imports_add_import_prefix().
  TestFormatGoFullTable.test_imports_no_imports_key: TestFormatGoFullTable#test_imports_no_imports_key().
  TestFormatGoFullTable.test_structs_section: TestFormatGoFullTable#test_structs_section().
  TestFormatGoFullTable.test_interfaces_section: TestFormatGoFullTable#test_interfaces_section().
  TestFormatGoFullTable.test_type_aliases_section: TestFormatGoFullTable#test_type_aliases_section().
  TestFormatGoFullTable.test_functions_section: TestFormatGoFullTable#test_functions_section().
  TestFormatGoFullTable.test_methods_section: TestFormatGoFullTable#test_methods_section().
  TestFormatGoFullTable.test_constants_section: TestFormatGoFullTable#test_constants_section().
  TestFormatGoFullTable.test_variables_section: TestFormatGoFullTable#test_variables_section().
  TestFormatGoFullTable.test_constants_and_variables_separated: TestFormatGoFullTable#test_constants_and_variables_separated().
  TestFormatGoFullTable.test_no_trailing_blank_lines: TestFormatGoFullTable#test_no_trailing_blank_lines().
  TestFormatGoFullTable.test_struct_no_interfaces: TestFormatGoFullTable#test_struct_no_interfaces().
  TestFormatGoFullTable.test_empty_structs_skipped: TestFormatGoFullTable#test_empty_structs_skipped().
  TestFormatGoFullTable.test_empty_interfaces_skipped: TestFormatGoFullTable#test_empty_interfaces_skipped().
  TestFormatGoFullTable.test_variable_type_fallback: TestFormatGoFullTable#test_variable_type_fallback().
  TestFormatGoFullTable.test_methods_key_fallback_for_functions: TestFormatGoFullTable#test_methods_key_fallback_for_functions().
  TestFormatGoFullTable.test_fields_key_fallback_for_variables: TestFormatGoFullTable#test_fields_key_fallback_for_variables().
  TestFormatGoFullTable: TestFormatGoFullTable#
---
# Module: [`tests/unit/formatters/test_go_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py)

## Classes
### `TestFormatGoFullTable`
- def: [`tests/unit/formatters/test_go_formatter_helpers.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L33)
- signature: `class TestFormatGoFullTable:`
- members:
  - `test_constants_and_variables_separated(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L342)
  - `test_constants_section(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L290)
  - `test_empty_interfaces_skipped(self)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L438)
  - `test_empty_structs_skipped(self)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L420)
  - `test_fields_key_fallback_for_variables(self)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L505)
  - `test_file_header_with_package(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L34)
  - `test_file_header_without_package(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L52)
  - `test_functions_section(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L233)
  - `test_imports_add_import_prefix(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L118)
  - `test_imports_no_imports_key(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L137)
  - `test_imports_section(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L93)
  - `test_interfaces_section(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L182)
  - `test_methods_key_fallback_for_functions(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L481)
  - `test_methods_section(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L264)
  - `test_no_trailing_blank_lines(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L377)
  - `test_package_info_section(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L70)
  - `test_struct_no_interfaces(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L395)
  - `test_structs_section(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L155)
  - `test_type_aliases_section(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L208)
  - `test_variable_type_fallback(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L456)
  - `test_variables_section(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L316)
- uses (calls/refs, reference-scoped): [`format_go_full_table`](../../../tree_sitter_analyzer/formatters/_go_formatter_helpers.md#format_go_full_table)  (5 test-only)

## Functions
- `_noop_doc(text: str)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L14)
- `_noop_func_row(func: dict)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L18)
- `_noop_method_row(method: dict)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L25)
- `_noop_package(data: dict)` — [`L6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L6)
- `_noop_visibility(name: str)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_go_formatter_helpers.py#L10)

