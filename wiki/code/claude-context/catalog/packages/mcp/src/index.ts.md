---
title: 'Module: packages/mcp/src/index.ts'
type: catalog
provenance: extracted
module: packages/mcp/src/index.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-mcp 0.1.15 src/`index.ts`/
symbols:
  ContextMcpServer.-constructor: ContextMcpServer#`<constructor>`().
  originalConsoleWarn: originalConsoleWarn.
  ContextMcpServer.setupTools: ContextMcpServer#setupTools().
  ContextMcpServer.start: ContextMcpServer#start().
  main: main().
  ContextMcpServer.toolHandlers: ContextMcpServer#toolHandlers.
  ContextMcpServer.snapshotManager: ContextMcpServer#snapshotManager.
  ContextMcpServer.syncManager: ContextMcpServer#syncManager.
  ContextMcpServer.server: ContextMcpServer#server.
  ContextMcpServer.context: ContextMcpServer#context.
  originalConsoleLog: originalConsoleLog.
  ContextMcpServer: ContextMcpServer#
---
# Module: [`packages/mcp/src/index.ts`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts)

## Classes
### `ContextMcpServer`
- def: [`packages/mcp/src/index.ts:34`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L34)
- signature: `class ContextMcpServer`
- members:
  - `<constructor>(config: ContextMcpConfig)` — [`L41`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L41)
  - `setupTools(method)` — [`L86`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L86) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `start(method)` — [`L249`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L249) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `context` — [`L36`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L36)
  - `server` — [`L35`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L35)
  - `snapshotManager` — [`L37`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L37)
  - `syncManager` — [`L38`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L38)
  - `toolHandlers` — [`L39`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L39)
- uses (calls/refs, reference-scoped): [`handleIndexCodebase`](handlers.ts.md#ToolHandlers.handleIndexCodebase), [`validateLegacyZeroEntries`](handlers.ts.md#ToolHandlers.validateLegacyZeroEntries), [`handleSearchCode`](handlers.ts.md#ToolHandlers.handleSearchCode), [`createEmbeddingInstance`](embedding.ts.md#createEmbeddingInstance), [`logEmbeddingProviderInfo`](embedding.ts.md#logEmbeddingProviderInfo), [`handleClearIndex`](handlers.ts.md#ToolHandlers.handleClearIndex), [`handleGetIndexingStatus`](handlers.ts.md#ToolHandlers.handleGetIndexingStatus), [`loadCodebaseSnapshot`](snapshot.ts.md#SnapshotManager.loadCodebaseSnapshot), [`embeddingModel`](config.ts.md#ContextMcpConfig.embeddingModel), [`startBackgroundSync`](sync.ts.md#SyncManager.startBackgroundSync), [`<constructor>`](handlers.ts.md#ToolHandlers.-constructor), [`SnapshotManager`](snapshot.ts.md#SnapshotManager), [`embeddingProvider`](config.ts.md#ContextMcpConfig.embeddingProvider), [`<constructor>`](snapshot.ts.md#SnapshotManager.-constructor), [`<constructor>`](sync.ts.md#SyncManager.-constructor), [`ContextMcpConfig`](config.ts.md#ContextMcpConfig), [`milvusToken`](config.ts.md#ContextMcpConfig.milvusToken), [`ToolHandlers`](handlers.ts.md#ToolHandlers), [`collectionNameOverride`](config.ts.md#ContextMcpConfig.collectionNameOverride), [`milvusAddress`](config.ts.md#ContextMcpConfig.milvusAddress), [`name`](config.ts.md#ContextMcpConfig.name), [`version`](config.ts.md#ContextMcpConfig.version), [`SyncManager`](sync.ts.md#SyncManager)
- used by: [`main`](index.ts.md#main)

## Functions
- `main()` — [`L273`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L273) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)

## Module values
- `originalConsoleLog` — [`L5`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L5)
- `originalConsoleWarn` — [`L6`](../../../../../../../raw/code/claude-context/packages/mcp/src/index.ts#L6) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)

