---
title: 'Module: packages/mcp/src/handlers.ts'
type: catalog
provenance: extracted
module: packages/mcp/src/handlers.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-mcp 0.1.15 src/`handlers.ts`/ToolHandlers#
symbols:
  ToolHandlers.handleIndexCodebase: handleIndexCodebase().
  ToolHandlers.snapshotManager: snapshotManager.
  ToolHandlers.validateLegacyZeroEntries: validateLegacyZeroEntries().
  ToolHandlers.handleSearchCode: handleSearchCode().
  ToolHandlers.startBackgroundIndexing: startBackgroundIndexing().
  ToolHandlers.handleClearIndex: handleClearIndex().
  ToolHandlers.context: context.
  ToolHandlers.syncIndexedCodebasesFromCloud: syncIndexedCodebasesFromCloud().
  ToolHandlers.handleGetIndexingStatus: handleGetIndexingStatus().
  ToolHandlers.-constructor: '`<constructor>`().'
  ToolHandlers.queryCollectionStats: queryCollectionStats().
  ToolHandlers.indexingTasks: indexingTasks.
  ToolHandlers: ''
  ToolHandlers.indexingTasks.Map.typeLiteral11.controller: indexingTasks.Map:typeLiteral11:controller.
  ToolHandlers.indexingStats: indexingStats.
  ToolHandlers.currentWorkspace: currentWorkspace.
  ToolHandlers.indexingTasks.Map.typeLiteral11.promise: indexingTasks.Map:typeLiteral11:promise.
---
# Module: [`packages/mcp/src/handlers.ts`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts)

## Classes
### `ToolHandlers`
- def: [`packages/mcp/src/handlers.ts:10`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L10)
- signature: `class ToolHandlers`
- members:
  - `<constructor>(context: Context, snapshotManager: SnapshotManager)` — [`L24`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L24) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `handleClearIndex(method)` — [`L854`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L854) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `handleGetIndexingStatus(method)` — [`L992`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L992) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `handleIndexCodebase(method)` — [`L324`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L324) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `handleSearchCode(method)` — [`L647`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L647) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `queryCollectionStats(method)` — [`L39`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L39) — Query Milvus for the real row count of a codebase's collection. — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `startBackgroundIndexing(method)` — [`L543`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L543) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `syncIndexedCodebasesFromCloud(method)` — [`L167`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L167) — Sync indexed codebases from Zilliz Cloud collections — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `validateLegacyZeroEntries(method)` — [`L71`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L71) — One-shot startup validation: find any legacy 0/0+completed entries on disk — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `context` — [`L11`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L11) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `controller` — [`L22`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L22)
  - `currentWorkspace` — [`L14`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L14)
  - `indexingStats` — [`L13`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L13)
  - `indexingTasks` — [`L22`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L22) — Tracks active background indexing tasks per absolute codebase path so — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `promise` — [`L22`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L22)
  - `snapshotManager` — [`L12`](../../../../../../../raw/code/claude-context/packages/mcp/src/handlers.ts#L12) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- uses (calls/refs, reference-scoped): [`saveCodebaseSnapshot`](snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot), [`setCodebaseIndexed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed), [`setCodebaseIndexing`](snapshot.ts.md#SnapshotManager.setCodebaseIndexing), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`setCodebaseIndexFailed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`removeCodebaseCompletely`](snapshot.ts.md#SnapshotManager.removeCodebaseCompletely), [`status`](config.ts.md#CodebaseInfoIndexFailed.status), [`status`](config.ts.md#CodebaseInfoIndexing.status), [`status`](config.ts.md#CodebaseInfoIndexed.status), [`getCodebaseInfo`](snapshot.ts.md#SnapshotManager.getCodebaseInfo), [`getCodebaseStatus`](snapshot.ts.md#SnapshotManager.getCodebaseStatus), [`requestSplitter`](config.ts.md#CodebaseIndexOptions.requestSplitter), [`CodebaseIndexOptions`](config.ts.md#CodebaseIndexOptions), [`RequestSplitterType`](config.ts.md#RequestSplitterType), [`SnapshotManager`](snapshot.ts.md#SnapshotManager), [`requestCustomExtensions`](config.ts.md#CodebaseIndexOptions.requestCustomExtensions), [`requestIgnorePatterns`](config.ts.md#CodebaseIndexOptions.requestIgnorePatterns), [`indexedFiles`](config.ts.md#CodebaseInfoIndexed.indexedFiles), [`status`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.status), [`createRequestSplitter`](splitter.ts.md#createRequestSplitter), [`ensureAbsolutePath`](utils.ts.md#ensureAbsolutePath), [`findIndexedCodebasePath`](snapshot.ts.md#SnapshotManager.findIndexedCodebasePath), [`findIndexingCodebasePath`](snapshot.ts.md#SnapshotManager.findIndexingCodebasePath), [`findTrackedCodebasePath`](snapshot.ts.md#SnapshotManager.findTrackedCodebasePath), [`indexedFiles`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.indexedFiles), [`isRequestSplitterType`](splitter.ts.md#isRequestSplitterType), [`trackCodebasePath`](utils.ts.md#trackCodebasePath), [`totalChunks`](config.ts.md#CodebaseInfoIndexed.totalChunks), [`totalChunks`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed.stats-typeLiteral146.totalChunks), [`truncateContent`](utils.ts.md#truncateContent)
- used by: [`<constructor>`](index.ts.md#ContextMcpServer.-constructor), [`originalConsoleWarn`](index.ts.md#originalConsoleWarn), [`handlers.get-indexing-status.test.ts`](handlers.get-indexing-status.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-handlers.get-indexing-status.test.ts), [`setupTools`](index.ts.md#ContextMcpServer.setupTools), [`start`](index.ts.md#ContextMcpServer.start), [`toolHandlers`](index.ts.md#ContextMcpServer.toolHandlers)

