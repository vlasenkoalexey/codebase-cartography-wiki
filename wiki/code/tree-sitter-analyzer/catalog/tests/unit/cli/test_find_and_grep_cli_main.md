---
title: 'Module: tests/unit/cli/test_find_and_grep_cli_main.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_find_and_grep_cli_main.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_find_and_grep_cli_main`/Test
symbols:
  TestMainFunction.test_main_success: MainFunction#test_main_success().
  TestMainFunction.test_main_error: MainFunction#test_main_error().
  TestMainFunction.test_main_keyboard_interrupt: MainFunction#test_main_keyboard_interrupt().
  TestMainFunction.test_main_invalid_arguments: MainFunction#test_main_invalid_arguments().
  TestEdgeCases.test_depth_zero: EdgeCases#test_depth_zero().
  TestEdgeCases.test_context_zero: EdgeCases#test_context_zero().
  TestEdgeCases.test_empty_result: EdgeCases#test_empty_result().
  TestEdgeCases.test_parser_help: EdgeCases#test_parser_help().
  TestMainFunction: MainFunction#
  TestEdgeCases: EdgeCases#
---
# Module: [`tests/unit/cli/test_find_and_grep_cli_main.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py)

## Classes
### `TestEdgeCases`
- def: [`tests/unit/cli/test_find_and_grep_cli_main.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L114)
- doc: Test edge cases and boundary conditions.
- signature: `class TestEdgeCases:`
- members:
  - `test_context_zero(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L183) — Test context lines = 0.
  - `test_depth_zero(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L118) — Test depth=0 (current directory only).
  - `test_empty_result(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L249) — Test empty search result.
  - `test_parser_help(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L315) — Test parser help output.
- uses (calls/refs, reference-scoped): [`_run`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_run), [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_build_parser)

### `TestMainFunction`
- def: [`tests/unit/cli/test_find_and_grep_cli_main.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L18)
- doc: Test the main() entry point.
- signature: `class TestMainFunction:`
- members:
  - `test_main_error(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L48) — Test main function with error.
  - `test_main_invalid_arguments(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L101) — Test main function with invalid arguments.
  - `test_main_keyboard_interrupt(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L75) — Test main function handles keyboard interrupt.
  - `test_main_success(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_main.py#L21) — Test main function with successful execution.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#main)

