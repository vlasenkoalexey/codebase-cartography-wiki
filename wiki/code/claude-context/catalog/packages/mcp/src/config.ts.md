---
title: 'Module: packages/mcp/src/config.ts'
type: catalog
provenance: extracted
module: packages/mcp/src/config.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-mcp 0.1.15 src/`config.ts`/
symbols:
  createMcpConfig: createMcpConfig().
  logConfigurationSummary: logConfigurationSummary().
  CodebaseInfoIndexing.status: CodebaseInfoIndexing#status.
  CodebaseInfoIndexFailed.status: CodebaseInfoIndexFailed#status.
  CodebaseInfoIndexed.status: CodebaseInfoIndexed#status.
  ContextMcpConfig.embeddingModel: ContextMcpConfig#embeddingModel.
  CodebaseInfo: CodebaseInfo#
  CodebaseSnapshotV1.indexingCodebases: CodebaseSnapshotV1#indexingCodebases.
  CodebaseIndexOptions.requestSplitter: CodebaseIndexOptions#requestSplitter.
  CodebaseIndexOptions: CodebaseIndexOptions#
  ContextMcpConfig.embeddingProvider: ContextMcpConfig#embeddingProvider.
  RequestSplitterType: RequestSplitterType#
  CodebaseIndexOptions.requestCustomExtensions: CodebaseIndexOptions#requestCustomExtensions.
  CodebaseIndexOptions.requestIgnorePatterns: CodebaseIndexOptions#requestIgnorePatterns.
  CodebaseSnapshot: CodebaseSnapshot#
  ContextMcpConfig.ollamaDimension: ContextMcpConfig#ollamaDimension.
  CodebaseSnapshotV2.codebases: CodebaseSnapshotV2#codebases.
  ContextMcpConfig: ContextMcpConfig#
  CodebaseInfoBase.lastUpdated: CodebaseInfoBase#lastUpdated.
  CodebaseInfoIndexed.indexedFiles: CodebaseInfoIndexed#indexedFiles.
  CodebaseInfoIndexing: CodebaseInfoIndexing#
  CodebaseInfoIndexed: CodebaseInfoIndexed#
  CodebaseInfoIndexFailed: CodebaseInfoIndexFailed#
  ContextMcpConfig.openaiBaseUrl: ContextMcpConfig#openaiBaseUrl.
  ContextMcpConfig.geminiBaseUrl: ContextMcpConfig#geminiBaseUrl.
  CodebaseInfoIndexing.indexingPercentage: CodebaseInfoIndexing#indexingPercentage.
  CodebaseInfoBase: CodebaseInfoBase#
  ContextMcpConfig.openaiApiKey: ContextMcpConfig#openaiApiKey.
  ContextMcpConfig.voyageaiApiKey: ContextMcpConfig#voyageaiApiKey.
  ContextMcpConfig.geminiApiKey: ContextMcpConfig#geminiApiKey.
  ContextMcpConfig.openrouterApiKey: ContextMcpConfig#openrouterApiKey.
  CodebaseInfoIndexed.totalChunks: CodebaseInfoIndexed#totalChunks.
  CodebaseSnapshotV2: CodebaseSnapshotV2#
  ContextMcpConfig.ollamaHost: ContextMcpConfig#ollamaHost.
  ContextMcpConfig.milvusToken: ContextMcpConfig#milvusToken.
  getEmbeddingModelForProvider: getEmbeddingModelForProvider().
  ContextMcpConfig.name: ContextMcpConfig#name.
  ContextMcpConfig.version: ContextMcpConfig#version.
  ContextMcpConfig.milvusAddress: ContextMcpConfig#milvusAddress.
  ContextMcpConfig.collectionNameOverride: ContextMcpConfig#collectionNameOverride.
  CodebaseSnapshotV1: CodebaseSnapshotV1#
  CodebaseInfoIndexed.indexStatus: CodebaseInfoIndexed#indexStatus.
  CodebaseInfoIndexFailed.errorMessage: CodebaseInfoIndexFailed#errorMessage.
  CodebaseInfoIndexFailed.lastAttemptedPercentage: CodebaseInfoIndexFailed#lastAttemptedPercentage.
  CodebaseSnapshotV1.indexedCodebases: CodebaseSnapshotV1#indexedCodebases.
  getDefaultModelForProvider: getDefaultModelForProvider().
  showHelpMessage: showHelpMessage().
  ContextMcpConfig.ollamaModel: ContextMcpConfig#ollamaModel.
  CodebaseSnapshotV2.formatVersion: CodebaseSnapshotV2#formatVersion.
  CodebaseSnapshotV2.lastUpdated: CodebaseSnapshotV2#lastUpdated.
  getPositiveIntegerFromEnv: getPositiveIntegerFromEnv().
  CodebaseSnapshotV1.lastUpdated: CodebaseSnapshotV1#lastUpdated.
