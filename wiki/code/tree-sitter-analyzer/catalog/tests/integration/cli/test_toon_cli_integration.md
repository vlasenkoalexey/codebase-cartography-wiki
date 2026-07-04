---
title: 'Module: tests/integration/cli/test_toon_cli_integration.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_toon_cli_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_toon_cli_integration`/TestToonCLI
symbols:
  TestToonCLIOptions: Options#
  TestToonCLIOptions.test_format_toon_option_in_help: Options#test_format_toon_option_in_help().
  TestToonCLIOptions.test_output_format_toon_option_in_help: Options#test_output_format_toon_option_in_help().
  TestToonCLIOptions.test_toon_use_tabs_option_in_help: Options#test_toon_use_tabs_option_in_help().
  TestToonCLIOutput: Output#
  TestToonCLIOutput.sample_python_file: Output#sample_python_file().
  TestToonCLIOutput.sample_java_file: Output#sample_java_file().
  TestToonCLIOutput.test_structure_command_with_toon_format: Output#test_structure_command_with_toon_format().
  TestToonCLIOutput.test_structure_command_with_format_alias: Output#test_structure_command_with_format_alias().
  TestToonCLIOutput.test_summary_command_with_toon_format: Output#test_summary_command_with_toon_format().
  TestToonCLIOutput.test_advanced_command_with_toon_format: Output#test_advanced_command_with_toon_format().
  TestToonCLIOutput.test_partial_read_command_with_toon_format: Output#test_partial_read_command_with_toon_format().
  TestToonCLIOutput.test_query_command_with_toon_format: Output#test_query_command_with_toon_format().
  TestToonCLIOutput.test_toon_use_tabs_option: Output#test_toon_use_tabs_option().
  TestToonCLIOutput.test_toon_output_vs_json_output: Output#test_toon_output_vs_json_output().
  TestToonCLIEdgeCases: EdgeCases#
  TestToonCLIEdgeCases.test_invalid_format_option: EdgeCases#test_invalid_format_option().
  TestToonCLIEdgeCases.test_format_and_output_format_both_specified: EdgeCases#test_format_and_output_format_both_specified().
  TestToonCLIEdgeCases.test_toon_use_tabs_without_toon_format: EdgeCases#test_toon_use_tabs_without_toon_format().
---
# Module: [`tests/integration/cli/test_toon_cli_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py)

## Classes
### `TestToonCLIEdgeCases`
- def: [`tests/integration/cli/test_toon_cli_integration.py:341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L341)
- doc: Tests for TOON CLI edge cases.
- signature: `class TestToonCLIEdgeCases:`
- members:
  - `test_format_and_output_format_both_specified(self, tmp_path)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L366) — Test behavior when both --format and --output-format are specified.
  - `test_invalid_format_option(self, tmp_path)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L344) — Test that invalid format option is rejected.
  - `test_toon_use_tabs_without_toon_format(self, tmp_path)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L393) — Test --toon-use-tabs is ignored when not using toon format.

### `TestToonCLIOptions`
- def: [`tests/integration/cli/test_toon_cli_integration.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L19)
- doc: Tests for TOON CLI option parsing.
- signature: `class TestToonCLIOptions:`
- members:
  - `test_format_toon_option_in_help(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L22) — Test that --format toon is documented in help.
  - `test_output_format_toon_option_in_help(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L33) — Test that --output-format toon is documented in help.
  - `test_toon_use_tabs_option_in_help(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L46) — Test that --toon-use-tabs is documented in help.

### `TestToonCLIOutput`
- def: [`tests/integration/cli/test_toon_cli_integration.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L58)
- doc: Tests for TOON format CLI output.
- signature: `class TestToonCLIOutput:`
- members:
  - `sample_java_file(self, tmp_path)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L90) — Create a sample Java file for testing.
  - `sample_python_file(self, tmp_path)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L62) — Create a sample Python file for testing.
  - `test_advanced_command_with_toon_format(self, sample_python_file)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L196) — Test --advanced command with --output-format toon.
  - `test_partial_read_command_with_toon_format(self, sample_python_file)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L219) — Test --partial-read command with --output-format toon.
  - `test_query_command_with_toon_format(self, sample_python_file)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L246) — Test --query-key command with --output-format toon.
  - `test_structure_command_with_format_alias(self, sample_python_file)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L148) — Test --structure command with --format toon alias.
  - `test_structure_command_with_toon_format(self, sample_python_file)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L116) — Test --structure command with --output-format toon.
  - `test_summary_command_with_toon_format(self, sample_python_file)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L173) — Test --summary command with --output-format toon.
  - `test_toon_output_vs_json_output(self, sample_python_file)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L292) — Test that TOON output is shorter than JSON output.
  - `test_toon_use_tabs_option(self, sample_python_file)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_cli_integration.py#L268) — Test --toon-use-tabs option produces tab-delimited output.

