---
title: 'Module: tests/unit/mcp/tools/test_batch_executor_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_batch_executor_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_batch_executor_execute`/TestExecuteBatch#
symbols:
  TestExecuteBatch._make_tool: _make_tool().
  TestExecuteBatch.test_truncation_on_too_many_files: test_truncation_on_too_many_files().
  TestExecuteBatch.test_reject_too_many_files_without_truncate: test_reject_too_many_files_without_truncate().
  TestExecuteBatch.test_fail_fast_on_section_limit: test_fail_fast_on_section_limit().
  TestExecuteBatch.test_truncate_on_section_limit: test_truncate_on_section_limit().
  TestExecuteBatch.test_content_bytes_limit_exceeded: test_content_bytes_limit_exceeded().
  TestExecuteBatch.test_content_bytes_limit_with_truncate: test_content_bytes_limit_with_truncate().
  TestExecuteBatch.test_content_lines_limit_exceeded: test_content_lines_limit_exceeded().
  TestExecuteBatch.test_empty_requests: test_empty_requests().
  TestExecuteBatch.test_single_file_single_section: test_single_file_single_section().
  TestExecuteBatch.test_invalid_file_path_in_batch: test_invalid_file_path_in_batch().
  TestExecuteBatch.test_non_dict_request_entry: test_non_dict_request_entry().
  TestExecuteBatch.test_fail_fast_on_invalid_entry: test_fail_fast_on_invalid_entry().
  TestExecuteBatch.test_invalid_section_entry_in_batch: test_invalid_section_entry_in_batch().
  TestExecuteBatch.test_invalid_start_line_in_section: test_invalid_start_line_in_section().
  TestExecuteBatch.test_invalid_end_line_in_section: test_invalid_end_line_in_section().
  TestExecuteBatch.test_empty_content_counts_as_error: test_empty_content_counts_as_error().
  TestExecuteBatch.test_batch_limits_in_response: test_batch_limits_in_response().
  TestExecuteBatch.test_agent_summary_in_response: test_agent_summary_in_response().
  TestExecuteBatch.test_output_format_json: test_output_format_json().
  TestExecuteBatch.test_output_format_toon: test_output_format_toon().
  TestExecuteBatch.test_multiple_files: test_multiple_files().
  TestExecuteBatch.test_label_preserved_in_section_result: test_label_preserved_in_section_result().
  TestExecuteBatch.test_end_line_none_in_section: test_end_line_none_in_section().
  TestExecuteBatch.test_whitespace_only_content_is_error: test_whitespace_only_content_is_error().
  TestExecuteBatch.test_content_raw_format: test_content_raw_format().
  TestExecuteBatch.test_errors_summary_count: test_errors_summary_count().
  TestExecuteBatch.test_file_resolve_error_continues: test_file_resolve_error_continues().
  TestExecuteBatch.test_success_false_when_all_errors: test_success_false_when_all_errors().
  TestExecuteBatch.read_fn: read_fn().
  TestExecuteBatch: ''
---
# Module: [`tests/unit/mcp/tools/test_batch_executor_execute.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py)

## Classes
### `TestExecuteBatch`
- def: [`tests/unit/mcp/tools/test_batch_executor_execute.py:13`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L13)
- signature: `class TestExecuteBatch:`
- members:
  - `read_fn(resolved, start, end)` — [`L301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L301)
  - `test_agent_summary_in_response(self, tmp_path)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L234)
  - `test_batch_limits_in_response(self, tmp_path)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L221)
  - `test_content_bytes_limit_exceeded(self, tmp_path)` — [`L401`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L401)
  - `test_content_bytes_limit_with_truncate(self, tmp_path)` — [`L421`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L421)
  - `test_content_lines_limit_exceeded(self, tmp_path)` — [`L442`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L442)
  - `test_content_raw_format(self, tmp_path)` — [`L467`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L467)
  - `test_empty_content_counts_as_error(self, tmp_path)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L164)
  - `test_empty_requests(self)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L20)
  - `test_end_line_none_in_section(self, tmp_path)` — [`L362`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L362)
  - `test_errors_summary_count(self, tmp_path)` — [`L505`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L505)
  - `test_fail_fast_on_invalid_entry(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L74)
  - `test_fail_fast_on_section_limit(self, tmp_path)` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L183)
  - `test_file_resolve_error_continues(self)` — [`L323`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L323)
  - `test_invalid_end_line_in_section(self, tmp_path)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L143)
  - `test_invalid_file_path_in_batch(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L53)
  - `test_invalid_section_entry_in_batch(self, tmp_path)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L105)
  - `test_invalid_start_line_in_section(self, tmp_path)` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L124)
  - `test_label_preserved_in_section_result(self, tmp_path)` — [`L338`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L338)
  - `test_multiple_files(self, tmp_path)` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L295)
  - `test_non_dict_request_entry(self)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L64)
  - `test_output_format_json(self, tmp_path)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L254)
  - `test_output_format_toon(self, tmp_path)` — [`L275`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L275)
  - `test_reject_too_many_files_without_truncate(self)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L97)
  - `test_single_file_single_section(self, tmp_path)` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L29)
  - `test_success_false_when_all_errors(self)` — [`L490`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L490)
  - `test_truncate_on_section_limit(self, tmp_path)` — [`L202`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L202)
  - `test_truncation_on_too_many_files(self)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L84)
  - `test_whitespace_only_content_is_error(self, tmp_path)` — [`L382`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L382)
- protocol/private: `_make_tool`[`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_execute.py#L14)
- uses (calls/refs, reference-scoped): [`execute_batch`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#execute_batch), [`BATCH_LIMITS`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#BATCH_LIMITS)

