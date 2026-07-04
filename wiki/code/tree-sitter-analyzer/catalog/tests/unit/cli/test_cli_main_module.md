---
title: 'Module: tests/unit/cli/test_cli_main_module.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_cli_main_module.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_cli_main_module`/Test
symbols:
  TestCLICommandFactory: CLICommandFactory#
  TestCLICommandFactory._cli_command_factory: CLICommandFactory#_cli_command_factory.
  TestCreateArgumentParser: CreateArgumentParser#
  TestHandleSpecialCommandsBranchCoverage.test_handle_show_query_languages: HandleSpecialCommandsBranchCoverage#test_handle_show_query_languages().
  TestHandleSpecialCommandsBranchCoverage.test_handle_agent_skills_outputs_inventory: HandleSpecialCommandsBranchCoverage#test_handle_agent_skills_outputs_inventory().
  TestHandleSpecialCommandsBranchCoverage.test_handle_agent_workflow_outputs_pack: HandleSpecialCommandsBranchCoverage#test_handle_agent_workflow_outputs_pack().
  TestHandleSpecialCommandsBranchCoverage.test_handle_show_common_queries: HandleSpecialCommandsBranchCoverage#test_handle_show_common_queries().
  TestHandleSpecialCommandsBranchCoverage.test_handle_partial_read_missing_start_line: HandleSpecialCommandsBranchCoverage#test_handle_partial_read_missing_start_line().
  TestHandleSpecialCommandsBranchCoverage.test_handle_partial_read_invalid_start_line: HandleSpecialCommandsBranchCoverage#test_handle_partial_read_invalid_start_line().
  TestHandleSpecialCommandsBranchCoverage.test_handle_partial_read_invalid_end_line: HandleSpecialCommandsBranchCoverage#test_handle_partial_read_invalid_end_line().
  TestHandleSpecialCommandsBranchCoverage.test_handle_partial_read_invalid_start_column: HandleSpecialCommandsBranchCoverage#test_handle_partial_read_invalid_start_column().
  TestHandleSpecialCommandsBranchCoverage.test_handle_partial_read_invalid_end_column: HandleSpecialCommandsBranchCoverage#test_handle_partial_read_invalid_end_column().
  TestHandleSpecialCommandsBranchCoverage.test_handle_metrics_only_no_file_paths: HandleSpecialCommandsBranchCoverage#test_handle_metrics_only_no_file_paths().
  TestHandleSpecialCommandsBranchCoverage.test_handle_no_special_command: HandleSpecialCommandsBranchCoverage#test_handle_no_special_command().
  TestMainFunction.test_main_format_alias: MainFunction#test_main_format_alias().
  TestMainFunction.test_main_creates_command: MainFunction#test_main_creates_command().
  TestMainFunction.test_main_no_command_no_file_path: MainFunction#test_main_no_command_no_file_path().
  TestMainFunction.test_main_keyboard_interrupt: MainFunction#test_main_keyboard_interrupt().
  TestArgumentValidation.test_mutually_exclusive_query_options: ArgumentValidation#test_mutually_exclusive_query_options().
  TestArgumentValidation.test_output_format_choices: ArgumentValidation#test_output_format_choices().
  TestArgumentValidation.test_table_format_choices: ArgumentValidation#test_table_format_choices().
  TestLoggingConfiguration.test_logging_configured_to_error: LoggingConfiguration#test_logging_configured_to_error().
  TestLoggingConfiguration.test_logging_configured_for_table_output: LoggingConfiguration#test_logging_configured_for_table_output().
  TestErrorHandling.test_validation_error_shows_usage: ErrorHandling#test_validation_error_shows_usage().
  TestErrorHandling.test_command_execute_error_exits_with_code: ErrorHandling#test_command_execute_error_exits_with_code().
  TestHandleSpecialCommands: HandleSpecialCommands#
  TestCLICommandFactory.__test__: CLICommandFactory#__test__.
  TestCreateArgumentParser.__test__: CreateArgumentParser#__test__.
  TestHandleSpecialCommandsBranchCoverage: HandleSpecialCommandsBranchCoverage#
  TestHandleSpecialCommandsBranchCoverage.test_handle_sql_platform_info: HandleSpecialCommandsBranchCoverage#test_handle_sql_platform_info().
  TestHandleSpecialCommandsBranchCoverage.test_handle_record_sql_profile: HandleSpecialCommandsBranchCoverage#test_handle_record_sql_profile().
  TestMainFunction: MainFunction#
  TestMainFunction.test_main_quiet_mode_sets_env_var: MainFunction#test_main_quiet_mode_sets_env_var().
  TestMainFunction.test_main_default_log_level: MainFunction#test_main_default_log_level().
  TestMainFunction.test_main_unexpected_exception: MainFunction#test_main_unexpected_exception().
  TestArgumentValidation: ArgumentValidation#
  TestSpecialCommandsIntegration: SpecialCommandsIntegration#
  TestSpecialCommandsIntegration.test_batch_partial_read_json: SpecialCommandsIntegration#test_batch_partial_read_json().
  TestSpecialCommandsIntegration.test_batch_metrics_only: SpecialCommandsIntegration#test_batch_metrics_only().
  TestLoggingConfiguration: LoggingConfiguration#
  TestErrorHandling: ErrorHandling#
  TestHandleSpecialCommands.__test__: HandleSpecialCommands#__test__.
