---
title: 'Module: tests/integration/cli/test_partial_read_command_validation.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_partial_read_command_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_partial_read_command_validation`/TestPartialReadCommandValidation#
symbols:
  TestPartialReadCommandValidation.test_file: test_file.
  TestPartialReadCommandValidation.test_missing_start_line_validation: test_missing_start_line_validation().
  TestPartialReadCommandValidation.test_start_line_zero_validation: test_start_line_zero_validation().
  TestPartialReadCommandValidation.test_start_line_negative_validation: test_start_line_negative_validation().
  TestPartialReadCommandValidation.test_end_line_less_than_start_line_validation: test_end_line_less_than_start_line_validation().
  TestPartialReadCommandValidation.test_end_line_equal_to_start_line_validation: test_end_line_equal_to_start_line_validation().
  TestPartialReadCommandValidation.test_valid_line_range_validation: test_valid_line_range_validation().
  TestPartialReadCommandValidation.test_start_line_only_validation: test_start_line_only_validation().
  TestPartialReadCommandValidation.test_nonexistent_file_validation: test_nonexistent_file_validation().
  TestPartialReadCommandValidation.test_large_line_numbers_validation: test_large_line_numbers_validation().
  TestPartialReadCommandValidation.test_boundary_line_numbers: test_boundary_line_numbers().
  TestPartialReadCommandValidation.test_json_output_format_validation: test_json_output_format_validation().
  TestPartialReadCommandValidation.test_column_parameters_validation: test_column_parameters_validation().
  TestPartialReadCommandValidation.test_error_message_content_for_missing_start_line: test_error_message_content_for_missing_start_line().
  TestPartialReadCommandValidation.test_error_message_content_for_invalid_start_line: test_error_message_content_for_invalid_start_line().
  TestPartialReadCommandValidation.test_error_message_content_for_negative_start_line: test_error_message_content_for_negative_start_line().
  TestPartialReadCommandValidation.test_error_message_content_for_invalid_end_line: test_error_message_content_for_invalid_end_line().
  TestPartialReadCommandValidation.test_error_message_content_for_missing_file: test_error_message_content_for_missing_file().
  TestPartialReadCommandValidation.test_successful_execution_with_valid_parameters: test_successful_execution_with_valid_parameters().
  TestPartialReadCommandValidation.test_missing_file_path_validation: test_missing_file_path_validation().
  TestPartialReadCommandValidation.test_empty_file_path_validation: test_empty_file_path_validation().
  TestPartialReadCommandValidation.test_validation_order: test_validation_order().
  TestPartialReadCommandValidation.temp_dir: temp_dir.
  TestPartialReadCommandValidation.teardown_method: teardown_method().
  TestPartialReadCommandValidation: ''
  TestPartialReadCommandValidation.setup_method: setup_method().
---
# Module: [`tests/integration/cli/test_partial_read_command_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py)

## Classes
### `TestPartialReadCommandValidation`
- def: [`tests/integration/cli/test_partial_read_command_validation.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L22)
- doc: Test class for PartialReadCommand validation enhancements.
- signature: `class TestPartialReadCommandValidation:`
- members:
  - `setup_method(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L25) — Set up test environment.
  - `teardown_method(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L45) — Clean up test environment.
  - `test_boundary_line_numbers(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L193) — Test with boundary line numbers (first and last lines).
  - `test_column_parameters_validation(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L228) — Test validation with column parameters.
  - `test_empty_file_path_validation(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L163) — Test validation when file_path is empty string.
  - `test_end_line_equal_to_start_line_validation(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L91) — Test validation when end_line equals start_line (should be valid).
  - `test_end_line_less_than_start_line_validation(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L81) — Test validation when end_line is less than start_line.
  - `test_error_message_content_for_invalid_end_line(self)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L288) — Test that correct error message is shown for invalid end_line.
  - `test_error_message_content_for_invalid_start_line(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L258) — Test that correct error message is shown for invalid start_line.
  - `test_error_message_content_for_missing_file(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L303) — Test that correct error message is shown for missing file.
  - `test_error_message_content_for_missing_start_line(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L245) — Test that correct error message is shown for missing start_line.
  - `test_error_message_content_for_negative_start_line(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L273) — Test that correct error message is shown for negative start_line.
  - `test_json_output_format_validation(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L211) — Test validation with JSON output format.
  - `test_large_line_numbers_validation(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L173) — Test validation with line numbers larger than file.
  - `test_missing_file_path_validation(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L153) — Test validation when file_path is missing.
  - `test_missing_start_line_validation(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L51) — Test validation when start_line is missing.
  - `test_nonexistent_file_validation(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L142) — Test validation with nonexistent file.
  - `test_start_line_negative_validation(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L71) — Test validation when start_line is negative.
  - `test_start_line_only_validation(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L125) — Test validation with only start_line specified.
  - `test_start_line_zero_validation(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L61) — Test validation when start_line is 0.
  - `test_successful_execution_with_valid_parameters(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L317) — Test successful execution with all valid parameters.
  - `test_valid_line_range_validation(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L108) — Test validation with valid line range.
  - `test_validation_order(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L334) — Test that validations are performed in the correct order.
  - `temp_dir` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L27)
  - `test_file` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_read_command_validation.py#L28)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/commands/partial_read_command.md#PartialReadCommand.execute), [`PartialReadCommand`](../../../tree_sitter_analyzer/cli/commands/partial_read_command.md#PartialReadCommand)

