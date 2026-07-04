---
title: 'Module: tests/unit/cli/test_search_content_cli_run.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_search_content_cli_run.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_search_content_cli_run`/TestRunFunction#
symbols:
  TestRunFunction.test_minimal_execution_with_roots: test_minimal_execution_with_roots().
  TestRunFunction.test_minimal_execution_with_files: test_minimal_execution_with_files().
  TestRunFunction.test_text_output_format: test_text_output_format().
  TestRunFunction.test_all_options_in_payload: test_all_options_in_payload().
  TestRunFunction.test_integer_result: test_integer_result().
  TestRunFunction.test_error_handling: test_error_handling().
  TestRunFunction.test_custom_project_root: test_custom_project_root().
  TestRunFunction: ''
---
# Module: [`tests/unit/cli/test_search_content_cli_run.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py)

## Classes
### `TestRunFunction`
- def: [`tests/unit/cli/test_search_content_cli_run.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L14)
- doc: Test the _run async function.
- signature: `class TestRunFunction:`
- members:
  - `test_all_options_in_payload(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L199) — Test all options are included in payload.
  - `test_custom_project_root(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L386) — Test custom project root is used.
  - `test_error_handling(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L330) — Test error handling in _run.
  - `test_integer_result(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L274) — Test integer result (count) is handled correctly.
  - `test_minimal_execution_with_files(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L86) — Test minimal execution with files.
  - `test_minimal_execution_with_roots(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L18) — Test minimal execution with roots.
  - `test_text_output_format(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_run.py#L142) — Test text output format.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/search_content_cli.md#_run)