---
# Module: [`tests/unit/cli/test_cli_main_module.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py)

## Classes
### `TestArgumentValidation`
- def: [`tests/unit/cli/test_cli_main_module.py:399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L399)
- doc: Tests for argument validation.
- signature: `class TestArgumentValidation:`
- members:
  - `test_mutually_exclusive_query_options(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L402) — Test that --query-key and --query-string are mutually exclusive.
  - `test_output_format_choices(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L410) — Test that --output-format accepts valid choices.
  - `test_table_format_choices(self)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L417) — Test that --table accepts valid choices.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

### `TestCLICommandFactory`  ·  implements/extends TestCLICommandFactoryTestMixin
- def: [`tests/unit/cli/test_cli_main_module.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L30)
- doc: Tests for CLICommandFactory class.
- signature: `class TestCLICommandFactory(TestCLICommandFactoryTestMixin):`
- protocol/private: `__test__`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L33), `_cli_command_factory`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L35)
- uses (calls/refs, reference-scoped): [`CLICommandFactory`](../../../tree_sitter_analyzer/cli_main.md#CLICommandFactory)  (1 test-only)
- used by: (1 test-only callers)

### `TestCreateArgumentParser`  ·  implements/extends TestCreateArgumentParserMixin
- def: [`tests/unit/cli/test_cli_main_module.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L38)
- doc: Tests for create_argument_parser function.
- signature: `class TestCreateArgumentParser(TestCreateArgumentParserMixin):`
- protocol/private: `__test__`[`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L41)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestErrorHandling`
- def: [`tests/unit/cli/test_cli_main_module.py:530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L530)
- doc: Tests for error handling.
- signature: `class TestErrorHandling:`
- members:
  - `test_command_execute_error_exits_with_code(self, mock_exit, mock_output_error, mock_parser)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L575) — Test that command execution error exits with error code.
  - `test_validation_error_shows_usage(self, mock_exit, mock_output_info, mock_parser)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L536) — Test that validation error shows usage examples.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestHandleSpecialCommands`  ·  implements/extends TestHandleSpecialCommandsTestMixin
- def: [`tests/unit/cli/test_cli_main_module.py:615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L615)
- doc: Tests for handle_special_commands() covering all branches.
- signature: `class TestHandleSpecialCommands(TestHandleSpecialCommandsTestMixin):`
- protocol/private: `__test__`[`L618`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L618)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestHandleSpecialCommandsBranchCoverage`
- def: [`tests/unit/cli/test_cli_main_module.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L44)
- doc: Tests for handle_special_commands function.
- signature: `class TestHandleSpecialCommandsBranchCoverage:`
- members:
  - `test_handle_agent_skills_outputs_inventory(self, mock_output_json, tmp_path)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L65) — Agent skills returns project-local skill metadata and gaps.
  - `test_handle_agent_workflow_outputs_pack(self, mock_output_json, tmp_path)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L99) — Agent workflow returns a structured SMART command pack.
  - `test_handle_metrics_only_no_file_paths(self, mock_output_json)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L227) — Test handling --metrics-only without --file-paths or --files-from.
  - `test_handle_no_special_command(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L245) — Test handling when no special command is given.
  - `test_handle_partial_read_invalid_end_column(self, mock_output_error)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L213) — Test handling partial read with invalid --end-column.
  - `test_handle_partial_read_invalid_end_line(self, mock_output_error)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L185) — Test handling partial read with invalid --end-line.
  - `test_handle_partial_read_invalid_start_column(self, mock_output_error)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L199) — Test handling partial read with invalid --start-column.
  - `test_handle_partial_read_invalid_start_line(self, mock_output_error)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L171) — Test handling partial read with invalid --start-line.
  - `test_handle_partial_read_missing_start_line(self, mock_output_error)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L157) — Test handling partial read without --start-line.
  - `test_handle_record_sql_profile(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L149) — Test handling --record-sql-profile - skipped due to internal imports.
  - `test_handle_show_common_queries(self, mock_output_list)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L126) — Test handling --show-common-queries.
  - `test_handle_show_query_languages(self, mock_output_list)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L48) — Test handling --show-query-languages.
  - `test_handle_sql_platform_info(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L142) — Test handling --sql-platform-info - skipped due to internal imports.
