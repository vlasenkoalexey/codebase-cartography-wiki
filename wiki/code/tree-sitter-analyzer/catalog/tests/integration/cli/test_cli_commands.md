---
title: 'Module: tests/integration/cli/test_cli_commands.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_commands`/
symbols:
  TestCLIQueryCommands.test_query_command_with_key: TestCLIQueryCommands#test_query_command_with_key().
  TestTableCommandCoverage.test_table_command_full: TestTableCommandCoverage#test_table_command_full().
  TestCLIInfoCommands.test_show_query_languages: TestCLIInfoCommands#test_show_query_languages().
  TestCLIInfoCommands.test_show_supported_languages: TestCLIInfoCommands#test_show_supported_languages().
  TestCLIInfoCommands.test_show_supported_extensions: TestCLIInfoCommands#test_show_supported_extensions().
  TestCLIInfoCommands.test_show_common_queries: TestCLIInfoCommands#test_show_common_queries().
  TestCLIInfoCommands.test_help_option: TestCLIInfoCommands#test_help_option().
  TestCLIInfoCommands.test_no_arguments: TestCLIInfoCommands#test_no_arguments().
  TestCLIQueryCommands.test_list_queries_with_language: TestCLIQueryCommands#test_list_queries_with_language().
  TestCLIQueryCommands.test_list_queries_without_language: TestCLIQueryCommands#test_list_queries_without_language().
  TestCLIQueryCommands.test_describe_query_with_language: TestCLIQueryCommands#test_describe_query_with_language().
  TestCLIAnalysisCommands.test_analyze_java_file: TestCLIAnalysisCommands#test_analyze_java_file().
  TestCLIAnalysisCommands.test_analyze_with_query_key: TestCLIAnalysisCommands#test_analyze_with_query_key().
  TestCLIAnalysisCommands.test_analyze_with_custom_query: TestCLIAnalysisCommands#test_analyze_with_custom_query().
  TestCLIAnalysisCommands.test_output_format_json: TestCLIAnalysisCommands#test_output_format_json().
  TestCLIAnalysisCommands.test_output_format_text: TestCLIAnalysisCommands#test_output_format_text().
  TestCLILanguageHandling.test_language_detection: TestCLILanguageHandling#test_language_detection().
  TestCLILanguageHandling.test_explicit_language_override: TestCLILanguageHandling#test_explicit_language_override().
  TestCLIErrorHandling.test_nonexistent_file: TestCLIErrorHandling#test_nonexistent_file().
  TestCLIErrorHandling.test_invalid_query_key: TestCLIErrorHandling#test_invalid_query_key().
  MockArgs: MockArgs#
  MockArgs.__init__: MockArgs#__init__().
  MockArgs.file: MockArgs#file.
  MockArgs.language: MockArgs#language.
  MockArgs.output_format: MockArgs#output_format.
  MockArgs.table: MockArgs#table.
  MockArgs.quiet: MockArgs#quiet.
  MockArgs.toon_use_tabs: MockArgs#toon_use_tabs.
  MockArgs.include_javadoc: MockArgs#include_javadoc.
  MockArgs.project: MockArgs#project.
  MockArgs.query_key: MockArgs#query_key.
  MockArgs.query_string: MockArgs#query_string.
  MockArgs.start_line: MockArgs#start_line.
  MockArgs.end_line: MockArgs#end_line.
  MockArgs.element_name: MockArgs#element_name.
  MockArgs.context_lines: MockArgs#context_lines.
  TestCLIInfoCommands: TestCLIInfoCommands#
  TestCLIQueryCommands: TestCLIQueryCommands#
  TestCLIAnalysisCommands: TestCLIAnalysisCommands#
  TestCLIAnalysisCommands.temp_java_file: TestCLIAnalysisCommands#temp_java_file().
  TestCLILanguageHandling: TestCLILanguageHandling#
  TestCLIErrorHandling: TestCLIErrorHandling#
  TestTableCommandCoverage: TestTableCommandCoverage#
---
# Module: [`tests/integration/cli/test_cli_commands.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py)