---
# Module: [`packages/mcp/src/config.ts`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts)

## Classes
### `CodebaseIndexOptions`
- def: [`packages/mcp/src/config.ts:39`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L39) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `interface CodebaseIndexOptions`
- members:
  - `requestCustomExtensions` — [`L41`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L41) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `requestIgnorePatterns` — [`L42`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L42) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `requestSplitter` — [`L40`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L40) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- uses (calls/refs, reference-scoped): [`RequestSplitterType`](config.ts.md#RequestSplitterType)
- used by: [`handleIndexCodebase`](handlers.ts.md#ToolHandlers.handleIndexCodebase), [`snapshot.request-options.test.ts`](snapshot.request-options.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.request-options.test.ts), [`setCodebaseIndexed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed), [`handleSyncIndex`](sync.ts.md#SyncManager.handleSyncIndex), [`handlers.ts`](handlers.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-handlers.ts), [`setCodebaseIndexing`](snapshot.ts.md#SnapshotManager.setCodebaseIndexing), [`setCodebaseIndexFailed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed), [`startBackgroundIndexing`](handlers.ts.md#ToolHandlers.startBackgroundIndexing), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexOptions`](snapshot.ts.md#SnapshotManager.getIndexOptions), [`resolveIndexOptions`](snapshot.ts.md#SnapshotManager.resolveIndexOptions), [`CodebaseInfoBase`](config.ts.md#CodebaseInfoBase)

### `CodebaseInfo`
- def: [`packages/mcp/src/config.ts:72`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L72) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `type CodebaseInfo`
- uses (calls/refs, reference-scoped): [`CodebaseInfoIndexed`](config.ts.md#CodebaseInfoIndexed), [`CodebaseInfoIndexing`](config.ts.md#CodebaseInfoIndexing), [`CodebaseInfoIndexFailed`](config.ts.md#CodebaseInfoIndexFailed)
- used by: [`saveCodebaseSnapshot`](snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot), [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`mergeExternalEntry`](snapshot.ts.md#SnapshotManager.mergeExternalEntry), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`codebaseInfoMap`](snapshot.ts.md#SnapshotManager.codebaseInfoMap), [`getCodebaseInfo`](snapshot.ts.md#SnapshotManager.getCodebaseInfo), [`codebases`](config.ts.md#CodebaseSnapshotV2.codebases)

### `CodebaseInfoBase`
- def: [`packages/mcp/src/config.ts:46`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L46) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- signature: `interface CodebaseInfoBase`
- members:
  - `lastUpdated` — [`L47`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L47) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- uses (calls/refs, reference-scoped): [`CodebaseIndexOptions`](config.ts.md#CodebaseIndexOptions)
- used by: [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`setCodebaseIndexed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed), [`loadV1Format`](snapshot.ts.md#SnapshotManager.loadV1Format), [`setCodebaseIndexing`](snapshot.ts.md#SnapshotManager.setCodebaseIndexing), [`setCodebaseIndexFailed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed), [`addIndexedCodebase`](snapshot.ts.md#SnapshotManager.addIndexedCodebase), [`addIndexingCodebase`](snapshot.ts.md#SnapshotManager.addIndexingCodebase), [`updateIndexingProgress`](snapshot.ts.md#SnapshotManager.updateIndexingProgress), [`CodebaseInfoIndexed`](config.ts.md#CodebaseInfoIndexed), [`CodebaseInfoIndexing`](config.ts.md#CodebaseInfoIndexing), [`CodebaseInfoIndexFailed`](config.ts.md#CodebaseInfoIndexFailed)

### `CodebaseInfoIndexFailed`
- def: [`packages/mcp/src/config.ts:65`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L65) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- signature: `interface CodebaseInfoIndexFailed`
- members:
  - `errorMessage` — [`L67`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L67) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `lastAttemptedPercentage` — [`L68`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L68) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `status` — [`L66`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L66) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- uses (calls/refs, reference-scoped): [`CodebaseInfoBase`](config.ts.md#CodebaseInfoBase)
- used by: [`snapshot.request-options.test.ts`](snapshot.request-options.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.request-options.test.ts), [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`validateLegacyZeroEntries`](handlers.ts.md#ToolHandlers.validateLegacyZeroEntries), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`setCodebaseIndexFailed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexFailed), [`mergeExternalEntry`](snapshot.ts.md#SnapshotManager.mergeExternalEntry), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`CodebaseInfo`](config.ts.md#CodebaseInfo), [`getCodebaseStatus`](snapshot.ts.md#SnapshotManager.getCodebaseStatus), [`getFailedCodebases`](snapshot.ts.md#SnapshotManager.getFailedCodebases)

### `CodebaseInfoIndexed`
- def: [`packages/mcp/src/config.ts:57`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L57) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `interface CodebaseInfoIndexed`
- members:
  - `indexStatus` — [`L61`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L61) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `indexedFiles` — [`L59`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L59) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `status` — [`L58`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L58) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `totalChunks` — [`L60`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L60) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- uses (calls/refs, reference-scoped): [`CodebaseInfoBase`](config.ts.md#CodebaseInfoBase)
- used by: [`snapshot.request-options.test.ts`](snapshot.request-options.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.request-options.test.ts), [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`setCodebaseIndexed`](snapshot.ts.md#SnapshotManager.setCodebaseIndexed), [`validateLegacyZeroEntries`](handlers.ts.md#ToolHandlers.validateLegacyZeroEntries), [`loadV1Format`](snapshot.ts.md#SnapshotManager.loadV1Format), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`mergeExternalEntry`](snapshot.ts.md#SnapshotManager.mergeExternalEntry), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`addIndexedCodebase`](snapshot.ts.md#SnapshotManager.addIndexedCodebase), [`CodebaseInfo`](config.ts.md#CodebaseInfo), [`getCodebaseStatus`](snapshot.ts.md#SnapshotManager.getCodebaseStatus), [`getFailedCodebases`](snapshot.ts.md#SnapshotManager.getFailedCodebases)

### `CodebaseInfoIndexing`
- def: [`packages/mcp/src/config.ts:51`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L51) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `interface CodebaseInfoIndexing`
- members:
  - `indexingPercentage` — [`L53`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L53) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `status` — [`L52`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L52) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- uses (calls/refs, reference-scoped): [`CodebaseInfoBase`](config.ts.md#CodebaseInfoBase)
- used by: [`snapshot.request-options.test.ts`](snapshot.request-options.test.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.request-options.test.ts), [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`validateLegacyZeroEntries`](handlers.ts.md#ToolHandlers.validateLegacyZeroEntries), [`setCodebaseIndexing`](snapshot.ts.md#SnapshotManager.setCodebaseIndexing), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`mergeExternalEntry`](snapshot.ts.md#SnapshotManager.mergeExternalEntry), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`CodebaseInfo`](config.ts.md#CodebaseInfo), [`addIndexingCodebase`](snapshot.ts.md#SnapshotManager.addIndexingCodebase), [`updateIndexingProgress`](snapshot.ts.md#SnapshotManager.updateIndexingProgress), [`getCodebaseStatus`](snapshot.ts.md#SnapshotManager.getCodebaseStatus), [`getFailedCodebases`](snapshot.ts.md#SnapshotManager.getFailedCodebases)

### `CodebaseSnapshot`
- def: [`packages/mcp/src/config.ts:81`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L81) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `type CodebaseSnapshot`
- uses (calls/refs, reference-scoped): [`CodebaseSnapshotV2`](config.ts.md#CodebaseSnapshotV2), [`CodebaseSnapshotV1`](config.ts.md#CodebaseSnapshotV1)
- used by: [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`loadCodebaseSnapshot`](snapshot.ts.md#SnapshotManager.loadCodebaseSnapshot)

### `CodebaseSnapshotV1`
- def: [`packages/mcp/src/config.ts:28`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L28) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- signature: `interface CodebaseSnapshotV1`
- members:
  - `indexedCodebases` — [`L29`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L29) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `indexingCodebases` — [`L30`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L30) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `lastUpdated` — [`L31`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L31)
- used by: [`loadV1Format`](snapshot.ts.md#SnapshotManager.loadV1Format), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`CodebaseSnapshot`](config.ts.md#CodebaseSnapshot)

### `CodebaseSnapshotV2`
- def: [`packages/mcp/src/config.ts:74`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L74) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- signature: `interface CodebaseSnapshotV2`
- members:
  - `codebases` — [`L76`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L76) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
  - `formatVersion` — [`L75`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L75) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
  - `lastUpdated` — [`L77`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L77) — documented in [packages-mcp-src-snapshot.ts](../../../../concepts/packages-mcp-src-snapshot.ts.md)
- uses (calls/refs, reference-scoped): [`CodebaseInfo`](config.ts.md#CodebaseInfo)
- used by: [`saveCodebaseSnapshot`](snapshot.ts.md#SnapshotManager.saveCodebaseSnapshot), [`loadV2Format`](snapshot.ts.md#SnapshotManager.loadV2Format), [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`getIndexingCodebases`](snapshot.ts.md#SnapshotManager.getIndexingCodebases), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-snapshot.ts), [`getIndexingProgress`](snapshot.ts.md#SnapshotManager.getIndexingProgress), [`CodebaseSnapshot`](config.ts.md#CodebaseSnapshot), [`isV2Format`](snapshot.ts.md#SnapshotManager.isV2Format)

### `ContextMcpConfig`
- def: [`packages/mcp/src/config.ts:3`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L3) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- signature: `interface ContextMcpConfig`
- members:
  - `collectionNameOverride` — [`L24`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L24) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `embeddingModel` — [`L8`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L8) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `embeddingProvider` — [`L7`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L7) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `geminiApiKey` — [`L13`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L13) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `geminiBaseUrl` — [`L14`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L14) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `milvusAddress` — [`L22`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L22) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `milvusToken` — [`L23`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L23) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `name` — [`L4`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L4) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `ollamaDimension` — [`L20`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L20) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `ollamaHost` — [`L19`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L19) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `ollamaModel` — [`L18`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L18) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `openaiApiKey` — [`L10`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L10) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `openaiBaseUrl` — [`L11`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L11) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `openrouterApiKey` — [`L16`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L16) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `version` — [`L5`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L5) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
  - `voyageaiApiKey` — [`L12`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L12) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- used by: [`<constructor>`](index.ts.md#ContextMcpServer.-constructor), [`createMcpConfig`](config.ts.md#createMcpConfig), [`logConfigurationSummary`](config.ts.md#logConfigurationSummary), [`originalConsoleWarn`](index.ts.md#originalConsoleWarn), [`createEmbeddingInstance`](embedding.ts.md#createEmbeddingInstance), [`logEmbeddingProviderInfo`](embedding.ts.md#logEmbeddingProviderInfo), [`embedding.ts`](embedding.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-embedding.ts)

### `RequestSplitterType`
- def: [`packages/mcp/src/config.ts:36`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L36) — documented in [packages-mcp-src-handlers.ts](../../../../concepts/packages-mcp-src-handlers.ts.md)
- signature: `type RequestSplitterType`
- used by: [`handleIndexCodebase`](handlers.ts.md#ToolHandlers.handleIndexCodebase), [`handleSyncIndex`](sync.ts.md#SyncManager.handleSyncIndex), [`handlers.ts`](handlers.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-handlers.ts), [`startBackgroundIndexing`](handlers.ts.md#ToolHandlers.startBackgroundIndexing), [`sync.ts`](sync.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-sync.ts), [`requestSplitter`](config.ts.md#CodebaseIndexOptions.requestSplitter), [`resolveRequestSplitterType`](splitter.ts.md#resolveRequestSplitterType), [`splitter.ts`](splitter.ts.md#scip-typescript-npm-zilliz-claude-context-mcp-0.1.15-src-splitter.ts), [`createRequestSplitter`](splitter.ts.md#createRequestSplitter), [`isRequestSplitterType`](splitter.ts.md#isRequestSplitterType)

## Functions
- `createMcpConfig()` — [`L136`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L136) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- `getDefaultModelForProvider(provider: string)` — [`L84`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L84) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- `getEmbeddingModelForProvider(provider: string)` — [`L102`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L102) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- `getPositiveIntegerFromEnv(name: string)` — [`L121`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L121) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- `logConfigurationSummary(config: ContextMcpConfig)` — [`L176`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L176) — documented in [packages-mcp-src-config.ts](../../../../concepts/packages-mcp-src-config.ts.md)
- `showHelpMessage()` — [`L220`](../../../../../../../raw/code/claude-context/packages/mcp/src/config.ts#L220)

