---
title: 'Module: packages/mcp/src/snapshot.ts'
type: catalog
provenance: extracted
module: packages/mcp/src/snapshot.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-mcp 0.1.15 src/`snapshot.ts`/SnapshotManager#
symbols:
  SnapshotManager.saveCodebaseSnapshot: saveCodebaseSnapshot().
  SnapshotManager.loadV2Format: loadV2Format().
  SnapshotManager.setCodebaseIndexed: setCodebaseIndexed().
  SnapshotManager.loadV1Format: loadV1Format().
  SnapshotManager.setCodebaseIndexing: setCodebaseIndexing().
  SnapshotManager.getIndexedCodebases: getIndexedCodebases().
  SnapshotManager.setCodebaseIndexFailed: setCodebaseIndexFailed().
  SnapshotManager.mergeExternalEntry: mergeExternalEntry().
  SnapshotManager.getIndexingCodebases: getIndexingCodebases().
  SnapshotManager.getIndexingProgress: getIndexingProgress().
  SnapshotManager.addIndexedCodebase: addIndexedCodebase().
  SnapshotManager.codebaseInfoMap: codebaseInfoMap.
  SnapshotManager.removeCodebaseCompletely: removeCodebaseCompletely().
  SnapshotManager.indexedCodebases: indexedCodebases.
  SnapshotManager.snapshotFilePath: snapshotFilePath.
  SnapshotManager.loadCodebaseSnapshot: loadCodebaseSnapshot().
  SnapshotManager.indexingCodebases: indexingCodebases.
  SnapshotManager.addIndexingCodebase: addIndexingCodebase().
  SnapshotManager.updateIndexingProgress: updateIndexingProgress().
  SnapshotManager.getCodebaseStatus: getCodebaseStatus().
  SnapshotManager.getCodebaseInfo: getCodebaseInfo().
  SnapshotManager.getIndexOptions: getIndexOptions().
  SnapshotManager.codebaseFileCount: codebaseFileCount.
  SnapshotManager.getFailedCodebases: getFailedCodebases().
  SnapshotManager.resolveIndexOptions: resolveIndexOptions().
  SnapshotManager: ''
  SnapshotManager.-constructor: '`<constructor>`().'
  SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.status: setCodebaseIndexed().(stats)typeLiteral146:status.
  SnapshotManager.isV2Format: isV2Format().
  SnapshotManager.removeIndexedCodebase: removeIndexedCodebase().
  SnapshotManager.recentlyRemoved: recentlyRemoved.
  SnapshotManager.findIndexedCodebasePath: findIndexedCodebasePath().
  SnapshotManager.findIndexingCodebasePath: findIndexingCodebasePath().
  SnapshotManager.findTrackedCodebasePath: findTrackedCodebasePath().
  SnapshotManager.removeIndexingCodebase: removeIndexingCodebase().
  SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.indexedFiles: setCodebaseIndexed().(stats)typeLiteral146:indexedFiles.
  SnapshotManager.findBestMatchingCodebasePath: findBestMatchingCodebasePath().
  SnapshotManager.moveFromIndexingToIndexed: moveFromIndexingToIndexed().
  SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.totalChunks: setCodebaseIndexed().(stats)typeLiteral146:totalChunks.
  SnapshotManager.acquireLock: acquireLock().
  SnapshotManager.releaseLock: releaseLock().
  SnapshotManager.getIndexingCodebasesWithProgress: getIndexingCodebasesWithProgress().
  SnapshotManager.getIndexedFileCount: getIndexedFileCount().
  SnapshotManager.setIndexedFileCount: setIndexedFileCount().
  SnapshotManager.isSameOrDescendantPath: isSameOrDescendantPath().
---
# Module: [`packages/mcp/src/snapshot.ts`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts)

