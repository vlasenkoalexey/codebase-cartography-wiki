---
title: 'Module: tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py'
type: catalog
provenance: extracted
module: tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli._test_cli_main_module_handle_special_commands_batch_mixin`/TestHandleSpecialCommandsBatchMixin#
symbols:
  TestHandleSpecialCommandsBatchMixin: ''
  TestHandleSpecialCommandsBatchMixin.test_partial_read_no_start_line: test_partial_read_no_start_line().
  TestHandleSpecialCommandsBatchMixin.test_partial_read_start_line_zero: test_partial_read_start_line_zero().
  TestHandleSpecialCommandsBatchMixin.test_partial_read_end_line_lt_start: test_partial_read_end_line_lt_start().
  TestHandleSpecialCommandsBatchMixin.test_partial_read_negative_start_column: test_partial_read_negative_start_column().
  TestHandleSpecialCommandsBatchMixin.test_partial_read_negative_end_column: test_partial_read_negative_end_column().
  TestHandleSpecialCommandsBatchMixin.test_batch_partial_read_json_input: test_batch_partial_read_json_input().
  TestHandleSpecialCommandsBatchMixin.test_batch_partial_read_failure: test_batch_partial_read_failure().
  TestHandleSpecialCommandsBatchMixin.test_batch_metrics_success: test_batch_metrics_success().
  TestHandleSpecialCommandsBatchMixin.test_batch_metrics_no_paths: test_batch_metrics_no_paths().
  TestHandleSpecialCommandsBatchMixin.test_batch_metrics_failure: test_batch_metrics_failure().
  TestHandleSpecialCommandsBatchMixin.test_show_query_languages: test_show_query_languages().
  TestHandleSpecialCommandsBatchMixin.__test__: __test__.
---
# Module: [`tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py)

## Classes
### `TestHandleSpecialCommandsBatchMixin`
- def: [`tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L14)
- doc: Batch/partial-read tests for handle_special_commands.
- signature: `class TestHandleSpecialCommandsBatchMixin:`
- members:
  - `test_batch_metrics_failure(self, mock_output_json, mock_scale_tool_cls)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L284) — batch metrics failure path (r37al: now emits JSON envelope).
  - `test_batch_metrics_no_paths(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L252) — batch metrics without file_paths or files_from.
  - `test_batch_metrics_success(self, mock_asyncio, mock_scale_tool_cls)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L224) — batch metrics success path.
  - `test_batch_partial_read_failure(self, mock_read_tool_cls, mock_output_json)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L185) — batch partial read handling exception (r37al: JSON envelope).
  - `test_batch_partial_read_json_input(self, mock_asyncio, mock_read_tool_cls)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L147) — batch partial read with JSON string input.
  - `test_partial_read_end_line_lt_start(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L69) — partial_read with --end-line < --start-line returns error.
  - `test_partial_read_negative_end_column(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L119) — partial_read with --end-column < 0 returns error.
  - `test_partial_read_negative_start_column(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L95) — partial_read with --start-column < 0 returns error.
  - `test_partial_read_no_start_line(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L21) — partial_read without --start-line returns error.
  - `test_partial_read_start_line_zero(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L45) — partial_read with --start-line < 1 returns error.
  - `test_show_query_languages(self, mock_output_list, mock_list_queries, mock_list_langs)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L316) — show_query_languages lists all supported languages.
- protocol/private: `__test__`[`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_batch_mixin.py#L17)
- uses (calls/refs, reference-scoped): [`handle_special_commands`](../../../tree_sitter_analyzer/cli_main.md#handle_special_commands)  (1 test-only)
- used by: (1 test-only callers)

