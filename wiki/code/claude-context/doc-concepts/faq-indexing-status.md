---
title: Reading indexing status — phase progress and snapshot metadata
type: doc-concept
provenance: doc
source: docs/troubleshooting/faq.md
updated: 2026-07-04
status: fresh
---
# Reading indexing status — phase progress and snapshot metadata

## Definition
Two FAQ entries explain quirks of `get_indexing_status`, and both trace to the same design decision:
the tool reports **stored bookkeeping**, not a live query of the vector database. First, the percentage
is a *phase-based* progress indicator (collection preparation → file scanning → processing/chunking/
embedding/insertion), so it can jump to roughly `10%` the instant setup finishes even on a huge repo —
that is expected, not a stall. Second, a completed codebase can show `0 files, 0 chunks` when the local
snapshot metadata is stale or was written before final statistics were refreshed.

## In claude-context (grounded)
`get_indexing_status` is served by
[`handleGetIndexingStatus`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleGetIndexingStatus),
which resolves the request path, then reads state from the
[`SnapshotManager`](../concepts/packages-mcp-src-snapshot.ts.md) — never from Milvus directly. It calls
[`getCodebaseStatus`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseStatus) and
[`getCodebaseInfo`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseInfo) and
formats the discriminated-union record. The phase percentage is the stored
[`CodebaseInfoIndexing.indexingPercentage`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexing.indexingPercentage)
field; the handler's own text buckets it — `< 10%` prints "Preparing and scanning files...", `< 100%`
prints "Processing files and generating embeddings..." — which is exactly the phase model the FAQ
describes. The completed-state counts are the stored
[`CodebaseInfoIndexed.indexedFiles`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed.indexedFiles)
and
[`CodebaseInfoIndexed.totalChunks`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed.totalChunks),
written at index completion; if that write was skipped, the record reads `0/0` even though Milvus holds
real rows.

The FAQ's remedy — re-run `clear_index` then `index_codebase` for the *exact* absolute path — maps to
[`handleClearIndex`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleClearIndex) and
[`handleIndexCodebase`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleIndexCodebase),
which rewrite the snapshot stats. Beyond that manual path, the server also self-heals legacy `0/0`
entries: [`validateLegacyZeroEntries`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.validateLegacyZeroEntries)
finds `indexed` records with zero counts and reconciles each against the real store — it probes
[`hasCollection`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.hasCollection)
(a missing collection ⇒ remove the phantom entry via
[`removeCodebaseCompletely`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.removeCodebaseCompletely)),
then reads
[`getCollectionRowCount`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.getCollectionRowCount)
and, if rows exist, heals the snapshot with
[`setCodebaseIndexed`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.setCodebaseIndexed).
A thrown error (Milvus unreachable) is treated as transient and the entry is left untouched, so a
network blip never destroys real state.

## Why it matters / when it applies
Keeping status in the snapshot rather than querying Milvus on every call is what makes
`get_indexing_status` cheap and lets it work while indexing is still running — but it is also why the
two surprising behaviors exist. The `10%` jump is not progress lost; it reflects that scanning/prep is
one coarse phase and the long tail is embedding+insertion. The `0/0`-on-complete case is a
snapshot-vs-store divergence, resolved either automatically by the zero-entry validator or manually by
clearing and reindexing the same absolute path. Both symptoms reinforce the key rule elsewhere in the
FAQ: everything is keyed by the exact absolute path you indexed (see
[faq-codebase-path-keying](faq-codebase-path-keying.md)).

## Connections
- Code concepts: [Snapshot persistence](../concepts/packages-mcp-src-snapshot.ts.md) — the metadata store
  the status is read from; [MCP tool handlers](../concepts/packages-mcp-src-handlers.ts.md) — where the
  status/clear/index tools live; [Milvus vector DB](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  — the live store the self-healer reconciles against; [MCP config resolution](../concepts/packages-mcp-src-config.ts.md)
  — defines the `CodebaseInfo` union.
- Module catalogs: [handlers.ts](../catalog/packages/mcp/src/handlers.ts.md) ·
  [snapshot.ts](../catalog/packages/mcp/src/snapshot.ts.md) ·
  [config.ts](../catalog/packages/mcp/src/config.ts.md) ·
  [milvus-vectordb.ts](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md)
- Related doc-concepts: [faq-codebase-path-keying](faq-codebase-path-keying.md) ·
  [faq-file-inclusion](faq-file-inclusion.md)

## Source
Extracted from `docs/troubleshooting/faq.md` (kept in place).
