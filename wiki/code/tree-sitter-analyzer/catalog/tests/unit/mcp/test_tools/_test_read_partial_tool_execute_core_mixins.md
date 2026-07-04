---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_execute_core_mixins`/ReadPartialTool
symbols:
  ReadPartialToolExecuteMixin.test_execute_missing_file_path: ExecuteMixin#test_execute_missing_file_path().
  ReadPartialToolExecuteMixin.test_execute_missing_start_line: ExecuteMixin#test_execute_missing_start_line().
  ReadPartialToolExecuteMixin.test_execute_invalid_path: ExecuteMixin#test_execute_invalid_path().
  ReadPartialToolExecuteMixin.test_execute_file_not_found: ExecuteMixin#test_execute_file_not_found().
  ReadPartialToolExecuteMixin.test_execute_invalid_start_line: ExecuteMixin#test_execute_invalid_start_line().
  ReadPartialToolExecuteMixin.test_execute_invalid_end_line: ExecuteMixin#test_execute_invalid_end_line().
  ReadPartialToolExecuteMixin.test_execute_invalid_start_column: ExecuteMixin#test_execute_invalid_start_column().
  ReadPartialToolExecuteMixin.test_execute_invalid_end_column: ExecuteMixin#test_execute_invalid_end_column().
  ReadPartialToolExecuteMixin.test_execute_success_text_format: ExecuteMixin#test_execute_success_text_format().
  ReadPartialToolExecuteMixin.test_execute_success_json_format: ExecuteMixin#test_execute_success_json_format().
  ReadPartialToolExecuteMixin.test_execute_suppress_output: ExecuteMixin#test_execute_suppress_output().
  ReadPartialToolExecuteMixin.test_execute_empty_content: ExecuteMixin#test_execute_empty_content().
  ReadPartialToolReadFilePartialMixin.test_read_file_partial_success: ReadFilePartialMixin#test_read_file_partial_success().
  ReadPartialToolReadFilePartialMixin.test_read_file_partial_with_columns: ReadFilePartialMixin#test_read_file_partial_with_columns().
  ReadPartialToolExecuteMixin: ExecuteMixin#
  ReadPartialToolReadFilePartialMixin: ReadFilePartialMixin#
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py)

## Classes
### `ReadPartialToolExecuteMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py:15`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L15)
- doc: Tests for execute method (single mode).
- signature: `class ReadPartialToolExecuteMixin:`
- members:
  - `test_execute_empty_content(self)` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L222) — Empty file with a non-trivial range used to fail with a
  - `test_execute_file_not_found(self)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L43) — Test execution fails when file doesn't exist.
  - `test_execute_invalid_end_column(self)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L102) — Test execution fails when end_column < 0.
  - `test_execute_invalid_end_line(self)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L70) — Test execution fails when end_line < start_line.
  - `test_execute_invalid_path(self)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L33) — Test execution fails for invalid file path.
  - `test_execute_invalid_start_column(self)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L86) — Test execution fails when start_column < 0.
  - `test_execute_invalid_start_line(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L56) — Test execution fails when start_line < 1.
  - `test_execute_missing_file_path(self)` — [`L19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L19) — Test execution fails when file_path is missing.
  - `test_execute_missing_start_line(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L26) — Test execution fails when start_line is missing.
  - `test_execute_success_json_format(self)` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L155) — Test successful execution with JSON format.
  - `test_execute_success_text_format(self)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L118) — Test successful execution with text format.
  - `test_execute_suppress_output(self)` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L190) — Test execution with suppress_output=True.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolReadFilePartialMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py:268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L268)
- doc: Tests for _read_file_partial method.
- signature: `class ReadPartialToolReadFilePartialMixin:`
- members:
  - `test_read_file_partial_success(self)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L272) — Test successful partial file read.
  - `test_read_file_partial_with_columns(self)` — [`L292`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_core_mixins.py#L292) — Test partial file read with column ranges.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_read_file_partial`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._read_file_partial)  (1 test-only)
- used by: (1 test-only callers)

