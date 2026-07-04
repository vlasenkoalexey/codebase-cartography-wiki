---
title: 'Module: tests/integration/cli/test_cli_regression.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_regression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_regression`/TestCLIRegression#
symbols:
  TestCLIRegression.run_cli_command: run_cli_command().
  TestCLIRegression._as_results_list: _as_results_list().
  TestCLIRegression.test_query_methods_consistency: test_query_methods_consistency().
  TestCLIRegression.test_query_classes_consistency: test_query_classes_consistency().
  TestCLIRegression.test_filter_main_method_consistency: test_filter_main_method_consistency().
  TestCLIRegression.test_filter_auth_pattern_consistency: test_filter_auth_pattern_consistency().
  TestCLIRegression.test_filter_public_no_params_consistency: test_filter_public_no_params_consistency().
  TestCLIRegression.test_filter_static_methods_consistency: test_filter_static_methods_consistency().
  TestCLIRegression.test_summary_command_consistency: test_summary_command_consistency().
  TestCLIRegression.test_table_full_command_consistency: test_table_full_command_consistency().
  TestCLIRegression.test_advanced_json_command_consistency: test_advanced_json_command_consistency().
  TestCLIRegression.test_advanced_text_command_consistency: test_advanced_text_command_consistency().
  TestCLIRegression.test_partial_read_command_consistency: test_partial_read_command_consistency().
  TestCLIRegression.test_structure_command_consistency: test_structure_command_consistency().
  TestCLIRegression.test_python_language_command_consistency: test_python_language_command_consistency().
  TestCLIRegression.test_all_commands_exit_successfully: test_all_commands_exit_successfully().
  TestCLIRegression.test_error_handling_consistency: test_error_handling_consistency().
  TestCLIRegression.test_output_format_consistency: test_output_format_consistency().
  TestCLIRegression.test_filter_help_consistency: test_filter_help_consistency().
  TestCLIRegression.test_all_query_commands_exit_successfully: test_all_query_commands_exit_successfully().
  TestCLIRegression.test_markdown_summary_consistency: test_markdown_summary_consistency().
  TestCLIRegression.test_markdown_structure_consistency: test_markdown_structure_consistency().
  TestCLIRegression.test_markdown_advanced_consistency: test_markdown_advanced_consistency().
  TestCLIRegression.test_markdown_table_consistency: test_markdown_table_consistency().
  TestCLIRegression.test_markdown_advanced_text_format_consistency: test_markdown_advanced_text_format_consistency().
  TestCLIRegression.test_all_markdown_commands_exit_successfully: test_all_markdown_commands_exit_successfully().
  TestCLIRegression: ''
  TestCLIRegression.bigservice_path: bigservice_path().
  TestCLIRegression.sample_py_path: sample_py_path().
  TestCLIRegression.test_markdown_path: test_markdown_path().
---
# Module: [`tests/integration/cli/test_cli_regression.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py)

## Classes
### `TestCLIRegression`
- def: [`tests/integration/cli/test_cli_regression.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L17)
- doc: Regression tests for CLI commands
- signature: `class TestCLIRegression:`
- members:
  - `_as_results_list(data)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L49) — Normalise CLI JSON output to a list of result rows.
  - `bigservice_path(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L21) — Path to the BigService.java test file
  - `run_cli_command(self, args)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L35) — Helper to run CLI commands and return output
  - `sample_py_path(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L26) — Path to the sample.py test file
  - `test_advanced_json_command_consistency(self, bigservice_path)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L107) — Test --advanced --output-format=json command produces consistent output
  - `test_advanced_text_command_consistency(self, bigservice_path)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L149) — Test --advanced --output-format=text command produces consistent output
  - `test_all_commands_exit_successfully(self, bigservice_path, sample_py_path)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L241) — Test that all documented CLI commands exit with code 0
  - `test_all_markdown_commands_exit_successfully(self, test_markdown_path)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L647) — Test that all Markdown CLI commands exit with code 0
  - `test_all_query_commands_exit_successfully(self, bigservice_path)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L467) — Test that all documented query CLI commands exit with code 0
  - `test_error_handling_consistency(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L270) — Test that error conditions are handled consistently
  - `test_filter_auth_pattern_consistency(self, bigservice_path)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L378) — Test --query-key methods --filter name=~auth* command produces consistent output
  - `test_filter_help_consistency(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L450) — Test --filter-help command produces consistent output
  - `test_filter_main_method_consistency(self, bigservice_path)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L357) — Test --query-key methods --filter name=main command produces consistent output
  - `test_filter_public_no_params_consistency(self, bigservice_path)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L399) — Test --query-key methods --filter params=0,public=true command produces consistent output
  - `test_filter_static_methods_consistency(self, bigservice_path)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L428) — Test --query-key methods --filter static=true command produces consistent output
  - `test_markdown_advanced_consistency(self, test_markdown_path)` — [`L572`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L572) — Test --advanced command for Markdown files produces consistent output
  - `test_markdown_advanced_text_format_consistency(self, test_markdown_path)` — [`L629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L629) — Test --advanced --output-format=text command for Markdown files
  - `test_markdown_path(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L31) — Path to the test_markdown.md test file
  - `test_markdown_structure_consistency(self, test_markdown_path)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L537) — Test --structure command for Markdown files produces consistent output
  - `test_markdown_summary_consistency(self, test_markdown_path)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L499) — Test --summary command for Markdown files produces consistent output
  - `test_markdown_table_consistency(self, test_markdown_path)` — [`L607`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L607) — Test --table=full command for Markdown files produces consistent output
  - `test_output_format_consistency(self, bigservice_path)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L284) — Test that different output formats are consistent in structure
  - `test_partial_read_command_consistency(self, bigservice_path)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L165) — Test --partial-read command produces consistent output
  - `test_python_language_command_consistency(self, sample_py_path)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L226) — Test --language python --table=full command produces consistent output
  - `test_query_classes_consistency(self, bigservice_path)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L332) — Test --query-key classes command produces consistent output
  - `test_query_methods_consistency(self, bigservice_path)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L305) — Test --query-key methods command produces consistent output
  - `test_structure_command_consistency(self, bigservice_path)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L196) — Test --structure command produces consistent output
  - `test_summary_command_consistency(self, bigservice_path)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L60) — Test --summary command produces consistent output
  - `test_table_full_command_consistency(self, bigservice_path)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_regression.py#L85) — Test --table=full command produces consistent output

