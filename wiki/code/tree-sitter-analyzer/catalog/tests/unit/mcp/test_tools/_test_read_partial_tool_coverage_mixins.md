---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_coverage_mixins`/ReadPartialToolCoverage
symbols:
  ReadPartialToolCoverageBatchMixin.test_batch_resolve_error_no_fail_fast: BatchMixin#test_batch_resolve_error_no_fail_fast().
  ReadPartialToolCoverageBatchMixin.test_batch_raw_content_format: BatchMixin#test_batch_raw_content_format().
  ReadPartialToolCoverageBatchMixin.test_batch_end_line_none_content_lines: BatchMixin#test_batch_end_line_none_content_lines().
  ReadPartialToolCoverageExecuteMixin.test_execute_empty_output_file_string: ExecuteMixin#test_execute_empty_output_file_string().
  ReadPartialToolCoverageExecuteMixin.test_execute_batch_via_execute_method: ExecuteMixin#test_execute_batch_via_execute_method().
  ReadPartialToolCoverageExecuteMixin.test_execute_no_end_line_single_line: ExecuteMixin#test_execute_no_end_line_single_line().
  ReadPartialToolCoverageExecuteMixin.test_execute_json_format_lines_padding: ExecuteMixin#test_execute_json_format_lines_padding().
  ReadPartialToolCoverageExecuteMixin.test_execute_no_end_line_no_next_steps: ExecuteMixin#test_execute_no_end_line_no_next_steps().
  ReadPartialToolCoverageValidateMixin.test_validate_file_path_not_string_branch: ValidateMixin#test_validate_file_path_not_string_branch().
  ReadPartialToolCoverageValidateMixin.test_validate_file_path_empty_branch: ValidateMixin#test_validate_file_path_empty_branch().
  ReadPartialToolCoverageExecuteMixin: ExecuteMixin#
  ReadPartialToolCoverageBatchMixin: BatchMixin#
  ReadPartialToolCoverageValidateMixin: ValidateMixin#
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py)

## Classes
### `ReadPartialToolCoverageBatchMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py:152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L152)
- doc: Coverage tests for batch execute branches.
- signature: `class ReadPartialToolCoverageBatchMixin:`
- members:
  - `test_batch_end_line_none_content_lines(self)` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L203) — Test batch section without end_line (branch 630->634).
  - `test_batch_raw_content_format(self)` — [`L172`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L172) — Test batch mode with content_format='raw' (line 659).
  - `test_batch_resolve_error_no_fail_fast(self)` — [`L156`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L156) — Test batch resolve error without fail_fast (lines 508-517).
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (3 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolCoverageExecuteMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L19)
- doc: Coverage tests for single-file execute branches.
- signature: `class ReadPartialToolCoverageExecuteMixin:`
- members:
  - `test_execute_batch_via_execute_method(self)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L23) — Test that execute() dispatches to _execute_batch (line 156).
  - `test_execute_empty_output_file_string(self)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L94) — Test empty output_file string generates base name from file path (line 343).
  - `test_execute_json_format_lines_padding(self)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L63) — Test JSON format with end_line where content has fewer lines (lines 316-318).
  - `test_execute_no_end_line_no_next_steps(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L128) — Test no end_line means no next_steps added (branch 301->308).
  - `test_execute_no_end_line_single_line(self)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L36) — Test execute without end_line (branches 265->269, 283->287).
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`file_output_manager`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.file_output_manager)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolCoverageValidateMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py:230`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L230)
- doc: Coverage tests for validation branches.
- signature: `class ReadPartialToolCoverageValidateMixin:`
- members:
  - `test_validate_file_path_empty_branch(self)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L239) — Test validate_arguments with empty file_path (branch 760->768).
  - `test_validate_file_path_not_string_branch(self)` — [`L233`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_coverage_mixins.py#L233) — Test validate_arguments with file_path as non-string (branch 752->760).
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments)  (1 test-only)
- used by: (1 test-only callers)

