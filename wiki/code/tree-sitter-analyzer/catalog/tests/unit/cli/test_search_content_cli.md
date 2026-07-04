---
title: 'Module: tests/unit/cli/test_search_content_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_search_content_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_search_content_cli`/
symbols:
  _run_with_mock_result: _run_with_mock_result().
  TestH1SearchContentExitCode.test_exception_returns_one: TestH1SearchContentExitCode#test_exception_returns_one().
  TestH1SearchContentExitCode.test_success_payload_returns_zero: TestH1SearchContentExitCode#test_success_payload_returns_zero().
  TestH1SearchContentExitCode.test_success_without_explicit_flag_returns_zero: TestH1SearchContentExitCode#test_success_without_explicit_flag_returns_zero().
  TestH1SearchContentExitCode.test_failure_payload_returns_one: TestH1SearchContentExitCode#test_failure_payload_returns_one().
  TestH1SearchContentExitCode.test_int_count_only_returns_zero: TestH1SearchContentExitCode#test_int_count_only_returns_zero().
  _base_args: _base_args().
  TestH1SearchContentExitCode: TestH1SearchContentExitCode#
---
# Module: [`tests/unit/cli/test_search_content_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py)

## Classes
### `TestH1SearchContentExitCode`
- def: [`tests/unit/cli/test_search_content_cli.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L87)
- doc: H1: standalone `search-content` exit code must reflect `success`.
- signature: `class TestH1SearchContentExitCode:`
- members:
  - `test_exception_returns_one(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L121) — An exception during execute → rc=1 via the except branch.
  - `test_failure_payload_returns_one(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L105) — H1 regression: ``success: false`` payload → rc=1, not rc=0.
  - `test_int_count_only_returns_zero(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L115) — Count-only mode legacy shape returns int — that's success, rc=0.
  - `test_success_payload_returns_zero(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L91) — A normal successful match → rc=0.
  - `test_success_without_explicit_flag_returns_zero(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L99) — A dict with no ``success`` key (legacy shape) is treated as success.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/search_content_cli.md#_run)  (2 test-only)

## Functions
- `_base_args()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L35) — Build a minimal but complete Namespace for ``_run``.
- `_run_with_mock_result(result: Any)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli.py#L67) — Run the CLI with a mocked tool result, return exit code.

