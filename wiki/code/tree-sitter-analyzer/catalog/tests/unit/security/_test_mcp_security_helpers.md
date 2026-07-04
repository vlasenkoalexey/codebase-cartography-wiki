---
title: 'Module: tests/unit/security/_test_mcp_security_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/security/_test_mcp_security_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security._test_mcp_security_helpers`/
symbols:
  assert_stack_trace_filtering: assert_stack_trace_filtering().
  assert_error_message_sanitization: assert_error_message_sanitization().
  assert_symlink_read_blocked: assert_symlink_read_blocked().
  assert_external_path_blocked_or_temp_allowed: assert_external_path_blocked_or_temp_allowed().
  assert_absolute_path_restricted: assert_absolute_path_restricted().
  EXPECTED_PATH_REJECTION_EXCEPTIONS: EXPECTED_PATH_REJECTION_EXCEPTIONS.
  assert_symlink_traversal_prevention: assert_symlink_traversal_prevention().
  assert_file_content_filtering: assert_file_content_filtering().
  assert_directory_path_rejected: assert_directory_path_rejected().
  assert_query_path_rejected: assert_query_path_rejected().
  ABSOLUTE_SECRET_PATH: ABSOLUTE_SECRET_PATH.
  assert_directory_paths_rejected: assert_directory_paths_rejected().
  assert_absolute_paths_restricted: assert_absolute_paths_restricted().
  assert_query_paths_rejected: assert_query_paths_rejected().
  assert_project_root_enforcement: assert_project_root_enforcement().
  assert_symlink_error_message: assert_symlink_error_message().
  ERROR_SENSITIVE_PATTERNS: ERROR_SENSITIVE_PATTERNS.
  STACK_TRACE_SENSITIVE_PATHS: STACK_TRACE_SENSITIVE_PATHS.
  create_symlink_traversal_fixture: create_symlink_traversal_fixture().
  mocked_is_symlink_for: mocked_is_symlink_for().
  assert_no_sensitive_patterns: assert_no_sensitive_patterns().
  SYMLINK_ERROR_TERMS: SYMLINK_ERROR_TERMS.
  try_create_symlink: try_create_symlink().
  mocked_is_symlink_for.mock_is_symlink: mocked_is_symlink_for().mock_is_symlink().
  result_indicates_security_block: result_indicates_security_block().
  path_is_allowed_temp: path_is_allowed_temp().
  build_sensitive_sample_content: build_sensitive_sample_content().
---
# Module: [`tests/unit/security/_test_mcp_security_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py)

## Functions
- `assert_absolute_path_restricted(tool: ListFilesTool, abs_path: str)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L76) — Assert one absolute root is rejected.
- `assert_absolute_paths_restricted(absolute_paths: list[str])` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L69) — Assert absolute roots are rejected by list-files.
- `assert_directory_path_rejected(tool: ListFilesTool, malicious_path: str)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L54) — Assert one malicious directory root is rejected.
- `assert_directory_paths_rejected(malicious_paths: list[str])` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L47) — Assert list-files rejects malicious directory roots.
- `assert_error_message_sanitization()` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L232) — Assert absolute-path failures do not leak sensitive details.
- `assert_external_path_blocked_or_temp_allowed(tool: FindAndGrepTool, external_path: str)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L201) — Assert an external root is blocked unless it is an allowed temp path.
- `assert_file_content_filtering(tmp_path: Path)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L289) — Assert sensitive-looking files can be read without logging checks here.
- `assert_no_sensitive_patterns(text: str, patterns: Any, failure_prefix: str)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L282) — Assert none of the sensitive patterns appear in text.
- `assert_project_root_enforcement(safe_project_structure: str)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L186) — Assert external project roots are rejected or safely ignored.
- `assert_query_path_rejected(tool: QueryTool, malicious_path: str)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L96) — Assert one malicious query file path is rejected.
- `assert_query_paths_rejected(malicious_paths: list[str])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L89) — Assert query tool rejects malicious file paths.
- `assert_stack_trace_filtering()` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L254) — Assert absolute-path failures do not expose stack trace details. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- `assert_symlink_error_message(message: str)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L178) — Assert a symlink block mentions link-related security context.
- `assert_symlink_read_blocked(symlink_path: Path)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L155) — Assert ReadPartialTool rejects a symlink path.
- `assert_symlink_traversal_prevention(tmp_path: Path)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L111) — Assert that real or mocked symlink traversal is blocked.
- `build_sensitive_sample_content()` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L307) — Build scanner fixture content without literal credentials.
- `create_symlink_traversal_fixture(tmp_path: Path)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L123) — Create a project, external secret, and symlink path for traversal tests.
- `mock_is_symlink(self: Path)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L149)
- `mocked_is_symlink_for(symlink_path: Path)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L146) — Return a Path.is_symlink replacement for the fallback branch.
- `path_is_allowed_temp(path: str)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L224) — Return whether a path is an allowed temporary directory for this test.
- `result_indicates_security_block(result: Any)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L173) — Return whether a tool result indicates the symlink was blocked.
- `try_create_symlink(symlink_path: Path, target: Path)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L137) — Try to create a symlink, returning whether the OS allowed it.

## Module values
- `ABSOLUTE_SECRET_PATH` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L19)
- `ERROR_SENSITIVE_PATTERNS` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L20)
- `EXPECTED_PATH_REJECTION_EXCEPTIONS` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L38)
- `STACK_TRACE_SENSITIVE_PATHS` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L30)
- `SYMLINK_ERROR_TERMS` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/_test_mcp_security_helpers.py#L18)

