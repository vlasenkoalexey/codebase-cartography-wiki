---
title: Codebases are keyed by absolute path
type: doc-concept
provenance: doc
source: docs/troubleshooting/faq.md
updated: 2026-07-04
status: fresh
---
# Codebases are keyed by absolute path

## Definition
Claude Context supports many projects at once, and it keys each indexed codebase by its **absolute
path**. The practical consequence the FAQ calls out: index the same repository through two different
paths — a symlink, a second clone, or a mounted path — and they are treated as **separate indexed
codebases**, each with its own collection and its own snapshot entry. In MCP mode the current path is
detected automatically from the client's workspace, and switching directories re-scopes all
index/search operations to the new project.

## In claude-context (grounded)
The path is the primary key throughout the snapshot control plane. Lookups first resolve the request
path to an absolute path and then match it against tracked codebases via
[`findTrackedCodebasePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.findTrackedCodebasePath),
which delegates to
[`findBestMatchingCodebasePath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.findBestMatchingCodebasePath).
That matcher uses
[`isSameOrDescendantPath`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.isSameOrDescendantPath)
— built on `path.resolve` / `path.relative` — so a query inside an indexed tree is covered by the
tracked root, but a *different* absolute path (a symlink or second clone that resolves elsewhere) is not
matched and therefore indexes separately. Per-codebase state lives in the discriminated-union map read
through [`getCodebaseInfo`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseInfo)
and [`getCodebaseStatus`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager.getCodebaseStatus),
and the Milvus collection name is derived per path by
[`getCollectionName`](../catalog/packages/core/src/context.ts.md#Context.getCollectionName) — so two
paths yield two collections, never a shared index.

The "continuously monitors for changes and re-indexes modified parts" behavior the FAQ advertises is the
background sync loop: [`SyncManager.startBackgroundSync`](../catalog/packages/mcp/src/sync.ts.md#SyncManager.startBackgroundSync)
runs on an interval
([`DEFAULT_SYNC_INTERVAL_MS`](../catalog/packages/mcp/src/sync.ts.md#DEFAULT_SYNC_INTERVAL_MS)) and, for
each tracked codebase, drives [`Context.reindexByChange`](../catalog/packages/core/src/context.ts.md#Context.reindexByChange)
— the Merkle-diff incremental re-index that touches only changed files, keeping every project's index
independently fresh.

## Why it matters / when it applies
Absolute-path keying is what makes multi-project isolation work without manual configuration: each
project has its own collection, snapshot entry, and background-sync cadence, so searches never leak
across repos. It also explains a common surprise — indexing "the same" repo twice (via a symlink or a
second clone) silently doubles the work and storage because the two paths key to two collections. When
diagnosing status or search issues, always check the **exact absolute path** you originally indexed;
this is the same invariant behind the `get_indexing_status` remedies in
[faq-indexing-status](faq-indexing-status.md).

## Connections
- Code concepts: [Snapshot persistence](../concepts/packages-mcp-src-snapshot.ts.md) — the path-keyed
  state map and matcher; [MCP background sync](../concepts/packages-mcp-src-sync.ts.md) — per-codebase
  incremental refresh; [Context orchestrator](../concepts/packages-core-src-context.ts.md) — collection
  naming and Merkle re-index; [FileSynchronizer incremental sync](../concepts/packages-core-src-sync-synchronizer.ts.md)
  and [Merkle change detection](../concepts/packages-core-src-sync-merkle.ts.md) — the diff that keeps
  each index current.
- Module catalogs: [snapshot.ts](../catalog/packages/mcp/src/snapshot.ts.md) ·
  [sync.ts](../catalog/packages/mcp/src/sync.ts.md) ·
  [context.ts](../catalog/packages/core/src/context.ts.md)
- Related doc-concepts: [faq-indexing-status](faq-indexing-status.md) ·
  [faq-file-inclusion](faq-file-inclusion.md)

## Source
Extracted from `docs/troubleshooting/faq.md` (kept in place).
