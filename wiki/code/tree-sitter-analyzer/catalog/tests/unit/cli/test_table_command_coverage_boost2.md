---
title: 'Module: tests/unit/cli/test_table_command_coverage_boost2.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_table_command_coverage_boost2.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_table_command_coverage_boost2`/
symbols:
  TestConvertToStructureFormatSQL.test_convert_with_all_sql_types: TestConvertToStructureFormatSQL#test_convert_with_all_sql_types().
  command: command().
  TestConvertToFormatterFormat.test_convert_to_formatter_format_with_elements: TestConvertToFormatterFormat#test_convert_to_formatter_format_with_elements().
  TestConvertToStructureFormatPackage.test_convert_with_package_element: TestConvertToStructureFormatPackage#test_convert_with_package_element().
  TestConvertToStructureFormatSQL.test_convert_with_sql_table: TestConvertToStructureFormatSQL#test_convert_with_sql_table().
  TestConvertToStructureFormatSQL.test_convert_with_sql_view: TestConvertToStructureFormatSQL#test_convert_with_sql_view().
  TestConvertToStructureFormatException.test_convert_with_element_exception: TestConvertToStructureFormatException#test_convert_with_element_exception().
  TestConvertSQLElement.test_convert_sql_element_basic: TestConvertSQLElement#test_convert_sql_element_basic().
  TestConvertSQLElement.test_convert_sql_element_with_all_metadata: TestConvertSQLElement#test_convert_sql_element_with_all_metadata().
  TestConvertSQLElement.test_convert_sql_element_return_type_fallback: TestConvertSQLElement#test_convert_sql_element_return_type_fallback().
  TestConvertToFormatterFormat: TestConvertToFormatterFormat#
  TestConvertToFormatterFormat.test_convert_to_formatter_format_basic: TestConvertToFormatterFormat#test_convert_to_formatter_format_basic().
  TestConvertToStructureFormatPackage: TestConvertToStructureFormatPackage#
  TestConvertToStructureFormatPackage.test_convert_with_package_object: TestConvertToStructureFormatPackage#test_convert_with_package_object().
  TestConvertToStructureFormatPackage.test_convert_with_default_package_java: TestConvertToStructureFormatPackage#test_convert_with_default_package_java().
  TestConvertToStructureFormatPackage.test_convert_with_default_package_python: TestConvertToStructureFormatPackage#test_convert_with_default_package_python().
  TestConvertToStructureFormatSQL: TestConvertToStructureFormatSQL#
  TestConvertToStructureFormatException: TestConvertToStructureFormatException#
  TestConvertSQLElement: TestConvertSQLElement#
  TestConvertSQLElement.test_convert_sql_element_no_attributes: TestConvertSQLElement#test_convert_sql_element_no_attributes().
  TestProcessSQLParameters: TestProcessSQLParameters#
  TestProcessSQLParameters.test_process_sql_params_empty_list: TestProcessSQLParameters#test_process_sql_params_empty_list().
  TestProcessSQLParameters.test_process_sql_params_none: TestProcessSQLParameters#test_process_sql_params_none().
  TestProcessSQLParameters.test_process_sql_params_falsy_zero: TestProcessSQLParameters#test_process_sql_params_falsy_zero().
  TestProcessSQLParameters.test_process_sql_params_empty_string: TestProcessSQLParameters#test_process_sql_params_empty_string().
  TestProcessSQLParameters.test_process_sql_params_list_of_strings: TestProcessSQLParameters#test_process_sql_params_list_of_strings().
  TestProcessSQLParameters.test_process_sql_params_list_of_dicts: TestProcessSQLParameters#test_process_sql_params_list_of_dicts().
  TestProcessSQLParameters.test_process_sql_params_non_list: TestProcessSQLParameters#test_process_sql_params_non_list().
  TestProcessSQLParameters.test_process_sql_params_mixed_list: TestProcessSQLParameters#test_process_sql_params_mixed_list().
---
# Module: [`tests/unit/cli/test_table_command_coverage_boost2.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py)

