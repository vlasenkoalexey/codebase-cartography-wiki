---
title: 'Module: packages/core/src/splitter/index.ts'
type: catalog
provenance: extracted
module: packages/core/src/splitter/index.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/splitter/`index.ts`/
symbols:
  Splitter: Splitter#
  CodeChunk.metadata: CodeChunk#metadata.
  CodeChunk: CodeChunk#
  CodeChunk.content: CodeChunk#content.
  Splitter.split: Splitter#split().
  CodeChunk.metadata.typeLiteral52.startLine: CodeChunk#metadata.typeLiteral52:startLine.
  CodeChunk.metadata.typeLiteral52.filePath: CodeChunk#metadata.typeLiteral52:filePath.
  Splitter.setChunkSize: Splitter#setChunkSize().
  Splitter.setChunkOverlap: Splitter#setChunkOverlap().
  CodeChunk.metadata.typeLiteral52.endLine: CodeChunk#metadata.typeLiteral52:endLine.
  CodeChunk.metadata.typeLiteral52.language: CodeChunk#metadata.typeLiteral52:language.
  SplitterType: SplitterType#
  SplitterConfig.type: SplitterConfig#type.
  SplitterConfig.chunkSize: SplitterConfig#chunkSize.
  SplitterConfig.chunkOverlap: SplitterConfig#chunkOverlap.
  SplitterConfig: SplitterConfig#
  SplitterType.LANGCHAIN: SplitterType#LANGCHAIN.
  SplitterType.AST: SplitterType#AST.
---
# Module: [`packages/core/src/splitter/index.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts)

## Classes
### `CodeChunk`
- def: [`packages/core/src/splitter/index.ts:2`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L2) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
- signature: `interface CodeChunk`
- members:
  - `content` — [`L3`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L3) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `endLine` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L6) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `filePath` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L8) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `language` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L7) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `metadata` — [`L4`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L4) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `startLine` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L5) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