- uses (calls/refs, reference-scoped): [`handle_special_commands`](../../../tree_sitter_analyzer/cli_main.md#handle_special_commands)

### `TestLoggingConfiguration`
- def: [`tests/unit/cli/test_cli_main_module.py:443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L443)
- doc: Tests for logging configuration.
- signature: `class TestLoggingConfiguration:`
- members:
  - `test_logging_configured_for_table_output(self, mock_exit, mock_handle_special, mock_parser)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L490) — Test that logging is configured for table output.
  - `test_logging_configured_to_error(self, mock_exit, mock_handle_special, mock_parser)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L449) — Test that logging is configured to ERROR level.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestMainFunction`
- def: [`tests/unit/cli/test_cli_main_module.py:261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L261)
- doc: Tests for main function.
- signature: `class TestMainFunction:`
- members:
  - `test_main_creates_command(self, mock_exit, mock_factory, mock_handle_special, mock_parser)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L311) — Test that main creates and executes command.
  - `test_main_default_log_level(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L270) — Test that default log level is ERROR - skipped due to complex mocking.
  - `test_main_format_alias(self, mock_exit, mock_handle_special, mock_parser)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L279) — Test that --format is aliased to --output-format.
  - `test_main_keyboard_interrupt(self, mock_exit, mock_output_error, mock_parser)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L380) — Test that main handles KeyboardInterrupt.
  - `test_main_no_command_no_file_path(self, mock_exit, mock_factory, mock_handle_special, mock_parser)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L348) — Test that main shows error when no command and no file path.
  - `test_main_quiet_mode_sets_env_var(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L264) — Test that --quiet sets LOG_LEVEL environment variable - skipped due to complex mocking.
  - `test_main_unexpected_exception(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L393) — Test that main handles unexpected exceptions - skipped due to complex mocking.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestSpecialCommandsIntegration`
- def: [`tests/unit/cli/test_cli_main_module.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L425)
- doc: Tests for special commands integration.
- signature: `class TestSpecialCommandsIntegration:`
- members:
  - `test_batch_metrics_only(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L435) — Test batch metrics only mode - skipped due to internal imports.
  - `test_batch_partial_read_json(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_main_module.py#L428) — Test batch partial read with JSON requests - skipped due to internal imports.

