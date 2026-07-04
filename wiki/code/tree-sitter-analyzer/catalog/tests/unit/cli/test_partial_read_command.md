---
title: 'Module: tests/unit/cli/test_partial_read_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_partial_read_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_partial_read_command`/
symbols:
  TestPartialReadCommandInit.test_init_with_args: TestPartialReadCommandInit#test_init_with_args().
  command: command().
  TestPartialReadCommandInit.test_init: TestPartialReadCommandInit#test_init().
  TestPartialReadCommandInit.test_init_no_super_call: TestPartialReadCommandInit#test_init_no_super_call().
  mock_args: mock_args().
  TestPartialReadCommandInit: TestPartialReadCommandInit#
  TestPartialReadCommandValidateFile: TestPartialReadCommandValidateFile#
  TestPartialReadCommandValidateFile.test_validate_file_success: TestPartialReadCommandValidateFile#test_validate_file_success().
  TestPartialReadCommandValidateFile.test_validate_file_no_file_path: TestPartialReadCommandValidateFile#test_validate_file_no_file_path().
  TestPartialReadCommandValidateFile.test_validate_file_empty_file_path: TestPartialReadCommandValidateFile#test_validate_file_empty_file_path().
  TestPartialReadCommandValidateFile.test_validate_file_not_exists: TestPartialReadCommandValidateFile#test_validate_file_not_exists().
  TestPartialReadCommandExecute: TestPartialReadCommandExecute#
  TestPartialReadCommandExecute.test_execute_success: TestPartialReadCommandExecute#test_execute_success().
  TestPartialReadCommandExecute.test_execute_validate_file_fails: TestPartialReadCommandExecute#test_execute_validate_file_fails().
  TestPartialReadCommandExecute.test_execute_no_start_line: TestPartialReadCommandExecute#test_execute_no_start_line().
  TestPartialReadCommandExecute.test_execute_start_line_less_than_1: TestPartialReadCommandExecute#test_execute_start_line_less_than_1().
  TestPartialReadCommandExecute.test_execute_end_line_less_than_start_line: TestPartialReadCommandExecute#test_execute_end_line_less_than_start_line().
  TestPartialReadCommandExecute.test_execute_read_file_partial_fails: TestPartialReadCommandExecute#test_execute_read_file_partial_fails().
  TestPartialReadCommandExecute.test_execute_exception: TestPartialReadCommandExecute#test_execute_exception().
  TestPartialReadCommandOutputPartialContent: TestPartialReadCommandOutputPartialContent#
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_text: TestPartialReadCommandOutputPartialContent#test_output_partial_content_text().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_json: TestPartialReadCommandOutputPartialContent#test_output_partial_content_json().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_toon: TestPartialReadCommandOutputPartialContent#test_output_partial_content_toon().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_with_start_column: TestPartialReadCommandOutputPartialContent#test_output_partial_content_with_start_column().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_with_end_column: TestPartialReadCommandOutputPartialContent#test_output_partial_content_with_end_column().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_no_end_line: TestPartialReadCommandOutputPartialContent#test_output_partial_content_no_end_line().
  TestPartialReadCommandOutputPartialContent.test_output_partial_content_toon_use_tabs: TestPartialReadCommandOutputPartialContent#test_output_partial_content_toon_use_tabs().
  TestPartialReadCommandExecuteAsync: TestPartialReadCommandExecuteAsync#
  TestPartialReadCommandExecuteAsync.test_execute_async_calls_execute: TestPartialReadCommandExecuteAsync#test_execute_async_calls_execute().
  TestPartialReadCommandExecuteAsync.test_execute_async_returns_execute_result: TestPartialReadCommandExecuteAsync#test_execute_async_returns_execute_result().
  TestPartialReadCommandIntegration: TestPartialReadCommandIntegration#
  TestPartialReadCommandIntegration.test_full_workflow_success: TestPartialReadCommandIntegration#test_full_workflow_success().
  TestPartialReadCommandIntegration.test_full_workflow_validation_failure: TestPartialReadCommandIntegration#test_full_workflow_validation_failure().
  TestPartialReadCommandIntegration.test_full_workflow_read_failure: TestPartialReadCommandIntegration#test_full_workflow_read_failure().
---
# Module: [`tests/unit/cli/test_partial_read_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py)