## Classes
### `MockArgs`
- def: [`tests/integration/cli/test_cli_commands.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L20)
- doc: Mock args object for CLI commands.
- signature: `class MockArgs:`
- members:
  - `context_lines` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L38)
  - `element_name` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L37)
  - `end_line` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L36)
  - `file` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L24)
  - `include_javadoc` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L30)
  - `language` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L25)
  - `output_format` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L26)
  - `project` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L31)
  - `query_key` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L32)
  - `query_string` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L33)
  - `quiet` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L28)
  - `start_line` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L35)
  - `table` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L27)
  - `toon_use_tabs` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L29)
- protocol/private: `__init__`[`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L23)
- used by: (2 test-only callers)

### `TestCLIAnalysisCommands`
- def: [`tests/integration/cli/test_cli_commands.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L196)
- doc: Test cases for file analysis commands
- signature: `class TestCLIAnalysisCommands:`
- members:
  - `temp_java_file(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L200) — Create a temporary Java file
  - `test_analyze_java_file(self, monkeypatch, temp_java_file)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L219) — Test analyzing a Java file
  - `test_analyze_with_custom_query(self, monkeypatch, temp_java_file)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L263) — Test analyzing file with custom query string
  - `test_analyze_with_query_key(self, monkeypatch, temp_java_file)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L238) — Test analyzing file with specific query
  - `test_output_format_json(self, monkeypatch, temp_java_file)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L290) — Test JSON output format
  - `test_output_format_text(self, monkeypatch, temp_java_file)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L315) — Test text output format
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIErrorHandling`
- def: [`tests/integration/cli/test_cli_commands.py:414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L414)
- doc: Test cases for error conditions
- signature: `class TestCLIErrorHandling:`
- members:
  - `test_invalid_query_key(self, monkeypatch)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L432) — Test with invalid query key
  - `test_nonexistent_file(self, monkeypatch)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L417) — Test handling of nonexistent files
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIInfoCommands`
- def: [`tests/integration/cli/test_cli_commands.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L43)
- doc: Test cases for informational CLI commands
- signature: `class TestCLIInfoCommands:`
- members:
  - `test_help_option(self, monkeypatch)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L109) — Test help option
  - `test_no_arguments(self, monkeypatch)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L121) — Test CLI with no arguments
  - `test_show_common_queries(self, monkeypatch)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L85) — Test --show-common-queries option
  - `test_show_query_languages(self, monkeypatch)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L46) — Test --show-query-languages option
  - `test_show_supported_extensions(self, monkeypatch)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L73) — Test --show-supported-extensions option
  - `test_show_supported_languages(self, monkeypatch)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L61) — Test --show-supported-languages option
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLILanguageHandling`
- def: [`tests/integration/cli/test_cli_commands.py:343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L343)
- doc: Test cases for language detection and overrides
- signature: `class TestCLILanguageHandling:`
- members:
  - `test_explicit_language_override(self, monkeypatch)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L374) — Test explicit language specification
  - `test_language_detection(self, monkeypatch)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L346) — Test automatic language detection
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIQueryCommands`
- def: [`tests/integration/cli/test_cli_commands.py:134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L134)
- doc: Test cases for query related CLI commands
- signature: `class TestCLIQueryCommands:`
- members:
  - `test_describe_query_with_language(self, monkeypatch)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L163) — Test --describe-query with --language option
  - `test_list_queries_with_language(self, monkeypatch)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L137) — Test --list-queries with --language option
  - `test_list_queries_without_language(self, monkeypatch)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L151) — Test --list-queries without language specification
  - `test_query_command_with_key(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L179) — Test QueryCommand with query key using MockArgs.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`QueryCommand`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand.execute_async)  (1 test-only)

### `TestTableCommandCoverage`
- def: [`tests/integration/cli/test_cli_commands.py:469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L469)
- doc: Test TableCommand for coverage boost.
- signature: `class TestTableCommandCoverage:`
- members:
  - `test_table_command_full(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_commands.py#L473) — Test TableCommand with full format.
- uses (calls/refs, reference-scoped): [`TableCommand`](../../../tree_sitter_analyzer/cli/commands/table_command.md#TableCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/table_command.md#TableCommand.execute_async)  (1 test-only)

