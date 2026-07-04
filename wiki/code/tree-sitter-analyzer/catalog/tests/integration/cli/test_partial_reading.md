---
title: 'Module: tests/integration/cli/test_partial_reading.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_partial_reading.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_partial_reading`/
symbols:
  test_read_line_range_1_to_5: test_read_line_range_1_to_5().
  test_read_single_line_5: test_read_single_line_5().
  test_read_column_range_line_1_cols_5_to_15: test_read_column_range_line_1_cols_5_to_15().
  test_read_from_line_10_to_end: test_read_from_line_10_to_end().
  test_read_file_lines_range_function: test_read_file_lines_range_function().
  test_invalid_start_line_zero: test_invalid_start_line_zero().
  test_invalid_range_end_before_start: test_invalid_range_end_before_start().
  test_nonexistent_file: test_nonexistent_file().
  test_read_beyond_file_end: test_read_beyond_file_end().
  test_read_file_lines_range_invalid_range: test_read_file_lines_range_invalid_range().
  test_read_file_lines_range_nonexistent_file: test_read_file_lines_range_nonexistent_file().
  test_read_empty_file: test_read_empty_file().
  test_read_single_line_file: test_read_single_line_file().
  test_read_beyond_single_line: test_read_beyond_single_line().
  test_column_range_beyond_line_length: test_column_range_beyond_line_length().
  test_cli_compatible_line_range_reading: test_cli_compatible_line_range_reading().
  test_cli_error_handling_scenarios: test_cli_error_handling_scenarios().
  test_file: test_file().
  empty_file: empty_file().
  single_line_file: single_line_file().
  cli_test_file: cli_test_file().
---
# Module: [`tests/integration/cli/test_partial_reading.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py)

## Functions
- `cli_test_file()` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L101) — Create a test file for CLI integration tests
- `empty_file()` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L68) — Create an empty test file
- `single_line_file()` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L84) — Create a single line test file
- `test_cli_compatible_line_range_reading(cli_test_file)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L254) — Test that partial reading works for CLI scenarios
- `test_cli_error_handling_scenarios(cli_test_file)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L274) — Test error handling scenarios that CLI might encounter
- `test_column_range_beyond_line_length(single_line_file)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L245) — Test column range beyond line length
- `test_file()` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L19) — Create a test Java file for testing
- `test_invalid_range_end_before_start(test_file)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L186) — Test error case with invalid range (end < start)
- `test_invalid_start_line_zero(test_file)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L179) — Test error case with invalid start line (0)
- `test_nonexistent_file()` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L193) — Test reading from nonexistent file
- `test_read_beyond_file_end(test_file)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L200) — Test reading beyond file end
- `test_read_beyond_single_line(single_line_file)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L238) — Test reading beyond single line file
- `test_read_column_range_line_1_cols_5_to_15(test_file)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L148) — Test reading columns 5-15 of line 1
- `test_read_empty_file(empty_file)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L223) — Test reading from empty file
- `test_read_file_lines_range_function(test_file)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L169) — Test read_file_lines_range function (lines 2-4)
- `test_read_file_lines_range_invalid_range(test_file)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L208) — Test read_file_lines_range with invalid range
- `test_read_file_lines_range_nonexistent_file()` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L215) — Test read_file_lines_range with nonexistent file
- `test_read_from_line_10_to_end(test_file)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L157) — Test reading from line 10 to end of file
- `test_read_line_range_1_to_5(test_file)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L127) — Test reading lines 1-5
- `test_read_single_line_5(test_file)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L139) — Test reading single line (line 5)
- `test_read_single_line_file(single_line_file)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_partial_reading.py#L230) — Test reading from single line file

