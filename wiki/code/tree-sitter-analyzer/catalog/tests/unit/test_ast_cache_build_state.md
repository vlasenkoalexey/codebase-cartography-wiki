---
title: 'Module: tests/unit/test_ast_cache_build_state.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_build_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_build_state`/
symbols:
  test_full_rebuild_sets_marker_during_empty_window_and_clears_after: test_full_rebuild_sets_marker_during_empty_window_and_clears_after().
  test_status_warns_when_rebuilding_with_partial_index: test_status_warns_when_rebuilding_with_partial_index().
  test_status_distinguishes_rebuild_from_missing_index: test_status_distinguishes_rebuild_from_missing_index().
  test_marker_cleared_when_delete_phase_raises: test_marker_cleared_when_delete_phase_raises().
  test_build_state_helpers_degrade_on_missing_table: test_build_state_helpers_degrade_on_missing_table().
  test_build_state_helpers_degrade_on_readonly_db: test_build_state_helpers_degrade_on_readonly_db().
  test_pid_alive_branches: test_pid_alive_branches().
  test_build_in_progress_is_stale_after_ttl: test_build_in_progress_is_stale_after_ttl().
  test_build_in_progress_stale_when_rebuilder_pid_is_dead: test_build_in_progress_stale_when_rebuilder_pid_is_dead().
  test_build_in_progress_stale_when_timestamp_is_in_the_future: test_build_in_progress_stale_when_timestamp_is_in_the_future().
  _project: _project().
  test_full_rebuild_sets_marker_during_empty_window_and_clears_after._spy_commit: test_full_rebuild_sets_marker_during_empty_window_and_clears_after()._spy_commit().
  test_build_in_progress_false_when_row_absent: test_build_in_progress_false_when_row_absent().
  test_pid_alive_branches._gone: test_pid_alive_branches()._gone().
  test_pid_alive_branches._eperm: test_pid_alive_branches()._eperm().
  test_marker_cleared_when_delete_phase_raises._RaiseOnDelete: test_marker_cleared_when_delete_phase_raises()._RaiseOnDelete#
  test_marker_cleared_when_delete_phase_raises._RaiseOnDelete.execute: test_marker_cleared_when_delete_phase_raises()._RaiseOnDelete#execute().
  test_marker_cleared_when_delete_phase_raises._RaiseOnDelete.__getattr__: test_marker_cleared_when_delete_phase_raises()._RaiseOnDelete#__getattr__().
---
# Module: [`tests/unit/test_ast_cache_build_state.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py)

## Classes
### `_RaiseOnDelete`
- def: [`tests/unit/test_ast_cache_build_state.py:228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L228)
- doc: Proxy that fails the ast_index DELETE but delegates everything else.
- signature: `class _RaiseOnDelete:`
- members:
  - `execute(self, sql, *args, **kwargs)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L231)
- protocol/private: `__getattr__`[`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L236)
- used by: (1 test-only callers)

## Functions
- `_eperm(*a)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L143)
- `_gone(*a)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L137)
- `_project(root: Path)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L166)
- `_spy_commit(conn, *args, **kwargs)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L195)
- `test_build_in_progress_false_when_row_absent()` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L72) — Table present but no id=1 row → not building (don't assume a row).
- `test_build_in_progress_is_stale_after_ttl()` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L88) — A crashed rebuild that never cleared must not wedge readers forever.
- `test_build_in_progress_stale_when_rebuilder_pid_is_dead()` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L112) — Crashed rebuild (pid gone) is stale immediately, before the TTL backstop.
- `test_build_in_progress_stale_when_timestamp_is_in_the_future()` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L150) — A clock that stepped backward (NTP) must not make a marker fresh forever.
- `test_build_state_helpers_degrade_on_missing_table()` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L33) — No ast_build_state table → safe defaults, no raise; mark creates it.
- `test_build_state_helpers_degrade_on_readonly_db(tmp_path: Path)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L53) — Write failures (read-only DB) must be swallowed — the marker never raises.
- `test_full_rebuild_sets_marker_during_empty_window_and_clears_after(tmp_path: Path, monkeypatch)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L173) — force=True must mark building across the DELETE→repopulate window.
- `test_marker_cleared_when_delete_phase_raises(tmp_path: Path, monkeypatch)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L215) — P2 regression: a failure in the DELETE/commit phase must not leak the marker.
- `test_pid_alive_branches(monkeypatch)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L130) — _pid_alive maps os.kill outcomes correctly: gone→False, EPERM→alive.
- `test_status_distinguishes_rebuild_from_missing_index(tmp_path: Path)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L271) — Mid-rebuild empty table must NOT read as 'index missing — run index'.
- `test_status_warns_when_rebuilding_with_partial_index(tmp_path: Path)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_build_state.py#L250) — A nonempty-but-rebuilding cache → status WARN + index_rebuilding flag.

