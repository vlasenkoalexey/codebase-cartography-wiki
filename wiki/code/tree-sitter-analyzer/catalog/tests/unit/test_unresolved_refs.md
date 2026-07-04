---
title: 'Module: tests/unit/test_unresolved_refs.py'
type: catalog
provenance: extracted
module: tests/unit/test_unresolved_refs.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_unresolved_refs`/
symbols:
  test_pending_refs_and_helper_branches: test_pending_refs_and_helper_branches().
  test_index_project_resolves_cross_file_extends_and_calls: test_index_project_resolves_cross_file_extends_and_calls().
  test_resolve_only_does_not_reparse: test_resolve_only_does_not_reparse().
  test_resolve_unresolved_refs_sqlite_error_paths_are_nonfatal: test_resolve_unresolved_refs_sqlite_error_paths_are_nonfatal().
  test_autoindex_resolves_pending_refs_when_cache_is_already_warm: test_autoindex_resolves_pending_refs_when_cache_is_already_warm().
  test_orchestration_error_paths: test_orchestration_error_paths().
  test_unknown_parent_stays_unresolved: test_unknown_parent_stays_unresolved().
  test_class_hierarchy_cli_reads_resolved_cross_file_edge: test_class_hierarchy_cli_reads_resolved_cross_file_edge().
  test_call_does_not_bind_across_languages: test_call_does_not_bind_across_languages().
  test_non_python_skips_second_pass_refs: test_non_python_skips_second_pass_refs().
  _pending_extends: _pending_extends().
  _rows: _rows().
  test_choose_candidate_prefers_source_over_test_shadow: test_choose_candidate_prefers_source_over_test_shadow().
  test_choose_candidate_allows_test_target_for_test_caller: test_choose_candidate_allows_test_target_for_test_caller().
  test_resolve_unresolved_refs_row_and_commit_error_paths: test_resolve_unresolved_refs_row_and_commit_error_paths().
  _write_project: _write_project().
  test_resolve_unresolved_refs_row_and_commit_error_paths.CommitFails.execute: test_resolve_unresolved_refs_row_and_commit_error_paths().CommitFails#execute().
  _choose_candidate_conn: _choose_candidate_conn().
  test_resolve_unresolved_refs_row_and_commit_error_paths.EmptyRows: test_resolve_unresolved_refs_row_and_commit_error_paths().EmptyRows#
  test_resolve_only_does_not_reparse.counting_parse: test_resolve_only_does_not_reparse().counting_parse().
  test_resolve_unresolved_refs_row_and_commit_error_paths.CommitFails: test_resolve_unresolved_refs_row_and_commit_error_paths().CommitFails#
  test_orchestration_error_paths.fail_unresolved: test_orchestration_error_paths().fail_unresolved().
  test_orchestration_error_paths.BrokenCache: test_orchestration_error_paths().BrokenCache#
  test_resolve_unresolved_refs_row_and_commit_error_paths.EmptyRows.fetchall: test_resolve_unresolved_refs_row_and_commit_error_paths().EmptyRows#fetchall().
  test_resolve_unresolved_refs_row_and_commit_error_paths.CommitFails.commit: test_resolve_unresolved_refs_row_and_commit_error_paths().CommitFails#commit().
  test_orchestration_error_paths.BrokenCache.get_conn: test_orchestration_error_paths().BrokenCache#get_conn().
---
# Module: [`tests/unit/test_unresolved_refs.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py)

## Classes
### `BrokenCache`
- def: [`tests/unit/test_unresolved_refs.py:693`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L693)
- signature: `class BrokenCache:`
- members:
  - `get_conn(self)` — [`L694`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L694)
- used by: (1 test-only callers)

### `CommitFails`
- def: [`tests/unit/test_unresolved_refs.py:506`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L506)
- signature: `class CommitFails:`
- members:
  - `commit(self)` — [`L510`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L510)
  - `execute(self, *_args: Any, **_kwargs: Any)` — [`L507`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L507)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `EmptyRows`
- def: [`tests/unit/test_unresolved_refs.py:502`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L502)
- signature: `class EmptyRows:`
- members:
  - `fetchall(self)` — [`L503`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L503)
- used by: (1 test-only callers)

## Functions
- `_choose_candidate_conn()` — [`L339`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L339) — Minimal conn for ``_choose_candidate`` (ast_index + ast_imports only).
- `_pending_extends(cache: ASTCache)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L75) — EXTENDS edges still pointing at an unresolved ``class:`` synthetic node.
- `_rows(cache: ASTCache, sql: str, params: tuple[Any, ...] = ())` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L69)
- `_write_project(root: Path)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L31)
- `counting_parse(self: Any, *args: Any, **kwargs: Any)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L181)
- `fail_unresolved()` — [`L672`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L672)
- `test_autoindex_resolves_pending_refs_when_cache_is_already_warm(tmp_path: Path)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L231)
- `test_call_does_not_bind_across_languages(tmp_path: Path)` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L304) — A Python call must not resolve to a same-named symbol in another language.
- `test_choose_candidate_allows_test_target_for_test_caller()` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L399) — A test caller may still bind to a test definition (no demotion).
- `test_choose_candidate_prefers_source_over_test_shadow()` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L357) — A non-test caller must bind to the source def, not the test mock.
- `test_class_hierarchy_cli_reads_resolved_cross_file_edge(tmp_path: Path)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L269)
- `test_index_project_resolves_cross_file_extends_and_calls(tmp_path: Path)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L86) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- `test_non_python_skips_second_pass_refs()` — [`L521`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L521) — A2/B1.3: non-Python languages emit no second-pass refs.
- `test_orchestration_error_paths(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L663`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L663)
- `test_pending_refs_and_helper_branches()` — [`L551`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L551)
- `test_resolve_only_does_not_reparse(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L161) — A warm cache resolves pending cross-file refs without re-parsing. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- `test_resolve_unresolved_refs_row_and_commit_error_paths()` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L450) — A resolvable ref whose UPDATE/upsert fails counts as an error, not a crash.
- `test_resolve_unresolved_refs_sqlite_error_paths_are_nonfatal()` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L425) — Missing schema / broken connections must degrade, not crash.
- `test_unknown_parent_stays_unresolved(tmp_path: Path)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs.py#L206)

