---
title: 'Module: tests/unit/cli/test_list_files_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_list_files_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_list_files_cli`/
symbols:
  _run_with_mock_result: _run_with_mock_result().
  TestH1ListFilesExitCode.test_exception_returns_one: TestH1ListFilesExitCode#test_exception_returns_one().
  TestH1ListFilesExitCode.test_success_payload_returns_zero: TestH1ListFilesExitCode#test_success_payload_returns_zero().
  TestH1ListFilesExitCode.test_success_without_explicit_flag_returns_zero: TestH1ListFilesExitCode#test_success_without_explicit_flag_returns_zero().
  TestH1ListFilesExitCode.test_failure_payload_returns_one: TestH1ListFilesExitCode#test_failure_payload_returns_one().
  TestH1ListFilesExitCode.test_int_count_only_returns_zero: TestH1ListFilesExitCode#test_int_count_only_returns_zero().
  _base_args: _base_args().
  TestH1ListFilesExitCode: TestH1ListFilesExitCode#
---
# Module: [`tests/unit/cli/test_list_files_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py)

## Classes
### `TestH1ListFilesExitCode`
- def: [`tests/unit/cli/test_list_files_cli.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L81)
- doc: H1: standalone `list-files` exit code must reflect `success`.
- signature: `class TestH1ListFilesExitCode:`
- members:
  - `test_exception_returns_one(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L119) — An exception during execute → rc=1 via the except branch.
  - `test_failure_payload_returns_one(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L99) — H1 regression: ``success: false`` payload → rc=1, not rc=0.
  - `test_int_count_only_returns_zero(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L113) — Count-only mode legacy shape returns int — that's success, rc=0.
  - `test_success_payload_returns_zero(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L85) — A normal successful listing → rc=0.
  - `test_success_without_explicit_flag_returns_zero(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L93) — A dict with no ``success`` key (legacy shape) is treated as success.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_run)  (2 test-only)

## Functions
- `_base_args()` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L28) — Build a minimal but complete Namespace for ``_run``.
- `_run_with_mock_result(result: Any)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli.py#L53) — Run the CLI with a mocked tool result, return exit code.

