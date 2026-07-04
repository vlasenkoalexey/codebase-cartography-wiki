---
title: Progress and status tracking for background indexing
type: doc-concept
provenance: doc
source: docs/dive-deep/asynchronous-indexing-workflow.md
updated: 2026-07-04
status: fresh
---
# Progress and status tracking for background indexing

## Definition
Because indexing runs detached (see [async-indexing-workflow](async-indexing-workflow.md)), the only
window an agent has into a running index is `get_indexing_status`. The doc is careful about what that
number means: it is a **coarse, phase-based percentage**, not an exact fraction of files completed —
0% (preparing the collection / validating prerequisites), ~5% (scanning and building the file list),
then a 10% → 100% band for the actual file processing (chunk → embed → upsert), reaching 100% only
when the run finishes. So a large codebase "jumping to ~10% quickly" is normal: it is the setup→
processing transition, not one-tenth of the files done. File and chunk *totals* are a separate story
— they appear only after a run completes and its final statistics are written.

## In claude-context (grounded)
`get_indexing_status` is
[`handleGetIndexingStatus`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleGetIndexingStatus):
it reconciles from cloud, resolves the tracked path, then reads
[`getCodebaseStatus`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseStatus)
and [`getCodebaseInfo`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseInfo)
and renders one message per state: `indexed` (with file/chunk counts), `indexing` (with a
percentage), `indexfailed`, or `not_found`.

The percentage lives on the `indexing` snapshot variant as
[`CodebaseInfoIndexing.indexingPercentage`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexing.indexingPercentage).
The background task's progress callback repeatedly calls
[`setCodebaseIndexing`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexing)
(which routes through
[`updateIndexingProgress`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.updateIndexingProgress)),
and the last-known value is read back by
[`getIndexingProgress`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getIndexingProgress)
— which is also what
[`setCodebaseIndexFailed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed)
captures as
[`lastAttemptedPercentage`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexFailed.lastAttemptedPercentage)
so a failed index reports how far it got.
[`getIndexingCodebasesWithProgress`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getIndexingCodebasesWithProgress)
exposes the same for all in-flight codebases at once.

**Persistence explains the jumps.** Progress is written to the local snapshot file at
`~/.context/mcp-codebase-snapshot.json`
([`snapshotFilePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.snapshotFilePath))
periodically — the background loop throttles
[`saveCodebaseSnapshot`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot)
to roughly once every 2s — so very fast phases surface as jumps rather than smooth increments,
exactly as the doc warns.

**File/chunk totals are post-hoc.** During active indexing the server tracks only the percentage; it
does **not** stream live file/chunk counts through `get_indexing_status`. Final counts are written by
[`setCodebaseIndexed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexed)
into
[`CodebaseInfoIndexed.indexedFiles`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed.indexedFiles)
and
[`CodebaseInfoIndexed.totalChunks`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed.totalChunks)
(read back via
[`getIndexedFileCount`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getIndexedFileCount)).
The doc's "`0 files, 0 chunks`" symptom is a stale-snapshot artifact — not a live vector-DB count — and
this is the very phantom the handler layer defends against:
[`setCodebaseIndexed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexed)
refuses to persist a `0/0 + completed` record, and
[`validateLegacyZeroEntries`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.validateLegacyZeroEntries)
heals older ones at startup. The doc's fix — clear and re-index the **same absolute path** — is the
supported way to refresh stale totals.

## Why it matters / when it applies
This is the transparency leg of the async design: an agent can poll a running index and reason about
it, but must not over-read the number (it is phase-based, and counts lag). For the survey it shows a
deliberate trade of *precision for cheapness* — a persisted coarse percentage costs almost nothing to
maintain across a detached task and two cooperating processes, where a true per-file fraction would
demand tight streaming coupling between the background loop and the status tool.

## Connections
- Code concepts: [snapshot status ledger](../concepts/packages-mcp-src-snapshot.ts.md), [MCP tool-handler layer](../concepts/packages-mcp-src-handlers.ts.md), [MCP background sync loop](../concepts/packages-mcp-src-sync.ts.md)
- Module catalogs: [snapshot.ts](../catalog/packages/mcp/src/snapshot.ts.md), [handlers.ts](../catalog/packages/mcp/src/handlers.ts.md), [mcp config.ts](../catalog/packages/mcp/src/config.ts.md)
- Related doc-concepts: [async-indexing-workflow](async-indexing-workflow.md), [async-snapshot-state](async-snapshot-state.md)

## Source
Extracted from `docs/dive-deep/asynchronous-indexing-workflow.md` (kept in place).