## Classes
### `SnapshotManager`
- def: [`packages/mcp/src/snapshot.ts:15`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L15) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `class SnapshotManager`
- members:
  - `<constructor>()` — [`L23`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L23)
  - `acquireLock(method)` — [`L555`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L555) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `addIndexedCodebase(method)` — [`L343`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L343)
  - `addIndexingCodebase(method)` — [`L302`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L302)
  - `findBestMatchingCodebasePath(method)` — [`L210`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L210)
  - `findIndexedCodebasePath(method)` — [`L245`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L245) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `findIndexingCodebasePath(method)` — [`L249`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L249) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `findTrackedCodebasePath(method)` — [`L253`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L253)
  - `getCodebaseInfo(method)` — [`L497`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L497) — Get complete codebase information — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `getCodebaseStatus(method)` — [`L488`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L488) — Get codebase status — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `getFailedCodebases(method)` — [`L504`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L504) — Get all failed codebases — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `getIndexOptions(method)` — [`L227`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L227) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `getIndexedCodebases(method)` — [`L146`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L146) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `getIndexedFileCount(method)` — [`L383`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L383)
  - `getIndexingCodebases(method)` — [`L171`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L171) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `getIndexingCodebasesWithProgress(method)` — [`L260`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L260)
  - `getIndexingProgress(method)` — [`L264`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L264) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `isSameOrDescendantPath(method)` — [`L204`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L204)
  - `isV2Format(method)` — [`L31`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L31) — Check if snapshot is v2 format — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `loadCodebaseSnapshot(method)` — [`L526`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L526) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `loadV1Format(method)` — [`L38`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L38) — Convert v1 format to internal state — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `loadV2Format(method)` — [`L98`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L98) — Convert v2 format to internal state — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `mergeExternalEntry(method)` — [`L584`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L584) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `moveFromIndexingToIndexed(method)` — [`L375`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L375)
  - `releaseLock(method)` — [`L578`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L578) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `removeCodebaseCompletely(method)` — [`L513`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L513) — Completely remove a codebase from all tracking (for clear_index operation) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `removeIndexedCodebase(method)` — [`L365`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L365)
  - `removeIndexingCodebase(method)` — [`L334`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L334)
  - `resolveIndexOptions(method)` — [`L241`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L241) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `saveCodebaseSnapshot(method)` — [`L603`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L603) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `setCodebaseIndexFailed(method)` — [`L461`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L461) — Set codebase to failed status — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `setCodebaseIndexed(method)` — [`L419`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L419) — Set codebase to indexed status with complete statistics — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `setCodebaseIndexing(method)` — [`L397`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L397) — Set codebase to indexing status — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `setIndexedFileCount(method)` — [`L390`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L390)
  - `updateIndexingProgress(method)` — [`L317`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L317)
  - `codebaseFileCount` — [`L19`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L19) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `codebaseInfoMap` — [`L20`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L20) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `indexedCodebases` — [`L17`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L17) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `indexedFiles` — [`L421`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L421) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `indexingCodebases` — [`L18`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L18) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `recentlyRemoved` — [`L21`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L21) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `snapshotFilePath` — [`L16`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L16) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `status` — [`L421`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L421) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `totalChunks` — [`L421`](../../../../../../../raw/code/claude-context/packages/mcp/src/snapshot.ts#L421) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- uses (calls/refs, reference-scoped): [`status`](config.ts.md#CodebaseInfoIndexFailed.status), [`status`](config.ts.md#CodebaseInfoIndexing.status), [`status`](config.ts.md#CodebaseInfoIndexed.status), [`CodebaseInfo`](config.ts.md#CodebaseInfo), [`indexingCodebases`](config.ts.md#CodebaseSnapshotV1.indexingCodebases), [`requestSplitter`](config.ts.md#CodebaseIndexOptions.requestSplitter), [`CodebaseIndexOptions`](config.ts.md#CodebaseIndexOptions), [`CodebaseSnapshot`](config.ts.md#CodebaseSnapshot), [`requestCustomExtensions`](config.ts.md#CodebaseIndexOptions.requestCustomExtensions), [`requestIgnorePatterns`](config.ts.md#CodebaseIndexOptions.requestIgnorePatterns), [`codebases`](config.ts.md#CodebaseSnapshotV2.codebases), [`indexedFiles`](config.ts.md#CodebaseInfoIndexed.indexedFiles), [`lastUpdated`](config.ts.md#CodebaseInfoBase.lastUpdated), [`CodebaseInfoIndexed`](config.ts.md#CodebaseInfoIndexed), [`CodebaseInfoIndexing`](config.ts.md#CodebaseInfoIndexing), [`CodebaseInfoIndexFailed`](config.ts.md#CodebaseInfoIndexFailed), [`indexingPercentage`](config.ts.md#CodebaseInfoIndexing.indexingPercentage), [`CodebaseSnapshotV2`](config.ts.md#CodebaseSnapshotV2), [`totalChunks`](config.ts.md#CodebaseInfoIndexed.totalChunks), [`CodebaseSnapshotV1`](config.ts.md#CodebaseSnapshotV1), [`errorMessage`](config.ts.md#CodebaseInfoIndexFailed.errorMessage), [`indexStatus`](config.ts.md#CodebaseInfoIndexed.indexStatus), [`lastAttemptedPercentage`](config.ts.md#CodebaseInfoIndexFailed.lastAttemptedPercentage), [`indexedCodebases`](config.ts.md#CodebaseSnapshotV1.indexedCodebases), [`formatVersion`](config.ts.md#CodebaseSnapshotV2.formatVersion), [`lastUpdated`](config.ts.md#CodebaseSnapshotV2.lastUpdated)
- used by: [`handleIndexCodebase`](handlers.ts.md#ToolHandlers.handleIndexCodebase), [`<constructor>`](index.ts.md#ContextMcpServer.-constructor), [`snapshotManager`](handlers.ts.md#ToolHandlers.snapshotManager), [`snapshot.request-options.test.ts`](snapshot.request-options.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.request-options.test.ts), [`validateLegacyZeroEntries`](handlers.ts.md#ToolHandlers.validateLegacyZeroEntries), [`handleSyncIndex`](sync.ts.md#SyncManager.handleSyncIndex), [`originalConsoleWarn`](index.ts.md#originalConsoleWarn), [`handlers.get-indexing-status.test.ts`](handlers.get-indexing-status.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-handlers.get-indexing-status.test.ts), [`handlers.ts`](handlers.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-handlers.ts), [`handleSearchCode`](handlers.ts.md#ToolHandlers.handleSearchCode), [`handleClearIndex`](handlers.ts.md#ToolHandlers.handleClearIndex), [`startBackgroundIndexing`](handlers.ts.md#ToolHandlers.startBackgroundIndexing), [`syncIndexedCodebasesFromCloud`](handlers.ts.md#ToolHandlers.syncIndexedCodebasesFromCloud), [`sync.ts`](sync.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-sync.ts), [`handleGetIndexingStatus`](handlers.ts.md#ToolHandlers.handleGetIndexingStatus), [`<constructor>`](handlers.ts.md#ToolHandlers.-constructor), [`<constructor>`](sync.ts.md#SyncManager.-constructor), [`snapshotManager`](index.ts.md#ContextMcpServer.snapshotManager), [`snapshotManager`](sync.ts.md#SyncManager.snapshotManager)

