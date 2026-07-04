---
title: 'Module: tests/unit/test_auto_index_guard_convergence.py'
type: catalog
provenance: extracted
module: tests/unit/test_auto_index_guard_convergence.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_auto_index_guard_convergence`/
symbols:
  test_ensure_indexed_resolves_when_not_converged: test_ensure_indexed_resolves_when_not_converged().
  test_ensure_indexed_does_not_mark_converged_on_resolve_failure: test_ensure_indexed_does_not_mark_converged_on_resolve_failure().
  test_index_project_marks_resolution_converged: test_index_project_marks_resolution_converged().
  test_converged_false_after_a_file_is_reindexed: test_converged_false_after_a_file_is_reindexed().
  test_ensure_indexed_skips_resolve_when_converged: test_ensure_indexed_skips_resolve_when_converged().
  test_resolution_converged_helpers_degrade_on_broken_cache: test_resolution_converged_helpers_degrade_on_broken_cache().
  test_resolution_helpers_degrade_on_missing_tables: test_resolution_helpers_degrade_on_missing_tables().
  _project: _project().
  test_resolution_converged_helpers_degrade_on_broken_cache.BrokenCache: test_resolution_converged_helpers_degrade_on_broken_cache().BrokenCache#
  test_resolution_converged_false_when_state_table_empty: test_resolution_converged_false_when_state_table_empty().
  test_mark_resolution_converged_handles_operational_error: test_mark_resolution_converged_handles_operational_error().
  test_ensure_indexed_skips_resolve_when_converged.spy: test_ensure_indexed_skips_resolve_when_converged().spy().
  test_ensure_indexed_resolves_when_not_converged.spy: test_ensure_indexed_resolves_when_not_converged().spy().
  test_ensure_indexed_does_not_mark_converged_on_resolve_failure.broken_index_project: test_ensure_indexed_does_not_mark_converged_on_resolve_failure().broken_index_project().
  test_resolution_converged_helpers_degrade_on_broken_cache.BrokenCache.get_conn: test_resolution_converged_helpers_degrade_on_broken_cache().BrokenCache#get_conn().
---
# Module: [`tests/unit/test_auto_index_guard_convergence.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py)

## Classes
### `BrokenCache`
- def: [`tests/unit/test_auto_index_guard_convergence.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L197)
- signature: `class BrokenCache:`
- members:
  - `get_conn(self)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L198)
- used by: (1 test-only callers)

## Functions
- `_project(root: Path)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L51)
- `broken_index_project(self: Any, *args: Any, **kwargs: Any)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L221)
- `spy(self: Any, *args: Any, **kwargs: Any)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L107)
- `spy(self: Any, *args: Any, **kwargs: Any)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L141)
- `test_converged_false_after_a_file_is_reindexed(tmp_path: Path)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L75)
- `test_ensure_indexed_does_not_mark_converged_on_resolve_failure(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L206) — If _resolve_pending_unresolved_refs fails, convergence must NOT be persisted.
- `test_ensure_indexed_resolves_when_not_converged(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L122)
- `test_ensure_indexed_skips_resolve_when_converged(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L93)
- `test_index_project_marks_resolution_converged(tmp_path: Path)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L63)
- `test_mark_resolution_converged_handles_operational_error(tmp_path: Path)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L173) — Read-only connection → mark_resolution_converged hits OperationalError handler without raising.
- `test_resolution_converged_false_when_state_table_empty()` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L156) — ast_resolve_state exists but has no rows → resolution_converged returns False (row is None).
- `test_resolution_converged_helpers_degrade_on_broken_cache()` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L189) — _resolution_converged/_mark_resolution_converged swallow exceptions from a broken cache.
- `test_resolution_helpers_degrade_on_missing_tables()` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_auto_index_guard_convergence.py#L28) — No ast_index / ast_resolve_state → helpers return safe defaults, no raise.

