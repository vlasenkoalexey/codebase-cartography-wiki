---
title: 'Module: tests/unit/cli/test_clean_state_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_clean_state_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_clean_state_command`/
symbols:
  test_absent_paths_are_reported_skipped: test_absent_paths_are_reported_skipped().
  test_removes_present_file: test_removes_present_file().
  test_removes_present_directory: test_removes_present_directory().
  test_dry_run_does_not_touch_filesystem: test_dry_run_does_not_touch_filesystem().
  test_handles_literal_colon_memory_directory: test_handles_literal_colon_memory_directory().
  test_clean_state_preserves_foreign_dbs_deletes_tsa_artifact: test_clean_state_preserves_foreign_dbs_deletes_tsa_artifact().
  test_format_json_emits_structured_envelope: test_format_json_emits_structured_envelope().
  _args: _args().
  _capture_errors: _capture_errors().
  test_returns_failure_when_project_root_invalid: test_returns_failure_when_project_root_invalid().
  test_allowlist_excludes_foreign_ruflo_artifacts: test_allowlist_excludes_foreign_ruflo_artifacts().
  test_returns_failure_when_project_root_invalid.boom: test_returns_failure_when_project_root_invalid().boom().
---
# Module: [`tests/unit/cli/test_clean_state_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py)

## Functions
- `_args(project_root: Path, **overrides: object)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L18)
- `_capture_errors()` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L28)
- `boom(_self: object)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L119)
- `test_absent_paths_are_reported_skipped(tmp_path: Path, capsys)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L63) — When nothing exists each path should yield a ``skipped`` line.
- `test_allowlist_excludes_foreign_ruflo_artifacts()` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L139) — The ephemeral allowlist must never contain Ruflo-owned databases (#988).
- `test_clean_state_preserves_foreign_dbs_deletes_tsa_artifact(tmp_path: Path)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L145) — Critical regression guard (#988).
- `test_dry_run_does_not_touch_filesystem(tmp_path: Path, capsys)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L74) — ``--clean-state-dry-run`` reports actions but doesn't delete anything.
- `test_format_json_emits_structured_envelope(tmp_path: Path, capsys)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L178) — ``--format json`` must emit a parseable JSON envelope (#988).
- `test_handles_literal_colon_memory_directory(tmp_path: Path, capsys)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L100) — The literal ``:memory:`` directory created by legacy code is swept.
- `test_removes_present_directory(tmp_path: Path, capsys)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L47) — A present directory should be removed recursively.
- `test_removes_present_file(tmp_path: Path, capsys)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L32) — A present TSA-owned file should be unlinked and reported as ``removed``.
- `test_returns_failure_when_project_root_invalid(monkeypatch)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_clean_state_command.py#L115) — A resolution error on the project root surfaces as exit 1.

