---
title: Asynchronous (fire-and-forget) indexing workflow
type: doc-concept
provenance: doc
source: docs/dive-deep/asynchronous-indexing-workflow.md
updated: 2026-07-04
status: fresh
---
# Asynchronous (fire-and-forget) indexing workflow

## Definition
Indexing a codebase — walking every file, AST-chunking it, embedding each chunk, and upserting
batches into a vector store — is minutes of work, far longer than an agent will wait on a single
tool call. Claude Context's MCP server resolves this by making `index_codebase` **non-blocking**:
the call marks the codebase as `indexing`, spawns the real work as a detached background task, and
returns *immediately* with a "started, you can search while it runs" message. The agent stays
responsive; `search_code` and `get_indexing_status` keep answering — against partial results —
while the background task grinds on. The whole document is one mental model: **start now, finish
later, observe any time.**

## In claude-context (grounded)
The four MCP tools the agent calls — `index_codebase`, `search_code`, `clear_index`,
`get_indexing_status` — are methods on a single `ToolHandlers` class, registered with the server by
[`setupTools`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.setupTools).

The fire-and-forget seam is [`handleIndexCodebase`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleIndexCodebase):
after validating arguments and reconciling snapshot-vs-cloud state (via
[`syncIndexedCodebasesFromCloud`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.syncIndexedCodebasesFromCloud)),
it flips the codebase to `indexing` at 0% with
[`setCodebaseIndexing`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexing),
persists that, then launches
[`startBackgroundIndexing`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.startBackgroundIndexing)
**without awaiting it** and returns. The background promise plus an `AbortController` are stashed in
[`indexingTasks`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.indexingTasks) so a later
`clear_index` can cancel it.

Inside the background task,
[`startBackgroundIndexing`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.startBackgroundIndexing)
wires a [`FileSynchronizer`](../catalog/packages/core/src/sync/synchronizer.ts.md#FileSynchronizer)
and delegates the heavy lifting to `context.indexCodebase(...)` with a progress callback. On success
it records final stats with
[`setCodebaseIndexed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexed);
on failure it records
[`setCodebaseIndexFailed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed)
— *except* an `IndexAbortError`, which returns silently so a concurrent `clear_index` owns the
teardown.

Searching during indexing is deliberately allowed:
[`handleSearchCode`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleSearchCode)
resolves the path against both indexed and indexing sets and, when it targets a still-`indexing`
codebase, returns hits with a "results may be incomplete" banner rather than an error. `clear_index`
([`handleClearIndex`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleClearIndex))
first `abort()`s and **awaits** any live
[`indexingTasks`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.indexingTasks) entry so a
background writer can't race the collection drop.

The four **status states** the doc names — `indexed`, `indexing`, `indexfailed`, `not_found` — are
exactly the discriminated-union variants the snapshot tracks
([`CodebaseInfoIndexed.status`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed.status),
[`CodebaseInfoIndexing.status`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexing.status),
[`CodebaseInfoIndexFailed.status`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexFailed.status),
with `not_found` returned by
[`getCodebaseStatus`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseStatus)
when nothing is tracked).

## Why it matters / when it applies
This is the load-bearing UX property of the MCP server, and the doc frames its benefits as
non-blocking, progressive (search partial results), resilient (retry on `indexfailed`), and
transparent (status always available). For the survey it is the concrete contrast with
synchronous "index-then-answer" tools: comprehension here is a *background service* the agent
subscribes to, not a blocking precondition. The design is only safe because a shared status ledger
(the [`SnapshotManager`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager)) lets four
independent tools agree on the state of a half-indexed codebase — see the snapshot-state page.

Once an initial index exists, a separate server-side loop keeps it current: the
[background sync loop](../concepts/packages-mcp-src-sync.ts.md) re-runs Merkle-diff
([`FileSynchronizer.checkForChanges`](../catalog/packages/core/src/sync/synchronizer.ts.md#FileSynchronizer.checkForChanges))
on an interval, so "asynchronous" applies both to the first build *and* to staying up to date.

## Connections
- Code concepts: [MCP tool-handler layer](../concepts/packages-mcp-src-handlers.ts.md), [snapshot status ledger](../concepts/packages-mcp-src-snapshot.ts.md), [MCP background sync loop](../concepts/packages-mcp-src-sync.ts.md), [FileSynchronizer](../concepts/packages-core-src-sync-synchronizer.ts.md), [Context orchestrator](../concepts/packages-core-src-context.ts.md)
- Module catalogs: [handlers.ts](../catalog/packages/mcp/src/handlers.ts.md), [snapshot.ts](../catalog/packages/mcp/src/snapshot.ts.md), [sync.ts](../catalog/packages/mcp/src/sync.ts.md), [core sync/synchronizer.ts](../catalog/packages/core/src/sync/synchronizer.ts.md), [mcp index.ts](../catalog/packages/mcp/src/index.ts.md)
- Related doc-concepts: [async-progress-tracking](async-progress-tracking.md), [async-snapshot-state](async-snapshot-state.md)

## Source
Extracted from `docs/dive-deep/asynchronous-indexing-workflow.md` (kept in place).
