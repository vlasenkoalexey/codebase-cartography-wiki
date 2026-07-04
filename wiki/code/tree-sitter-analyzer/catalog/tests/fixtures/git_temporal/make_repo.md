---
title: 'Module: tests/fixtures/git_temporal/make_repo.py'
type: catalog
provenance: extracted
module: tests/fixtures/git_temporal/make_repo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.git_temporal.make_repo`/
symbols:
  make_repo: make_repo().
  _run: _run().
  make_shallow_marker: make_shallow_marker().
  Commit: Commit#
  _resolve_date: _resolve_date().
  _GIT_TIMEOUT_SECONDS: _GIT_TIMEOUT_SECONDS.
  _ensure_git_available: _ensure_git_available().
  Commit.message: Commit#message.
  Commit.files: Commit#files.
  Commit.date: Commit#date.
  Commit.rename: Commit#rename.
---
# Module: [`tests/fixtures/git_temporal/make_repo.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py)

## Classes
### `Commit`  ·  implements/extends _TypedDict
- def: [`tests/fixtures/git_temporal/make_repo.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L59)
- doc: Type hint for a commit description. `files` and `message` required.
- signature: `class Commit(TypedDict, total=False):`
- members:
  - `date` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L64)
  - `files` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L63)
  - `message` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L62)
  - `rename` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L65)

## Functions
- `_ensure_git_available()` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L113) — Skip test if git is missing (e.g. minimal CI images).
- `_resolve_date(date_spec: str)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L68) — Convert a relative date like '100 days ago' to an absolute ISO timestamp.
- `_run(repo: Path, args: list[str], env: dict[str, str] | None = None)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L90) — Run a git command inside ``repo`` and return stdout.
- `make_repo(tmp_path: Path, commits: list[dict[str, Any]])` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L121) — Initialize a fresh git repo in ``tmp_path/repo`` and seed commits.
- `make_shallow_marker(repo: Path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L183) — Mark ``repo`` as a shallow clone by creating ``.git/shallow``.

## Module values
- `_GIT_TIMEOUT_SECONDS` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/git_temporal/make_repo.py#L87)

