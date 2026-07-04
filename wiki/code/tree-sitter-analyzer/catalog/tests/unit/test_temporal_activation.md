---
title: 'Module: tests/unit/test_temporal_activation.py'
type: catalog
provenance: extracted
module: tests/unit/test_temporal_activation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_temporal_activation`/
symbols:
  _import_git_activation: _import_git_activation().
  _index_with_activation: _index_with_activation().
  TestSymbolAttribution.test_symbol_attribution_overlaps_hunk_line_range: TestSymbolAttribution#test_symbol_attribution_overlaps_hunk_line_range().
  TestColdStart.test_shallow_clone_marker: TestColdStart#test_shallow_clone_marker().
  TestReindexIdempotence.test_reindex_replaces_activation: TestReindexIdempotence#test_reindex_replaces_activation().
  _run_git: _run_git().
  _seven_line_function: _seven_line_function().
  TestSymbolAttribution.test_follow_tracks_renamed_file: TestSymbolAttribution#test_follow_tracks_renamed_file().
  TestWindowing.test_30d_window_excludes_old_commits: TestWindowing#test_30d_window_excludes_old_commits().
  TestColdStart.test_cold_start_no_git_history: TestColdStart#test_cold_start_no_git_history().
  TestEnvDisable.test_index_disabled_via_env: TestEnvDisable#test_index_disabled_via_env().
  TestModuleSurface.test_activation_row_has_required_fields: TestModuleSurface#test_activation_row_has_required_fields().
  _init_git_repo: _init_git_repo().
  _sym: _sym().
  TestDetectGitState.test_shallow_clone_returns_shallow: TestDetectGitState#test_shallow_clone_returns_shallow().
  TestColdStart.test_file_not_in_repo: TestColdStart#test_file_not_in_repo().
  test_perf_indexing_budget_smoke: test_perf_indexing_budget_smoke().
  TestDetectGitState.test_tracked_file_returns_tracked: TestDetectGitState#test_tracked_file_returns_tracked().
  TestDetectGitState.test_untracked_file_returns_untracked: TestDetectGitState#test_untracked_file_returns_untracked().
  TestDetectGitState.test_no_repo_returns_no_repo: TestDetectGitState#test_no_repo_returns_no_repo().
  TestParseLogHunks.test_parses_single_commit_single_hunk: TestParseLogHunks#test_parses_single_commit_single_hunk().
  TestParseLogHunks.test_parses_multiple_commits: TestParseLogHunks#test_parses_multiple_commits().
  TestParseLogHunks.test_zero_length_hunk_is_ignored: TestParseLogHunks#test_zero_length_hunk_is_ignored().
  TestParseLogHunks.test_empty_input_returns_empty: TestParseLogHunks#test_empty_input_returns_empty().
  TestModuleSurface.test_exports_compute_symbol_activation: TestModuleSurface#test_exports_compute_symbol_activation().
  TestModuleSurface.test_exports_detect_git_state: TestModuleSurface#test_exports_detect_git_state().
  TestModuleSurface.test_exports_parse_log_hunks: TestModuleSurface#test_exports_parse_log_hunks().
  test_fixture_does_not_pollute_global_git_config: test_fixture_does_not_pollute_global_git_config().
  _GIT_TIMEOUT_SECONDS: _GIT_TIMEOUT_SECONDS.
  _read_activation_rows: _read_activation_rows().
  _git_env: _git_env().
  TestDetectGitState: TestDetectGitState#
  TestParseLogHunks: TestParseLogHunks#
  TestSymbolAttribution: TestSymbolAttribution#
  TestWindowing: TestWindowing#
  TestColdStart: TestColdStart#
  TestReindexIdempotence: TestReindexIdempotence#
  TestEnvDisable: TestEnvDisable#
  TestModuleSurface: TestModuleSurface#
---
# Module: [`tests/unit/test_temporal_activation.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py)

