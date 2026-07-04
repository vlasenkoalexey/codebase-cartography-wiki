---
title: 'Module: tests/unit/test_no_project_root_traps.py'
type: catalog
provenance: extracted
module: tests/unit/test_no_project_root_traps.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_no_project_root_traps`/
symbols:
  _collect_violations: _collect_violations().
  test_no_project_root_eq_tmp_in_tests: test_no_project_root_eq_tmp_in_tests().
  test_no_project_root_eq_none_in_tests: test_no_project_root_eq_none_in_tests().
  _iter_test_files: _iter_test_files().
  _TESTS_DIR: _TESTS_DIR.
  _REPO_ROOT: _REPO_ROOT.
  _TMP_PATTERN: _TMP_PATTERN.
  _NONE_PATTERN: _NONE_PATTERN.
  _GRAPH_BUILDERS_NEAR_NONE: _GRAPH_BUILDERS_NEAR_NONE.
---
# Module: [`tests/unit/test_no_project_root_traps.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py)

## Functions
- `_collect_violations(pattern: re.Pattern, allowed_comment: str, skip_conftest: bool = False, extra_skip_words: tuple[str, ...] = ())` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L75) — Return a list of ``file:line: text`` strings for pattern violations.
- `_iter_test_files()` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L71)
- `test_no_project_root_eq_none_in_tests()` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L145) — Banner: ``project_root=None`` in graph-building tools silently uses cwd.
- `test_no_project_root_eq_tmp_in_tests()` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L111) — Banner: ``project_root='/tmp'`` inside tests/ is a perf trap.

## Module values
- `_GRAPH_BUILDERS_NEAR_NONE` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L59)
- `_NONE_PATTERN` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L50)
- `_REPO_ROOT` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L41)
- `_TESTS_DIR` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L42)
- `_TMP_PATTERN` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_no_project_root_traps.py#L46)

