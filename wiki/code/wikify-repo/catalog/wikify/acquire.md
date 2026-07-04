---
title: 'Module: wikify/acquire.py'
type: catalog
provenance: extracted
module: wikify/acquire.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.acquire`/
symbols:
  acquire: acquire().
  Acquired.repo_dir: Acquired#repo_dir.
  Acquired.commit: Acquired#commit.
  _git: _git().
  _toplevel: _toplevel().
  commit_of: commit_of().
  checkout: checkout().
  Acquired: Acquired#
  Acquired.slug: Acquired#slug.
---
# Module: [`wikify/acquire.py`](../../../../../raw/code/wikify-repo/wikify/acquire.py)

## Classes
### `Acquired`
- def: [`wikify/acquire.py:17`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L17) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- signature: `class Acquired:`
- members:
  - `commit` — [`L20`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L20) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
  - `repo_dir` — [`L19`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L19) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
  - `slug` — [`L18`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L18) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- used by: [`prepare`](cli.md#prepare), [`finalize`](cli.md#finalize), [`_finalize_docs`](cli.md#_finalize_docs), [`plan`](cli.md#plan), [`acquire`](acquire.md#acquire)  (2 test-only)

## Functions
- `_git(args: list[str], cwd: str | Path)` — [`L23`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L23) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `_toplevel(path: str | Path)` — [`L40`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L40) — The git work-tree root containing ``path``, or None if not in a repo. — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `acquire(source: str, slug: str, raw_dir: str | Path, ref: str | None = None, mode: str | None = None)` — [`L48`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L48) — Resolve ``source`` (local path or git URL) to a pinned source tree. — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `checkout(repo_dir: str | Path, ref: str)` — [`L36`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L36) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `commit_of(repo_dir: str | Path)` — [`L32`](../../../../../raw/code/wikify-repo/wikify/acquire.py#L32) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)