## Classes
### `TestColdStart`
- def: [`tests/unit/test_temporal_activation.py:289`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L289)
- signature: `class TestColdStart:`
- members:
  - `test_cold_start_no_git_history(self, tmp_path, monkeypatch)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L290) — Fresh ``git init`` with no commits: counts all zero, no exception.
  - `test_file_not_in_repo(self, tmp_path, monkeypatch)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L308) — Outside any git dir: git_state='no_repo', zero counts, row exists.
  - `test_shallow_clone_marker(self, tmp_path, monkeypatch)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L324) — ``.git/shallow`` marker → git_state='shallow'.
- uses (calls/refs, reference-scoped): (6 test-only callers)

### `TestDetectGitState`
- def: [`tests/unit/test_temporal_activation.py:125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L125)
- signature: `class TestDetectGitState:`
- members:
  - `test_no_repo_returns_no_repo(self, tmp_path)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L142)
  - `test_shallow_clone_returns_shallow(self, tmp_path)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L148)
  - `test_tracked_file_returns_tracked(self, tmp_path)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L126)
  - `test_untracked_file_returns_untracked(self, tmp_path)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L133)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestEnvDisable`
- def: [`tests/unit/test_temporal_activation.py:373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L373)
- signature: `class TestEnvDisable:`
- members:
  - `test_index_disabled_via_env(self, tmp_path, monkeypatch)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L374) — ``TSA_INDEX_ACTIVATION=0`` skips writes AND skips git subprocess.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestModuleSurface`
- def: [`tests/unit/test_temporal_activation.py:440`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L440)
- signature: `class TestModuleSurface:`
- members:
  - `test_activation_row_has_required_fields(self, tmp_path, monkeypatch)` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L453) — ActivationRow exposes every column the SQLite table needs.
  - `test_exports_compute_symbol_activation(self)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L441)
  - `test_exports_detect_git_state(self)` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L445)
  - `test_exports_parse_log_hunks(self)` — [`L449`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L449)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestParseLogHunks`
- def: [`tests/unit/test_temporal_activation.py:158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L158)
- signature: `class TestParseLogHunks:`
- members:
  - `test_empty_input_returns_empty(self)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L198)
  - `test_parses_multiple_commits(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L179)
  - `test_parses_single_commit_single_hunk(self)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L159)
  - `test_zero_length_hunk_is_ignored(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L190) — ``@@ -1,1 +1,0 @@`` (pure deletion) yields no addition hunks.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestReindexIdempotence`
- def: [`tests/unit/test_temporal_activation.py:341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L341)
- signature: `class TestReindexIdempotence:`
- members:
  - `test_reindex_replaces_activation(self, tmp_path, monkeypatch)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L342) — Re-indexing leaves a single row per symbol with refreshed counts.
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestSymbolAttribution`
- def: [`tests/unit/test_temporal_activation.py:206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L206)
- signature: `class TestSymbolAttribution:`
- members:
  - `test_follow_tracks_renamed_file(self, tmp_path, monkeypatch)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L236) — ``--follow`` semantics: renamed file's history carries forward.
  - `test_symbol_attribution_overlaps_hunk_line_range(self, tmp_path, monkeypatch)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L207) — Commit modifying lines ~10-15 hits the symbol at 5-25, not 30-40.
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestWindowing`
- def: [`tests/unit/test_temporal_activation.py:261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L261)
- signature: `class TestWindowing:`
- members:
  - `test_30d_window_excludes_old_commits(self, tmp_path, monkeypatch)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L262)
- uses (calls/refs, reference-scoped): (4 test-only callers)

## Functions
- `_git_env()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L70) — Return the same isolated git environment used by the fixture builder.
- `_import_git_activation()` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L27) — Deferred import so collection works before the module exists.
- `_index_with_activation(repo: Path, files: list[str])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L105) — Run ASTCache.index_file on each rel-path and return the db_path.
- `_init_git_repo(repo: Path)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L90) — Initialize and configure a bounded disposable git repository.
- `_read_activation_rows(db_path: str)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L56) — Read all ast_symbol_activation rows; [] if the table is missing.
- `_run_git(repo: Path, args: list[str])` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L78) — Run a bounded git command in a test repo.
- `_seven_line_function(label: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L43) — 7-line python function body for fixture files.
- `_sym(name: str, line: int, end_line: int, sid: int)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L32) — Minimal ast_symbol_rows-shaped dict used as compute_symbol_activation input.
- `test_fixture_does_not_pollute_global_git_config(tmp_path)` — [`L481`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L481) — make_repo must leave ``$GIT_CONFIG_GLOBAL`` untouched (project rule).
- `test_perf_indexing_budget_smoke(tmp_path, monkeypatch)` — [`L410`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L410) — 50-file index with activation must stay within 40% of the baseline.

## Module values
- `_GIT_TIMEOUT_SECONDS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_activation.py#L24)

