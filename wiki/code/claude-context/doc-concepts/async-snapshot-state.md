---
title: Snapshot state and absolute-path codebase identity
type: doc-concept
provenance: doc
source: docs/dive-deep/asynchronous-indexing-workflow.md
updated: 2026-07-04
status: fresh
---
# Snapshot state and absolute-path codebase identity

## Definition
The asynchronous workflow only works because there is a durable, shared place to record "what is the
state of each codebase" that all four MCP tools — and a second background sync process — can read and
write between calls. That place is the **local MCP snapshot**, a JSON file at
`~/.context/mcp-codebase-snapshot.json`. Two facts make it the backbone of the design: (1) codebases
are keyed by their **resolved absolute path**, so identity is stable across tool calls and processes;
and (2) progress and final statistics are *persisted* into it, so a status query after a crash, or
from a different process, still sees the last-known truth. Index the same repo via a symlink, a
different clone, or a mounted path and Claude Context treats them as *separate* codebases — the path
is the identity.

## In claude-context (grounded)
The snapshot is owned by
[`SnapshotManager`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager), persisted at
[`snapshotFilePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.snapshotFilePath) and
written by
[`saveCodebaseSnapshot`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot).
On-disk it is a
[`CodebaseSnapshot`](../catalog/packages/mcp/src/config.ts.md#CodebaseSnapshot) v1/v2 union
([`isV2Format`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.isV2Format) discriminates
the newer
[`CodebaseSnapshotV2.codebases`](../catalog/packages/mcp/src/config.ts.md#CodebaseSnapshotV2.codebases)
map from the legacy arrays). Each entry is a discriminated union — `indexing` /
`indexed` / `indexfailed` — held in memory as
[`codebaseInfoMap`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.codebaseInfoMap) and
transitioned by
[`setCodebaseIndexing`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexing),
[`setCodebaseIndexed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexed),
[`setCodebaseIndexFailed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed),
and cleared by
[`removeCodebaseCompletely`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.removeCodebaseCompletely).
State is read back by
[`getCodebaseStatus`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseStatus)
and [`getCodebaseInfo`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseInfo).

**Absolute path = identity.** Every handler forces the agent-supplied path to absolute via
[`ensureAbsolutePath`](../catalog/packages/mcp/src/utils.ts.md#ensureAbsolutePath) before indexing,
searching, clearing, or checking status — which is why the doc insists on using the *same* absolute
path across all four tools. Path lookup is not just exact-match:
[`findIndexedCodebasePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.findIndexedCodebasePath)
/
[`findIndexingCodebasePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.findIndexingCodebasePath)
route through
[`findBestMatchingCodebasePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.findBestMatchingCodebasePath)
+
[`isSameOrDescendantPath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.isSameOrDescendantPath)
so a search inside a subdirectory of an indexed root still resolves to that root's collection
(longest match wins). The doc's note that collection identity derives from the normalized absolute
path is this keying made explicit.

**Cross-process durability.** The reads
([`getIndexedCodebases`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getIndexedCodebases),
[`getIndexingCodebases`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getIndexingCodebases))
re-read the JSON file each call, and
[`saveCodebaseSnapshot`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot)
folds in on-disk entries this process doesn't know about via
[`mergeExternalEntry`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.mergeExternalEntry),
so two MCP processes sharing one snapshot file don't clobber each other. This is exactly what lets the
[background sync loop](../concepts/packages-mcp-src-sync.ts.md) —
[`startBackgroundSync`](../catalog/packages/mcp/src/sync.ts.md#SyncManager.startBackgroundSync) firing
[`handleSyncIndex`](../catalog/packages/mcp/src/sync.ts.md#SyncManager.handleSyncIndex) on an
interval — read the same ledger the handlers write, re-diff each indexed codebase with
[`FileSynchronizer.checkForChanges`](../catalog/packages/core/src/sync/synchronizer.ts.md#FileSynchronizer.checkForChanges),
and update the same entries the status tool reports on.

## Why it matters / when it applies
The snapshot is the *coordination substrate* the whole async story rests on: it is how a fire-and-
forget index communicates progress to a later status poll, how `clear_index` knows what to tear down,
and how the sync loop and the handlers stay consistent across process boundaries. Understanding that
identity is the absolute path — and that the file is the source of truth, not the vector DB — explains
the doc's two most surprising behaviors: "same repo via different paths = two codebases," and
"`0 files, 0 chunks` is stale snapshot metadata, fixed by clear + re-index of the same path."

## Connections
- Code concepts: [snapshot status ledger](../concepts/packages-mcp-src-snapshot.ts.md), [MCP tool-handler layer](../concepts/packages-mcp-src-handlers.ts.md), [MCP background sync loop](../concepts/packages-mcp-src-sync.ts.md), [FileSynchronizer](../concepts/packages-core-src-sync-synchronizer.ts.md)
- Module catalogs: [snapshot.ts](../catalog/packages/mcp/src/snapshot.ts.md), [handlers.ts](../catalog/packages/mcp/src/handlers.ts.md), [sync.ts](../catalog/packages/mcp/src/sync.ts.md), [core sync/synchronizer.ts](../catalog/packages/core/src/sync/synchronizer.ts.md), [mcp utils.ts](../catalog/packages/mcp/src/utils.ts.md), [mcp config.ts](../catalog/packages/mcp/src/config.ts.md)
- Related doc-concepts: [async-indexing-workflow](async-indexing-workflow.md), [async-progress-tracking](async-progress-tracking.md)

## Source
Extracted from `docs/dive-deep/asynchronous-indexing-workflow.md` (kept in place).
