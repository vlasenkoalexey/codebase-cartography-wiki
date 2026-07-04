---
title: 'Module: src/sync/git-hooks.ts'
type: catalog
provenance: extracted
module: src/sync/git-hooks.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/sync/`git-hooks.ts`/
symbols:
  removeGitSyncHook: removeGitSyncHook().
  installGitSyncHook: installGitSyncHook().
  GitHookResult.installed: GitHookResult#installed.
  isSyncHookInstalled: isSyncHookInstalled().
  GitHookName: GitHookName#
  stripMarkerBlock: stripMarkerBlock().
  DEFAULT_SYNC_HOOKS: DEFAULT_SYNC_HOOKS.
  markerBlock: markerBlock().
  GitHookResult.hooksDir: GitHookResult#hooksDir.
  GitHookResult.skipped: GitHookResult#skipped.
  MARKER_BEGIN: MARKER_BEGIN.
  GitHookResult: GitHookResult#
  isGitRepo: isGitRepo().
  gitHooksDir: gitHooksDir().
  MARKER_END: MARKER_END.
  chmodExecutable: chmodExecutable().
  isEffectivelyEmpty: isEffectivelyEmpty().
---
# Module: [`src/sync/git-hooks.ts`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts)

## Classes
### `GitHookName`
- def: [`src/sync/git-hooks.ts:23`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L23)
- signature: `type GitHookName`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`removeGitSyncHook`](git-hooks.ts.md#removeGitSyncHook), [`installGitSyncHook`](git-hooks.ts.md#installGitSyncHook), [`installed`](git-hooks.ts.md#GitHookResult.installed), [`isSyncHookInstalled`](git-hooks.ts.md#isSyncHookInstalled), [`DEFAULT_SYNC_HOOKS`](git-hooks.ts.md#DEFAULT_SYNC_HOOKS)

### `GitHookResult`
- def: [`src/sync/git-hooks.ts:28`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L28)
- signature: `interface GitHookResult`
- members:
  - `hooksDir` — [`L32`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L32) — Resolved hooks directory, or null when not a git repo.
  - `installed` — [`L30`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L30) — Hook names that were created or updated.
  - `skipped` — [`L34`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L34) — Reason nothing happened (e.g. not a git repository).
- uses (calls/refs, reference-scoped): [`GitHookName`](git-hooks.ts.md#GitHookName)
- used by: [`main`](../bin/codegraph.ts.md#main), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`offerWatchFallback`](../installer/index.ts.md#offerWatchFallback), [`removeGitSyncHook`](git-hooks.ts.md#removeGitSyncHook), [`installGitSyncHook`](git-hooks.ts.md#installGitSyncHook)

## Functions
- `chmodExecutable(file: string)` — [`L112`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L112)
- `gitHooksDir(projectRoot: string)` — [`L60`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L60) — Resolve the git hooks directory for a project, honoring `core.hooksPath`
- `installGitSyncHook(projectRoot: string, hooks?: GitHookName[])` — [`L125`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L125) — Install (or update) the CodeGraph sync hooks in a git repository.
- `isEffectivelyEmpty(content: string)` — [`L105`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L105) — Whether a hook body is just a shebang / blank lines (i.e. only ever ours).
- `isGitRepo(projectRoot: string)` — [`L41`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L41) — Whether `projectRoot` is inside a git working tree. Returns false if git
- `isSyncHookInstalled(projectRoot: string, hooks?: GitHookName[])` — [`L202`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L202) — Whether any CodeGraph sync hook is currently installed.
- `markerBlock()` — [`L77`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L77) — The shell snippet (between markers) injected into each hook.
- `removeGitSyncHook(projectRoot: string, hooks?: GitHookName[])` — [`L170`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L170) — Remove the CodeGraph sync hooks. Strips only our marker block; deletes the
- `stripMarkerBlock(content: string)` — [`L91`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L91) — Remove our marker block (and the marker lines) from hook content.

## Module values
- `DEFAULT_SYNC_HOOKS` — [`L26`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L26) — Hooks installed by default: commit, merge (git pull), and checkout.
- `MARKER_BEGIN` — [`L20`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L20)
- `MARKER_END` — [`L21`](../../../../../../raw/code/codegraph/src/sync/git-hooks.ts#L21)

