---
title: 'Module: tree_sitter_analyzer/git_activation.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/git_activation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.git_activation`/
symbols:
  compute_symbol_activation: compute_symbol_activation().
  _zero_rows: _zero_rows().
  parse_log_hunks.flush: parse_log_hunks().flush().
  parse_log_hunks: parse_log_hunks().
  detect_git_state: detect_git_state().
  _run_git_log: _run_git_log().
  _newest_commit: _newest_commit().
  Commit: Commit#
  _git_log_simple: _git_log_simple().
  _attribute_commits: _attribute_commits().
  Commit.ts: Commit#ts.
  ActivationRow: ActivationRow#
  _is_tracked: _is_tracked().
  _newest_attribution: _newest_attribution().
  ActivationRow.git_state: ActivationRow#git_state.
  GitState: GitState.
  _COMMIT_HEADER_RE: _COMMIT_HEADER_RE.
  _git_log_hunks: _git_log_hunks().
  ActivationRow.symbol_id: ActivationRow#symbol_id.
  ActivationRow.last_modified_commit: ActivationRow#last_modified_commit.
  ActivationRow.last_modified_at: ActivationRow#last_modified_at.
  ActivationRow.mod_count_30d: ActivationRow#mod_count_30d.
  ActivationRow.mod_count_90d: ActivationRow#mod_count_90d.
  ActivationRow.mod_count_all: ActivationRow#mod_count_all.
  ActivationRow.computed_at: ActivationRow#computed_at.
  logger: logger.
  _SECONDS_PER_DAY: _SECONDS_PER_DAY.
  _DEFAULT_GIT_TIMEOUT: _DEFAULT_GIT_TIMEOUT.
  _COMMIT_MARKER: _COMMIT_MARKER.
  Commit.sha: Commit#sha.
  Commit.hunks: Commit#hunks.
  Commit.creation_hunks: Commit#creation_hunks.
  ActivationRow.file_path: ActivationRow#file_path.
  _activation_disabled: _activation_disabled().
  _find_repo_root: _find_repo_root().
  _rel_to_repo: _rel_to_repo().
  _normalize_symbol: _normalize_symbol().
  _HUNK_RE: _HUNK_RE.
---
# Module: [`tree_sitter_analyzer/git_activation.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py)

## Classes
### `ActivationRow`
- def: [`tree_sitter_analyzer/git_activation.py:87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L87)
- doc: One row in the `ast_symbol_activation` SQLite table.
- signature: `class ActivationRow:`
- members:
  - `computed_at` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L102)
  - `file_path` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L96)
  - `git_state` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L103)
  - `last_modified_at` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L98)
  - `last_modified_commit` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L97)
  - `mod_count_30d` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L99)
  - `mod_count_90d` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L100)
  - `mod_count_all` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L101)
  - `symbol_id` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L95)
- uses (calls/refs, reference-scoped): [`GitState`](git_activation.md#GitState)
- used by: [`compute_symbol_activation`](git_activation.md#compute_symbol_activation), [`_zero_rows`](git_activation.md#_zero_rows), [`write_activation_for_file`](_ast_cache_write.md#write_activation_for_file)

### `Commit`
- def: [`tree_sitter_analyzer/git_activation.py:66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L66)
- doc: One commit's hunks against a single file.
- signature: `class Commit:`
- members:
  - `creation_hunks` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L83)
  - `hunks` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L82)
  - `sha` — [`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L80)
  - `ts` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L81)
- used by: [`compute_symbol_activation`](git_activation.md#compute_symbol_activation), [`flush`](git_activation.md#parse_log_hunks.flush), [`parse_log_hunks`](git_activation.md#parse_log_hunks), [`_newest_commit`](git_activation.md#_newest_commit), [`_attribute_commits`](git_activation.md#_attribute_commits), [`_git_log_simple`](git_activation.md#_git_log_simple), [`_newest_attribution`](git_activation.md#_newest_attribution)

## Functions
- `_activation_disabled()` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L311) — Check the env-var disable switch. ``0`` / ``false`` / ``no`` → off.
- `_attribute_commits(commits: list[Commit], line_start: int, line_end: int)` — [`L433`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L433) — Return the subset of ``commits`` whose hunks credit [start, end].
- `_find_repo_root(start: str)` — [`L317`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L317) — Walk up from ``start`` to find an enclosing ``.git`` directory.
- `_git_log_hunks(repo_root: str, rel_path: str, *, since_days: int)` — [`L391`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L391) — ``git log -p -U0`` for the last ``since_days``. Raw output to parse.
- `_git_log_simple(repo_root: str, rel_path: str)` — [`L386`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L386) — File-level history (no hunks). Cheap walk, used for ``mod_count_all``.
- `_is_tracked(repo_root: str, abs_path: str)` — [`L328`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L328) — Return True when git knows about ``abs_path`` inside ``repo_root``.
- `_newest_attribution(commits: list[Commit])` — [`L406`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L406) — Most recent commit from an already-filtered attribution list.
- `_newest_commit(commits: list[Commit])` — [`L396`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L396) — Return (sha, ts) for the most recent commit, or (None, None).
- `_normalize_symbol(sym: dict)` — [`L413`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L413) — Extract (id, line_start, line_end) from a symbol dict.
- `_rel_to_repo(repo_root: str, abs_path: str)` — [`L346`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L346) — Convert ``abs_path`` to a forward-slash path relative to ``repo_root``.
- `_run_git_log(repo_root: str, rel_path: str, *, with_hunks: bool, since_days: int | None = None)` — [`L356`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L356) — Run ``git log --follow`` against a file; return raw stdout or ''.
- `_zero_rows(symbols: list[dict], file_path: str, now_ts: int, state: GitState)` — [`L468`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L468) — Return one zero-count ``ActivationRow`` per symbol for cold paths.
- `compute_symbol_activation(file_path: str, symbols: Iterable[dict], *, now_ts: int | None = None, repo_root: str | None = None)` — [`L215`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L215) — Compute one ``ActivationRow`` per symbol from git history.
- `detect_git_state(path: str)` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L111) — Classify how useful git history will be for ``path``.
- `flush()` — [`L163`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L163)
- `parse_log_hunks(git_log_output: str)` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L139) — Parse ``git log --pretty=__C__ %H %at -p -U0`` output into commits.

## Module values
- `GitState` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L43)
- `_COMMIT_HEADER_RE` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L49)
- `_COMMIT_MARKER` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L48)
- `_DEFAULT_GIT_TIMEOUT` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L47)
- `_HUNK_RE` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L59)
- `_SECONDS_PER_DAY` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L46)
- `logger` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/git_activation.py#L39)

