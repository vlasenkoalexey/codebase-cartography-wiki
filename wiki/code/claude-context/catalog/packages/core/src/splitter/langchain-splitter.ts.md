---
title: 'Module: packages/core/src/splitter/langchain-splitter.ts'
type: catalog
provenance: extracted
module: packages/core/src/splitter/langchain-splitter.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/splitter/`langchain-splitter.ts`/
symbols:
  LangChainCodeSplitter.fallbackSplit: LangChainCodeSplitter#fallbackSplit().
  LangChainCodeSplitter.split: LangChainCodeSplitter#split().
  LangChainCodeSplitter.-constructor: LangChainCodeSplitter#`<constructor>`().
  LangChainCodeSplitter.estimateLines: LangChainCodeSplitter#estimateLines().
  LangChainCodeSplitter: LangChainCodeSplitter#
  LangChainCodeSplitter.chunkSize: LangChainCodeSplitter#chunkSize.
  LangChainCodeSplitter.chunkOverlap: LangChainCodeSplitter#chunkOverlap.
  LangChainCodeSplitter.mapLanguage: LangChainCodeSplitter#mapLanguage().
  LangChainCodeSplitter.estimateLines.typeLiteral38.start: LangChainCodeSplitter#estimateLines().typeLiteral38:start.
  LangChainCodeSplitter.estimateLines.typeLiteral38.end: LangChainCodeSplitter#estimateLines().typeLiteral38:end.
  LangChainCodeSplitter.setChunkSize: LangChainCodeSplitter#setChunkSize().
  LangChainCodeSplitter.setChunkOverlap: LangChainCodeSplitter#setChunkOverlap().
  SupportedLanguage: SupportedLanguage#
---
# Module: [`packages/core/src/splitter/langchain-splitter.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts)

## Classes
### `LangChainCodeSplitter`  ·  implements/extends Splitter
- def: [`packages/core/src/splitter/langchain-splitter.ts:7`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L7) — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
- signature: `class LangChainCodeSplitter`
- members:
  - `<constructor>(chunkSize?: number | undefined, chunkOverlap?: number | undefined)` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L11)
  - `estimateLines(method)` — [`L115`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L115)
  - `fallbackSplit(method)` — [`L92`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L92) — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
  - `mapLanguage(method)` — [`L64`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L64)
  - `setChunkOverlap(method)` — [`L60`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L60) — Set chunk overlap size
  - `setChunkSize(method)` — [`L56`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L56) — Set chunk size
  - `split(method)` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L16) — Split code into code chunks — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
  - `chunkOverlap` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L9)
  - `chunkSize` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L8)
  - `end` — [`L115`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L115)
  - `start` — [`L115`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L115)
- uses (calls/refs, reference-scoped): [`Splitter`](index.ts.md#Splitter), [`CodeChunk`](index.ts.md#CodeChunk), [`SupportedLanguage`](langchain-splitter.ts.md#SupportedLanguage)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`Splitter`](index.ts.md#Splitter), [`SPLITTER_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#SPLITTER_PROVIDERS), [`split`](index.ts.md#Splitter.split), [`setChunkOverlap`](index.ts.md#Splitter.setChunkOverlap), [`setChunkSize`](index.ts.md#Splitter.setChunkSize)

### `SupportedLanguage`
- def: [`packages/core/src/splitter/langchain-splitter.ts:5`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/langchain-splitter.ts#L5)
- signature: `type SupportedLanguage`
- used by: [`mapLanguage`](langchain-splitter.ts.md#LangChainCodeSplitter.mapLanguage)

