---
title: 'Module: wikify/diff.py'
type: catalog
provenance: extracted
module: wikify/diff.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.diff`/
symbols:
  compute_plan: compute_plan().
  Plan.render: Plan#render().
  current_hashes: current_hashes().
  Plan.is_noop: Plan#is_noop().
  Plan.todo: Plan#todo().
  Plan.build: Plan#build.
  Plan.rebuild: Plan#rebuild.
  Plan: Plan#
  Plan.leave: Plan#leave.
  Plan.changed_symbols: Plan#changed_symbols.
  Plan.removed_symbols: Plan#removed_symbols.
---
# Module: [`wikify/diff.py`](../../../../../raw/code/wikify-repo/wikify/diff.py)

## Classes
### `Plan`
- def: [`wikify/diff.py:19`](../../../../../raw/code/wikify-repo/wikify/diff.py#L19) — documented in [wikify-diff](../../concepts/wikify-diff.md)
- signature: `class Plan:`
- members:
  - `is_noop(self)` — [`L27`](../../../../../raw/code/wikify-repo/wikify/diff.py#L27)
  - `render(self)` — [`L34`](../../../../../raw/code/wikify-repo/wikify/diff.py#L34) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `todo(self)` — [`L31`](../../../../../raw/code/wikify-repo/wikify/diff.py#L31)
  - `build` — [`L20`](../../../../../raw/code/wikify-repo/wikify/diff.py#L20) — documented in [wikify-diff](../../concepts/wikify-diff.md)
  - `changed_symbols` — [`L23`](../../../../../raw/code/wikify-repo/wikify/diff.py#L23) — documented in [wikify-diff](../../concepts/wikify-diff.md)
  - `leave` — [`L22`](../../../../../raw/code/wikify-repo/wikify/diff.py#L22) — documented in [wikify-diff](../../concepts/wikify-diff.md)
  - `rebuild` — [`L21`](../../../../../raw/code/wikify-repo/wikify/diff.py#L21) — documented in [wikify-diff](../../concepts/wikify-diff.md)
  - `removed_symbols` — [`L24`](../../../../../raw/code/wikify-repo/wikify/diff.py#L24) — documented in [wikify-diff](../../concepts/wikify-diff.md)
- used by: [`prepare`](cli.md#prepare), [`plan`](cli.md#plan), [`compute_plan`](diff.md#compute_plan)

## Functions
- `compute_plan(graph: SymbolGraph, repo_root: str | Path, state: dict, config: RepoConfig, hashes: dict[str, str] | None = None)` — [`L51`](../../../../../raw/code/wikify-repo/wikify/diff.py#L51) — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `current_hashes(graph: SymbolGraph, repo_root: str | Path)` — [`L47`](../../../../../raw/code/wikify-repo/wikify/diff.py#L47) — documented in [wikify-cli](../../concepts/wikify-cli.md)

