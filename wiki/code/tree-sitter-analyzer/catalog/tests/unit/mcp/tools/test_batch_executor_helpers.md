---
title: 'Module: tests/unit/mcp/tools/test_batch_executor_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_batch_executor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_batch_executor_helpers`/Test
symbols:
  TestResolveFile._make_tool: ResolveFile#_make_tool().
  TestResolveFile.test_resolve_file_too_large_fail_fast: ResolveFile#test_resolve_file_too_large_fail_fast().
  TestResolveFile.test_resolve_file_too_large_no_fail_fast: ResolveFile#test_resolve_file_too_large_no_fail_fast().
  TestResolveFile.test_resolve_file_exact_size_limit: ResolveFile#test_resolve_file_exact_size_limit().
  TestClampRequests.test_clamps_when_over_limit_with_truncate: ClampRequests#test_clamps_when_over_limit_with_truncate().
  TestClampRequests.test_raises_when_over_limit_without_truncate: ClampRequests#test_raises_when_over_limit_without_truncate().
  TestClampRequests.test_exact_limit_not_clamped: ClampRequests#test_exact_limit_not_clamped().
  TestValidateFileRequest.test_too_many_sections_without_truncate_fail_fast: ValidateFileRequest#test_too_many_sections_without_truncate_fail_fast().
  TestValidateFileRequest.test_too_many_sections_with_truncate: ValidateFileRequest#test_too_many_sections_with_truncate().
  TestValidateFileRequest.test_too_many_sections_without_truncate_no_fail_fast: ValidateFileRequest#test_too_many_sections_without_truncate_no_fail_fast().
  TestResolveFile.test_resolve_success: ResolveFile#test_resolve_success().
  TestResolveFile.test_resolve_file_not_exist_fail_fast: ResolveFile#test_resolve_file_not_exist_fail_fast().
  TestResolveFile.test_resolve_file_not_exist_no_fail_fast: ResolveFile#test_resolve_file_not_exist_no_fail_fast().
  TestResolveFile.test_resolve_os_error_fail_fast: ResolveFile#test_resolve_os_error_fail_fast().
  TestResolveFile.test_resolve_os_error_no_fail_fast: ResolveFile#test_resolve_os_error_no_fail_fast().
  TestBatchLimits.test_batch_limits_values: BatchLimits#test_batch_limits_values().
  TestValidateBatchTopLevel.test_returns_requests_list: ValidateBatchTopLevel#test_returns_requests_list().
  TestValidateBatchTopLevel.test_rejects_file_path_with_requests: ValidateBatchTopLevel#test_rejects_file_path_with_requests().
  TestValidateBatchTopLevel.test_rejects_start_line_with_requests: ValidateBatchTopLevel#test_rejects_start_line_with_requests().
  TestValidateBatchTopLevel.test_rejects_end_line_with_requests: ValidateBatchTopLevel#test_rejects_end_line_with_requests().
  TestValidateBatchTopLevel.test_rejects_start_column_with_requests: ValidateBatchTopLevel#test_rejects_start_column_with_requests().
  TestValidateBatchTopLevel.test_rejects_end_column_with_requests: ValidateBatchTopLevel#test_rejects_end_column_with_requests().
  TestValidateBatchTopLevel.test_rejects_output_file_with_requests: ValidateBatchTopLevel#test_rejects_output_file_with_requests().
  TestValidateBatchTopLevel.test_rejects_suppress_output_with_requests: ValidateBatchTopLevel#test_rejects_suppress_output_with_requests().
  TestValidateBatchTopLevel.test_rejects_non_list_requests: ValidateBatchTopLevel#test_rejects_non_list_requests().
  TestValidateBatchTopLevel.test_rejects_dict_requests: ValidateBatchTopLevel#test_rejects_dict_requests().
  TestValidateBatchTopLevel.test_accepts_empty_requests_list: ValidateBatchTopLevel#test_accepts_empty_requests_list().
  TestClampRequests.test_no_clamping_under_limit: ClampRequests#test_no_clamping_under_limit().
  TestMakeErrorResult.test_basic_error_result: MakeErrorResult#test_basic_error_result().
  TestMakeErrorResult.test_empty_strings: MakeErrorResult#test_empty_strings().
  TestMakeErrorResult.test_error_is_dict: MakeErrorResult#test_error_is_dict().
  TestValidateFileRequest.test_non_dict_with_fail_fast: ValidateFileRequest#test_non_dict_with_fail_fast().
  TestValidateFileRequest.test_non_dict_without_fail_fast: ValidateFileRequest#test_non_dict_without_fail_fast().
  TestValidateFileRequest.test_missing_file_path_with_fail_fast: ValidateFileRequest#test_missing_file_path_with_fail_fast().
  TestValidateFileRequest.test_missing_file_path_without_fail_fast: ValidateFileRequest#test_missing_file_path_without_fail_fast().
  TestValidateFileRequest.test_empty_file_path_with_fail_fast: ValidateFileRequest#test_empty_file_path_with_fail_fast().
  TestValidateFileRequest.test_missing_sections_with_fail_fast: ValidateFileRequest#test_missing_sections_with_fail_fast().
  TestValidateFileRequest.test_missing_sections_without_fail_fast: ValidateFileRequest#test_missing_sections_without_fail_fast().
  TestValidateFileRequest.test_valid_request: ValidateFileRequest#test_valid_request().
  TestResolveFile.test_resolve_validation_error_fail_fast: ResolveFile#test_resolve_validation_error_fail_fast().
  TestResolveFile.test_resolve_validation_error_no_fail_fast: ResolveFile#test_resolve_validation_error_no_fail_fast().
  TestBatchLimits: BatchLimits#
  TestValidateBatchTopLevel: ValidateBatchTopLevel#
  TestClampRequests: ClampRequests#
  TestMakeErrorResult: MakeErrorResult#
  TestValidateFileRequest: ValidateFileRequest#
  TestResolveFile: ResolveFile#
