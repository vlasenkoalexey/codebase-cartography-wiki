---
title: 'Module: tests/unit/runtime/test_autonomous_status_script.py'
type: catalog
provenance: extracted
module: tests/unit/runtime/test_autonomous_status_script.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.runtime.test_autonomous_status_script`/
symbols:
  run_status: run_status().
  make_runtime_project: make_runtime_project().
  test_status_json_reports_recent_heartbeat_and_pending_changes: test_status_json_reports_recent_heartbeat_and_pending_changes().
  test_status_json_reports_stopped_when_heartbeat_is_stale: test_status_json_reports_stopped_when_heartbeat_is_stale().
  test_status_text_includes_heartbeat_section: test_status_text_includes_heartbeat_section().
  test_tick_writes_machine_readable_state: test_tick_writes_machine_readable_state().
  test_tick_reuses_existing_loop_lock: test_tick_reuses_existing_loop_lock().
  run_tick: run_tick().
  STATUS_SCRIPT: STATUS_SCRIPT.
  TICK_SCRIPT: TICK_SCRIPT.
  PROJECT_ROOT: PROJECT_ROOT.
---
# Module: [`tests/unit/runtime/test_autonomous_status_script.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py)

## Functions
- `make_runtime_project(tmp_path: Path)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L48)
- `run_status(project_dir: Path, *args: str, env: dict[str, str] | None = None)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L18)
- `run_tick(project_dir: Path, env: dict[str, str] | None = None)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L33)
- `test_status_json_reports_recent_heartbeat_and_pending_changes(tmp_path: Path)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L97)
- `test_status_json_reports_stopped_when_heartbeat_is_stale(tmp_path: Path)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L115)
- `test_status_text_includes_heartbeat_section(tmp_path: Path)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L135)
- `test_tick_reuses_existing_loop_lock(tmp_path: Path)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L172)
- `test_tick_writes_machine_readable_state(tmp_path: Path)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L148)

## Module values
- `PROJECT_ROOT` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L13)
- `STATUS_SCRIPT` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L14)
- `TICK_SCRIPT` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/runtime/test_autonomous_status_script.py#L15)

