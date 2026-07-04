---
title: 'Module: tests/unit/cli/test_find_and_grep_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_find_and_grep_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_find_and_grep_cli`/
symbols:
  _run_with_mock_result: _run_with_mock_result().
  TestH1FindAndGrepExitCode.test_exception_returns_one: TestH1FindAndGrepExitCode#test_exception_returns_one().
  TestH1FindAndGrepExitCode.test_success_payload_returns_zero: TestH1FindAndGrepExitCode#test_success_payload_returns_zero().
  TestH1FindAndGrepExitCode.test_success_without_explicit_flag_returns_zero: TestH1FindAndGrepExitCode#test_success_without_explicit_flag_returns_zero().
  TestH1FindAndGrepExitCode.test_failure_payload_returns_one: TestH1FindAndGrepExitCode#test_failure_payload_returns_one().
  TestH1FindAndGrepExitCode.test_int_count_only_returns_zero: TestH1FindAndGrepExitCode#test_int_count_only_returns_zero().
  _base_args: _base_args().
  TestH1FindAndGrepExitCode: TestH1FindAndGrepExitCode#
---
# Module: [`tests/unit/cli/test_find_and_grep_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py)

## Classes
### `TestH1FindAndGrepExitCode`
- def: [`tests/unit/cli/test_find_and_grep_cli.py:102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L102)
- doc: H1: standalone `find-and-grep` exit code must reflect `success`.
- signature: `class TestH1FindAndGrepExitCode:`
- members:
  - `test_exception_returns_one(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L136) — An exception during execute → rc=1 via the except branch.
  - `test_failure_payload_returns_one(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L120) — H1 regression: ``success: false`` payload → rc=1, not rc=0.
  - `test_int_count_only_returns_zero(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L130) — Count-only mode legacy shape returns int — that's success, rc=0.
  - `test_success_payload_returns_zero(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L106) — A normal successful match → rc=0.
  - `test_success_without_explicit_flag_returns_zero(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L114) — A dict with no ``success`` key (legacy shape) is treated as success.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_run)  (2 test-only)

## Functions
- `_base_args()` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L28) — Build a minimal but complete Namespace for ``_run``.
- `_run_with_mock_result(result: Any)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli.py#L75) — Run the CLI with a mocked tool result, return exit code.