- used by: [`context.splitter.test.ts`](../context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`context.ignore-patterns.test.ts`](../context.ignore-patterns.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ignore-patterns.test.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`processChunkBatch`](../context.ts.md#Context.processChunkBatch), [`context.abort.test.ts`](../context.abort.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.abort.test.ts), [`context.embedding-error.test.ts`](../context.embedding-error.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.embedding-error.test.ts), [`split`](../context.splitter.test.ts.md#RecordingSplitter.split), [`status`](../context.ts.md#Context.processFileList.Promise.typeLiteral113.status), [`splitLargeChunk`](ast-splitter.ts.md#AstCodeSplitter.splitLargeChunk), [`split`](../context.abort.test.ts.md#CountingSplitter.split), [`extractChunks`](ast-splitter.ts.md#AstCodeSplitter.extractChunks), [`split`](index.ts.md#Splitter.split), [`split`](../context.embedding-error.test.ts.md#OneChunkSplitter.split), [`split`](../context.ignore-patterns.test.ts.md#TestSplitter.split), [`fallbackSplit`](langchain-splitter.ts.md#LangChainCodeSplitter.fallbackSplit), [`addOverlap`](ast-splitter.ts.md#AstCodeSplitter.addOverlap), [`split`](ast-splitter.ts.md#AstCodeSplitter.split), [`processChunkBuffer`](../context.ts.md#Context.processChunkBuffer), [`refineChunks`](ast-splitter.ts.md#AstCodeSplitter.refineChunks), [`split`](langchain-splitter.ts.md#LangChainCodeSplitter.split), [`ast-splitter.ts`](ast-splitter.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-splitter-ast-splitter.ts), [`langchain-splitter.ts`](langchain-splitter.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-splitter-langchain-splitter.ts), [`chunk`](../context.ts.md#Context.processChunkBuffer.chunkBuffer-Array.typeLiteral402.chunk)

### `Splitter`
- def: [`packages/core/src/splitter/index.ts:25`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L25) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
- signature: `interface Splitter`
- members:
  - `setChunkOverlap(method)` — [`L45`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L45) — Set chunk overlap size
  - `setChunkSize(method)` — [`L39`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L39) — Set chunk size
  - `split(method)` — [`L33`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L33) — Split code into code chunks — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
- uses (calls/refs, reference-scoped): [`CodeChunk`](index.ts.md#CodeChunk), [`split`](../context.splitter.test.ts.md#RecordingSplitter.split), [`split`](../context.abort.test.ts.md#CountingSplitter.split), [`split`](../context.embedding-error.test.ts.md#OneChunkSplitter.split), [`split`](../context.ignore-patterns.test.ts.md#TestSplitter.split), [`split`](ast-splitter.ts.md#AstCodeSplitter.split), [`split`](langchain-splitter.ts.md#LangChainCodeSplitter.split), [`TestSplitter`](../context.ignore-patterns.test.ts.md#TestSplitter), [`AstCodeSplitter`](ast-splitter.ts.md#AstCodeSplitter), [`LangChainCodeSplitter`](langchain-splitter.ts.md#LangChainCodeSplitter), [`OneChunkSplitter`](../context.embedding-error.test.ts.md#OneChunkSplitter), [`setChunkOverlap`](ast-splitter.ts.md#AstCodeSplitter.setChunkOverlap), [`setChunkSize`](ast-splitter.ts.md#AstCodeSplitter.setChunkSize), [`CountingSplitter`](../context.abort.test.ts.md#CountingSplitter), [`RecordingSplitter`](../context.splitter.test.ts.md#RecordingSplitter), [`setChunkOverlap`](langchain-splitter.ts.md#LangChainCodeSplitter.setChunkOverlap), [`setChunkSize`](langchain-splitter.ts.md#LangChainCodeSplitter.setChunkSize), [`setChunkOverlap`](../context.abort.test.ts.md#CountingSplitter.setChunkOverlap), [`setChunkOverlap`](../context.embedding-error.test.ts.md#OneChunkSplitter.setChunkOverlap), [`setChunkOverlap`](../context.ignore-patterns.test.ts.md#TestSplitter.setChunkOverlap), [`setChunkOverlap`](../context.splitter.test.ts.md#RecordingSplitter.setChunkOverlap), [`setChunkSize`](../context.abort.test.ts.md#CountingSplitter.setChunkSize), [`setChunkSize`](../context.embedding-error.test.ts.md#OneChunkSplitter.setChunkSize), [`setChunkSize`](../context.ignore-patterns.test.ts.md#TestSplitter.setChunkSize), [`setChunkSize`](../context.splitter.test.ts.md#RecordingSplitter.setChunkSize)
- used by: [`context.splitter.test.ts`](../context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`context.ignore-patterns.test.ts`](../context.ignore-patterns.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ignore-patterns.test.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`context.abort.test.ts`](../context.abort.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.abort.test.ts), [`context.embedding-error.test.ts`](../context.embedding-error.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.embedding-error.test.ts), [`status`](../context.ts.md#Context.processFileList.Promise.typeLiteral113.status), [`indexCodebase`](../context.ts.md#Context.indexCodebase), [`codeSplitter`](../context.ts.md#Context.codeSplitter), [`ast-splitter.ts`](ast-splitter.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-splitter-ast-splitter.ts), [`langchain-splitter.ts`](langchain-splitter.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-splitter-langchain-splitter.ts), [`TestSplitter`](../context.ignore-patterns.test.ts.md#TestSplitter), [`getCodeSplitter`](../context.ts.md#Context.getCodeSplitter), [`processFileList`](../context.ts.md#Context.processFileList), [`updateSplitter`](../context.ts.md#Context.updateSplitter), [`AstCodeSplitter`](ast-splitter.ts.md#AstCodeSplitter), [`reindexByChange`](../context.ts.md#Context.reindexByChange), [`LangChainCodeSplitter`](langchain-splitter.ts.md#LangChainCodeSplitter), [`OneChunkSplitter`](../context.embedding-error.test.ts.md#OneChunkSplitter), [`codeSplitter`](../context.ts.md#ContextConfig.codeSplitter), [`CountingSplitter`](../context.abort.test.ts.md#CountingSplitter), [`RecordingSplitter`](../context.splitter.test.ts.md#RecordingSplitter)

### `SplitterConfig`
- def: [`packages/core/src/splitter/index.ts:19`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L19) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- signature: `interface SplitterConfig`
- members:
  - `chunkOverlap` — [`L22`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L22) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `chunkSize` — [`L21`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L21) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `type` — [`L20`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L20) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- uses (calls/refs, reference-scoped): [`SplitterType`](index.ts.md#SplitterType)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`saveSplitterConfig`](../../../vscode-extension/src/config/configManager.ts.md#ConfigManager.saveSplitterConfig), [`getSplitterConfig`](../../../vscode-extension/src/config/configManager.ts.md#ConfigManager.getSplitterConfig), [`splitterConfig`](../../../vscode-extension/src/config/configManager.ts.md#PluginConfig.splitterConfig)

### `SplitterType`
- def: [`packages/core/src/splitter/index.ts:13`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L13) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- signature: `enum SplitterType`
- members:
  - `AST` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L15) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `LANGCHAIN` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/index.ts#L14)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`saveSplitterConfig`](../../../vscode-extension/src/config/configManager.ts.md#ConfigManager.saveSplitterConfig), [`getSplitterConfig`](../../../vscode-extension/src/config/configManager.ts.md#ConfigManager.getSplitterConfig), [`type`](index.ts.md#SplitterConfig.type)

