---
title: 'Module: src/sync/worktree.ts'
type: catalog
provenance: extracted
module: src/sync/worktree.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/sync/`worktree.ts`/
symbols:
  detectWorktreeIndexMismatch: detectWorktreeIndexMismatch().
  worktreeMismatchWarning: worktreeMismatchWarning().
  worktreeMismatchNotice: worktreeMismatchNotice().
  WorktreeIndexMismatch: WorktreeIndexMismatch#
  gitWorktreeRoot: gitWorktreeRoot().
  gitCommonDir: gitCommonDir().
  WorktreeIndexMismatch.worktreeRoot: WorktreeIndexMismatch#worktreeRoot.
  WorktreeIndexMismatch.indexRoot: WorktreeIndexMismatch#indexRoot.
  realpath: realpath().
---
# Module: [`src/sync/worktree.ts`](../../../../../../raw/code/codegraph/src/sync/worktree.ts)

## Classes
### `WorktreeIndexMismatch`
- def: [`src/sync/worktree.ts:75`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L75)
- signature: `interface WorktreeIndexMismatch`
- members:
  - `indexRoot` — [`L79`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L79) — The (different) working tree whose `.codegraph` index is being used.
  - `worktreeRoot` — [`L77`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L77) — The git working tree the command was run from.
- used by: [`main`](../bin/codegraph.ts.md#main), [`tools.ts`](../mcp/tools.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-tools.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`worktreeMismatchFor`](../mcp/tools.ts.md#ToolHandler.worktreeMismatchFor), [`detectWorktreeIndexMismatch`](worktree.ts.md#detectWorktreeIndexMismatch), [`worktreeMismatchWarning`](worktree.ts.md#worktreeMismatchWarning), [`worktreeMismatchNotice`](worktree.ts.md#worktreeMismatchNotice), [`worktreeMismatchCache`](../mcp/tools.ts.md#ToolHandler.worktreeMismatchCache)

## Functions
- `detectWorktreeIndexMismatch(startPath: string, indexRoot: string)` — [`L93`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L93) — Detect when `startPath` lives in one git working tree but the resolved
- `gitCommonDir(dir: string)` — [`L58`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L58) — Absolute, symlink-resolved git **common** directory for `dir` — the shared
- `gitWorktreeRoot(dir: string)` — [`L32`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L32) — Absolute, symlink-resolved toplevel of the git working tree that `dir`
- `realpath(p: string)` — [`L152`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L152) — Resolve symlinks where possible so tmp/realpath quirks don't break equality.
- `worktreeMismatchNotice(m: WorktreeIndexMismatch)` — [`L142`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L142) — Compact, single-line variant for prefixing a tool's result. Read tools
- `worktreeMismatchWarning(m: WorktreeIndexMismatch)` — [`L126`](../../../../../../raw/code/codegraph/src/sync/worktree.ts#L126) — One-line-per-fact warning describing a detected mismatch.