---
# Module: [`tests/unit/mcp/tools/test_batch_executor_helpers.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py)

## Classes
### `TestBatchLimits`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L17)
- signature: `class TestBatchLimits:`
- members:
  - `test_batch_limits_values(self)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L18)
- uses (calls/refs, reference-scoped): [`BATCH_LIMITS`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#BATCH_LIMITS)

### `TestClampRequests`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L74)
- signature: `class TestClampRequests:`
- members:
  - `test_clamps_when_over_limit_with_truncate(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L81)
  - `test_exact_limit_not_clamped(self)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L94)
  - `test_no_clamping_under_limit(self)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L75)
  - `test_raises_when_over_limit_without_truncate(self)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L88)
- uses (calls/refs, reference-scoped): [`BATCH_LIMITS`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#BATCH_LIMITS), [`_clamp_requests`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#_clamp_requests)

### `TestMakeErrorResult`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L102)
- signature: `class TestMakeErrorResult:`
- members:
  - `test_basic_error_result(self)` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L103)
  - `test_empty_strings(self)` — [`L111`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L111)
  - `test_error_is_dict(self)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L116)
- uses (calls/refs, reference-scoped): [`_make_error_result`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#_make_error_result)

### `TestResolveFile`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L221)
- signature: `class TestResolveFile:`
- members:
  - `test_resolve_file_exact_size_limit(self, tmp_path)` — [`L277`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L277)
  - `test_resolve_file_not_exist_fail_fast(self, tmp_path)` — [`L249`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L249)
  - `test_resolve_file_not_exist_no_fail_fast(self, tmp_path)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L254)
  - `test_resolve_file_too_large_fail_fast(self, tmp_path)` — [`L261`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L261)
  - `test_resolve_file_too_large_no_fail_fast(self, tmp_path)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L268)
  - `test_resolve_os_error_fail_fast(self, tmp_path)` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L285)
  - `test_resolve_os_error_no_fail_fast(self, tmp_path)` — [`L301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L301)
  - `test_resolve_success(self, tmp_path)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L227)
  - `test_resolve_validation_error_fail_fast(self)` — [`L235`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L235)
  - `test_resolve_validation_error_no_fail_fast(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L241)
- protocol/private: `_make_tool`[`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L222)
- uses (calls/refs, reference-scoped): [`BATCH_LIMITS`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#BATCH_LIMITS), [`_resolve_file`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#_resolve_file)

### `TestValidateBatchTopLevel`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L27)
- signature: `class TestValidateBatchTopLevel:`
- members:
  - `test_accepts_empty_requests_list(self)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L69)
  - `test_rejects_dict_requests(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L65)
  - `test_rejects_end_column_with_requests(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L49)
  - `test_rejects_end_line_with_requests(self)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L41)
  - `test_rejects_file_path_with_requests(self)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L33)
  - `test_rejects_non_list_requests(self)` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L61)
  - `test_rejects_output_file_with_requests(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L53)
  - `test_rejects_start_column_with_requests(self)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L45)
  - `test_rejects_start_line_with_requests(self)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L37)
  - `test_rejects_suppress_output_with_requests(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L57)
  - `test_returns_requests_list(self)` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L28)
- uses (calls/refs, reference-scoped): [`_validate_batch_top_level`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#_validate_batch_top_level)

### `TestValidateFileRequest`
- def: [`tests/unit/mcp/tools/test_batch_executor_helpers.py:123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L123)
- signature: `class TestValidateFileRequest:`
- members:
  - `test_empty_file_path_with_fail_fast(self)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L152)
  - `test_missing_file_path_with_fail_fast(self)` — [`L138`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L138)
  - `test_missing_file_path_without_fail_fast(self)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L144)
  - `test_missing_sections_with_fail_fast(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L160)
  - `test_missing_sections_without_fail_fast(self)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L166)
  - `test_non_dict_with_fail_fast(self)` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L124)
  - `test_non_dict_without_fail_fast(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L128)
  - `test_too_many_sections_with_truncate(self)` — [`L195`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L195)
  - `test_too_many_sections_without_truncate_fail_fast(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L185)
  - `test_too_many_sections_without_truncate_no_fail_fast(self)` — [`L208`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L208)
  - `test_valid_request(self)` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_batch_executor_helpers.py#L174)
- uses (calls/refs, reference-scoped): [`BATCH_LIMITS`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#BATCH_LIMITS), [`_validate_file_request`](../../../../tree_sitter_analyzer/mcp/tools/batch_executor.md#_validate_file_request)

