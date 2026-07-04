---
title: 'Module: tests/unit/test_health_score_cache.py'
type: catalog
provenance: extracted
module: tests/unit/test_health_score_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_health_score_cache`/
symbols:
  test_cache_handles_broken_db_path: test_cache_handles_broken_db_path().
  test_cache_roundtrip: test_cache_roundtrip().
  test_invalidate_removes_entry: test_invalidate_removes_entry().
  test_cache_misses_on_mtime_change: test_cache_misses_on_mtime_change().
  test_cache_misses_on_missing_file: test_cache_misses_on_missing_file().
  test_score_project_warm_run_is_fast: test_score_project_warm_run_is_fast().
  test_score_project_use_cache_false_still_works: test_score_project_use_cache_false_still_works().
  project: project().
---
# Module: [`tests/unit/test_health_score_cache.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py)

## Functions
- `project(tmp_path)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L21)
- `test_cache_handles_broken_db_path(tmp_path)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L114) — When the cache DB cannot be opened, scoring still proceeds.
- `test_cache_misses_on_missing_file(project, tmp_path)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L60)
- `test_cache_misses_on_mtime_change(project)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L46)
- `test_cache_roundtrip(project)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L29)
- `test_invalidate_removes_entry(project)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L70)
- `test_score_project_use_cache_false_still_works(project)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L106) — ``use_cache=False`` is a valid opt-out and must produce same results.
- `test_score_project_warm_run_is_fast(project)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_score_cache.py#L80) — The warm run MUST be substantially faster than the cold run.

