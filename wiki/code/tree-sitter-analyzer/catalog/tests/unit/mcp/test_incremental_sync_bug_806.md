---
title: 'Module: tests/unit/mcp/test_incremental_sync_bug_806.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_incremental_sync_bug_806.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_incremental_sync_bug_806`/
symbols:
  _make_sync_result_with_one_error: _make_sync_result_with_one_error().
  TestMCPResponseEnvelopeOnPerFileError.test_response_success_true_when_partial_success: TestMCPResponseEnvelopeOnPerFileError#test_response_success_true_when_partial_success().
  TestMCPResponseEnvelopeOnPerFileError.test_response_contains_error_count: TestMCPResponseEnvelopeOnPerFileError#test_response_contains_error_count().
  TestMCPResponseEnvelopeOnPerFileError.test_response_details_include_failing_file_path: TestMCPResponseEnvelopeOnPerFileError#test_response_details_include_failing_file_path().
  TestMCPResponseEnvelopeOnPerFileError.test_response_error_detail_has_exception_type: TestMCPResponseEnvelopeOnPerFileError#test_response_error_detail_has_exception_type().
  TestMCPResponseEnvelopeOnPerFileError.test_response_error_detail_has_error_message: TestMCPResponseEnvelopeOnPerFileError#test_response_error_detail_has_error_message().
  TestMCPResponseEnvelopeOnPerFileError.test_sibling_files_still_indexed_after_per_file_error: TestMCPResponseEnvelopeOnPerFileError#test_sibling_files_still_indexed_after_per_file_error().
  TestMCPResponseEnvelopeOnPerFileError.test_response_includes_scanned_count: TestMCPResponseEnvelopeOnPerFileError#test_response_includes_scanned_count().
  TestMCPResponseEnvelopeOnPerFileErrorToon.test_toon_response_toon_content_contains_error_path: TestMCPResponseEnvelopeOnPerFileErrorToon#test_toon_response_toon_content_contains_error_path().
  TestMCPResponseEnvelopeOnPerFileErrorToon.test_toon_response_errors_field_surfaced: TestMCPResponseEnvelopeOnPerFileErrorToon#test_toon_response_errors_field_surfaced().
  mcp_tool: mcp_tool().
  TestMCPOuterExceptionSurface.test_outer_exception_returns_error_envelope: TestMCPOuterExceptionSurface#test_outer_exception_returns_error_envelope().
  TestMCPOuterExceptionSurface.test_outer_exception_error_message_includes_exception_type: TestMCPOuterExceptionSurface#test_outer_exception_error_message_includes_exception_type().
  project: project().
  TestMCPResponseEnvelopeOnPerFileError: TestMCPResponseEnvelopeOnPerFileError#
  TestMCPOuterExceptionSurface: TestMCPOuterExceptionSurface#
  TestMCPResponseEnvelopeOnPerFileErrorToon: TestMCPResponseEnvelopeOnPerFileErrorToon#
---
# Module: [`tests/unit/mcp/test_incremental_sync_bug_806.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py)

## Classes
### `TestMCPOuterExceptionSurface`
- def: [`tests/unit/mcp/test_incremental_sync_bug_806.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L194)
- doc: Outer sync.sync() exception must surface as error envelope, not be swallowed.
- signature: `class TestMCPOuterExceptionSurface:`
- members:
  - `test_outer_exception_error_message_includes_exception_type(self, mcp_tool, project)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L210) — Error message must name the exception type (not just a bare message).
  - `test_outer_exception_returns_error_envelope(self, mcp_tool, project)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L197) — If sync.sync() itself raises (not per-file), MCP layer returns error.
- uses (calls/refs, reference-scoped): [`IncrementalSync`](../../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync)

### `TestMCPResponseEnvelopeOnPerFileError`
- def: [`tests/unit/mcp/test_incremental_sync_bug_806.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L87)
- doc: Issue #806: MCP _sync() response must surface per-file errors.
- signature: `class TestMCPResponseEnvelopeOnPerFileError:`
- members:
  - `test_response_contains_error_count(self, mcp_tool, project)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L102) — errors field in response must equal exactly 1 (one file failed).
  - `test_response_details_include_failing_file_path(self, mcp_tool, project)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L114) — details list must include the file that raised RecursionError.
  - `test_response_error_detail_has_error_message(self, mcp_tool, project)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L144) — Error detail must carry the exception message (Issue #806).
  - `test_response_error_detail_has_exception_type(self, mcp_tool, project)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L130) — Error detail must carry error_type=RecursionError (Issue #806).
  - `test_response_includes_scanned_count(self, mcp_tool, project)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L175) — scanned field must report total files examined (for partial-success context).
  - `test_response_success_true_when_partial_success(self, mcp_tool, project)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L90) — success=True when some files indexed; one file errored (partial success).
  - `test_sibling_files_still_indexed_after_per_file_error(self, mcp_tool, project)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L160) — good_a.py and good_b.py must be indexed despite pathological.py error.
- uses (calls/refs, reference-scoped): [`IncrementalSync`](../../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync)  (1 test-only)

### `TestMCPResponseEnvelopeOnPerFileErrorToon`
- def: [`tests/unit/mcp/test_incremental_sync_bug_806.py:233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L233)
- doc: Issue #806: per-file error detail must be visible in the default TOON path.
- signature: `class TestMCPResponseEnvelopeOnPerFileErrorToon:`
- members:
  - `test_toon_response_errors_field_surfaced(self, mcp_tool, project)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L252) — errors=1 must be present in the TOON envelope (not stripped).
  - `test_toon_response_toon_content_contains_error_path(self, mcp_tool, project)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L236) — Default TOON format must preserve the failing file path in toon_content.
- uses (calls/refs, reference-scoped): [`IncrementalSync`](../../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync)  (1 test-only)

## Functions
- `_make_sync_result_with_one_error()` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L46) — SyncResult representing 2 successes + 1 RecursionError.
- `mcp_tool(project)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L42)
- `project(tmp_path)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_incremental_sync_bug_806.py#L32)

