---
title: 'Module: tests/unit/cli/_test_cli_main_module_test_mixin.py'
type: catalog
provenance: extracted
module: tests/unit/cli/_test_cli_main_module_test_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli._test_cli_main_module_test_mixin`/TestCLICommandFactoryTestMixin#
symbols:
  TestCLICommandFactoryTestMixin._create_command: _create_command().
  TestCLICommandFactoryTestMixin: ''
  TestCLICommandFactoryTestMixin.test_create_command_list_queries: test_create_command_list_queries().
  TestCLICommandFactoryTestMixin.test_create_command_describe_query: test_create_command_describe_query().
  TestCLICommandFactoryTestMixin.test_create_command_show_languages: test_create_command_show_languages().
  TestCLICommandFactoryTestMixin.test_create_command_show_extensions: test_create_command_show_extensions().
  TestCLICommandFactoryTestMixin.test_create_command_filter_help: test_create_command_filter_help().
  TestCLICommandFactoryTestMixin.test_create_command_table: test_create_command_table().
  TestCLICommandFactoryTestMixin.test_create_command_structure: test_create_command_structure().
  TestCLICommandFactoryTestMixin.test_create_command_summary: test_create_command_summary().
  TestCLICommandFactoryTestMixin.test_create_command_advanced: test_create_command_advanced().
  TestCLICommandFactoryTestMixin.test_create_command_query_key: test_create_command_query_key().
  TestCLICommandFactoryTestMixin.test_create_command_query_string: test_create_command_query_string().
  TestCLICommandFactoryTestMixin.test_create_command_default: test_create_command_default().
  TestCLICommandFactoryTestMixin.test_create_command_partial_read: test_create_command_partial_read().
  TestCLICommandFactoryTestMixin.test_create_command_no_file_path: test_create_command_no_file_path().
  TestCLICommandFactoryTestMixin.__test__: __test__.
---
# Module: [`tests/unit/cli/_test_cli_main_module_test_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py)

## Classes
### `TestCLICommandFactoryTestMixin`
- def: [`tests/unit/cli/_test_cli_main_module_test_mixin.py:7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L7)
- doc: Tests for CLICommandFactory class.
- signature: `class TestCLICommandFactoryTestMixin:`
- members:
  - `test_create_command_advanced(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L127) — Test creating AdvancedCommand.
  - `test_create_command_default(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L172) — Test creating DefaultCommand when no specific command is given.
  - `test_create_command_describe_query(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L26) — Test creating DescribeQueryCommand.
  - `test_create_command_filter_help(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L68) — Test creating filter help command.
  - `test_create_command_list_queries(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L12) — Test creating ListQueriesCommand.
  - `test_create_command_no_file_path(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L203) — Test that command is None when file_path is not provided.
  - `test_create_command_partial_read(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L186) — Test creating PartialReadCommand.
  - `test_create_command_query_key(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L142) — Test creating QueryCommand with query_key.
  - `test_create_command_query_string(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L157) — Test creating QueryCommand with query_string.
  - `test_create_command_show_extensions(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L54) — Test creating ShowExtensionsCommand.
  - `test_create_command_show_languages(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L40) — Test creating ShowLanguagesCommand.
  - `test_create_command_structure(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L97) — Test creating StructureCommand.
  - `test_create_command_summary(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L112) — Test creating SummaryCommand.
  - `test_create_command_table(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L82) — Test creating TableCommand.
- protocol/private: `__test__`[`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L10), `_create_command`[`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_test_mixin.py#L216)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

