---
title: 'Module: tests/unit/cli/test_table_command_core.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_table_command_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_table_command_core`/
symbols:
  TestTableCommandInit.test_init_with_args: TestTableCommandInit#test_init_with_args().
  command: command().
  TestTableCommandInit.test_init: TestTableCommandInit#test_init().
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_with_class: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_with_class().
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_with_method: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_with_method().
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_with_field: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_with_field().
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_with_import: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_with_import().
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_statistics: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_statistics().
  mock_args: mock_args().
  TestTableCommandInit: TestTableCommandInit#
  TestTableCommandExecuteAsync: TestTableCommandExecuteAsync#
  TestTableCommandExecuteAsync.test_execute_async_success: TestTableCommandExecuteAsync#test_execute_async_success().
  TestTableCommandExecuteAsync.test_execute_async_no_analysis_result: TestTableCommandExecuteAsync#test_execute_async_no_analysis_result().
  TestTableCommandExecuteAsync.test_execute_async_exception: TestTableCommandExecuteAsync#test_execute_async_exception().
  TestTableCommandExecuteAsync.test_execute_async_toon_format: TestTableCommandExecuteAsync#test_execute_async_toon_format().
  TestTableCommandExecuteAsync.test_execute_async_full_format: TestTableCommandExecuteAsync#test_execute_async_full_format().
  TestTableCommandFormatAsToon: TestTableCommandFormatAsToon#
  TestTableCommandFormatAsToon.test_format_as_toon_basic: TestTableCommandFormatAsToon#test_format_as_toon_basic().
  TestTableCommandFormatAsToon.test_format_as_toon_with_tabs: TestTableCommandFormatAsToon#test_format_as_toon_with_tabs().
  TestTableCommandConvertToToonFormat: TestTableCommandConvertToToonFormat#
  TestTableCommandConvertToToonFormat.test_convert_to_toon_format_empty: TestTableCommandConvertToToonFormat#test_convert_to_toon_format_empty().
  TestTableCommandGetDefaultPackageName: TestTableCommandGetDefaultPackageName#
  TestTableCommandGetDefaultPackageName.test_get_default_package_name_java: TestTableCommandGetDefaultPackageName#test_get_default_package_name_java().
  TestTableCommandGetDefaultPackageName.test_get_default_package_name_kotlin: TestTableCommandGetDefaultPackageName#test_get_default_package_name_kotlin().
  TestTableCommandGetDefaultPackageName.test_get_default_package_name_python: TestTableCommandGetDefaultPackageName#test_get_default_package_name_python().
  TestTableCommandGetDefaultPackageName.test_get_default_package_name_javascript: TestTableCommandGetDefaultPackageName#test_get_default_package_name_javascript().
  TestTableCommandGetDefaultPackageName.test_get_default_package_name_cpp: TestTableCommandGetDefaultPackageName#test_get_default_package_name_cpp().
---
# Module: [`tests/unit/cli/test_table_command_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py)

## Classes
### `TestTableCommandConvertToToonFormat`
- def: [`tests/unit/cli/test_table_command_core.py:212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L212)
- doc: Tests for TableCommand._convert_to_toon_format method.
- signature: `class TestTableCommandConvertToToonFormat:`
- members:
  - `test_convert_to_toon_format_empty(self, command)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L215) — Test _convert_to_toon_format with empty elements.
  - `test_convert_to_toon_format_statistics(self, command)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L332) — Test _convert_to_toon_format includes statistics.
  - `test_convert_to_toon_format_with_class(self, command)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L234) — Test _convert_to_toon_format with class element.
  - `test_convert_to_toon_format_with_field(self, command)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L282) — Test _convert_to_toon_format with field element.
  - `test_convert_to_toon_format_with_import(self, command)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L306) — Test _convert_to_toon_format with import element.
  - `test_convert_to_toon_format_with_method(self, command)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L258) — Test _convert_to_toon_format with method element.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT)

### `TestTableCommandExecuteAsync`
- def: [`tests/unit/cli/test_table_command_core.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L70)
- doc: Tests for TableCommand.execute_async method.
- signature: `class TestTableCommandExecuteAsync:`
- members:
  - `test_execute_async_exception(self, command)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L105) — Test execute_async handles exceptions.
  - `test_execute_async_full_format(self, command)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L139) — Test execute_async with full table type.
  - `test_execute_async_no_analysis_result(self, command)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L94) — Test execute_async returns 1 when no analysis result.
  - `test_execute_async_success(self, command)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L74) — Test execute_async returns 0 on success.
  - `test_execute_async_toon_format(self, command)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L116) — Test execute_async with toon table type.

### `TestTableCommandFormatAsToon`
- def: [`tests/unit/cli/test_table_command_core.py:166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L166)
- doc: Tests for TableCommand._format_as_toon method.
- signature: `class TestTableCommandFormatAsToon:`
- members:
  - `test_format_as_toon_basic(self, command)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L169) — Test _format_as_toon with basic result.
  - `test_format_as_toon_with_tabs(self, command)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L190) — Test _format_as_toon with use_tabs=True.

### `TestTableCommandGetDefaultPackageName`
- def: [`tests/unit/cli/test_table_command_core.py:361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L361)
- doc: Tests for TableCommand._get_default_package_name method.
- signature: `class TestTableCommandGetDefaultPackageName:`
- members:
  - `test_get_default_package_name_cpp(self, command)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L384) — Test _get_default_package_name for C++.
  - `test_get_default_package_name_java(self, command)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L364) — Test _get_default_package_name for Java.
  - `test_get_default_package_name_javascript(self, command)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L379) — Test _get_default_package_name for JavaScript.
  - `test_get_default_package_name_kotlin(self, command)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L369) — Test _get_default_package_name for Kotlin.
  - `test_get_default_package_name_python(self, command)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L374) — Test _get_default_package_name for Python.

### `TestTableCommandInit`
- def: [`tests/unit/cli/test_table_command_core.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L55)
- doc: Tests for TableCommand initialization.
- signature: `class TestTableCommandInit:`
- members:
  - `test_init(self, command)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L58) — Test TableCommand initialization.
  - `test_init_with_args(self, mock_args)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L64) — Test TableCommand initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`TableCommand`](../../../tree_sitter_analyzer/cli/commands/table_command.md#TableCommand)

## Functions
- `command(mock_args)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L50) — Create TableCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_core.py#L15) — Create mock args for BaseCommand initialization.

