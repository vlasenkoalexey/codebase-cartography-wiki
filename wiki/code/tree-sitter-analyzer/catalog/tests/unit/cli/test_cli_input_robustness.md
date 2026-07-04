---
title: 'Module: tests/unit/cli/test_cli_input_robustness.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_cli_input_robustness.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_cli_input_robustness`/
symbols:
  _run_cli: _run_cli().
  TestBatchSearchInputRobustness.test_batch_search_missing_queries_json_returns_structured_error: TestBatchSearchInputRobustness#test_batch_search_missing_queries_json_returns_structured_error().
  TestBatchSearchInputRobustness.test_batch_search_malformed_json_returns_structured_error: TestBatchSearchInputRobustness#test_batch_search_malformed_json_returns_structured_error().
  TestSafeToEditDirectoryRejection.test_safe_to_edit_directory_returns_structured_error: TestSafeToEditDirectoryRejection#test_safe_to_edit_directory_returns_structured_error().
  TestAgentWorkflowDirectoryRejection.test_agent_workflow_directory_returns_nonzero_exit: TestAgentWorkflowDirectoryRejection#test_agent_workflow_directory_returns_nonzero_exit().
  _assert_no_traceback: _assert_no_traceback().
  PROJECT_ROOT: PROJECT_ROOT.
  TestBatchSearchInputRobustness: TestBatchSearchInputRobustness#
  TestSafeToEditDirectoryRejection: TestSafeToEditDirectoryRejection#
  TestAgentWorkflowDirectoryRejection: TestAgentWorkflowDirectoryRejection#
---
# Module: [`tests/unit/cli/test_cli_input_robustness.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py)

## Classes
### `TestAgentWorkflowDirectoryRejection`
- def: [`tests/unit/cli/test_cli_input_robustness.py:109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L109)
- doc: #1002 finding 3 — --agent-workflow must exit non-zero for a dir.
- signature: `class TestAgentWorkflowDirectoryRejection:`
- members:
  - `test_agent_workflow_directory_returns_nonzero_exit(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L112)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestBatchSearchInputRobustness`
- def: [`tests/unit/cli/test_cli_input_robustness.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L53)
- doc: #1003 — no raw traceback for bad --batch-search-queries-json.
- signature: `class TestBatchSearchInputRobustness:`
- members:
  - `test_batch_search_malformed_json_returns_structured_error(self, tmp_path: Path)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L71)
  - `test_batch_search_missing_queries_json_returns_structured_error(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L56)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestSafeToEditDirectoryRejection`
- def: [`tests/unit/cli/test_cli_input_robustness.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L91)
- doc: #1002 finding 1 — --safe-to-edit must reject a directory.
- signature: `class TestSafeToEditDirectoryRejection:`
- members:
  - `test_safe_to_edit_directory_returns_structured_error(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L94)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_assert_no_traceback(proc: subprocess.CompletedProcess[str])` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L48)
- `_run_cli(*cli_args: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L35) — Invoke the TSA CLI in a subprocess from the project root.

## Module values
- `PROJECT_ROOT` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_input_robustness.py#L32)

