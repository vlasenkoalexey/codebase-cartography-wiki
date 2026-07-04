---
title: 'Module: tests/unit/test_affected_command.py'
type: catalog
provenance: extracted
module: tests/unit/test_affected_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_affected_command`/Test
symbols:
  TestIsTestPath.test_recognised_test_paths: IsTestPath#test_recognised_test_paths().
  TestIsTestPath.test_non_test_paths_rejected: IsTestPath#test_non_test_paths_rejected().
  TestRunAffected.test_happy_path_with_test_files: RunAffected#test_happy_path_with_test_files().
  TestRunAffected.fake_execute: RunAffected#fake_execute().
  TestRunAffected.test_no_matches_returns_not_found_verdict: RunAffected#test_no_matches_returns_not_found_verdict().
  TestRunAffected.test_quiet_mode_emits_paths_only: RunAffected#test_quiet_mode_emits_paths_only().
  TestRunAffected.test_custom_filter_used: RunAffected#test_custom_filter_used().
  TestRunAffected.test_invalid_files_listed_when_any_succeed: RunAffected#test_invalid_files_listed_when_any_succeed().
  TestIsTestPath.test_custom_filter_overrides_defaults: IsTestPath#test_custom_filter_overrides_defaults().
  TestRunAffected.test_missing_project_root_returns_1: RunAffected#test_missing_project_root_returns_1().
  TestRunAffected.test_no_files_returns_1: RunAffected#test_no_files_returns_1().
  TestRunAffected.test_invalid_files_only_returns_1: RunAffected#test_invalid_files_only_returns_1().
  TestIsTestPath: IsTestPath#
  TestRunAffected: RunAffected#
---
# Module: [`tests/unit/test_affected_command.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py)

## Classes
### `TestIsTestPath`
- def: [`tests/unit/test_affected_command.py:23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L23)
- signature: `class TestIsTestPath:`
- members:
  - `test_custom_filter_overrides_defaults(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L57)
  - `test_non_test_paths_rejected(self, path: str)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L54)
  - `test_recognised_test_paths(self, path: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L40)
- uses (calls/refs, reference-scoped): [`_is_test_path`](../../tree_sitter_analyzer/cli/commands/affected_command.md#_is_test_path), [`_DEFAULT_TEST_GLOBS`](../../tree_sitter_analyzer/cli/commands/affected_command.md#_DEFAULT_TEST_GLOBS._DEFAULT_TEST_GLOBS)

### `TestRunAffected`
- def: [`tests/unit/test_affected_command.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L65)
- doc: End-to-end smoke tests using a mocked DependencyAnalysisTool.
- signature: `class TestRunAffected:`
- members:
  - `fake_execute(self, args)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L105)
  - `test_custom_filter_used(self, tmp_path, capsys)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L194)
  - `test_happy_path_with_test_files(self, tmp_path, capsys)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L100)
  - `test_invalid_files_listed_when_any_succeed(self, tmp_path, capsys)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L226)
  - `test_invalid_files_only_returns_1(self, tmp_path, capsys)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L90)
  - `test_missing_project_root_returns_1(self, tmp_path, capsys)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L73)
  - `test_no_files_returns_1(self, tmp_path, capsys)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L83)
  - `test_no_matches_returns_not_found_verdict(self, tmp_path, capsys)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L139)
  - `test_quiet_mode_emits_paths_only(self, tmp_path, capsys)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_affected_command.py#L162)
- uses (calls/refs, reference-scoped): [`run_affected`](../../tree_sitter_analyzer/cli/commands/affected_command.md#run_affected)

