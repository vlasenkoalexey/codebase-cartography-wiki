---
title: 'Module: tests/integration/cli/test_quiet_option.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_quiet_option.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_quiet_option`/
symbols:
  TestQuietOption.test_java_file: TestQuietOption#test_java_file.
  MockCommand: MockCommand#
  TestQuietOption.test_quiet_option_suppresses_info_messages: TestQuietOption#test_quiet_option_suppresses_info_messages().
  TestQuietOption.test_quiet_option_allows_error_messages: TestQuietOption#test_quiet_option_allows_error_messages().
  TestQuietOption.test_quiet_option_vs_table_option: TestQuietOption#test_quiet_option_vs_table_option().
  TestQuietOption.test_quiet_option_with_language_detection_error: TestQuietOption#test_quiet_option_with_language_detection_error().
  TestQuietOption.test_quiet_option_without_table_shows_no_info: TestQuietOption#test_quiet_option_without_table_shows_no_info().
  TestQuietOption.test_no_quiet_option_shows_info_messages: TestQuietOption#test_no_quiet_option_shows_info_messages().
  TestQuietOption.test_quiet_option_in_cli_main: TestQuietOption#test_quiet_option_in_cli_main().
  TestQuietOption.temp_dir: TestQuietOption#temp_dir.
  TestQuietOption.teardown_method: TestQuietOption#teardown_method().
  TestQuietOption.test_quiet_option_environment_variable_early_setting: TestQuietOption#test_quiet_option_environment_variable_early_setting().
  TestQuietOption.test_quiet_option_help_text: TestQuietOption#test_quiet_option_help_text().
  MockCommand.execute_async: MockCommand#execute_async().
  TestQuietOption: TestQuietOption#
  TestQuietOption.setup_method: TestQuietOption#setup_method().
  TestQuietOption.test_logging_level_configuration_with_quiet: TestQuietOption#test_logging_level_configuration_with_quiet().
---
# Module: [`tests/integration/cli/test_quiet_option.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py)

## Classes
### `MockCommand`  ·  implements/extends BaseCommand
- def: [`tests/integration/cli/test_quiet_option.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L24)
- doc: Mock implementation of BaseCommand for testing purposes.
- signature: `class MockCommand(BaseCommand):`
- members:
  - `execute_async(self, language: str)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L27) — Mock implementation of execute_async.
- uses (calls/refs, reference-scoped): [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand)
- used by: [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.execute_async)  (6 test-only)

### `TestQuietOption`
- def: [`tests/integration/cli/test_quiet_option.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L32)
- doc: Test class for --quiet option functionality.
- signature: `class TestQuietOption:`
- members:
  - `setup_method(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L35) — Set up test environment.
  - `teardown_method(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L52) — Clean up test environment.
  - `test_logging_level_configuration_with_quiet(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L144) — Test that logging level is configured correctly with --quiet option.
  - `test_no_quiet_option_shows_info_messages(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L241) — Test that without --quiet option, language detection still works.
  - `test_quiet_option_allows_error_messages(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L75) — Test that --quiet option still allows error messages.
  - `test_quiet_option_environment_variable_early_setting(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L200) — Test that LOG_LEVEL environment variable is set early in main().
  - `test_quiet_option_help_text(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L258) — Test that --quiet option has correct help text.
  - `test_quiet_option_in_cli_main(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L88) — Test that --quiet option sets environment variable correctly.
  - `test_quiet_option_suppresses_info_messages(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L58) — Test that --quiet option suppresses INFO messages in BaseCommand.
  - `test_quiet_option_vs_table_option(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L167) — Test interaction between --quiet and --table options.
  - `test_quiet_option_with_language_detection_error(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L184) — Test that --quiet option still shows language detection errors.
  - `test_quiet_option_without_table_shows_no_info(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L224) — Test that quiet option without table option suppresses info messages.
  - `temp_dir` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L37)
  - `test_java_file` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_quiet_option.py#L38)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser), [`detect_language`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.detect_language), [`validate_file`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.validate_file)  (1 test-only)

