---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_batch_core_mixins`/ReadPartialToolExecuteBatch
symbols:
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_invalid_section_entry: ProcessingMixin#test_execute_batch_invalid_section_entry().
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_invalid_start_line: ProcessingMixin#test_execute_batch_invalid_start_line().
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_invalid_end_line: ProcessingMixin#test_execute_batch_invalid_end_line().
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_success: ProcessingMixin#test_execute_batch_success().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_mutually_exclusive: ValidationMixin#test_execute_batch_mutually_exclusive().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_file_output_not_supported: ValidationMixin#test_execute_batch_file_output_not_supported().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_invalid_requests_type: ValidationMixin#test_execute_batch_invalid_requests_type().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_too_many_files: ValidationMixin#test_execute_batch_too_many_files().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_too_many_files_with_truncate: ValidationMixin#test_execute_batch_too_many_files_with_truncate().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_invalid_request_entry: ValidationMixin#test_execute_batch_invalid_request_entry().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_invalid_file_path: ValidationMixin#test_execute_batch_invalid_file_path().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_invalid_sections: ValidationMixin#test_execute_batch_invalid_sections().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_too_many_sections_per_file: ValidationMixin#test_execute_batch_too_many_sections_per_file().
  ReadPartialToolExecuteBatchValidationMixin.test_execute_batch_too_many_sections_per_file_with_truncate: ValidationMixin#test_execute_batch_too_many_sections_per_file_with_truncate().
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_file_not_found: ProcessingMixin#test_execute_batch_file_not_found().
  ReadPartialToolExecuteBatchProcessingMixin.test_execute_batch_fail_fast: ProcessingMixin#test_execute_batch_fail_fast().
  ReadPartialToolExecuteBatchValidationMixin: ValidationMixin#
  ReadPartialToolExecuteBatchProcessingMixin: ProcessingMixin#
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py)

## Classes
### `ReadPartialToolExecuteBatchProcessingMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py:157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L157)
- doc: Batch-mode file processing tests.
- signature: `class ReadPartialToolExecuteBatchProcessingMixin:`
- members:
  - `test_execute_batch_fail_fast(self)` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L300) — Test that batch mode stops on first error when fail_fast=True.
  - `test_execute_batch_file_not_found(self)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L161) — Test that batch mode handles file not found.
  - `test_execute_batch_invalid_end_line(self)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L240) — Test that batch mode handles invalid end_line.
  - `test_execute_batch_invalid_section_entry(self)` — [`L182`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L182) — Test that batch mode handles invalid section entries.
  - `test_execute_batch_invalid_start_line(self)` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L211) — Test that batch mode handles invalid start_line.
  - `test_execute_batch_success(self)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L269) — Test successful batch execution.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (3 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolExecuteBatchValidationMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L19)
- doc: Batch-mode validation and truncation tests.
- signature: `class ReadPartialToolExecuteBatchValidationMixin:`
- members:
  - `test_execute_batch_file_output_not_supported(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L34) — Test that batch mode doesn't support file output options.
  - `test_execute_batch_invalid_file_path(self)` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L92) — Test that batch mode handles invalid file_path.
  - `test_execute_batch_invalid_request_entry(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L80) — Test that batch mode handles invalid request entries.
  - `test_execute_batch_invalid_requests_type(self)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L47) — Test that batch mode fails when requests is not a list.
  - `test_execute_batch_invalid_sections(self)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L105) — Test that batch mode handles invalid sections.
  - `test_execute_batch_mutually_exclusive(self)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L23) — Test that batch mode fails with single mode arguments.
  - `test_execute_batch_too_many_files(self)` — [`L55`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L55) — Test that batch mode fails when too many files.
  - `test_execute_batch_too_many_files_with_truncate(self)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L67) — Test that batch mode truncates when allow_truncate=True.
  - `test_execute_batch_too_many_sections_per_file(self)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L118) — Test that batch mode fails when too many sections per file.
  - `test_execute_batch_too_many_sections_per_file_with_truncate(self)` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_batch_core_mixins.py#L130) — Test that batch mode truncates sections when allow_truncate=True.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`_execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool._execute_batch)  (1 test-only)
- used by: (1 test-only callers)

