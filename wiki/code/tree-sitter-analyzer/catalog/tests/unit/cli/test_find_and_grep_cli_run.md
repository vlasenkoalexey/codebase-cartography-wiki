---
title: 'Module: tests/unit/cli/test_find_and_grep_cli_run.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_find_and_grep_cli_run.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_find_and_grep_cli_run`/
symbols:
  _make_default_args: _make_default_args().
  TestRunFunction.test_minimal_execution: TestRunFunction#test_minimal_execution().
  TestRunFunction.test_text_output_format: TestRunFunction#test_text_output_format().
  TestRunFunction.test_all_fd_options_in_payload: TestRunFunction#test_all_fd_options_in_payload().
  TestRunFunction.test_all_rg_options_in_payload: TestRunFunction#test_all_rg_options_in_payload().
  TestRunFunction.test_integer_result: TestRunFunction#test_integer_result().
  TestRunFunction.test_error_handling: TestRunFunction#test_error_handling().
  TestRunFunction.test_custom_project_root: TestRunFunction#test_custom_project_root().
  TestRunFunction: TestRunFunction#
---
# Module: [`tests/unit/cli/test_find_and_grep_cli_run.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py)

## Classes
### `TestRunFunction`
- def: [`tests/unit/cli/test_find_and_grep_cli_run.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L61)
- doc: Test the _run async function.
- signature: `class TestRunFunction:`
- members:
  - `test_all_fd_options_in_payload(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L132) — Test all fd options are included in payload.
  - `test_all_rg_options_in_payload(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L194) — Test all ripgrep options are included in payload.
  - `test_custom_project_root(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L314) — Test custom project root is used.
  - `test_error_handling(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L285) — Test error handling in _run.
  - `test_integer_result(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L256) — Test integer result (count) is handled correctly.
  - `test_minimal_execution(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L65) — Test minimal execution with required arguments.
  - `test_text_output_format(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L100) — Test text output format.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_run)  (1 test-only)

## Functions
- `_make_default_args(**overrides)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_run.py#L16) — Return a Namespace with all _run defaults; overrides replace specific fields.