## Classes
### `TestPartialReadCommandExecute`
- def: [`tests/unit/cli/test_partial_read_command.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L87)
- doc: Tests for PartialReadCommand.execute method.
- signature: `class TestPartialReadCommandExecute:`
- members:
  - `test_execute_end_line_less_than_start_line(self, command)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L123) — Test execute returns 1 when end_line < start_line.
  - `test_execute_exception(self, command)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L143) — Test execute handles exceptions.
  - `test_execute_no_start_line(self, command)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L107) — Test execute returns 1 when start_line is missing.
  - `test_execute_read_file_partial_fails(self, command)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L132) — Test execute returns 1 when read_file_partial fails.
  - `test_execute_start_line_less_than_1(self, command)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L115) — Test execute returns 1 when start_line < 1.
  - `test_execute_success(self, command)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L90) — Test execute returns 0 on success.
  - `test_execute_validate_file_fails(self, command)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L101) — Test execute returns 1 when validate_file fails.

### `TestPartialReadCommandExecuteAsync`
- def: [`tests/unit/cli/test_partial_read_command.py:254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L254)
- doc: Tests for PartialReadCommand.execute_async method.
- signature: `class TestPartialReadCommandExecuteAsync:`
- members:
  - `test_execute_async_calls_execute(self, command)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L258) — Test execute_async calls execute method.
  - `test_execute_async_returns_execute_result(self, command)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L266) — Test execute_async returns execute result.

### `TestPartialReadCommandInit`
- def: [`tests/unit/cli/test_partial_read_command.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L35)
- doc: Tests for PartialReadCommand initialization.
- signature: `class TestPartialReadCommandInit:`
- members:
  - `test_init(self, command)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L38) — Test PartialReadCommand initialization.
  - `test_init_no_super_call(self, mock_args)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L49) — Test PartialReadCommand doesn't call super().__init__().
  - `test_init_with_args(self, mock_args)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L44) — Test PartialReadCommand initialization with args.
- uses (calls/refs, reference-scoped): [`PartialReadCommand`](../../../tree_sitter_analyzer/cli/commands/partial_read_command.md#PartialReadCommand), [`args`](../../../tree_sitter_analyzer/cli/commands/partial_read_command.md#PartialReadCommand.args)

### `TestPartialReadCommandIntegration`
- def: [`tests/unit/cli/test_partial_read_command.py:273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L273)
- doc: Integration tests for PartialReadCommand.
- signature: `class TestPartialReadCommandIntegration:`
- members:
  - `test_full_workflow_read_failure(self, command)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L300) — Test full workflow with read failure.
  - `test_full_workflow_success(self, command)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L276) — Test full workflow with successful read.
  - `test_full_workflow_validation_failure(self, command)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L294) — Test full workflow with validation failure.

### `TestPartialReadCommandOutputPartialContent`
- def: [`tests/unit/cli/test_partial_read_command.py:155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L155)
- doc: Tests for PartialReadCommand._output_partial_content method.
- signature: `class TestPartialReadCommandOutputPartialContent:`
- members:
  - `test_output_partial_content_json(self, command)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L172) — Test _output_partial_content with JSON format.
  - `test_output_partial_content_no_end_line(self, command)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L227) — Test _output_partial_content without end_line.
  - `test_output_partial_content_text(self, command)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L158) — Test _output_partial_content with text format.
  - `test_output_partial_content_toon(self, command)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L189) — Test _output_partial_content with TOON format.
  - `test_output_partial_content_toon_use_tabs(self, command)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L239) — Test _output_partial_content with TOON and use_tabs=True.
  - `test_output_partial_content_with_end_column(self, command)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L215) — Test _output_partial_content with end_column.
  - `test_output_partial_content_with_start_column(self, command)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L203) — Test _output_partial_content with start_column.

### `TestPartialReadCommandValidateFile`
- def: [`tests/unit/cli/test_partial_read_command.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L56)
- doc: Tests for PartialReadCommand.validate_file method.
- signature: `class TestPartialReadCommandValidateFile:`
- members:
  - `test_validate_file_empty_file_path(self, command)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L72) — Test validate_file with empty file_path.
  - `test_validate_file_no_file_path(self, command)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L65) — Test validate_file without file_path attribute.
  - `test_validate_file_not_exists(self, command)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L79) — Test validate_file with non-existent file.
  - `test_validate_file_success(self, command)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L59) — Test validate_file with valid file.

## Functions
- `command(mock_args)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L30) — Create PartialReadCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_partial_read_command.py#L15) — Create mock args for PartialReadCommand.

