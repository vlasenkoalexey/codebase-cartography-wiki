---
title: 'Module: tests/unit/cli/test_list_files_cli_comprehensive_execution.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_list_files_cli_comprehensive_execution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_list_files_cli_comprehensive_execution`/
symbols:
  _make_args: _make_args().
  TestRunFunction.test_minimal_execution: TestRunFunction#test_minimal_execution().
  TestRunFunction.test_text_output_format: TestRunFunction#test_text_output_format().
  TestRunFunction.test_all_options_in_payload: TestRunFunction#test_all_options_in_payload().
  TestRunFunction.test_error_handling: TestRunFunction#test_error_handling().
  TestRunFunction.test_custom_project_root: TestRunFunction#test_custom_project_root().
  TestRunFunction.test_result_without_success_key: TestRunFunction#test_result_without_success_key().
  TestEdgeCases.test_depth_zero: TestEdgeCases#test_depth_zero().
  TestEdgeCases.test_limit_zero: TestEdgeCases#test_limit_zero().
  TestEdgeCases.test_empty_result: TestEdgeCases#test_empty_result().
  TestMainFunction.test_main_success: TestMainFunction#test_main_success().
  TestMainFunction.test_main_error: TestMainFunction#test_main_error().
  TestMainFunction.test_main_keyboard_interrupt: TestMainFunction#test_main_keyboard_interrupt().
  TestMainFunction.test_main_invalid_arguments: TestMainFunction#test_main_invalid_arguments().
  TestRunFunction: TestRunFunction#
  TestMainFunction: TestMainFunction#
  TestEdgeCases: TestEdgeCases#
---
# Module: [`tests/unit/cli/test_list_files_cli_comprehensive_execution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py)

## Classes
### `TestEdgeCases`
- def: [`tests/unit/cli/test_list_files_cli_comprehensive_execution.py:335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L335)
- doc: Test edge cases and boundary conditions.
- signature: `class TestEdgeCases:`
- members:
  - `test_depth_zero(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L339) — Test depth=0 (current directory only).
  - `test_empty_result(self)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L389) — Test empty file list result.
  - `test_limit_zero(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L364) — Test limit=0.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_run)  (1 test-only)

### `TestMainFunction`
- def: [`tests/unit/cli/test_list_files_cli_comprehensive_execution.py:245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L245)
- doc: Test the main() entry point.
- signature: `class TestMainFunction:`
- members:
  - `test_main_error(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L273) — Test main function with error.
  - `test_main_invalid_arguments(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L322) — Test main function with invalid arguments.
  - `test_main_keyboard_interrupt(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L298) — Test main function handles keyboard interrupt.
  - `test_main_success(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L248) — Test main function with successful execution.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#main)

### `TestRunFunction`
- def: [`tests/unit/cli/test_list_files_cli_comprehensive_execution.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L41)
- doc: Test the _run async function.
- signature: `class TestRunFunction:`
- members:
  - `test_all_options_in_payload(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L110) — Test all options are included in payload.
  - `test_custom_project_root(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L194) — Test custom project root is used.
  - `test_error_handling(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L167) — Test error handling in _run.
  - `test_minimal_execution(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L45) — Test minimal execution with required arguments.
  - `test_result_without_success_key(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L219) — Test result dict without success key returns 0.
  - `test_text_output_format(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L80) — Test text output format.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_run)  (1 test-only)

## Functions
- `_make_args(**overrides: object)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_execution.py#L14) — Build a default args namespace with optional overrides.

