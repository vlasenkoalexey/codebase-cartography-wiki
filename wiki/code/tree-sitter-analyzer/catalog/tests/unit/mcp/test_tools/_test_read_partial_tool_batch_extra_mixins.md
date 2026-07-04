---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_batch_extra_mixins`/ReadPartialToolBatchExtra
symbols:
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_fail_fast_resolve_error: FileErrorMixin#test_batch_fail_fast_resolve_error().
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_fail_fast_file_not_exist: FileErrorMixin#test_batch_fail_fast_file_not_exist().
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_file_too_large_fail_fast: FileErrorMixin#test_batch_file_too_large_fail_fast().
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_file_too_large_no_fail_fast: FileErrorMixin#test_batch_file_too_large_no_fail_fast().
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_stat_oserror_fail_fast: FileErrorMixin#test_batch_stat_oserror_fail_fast().
  ReadPartialToolBatchExtraFileErrorMixin.test_batch_stat_oserror_no_fail_fast: FileErrorMixin#test_batch_stat_oserror_no_fail_fast().
  ReadPartialToolBatchExtraLimitMixin.test_batch_total_bytes_limit_no_truncate: LimitMixin#test_batch_total_bytes_limit_no_truncate().
  ReadPartialToolBatchExtraLimitMixin.test_batch_total_bytes_limit_with_truncate: LimitMixin#test_batch_total_bytes_limit_with_truncate().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_invalid_start_line: ValidationMixin#test_batch_fail_fast_invalid_start_line().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_invalid_end_line: ValidationMixin#test_batch_fail_fast_invalid_end_line().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_empty_content: ValidationMixin#test_batch_fail_fast_empty_content().
  ReadPartialToolBatchExtraLimitMixin.test_batch_sections_total_limit_no_truncate: LimitMixin#test_batch_sections_total_limit_no_truncate().
  ReadPartialToolBatchExtraLimitMixin.test_batch_sections_total_limit_with_truncate: LimitMixin#test_batch_sections_total_limit_with_truncate().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_invalid_request_entry: ValidationMixin#test_batch_fail_fast_invalid_request_entry().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_empty_file_path: ValidationMixin#test_batch_fail_fast_empty_file_path().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_invalid_sections_type: ValidationMixin#test_batch_fail_fast_invalid_sections_type().
  ReadPartialToolBatchExtraValidationMixin.test_batch_fail_fast_invalid_section_entry: ValidationMixin#test_batch_fail_fast_invalid_section_entry().
  ReadPartialToolBatchExtraValidationMixin.test_batch_too_many_sections_per_file_no_fail_fast: ValidationMixin#test_batch_too_many_sections_per_file_no_fail_fast().
  ReadPartialToolBatchExtraFileErrorMixin: FileErrorMixin#
  ReadPartialToolBatchExtraLimitMixin: LimitMixin#
  ReadPartialToolBatchExtraValidationMixin: ValidationMixin#
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py)

## Classes
### `ReadPartialToolBatchExtraFileErrorMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L19)
- doc: Batch error handling tests for file and stat failures.
- signature: `class ReadPartialToolBatchExtraFileErrorMixin:`
- members:
  - `test_batch_fail_fast_file_not_exist(self)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L35)
  - `test_batch_fail_fast_resolve_error(self)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L23)
  - `test_batch_file_too_large_fail_fast(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L46)
  - `test_batch_file_too_large_no_fail_fast(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L68)
  - `test_batch_stat_oserror_fail_fast(self)` — [`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L95)
  - `test_batch_stat_oserror_no_fail_fast(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L107)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (3 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolBatchExtraLimitMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py:124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L124)
- doc: Batch aggregate limit and truncation tests.
- signature: `class ReadPartialToolBatchExtraLimitMixin:`
- members:
  - `test_batch_sections_total_limit_no_truncate(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L128)
  - `test_batch_sections_total_limit_with_truncate(self)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L147)
  - `test_batch_total_bytes_limit_no_truncate(self)` — [`L168`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L168)
  - `test_batch_total_bytes_limit_with_truncate(self)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L188)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (3 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolBatchExtraValidationMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py:208`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L208)
- doc: Batch request validation edge-case tests.
- signature: `class ReadPartialToolBatchExtraValidationMixin:`
- members:
  - `test_batch_fail_fast_empty_content(self)` — [`L305`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L305)
  - `test_batch_fail_fast_empty_file_path(self)` — [`L218`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L218)
  - `test_batch_fail_fast_invalid_end_line(self)` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L285)
  - `test_batch_fail_fast_invalid_request_entry(self)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L212)
  - `test_batch_fail_fast_invalid_section_entry(self)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L240)
  - `test_batch_fail_fast_invalid_sections_type(self)` — [`L229`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L229)
  - `test_batch_fail_fast_invalid_start_line(self)` — [`L263`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L263)
  - `test_batch_too_many_sections_per_file_no_fail_fast(self)` — [`L332`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_extra_mixins.py#L332)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (3 test-only)
- used by: (1 test-only callers)