## Classes
### `TestConvertSQLElement`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L277)
- doc: Tests for _convert_sql_element (lines 407-417).
- signature: `class TestConvertSQLElement:`
- members:
  - `test_convert_sql_element_basic(self, command)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L280) — Test _convert_sql_element with basic SQL element.
  - `test_convert_sql_element_no_attributes(self, command)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L325) — Test _convert_sql_element with element missing optional attributes.
  - `test_convert_sql_element_return_type_fallback(self, command)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L337) — Test _convert_sql_element with empty return_type (line 420-422).
  - `test_convert_sql_element_with_all_metadata(self, command)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L301) — Test _convert_sql_element with full metadata.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_SQL_TABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_TABLE), [`ELEMENT_TYPE_SQL_PROCEDURE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_PROCEDURE)

### `TestConvertToFormatterFormat`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L28)
- doc: Tests for _convert_to_formatter_format (line 182).
- signature: `class TestConvertToFormatterFormat:`
- members:
  - `test_convert_to_formatter_format_basic(self, command)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L31) — Test _convert_to_formatter_format returns expected structure.
  - `test_convert_to_formatter_format_with_elements(self, command)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L48) — Test _convert_to_formatter_format with elements.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS)

### `TestConvertToStructureFormatException`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L232)
- doc: Tests for _convert_to_structure_format exception handler (lines 282-284).
- signature: `class TestConvertToStructureFormatException:`
- members:
  - `test_convert_with_element_exception(self, command)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L235) — Test _convert_to_structure_format handles element processing exception.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS)

### `TestConvertToStructureFormatPackage`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L82)
- doc: Tests for _convert_to_structure_format with package handling (lines 154-155, 253).
- signature: `class TestConvertToStructureFormatPackage:`
- members:
  - `test_convert_with_default_package_java(self, command)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L100) — Test _convert_to_structure_format uses _get_default_package_name for java (line 253).
  - `test_convert_with_default_package_python(self, command)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L113) — Test _convert_to_structure_format uses _get_default_package_name for python (line 253).
  - `test_convert_with_package_element(self, command)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L125) — Test _convert_to_structure_format when element is PACKAGE type.
  - `test_convert_with_package_object(self, command)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L85) — Test _convert_to_structure_format when analysis_result has package attr.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_PACKAGE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_PACKAGE)

### `TestConvertToStructureFormatSQL`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L143)
- doc: Tests for _convert_to_structure_format with SQL elements (lines 272, 280).
- signature: `class TestConvertToStructureFormatSQL:`
- members:
  - `test_convert_with_all_sql_types(self, command)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L195) — Test _convert_to_structure_format with all SQL element types.
  - `test_convert_with_sql_table(self, command)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L146) — Test _convert_to_structure_format with SQL table element.
  - `test_convert_with_sql_view(self, command)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L171) — Test _convert_to_structure_format with SQL view element.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_SQL_TABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_TABLE), [`ELEMENT_TYPE_SQL_PROCEDURE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_PROCEDURE), [`ELEMENT_TYPE_SQL_VIEW`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_VIEW), [`ELEMENT_TYPE_SQL_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_FUNCTION), [`ELEMENT_TYPE_SQL_INDEX`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_INDEX), [`ELEMENT_TYPE_SQL_TRIGGER`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_TRIGGER)

### `TestProcessSQLParameters`
- def: [`tests/unit/cli/test_table_command_coverage_boost2.py:354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L354)
- doc: Tests for _process_sql_parameters (lines 440-443).
- signature: `class TestProcessSQLParameters:`
- members:
  - `test_process_sql_params_empty_list(self, command)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L357) — Test _process_sql_parameters with empty list.
  - `test_process_sql_params_empty_string(self, command)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L372) — Test _process_sql_parameters with empty string.
  - `test_process_sql_params_falsy_zero(self, command)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L367) — Test _process_sql_parameters with falsy value 0.
  - `test_process_sql_params_list_of_dicts(self, command)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L387) — Test _process_sql_parameters with list of dicts.
  - `test_process_sql_params_list_of_strings(self, command)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L377) — Test _process_sql_parameters with list of strings (line 443-449).
  - `test_process_sql_params_mixed_list(self, command)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L406) — Test _process_sql_parameters with mixed types in list.
  - `test_process_sql_params_non_list(self, command)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L398) — Test _process_sql_parameters with non-list value (else branch line 451-452).
  - `test_process_sql_params_none(self, command)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L362) — Test _process_sql_parameters with None (line 440-441).

## Functions
- `command()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_coverage_boost2.py#L20) — Create a TableCommand with minimal args.

