---
title: 'Module: tests/unit/mcp/utils/test_error_sanitizer.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/utils/test_error_sanitizer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.utils.test_error_sanitizer`/Test
symbols:
  TestFileOutputManagerPathTraversal.test_rejects_parent_traversal: FileOutputManagerPathTraversal#test_rejects_parent_traversal().
  TestFileOutputManagerPathTraversal.test_rejects_absolute_path_outside: FileOutputManagerPathTraversal#test_rejects_absolute_path_outside().
  TestFileOutputManagerPathTraversal.test_allows_in_directory_path: FileOutputManagerPathTraversal#test_allows_in_directory_path().
  TestSanitizeMessage.test_empty_string: SanitizeMessage#test_empty_string().
  TestSanitizeMessage.test_no_paths_in_message: SanitizeMessage#test_no_paths_in_message().
  TestSanitizeMessage.test_inside_project_root_becomes_relative: SanitizeMessage#test_inside_project_root_becomes_relative().
  TestSanitizeMessage.test_outside_project_root_is_redacted: SanitizeMessage#test_outside_project_root_is_redacted().
  TestSanitizeMessage.test_no_project_root_redacts_everything: SanitizeMessage#test_no_project_root_redacts_everything().
  TestSanitizeMessage.test_idempotent: SanitizeMessage#test_idempotent().
  TestSanitizeException.test_includes_exception_class_name: SanitizeException#test_includes_exception_class_name().
  TestSanitizeException.test_strips_absolute_path_from_message: SanitizeException#test_strips_absolute_path_from_message().
  TestSanitizeException.test_redacts_external_paths: SanitizeException#test_redacts_external_paths().
  TestSafeErrorMessage.test_safe_error_message_with_class: SafeErrorMessage#test_safe_error_message_with_class().
  TestSafeErrorMessage.test_safe_error_message_without_class: SafeErrorMessage#test_safe_error_message_without_class().
  TestIntegrationWithErrorRecovery.test_build_agent_friendly_error_redacts_paths: IntegrationWithErrorRecovery#test_build_agent_friendly_error_redacts_paths().
  TestSanitizeMessage: SanitizeMessage#
  TestSanitizeException: SanitizeException#
  TestSafeErrorMessage: SafeErrorMessage#
  TestIntegrationWithErrorRecovery: IntegrationWithErrorRecovery#
  TestFileOutputManagerPathTraversal: FileOutputManagerPathTraversal#
---
# Module: [`tests/unit/mcp/utils/test_error_sanitizer.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py)

## Classes
### `TestFileOutputManagerPathTraversal`
- def: [`tests/unit/mcp/utils/test_error_sanitizer.py:116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L116)
- doc: SEC-1: refusing to write outside the configured output directory.
- signature: `class TestFileOutputManagerPathTraversal:`
- members:
  - `test_allows_in_directory_path(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L141)
  - `test_rejects_absolute_path_outside(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L131)
  - `test_rejects_parent_traversal(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L119)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`save_to_file`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.save_to_file)

### `TestIntegrationWithErrorRecovery`
- def: [`tests/unit/mcp/utils/test_error_sanitizer.py:97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L97)
- doc: The error_recovery helper is the central error response builder.
- signature: `class TestIntegrationWithErrorRecovery:`
- members:
  - `test_build_agent_friendly_error_redacts_paths(self, tmp_path: Path)` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L101)
- uses (calls/refs, reference-scoped): [`build_agent_friendly_error`](../../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#build_agent_friendly_error)

### `TestSafeErrorMessage`
- def: [`tests/unit/mcp/utils/test_error_sanitizer.py:79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L79)
- signature: `class TestSafeErrorMessage:`
- members:
  - `test_safe_error_message_with_class(self, tmp_path: Path)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L80)
  - `test_safe_error_message_without_class(self, tmp_path: Path)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L88)
- uses (calls/refs, reference-scoped): [`safe_error_message`](../../../../tree_sitter_analyzer/mcp/utils/error_sanitizer.md#safe_error_message)

### `TestSanitizeException`
- def: [`tests/unit/mcp/utils/test_error_sanitizer.py:51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L51)
- signature: `class TestSanitizeException:`
- members:
  - `test_includes_exception_class_name(self, tmp_path: Path)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L52)
  - `test_redacts_external_paths(self)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L69)
  - `test_strips_absolute_path_from_message(self, tmp_path: Path)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L59)
- uses (calls/refs, reference-scoped): [`sanitize_exception`](../../../../tree_sitter_analyzer/mcp/utils/error_sanitizer.md#sanitize_exception)

### `TestSanitizeMessage`
- def: [`tests/unit/mcp/utils/test_error_sanitizer.py:16`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L16)
- signature: `class TestSanitizeMessage:`
- members:
  - `test_empty_string(self)` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L17)
  - `test_idempotent(self, tmp_path: Path)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L44)
  - `test_inside_project_root_becomes_relative(self, tmp_path: Path)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L23)
  - `test_no_paths_in_message(self)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L20)
  - `test_no_project_root_redacts_everything(self)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L38)
  - `test_outside_project_root_is_redacted(self, tmp_path: Path)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_error_sanitizer.py#L32)
- uses (calls/refs, reference-scoped): [`sanitize_message`](../../../../tree_sitter_analyzer/mcp/utils/error_sanitizer.md#sanitize_message)

