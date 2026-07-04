---
title: 'Module: packages/core/src/embedding/gemini-embedding.ts'
type: catalog
provenance: extracted
module: packages/core/src/embedding/gemini-embedding.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/embedding/`gemini-embedding.ts`/Gemini
symbols:
  GeminiEmbedding.-constructor: Embedding#`<constructor>`().
  GeminiEmbedding.embedBatch: Embedding#embedBatch().
  GeminiEmbedding.getSupportedDimensions: Embedding#getSupportedDimensions().
  GeminiEmbedding.updateDimensionForModel: Embedding#updateDimensionForModel().
  GeminiEmbedding.getSupportedModels: Embedding#getSupportedModels().
  GeminiEmbedding.embedProcessedText: Embedding#embedProcessedText().
  GeminiEmbedding.embed: Embedding#embed().
  GeminiEmbeddingConfig.model: EmbeddingConfig#model.
  GeminiEmbedding.config: Embedding#config.
  GeminiEmbedding: Embedding#
  GeminiEmbedding.dimension: Embedding#dimension.
  GeminiEmbedding.setModel: Embedding#setModel().
  GeminiEmbedding.setOutputDimensionality: Embedding#setOutputDimensionality().
  GeminiEmbeddingConfig.apiKey: EmbeddingConfig#apiKey.
  GeminiEmbeddingConfig.outputDimensionality: EmbeddingConfig#outputDimensionality.
  GeminiEmbeddingConfig: EmbeddingConfig#
  GeminiEmbedding.client: Embedding#client.
  GeminiEmbedding.getDimension: Embedding#getDimension().
  GeminiModelInfo.typeLiteral1.dimension: ModelInfo#typeLiteral1:dimension.
  GeminiModelInfo.typeLiteral1.contextLength: ModelInfo#typeLiteral1:contextLength.
  GeminiModelInfo.typeLiteral1.supportedDimensions: ModelInfo#typeLiteral1:supportedDimensions.
  GeminiEmbedding.detectDimension: Embedding#detectDimension().
  GeminiEmbedding.getClient: Embedding#getClient().
  GeminiEmbedding.isDimensionSupported: Embedding#isDimensionSupported().
  GeminiModelInfo.typeLiteral1.description: ModelInfo#typeLiteral1:description.
  GeminiEmbeddingConfig.baseURL: EmbeddingConfig#baseURL.
  GeminiEmbedding.maxTokens: Embedding#maxTokens.
  GeminiModelInfo: ModelInfo#
  GeminiEmbedding.getProvider: Embedding#getProvider().
---
# Module: [`packages/core/src/embedding/gemini-embedding.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts)

## Classes
### `GeminiEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/embedding/gemini-embedding.ts:18`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L18) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class GeminiEmbedding`
- members:
  - `<constructor>(config: GeminiEmbeddingConfig)` — [`L24`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L24) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `detectDimension(method)` — [`L59`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L59) — Detect embedding dimension
  - `embed(method)` — [`L64`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L64) — Generate text embedding vector — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embedBatch(method)` — [`L75`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L75) — Generate text embedding vectors in batch — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embedProcessedText(method)` — [`L114`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L114) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `getClient(method)` — [`L162`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L162) — Get client instance (for advanced usage)
  - `getDimension(method)` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L133) — Get embedding vector dimension
  - `getProvider(method)` — [`L137`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L137) — Get service provider name
  - `getSupportedDimensions(method)` — [`L189`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L189) — Get supported dimensions for the current model — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `getSupportedModels(method)` — [`L169`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L169) — Get list of supported models — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `isDimensionSupported(method)` — [`L197`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L197) — Validate if a dimension is supported by the current model — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `setModel(method)` — [`L145`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L145) — Set model type — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `setOutputDimensionality(method)` — [`L154`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L154) — Set output dimensionality
  - `updateDimensionForModel(method)` — [`L45`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L45) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `client` — [`L19`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L19) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `config` — [`L20`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L20) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `dimension` — [`L21`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L21) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `maxTokens` — [`L22`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L22) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](base-embedding.ts.md#Embedding), [`EmbeddingVector`](base-embedding.ts.md#EmbeddingVector), [`model`](gemini-embedding.ts.md#GeminiEmbeddingConfig.model), [`preprocessText`](base-embedding.ts.md#Embedding.preprocessText), [`preprocessTexts`](base-embedding.ts.md#Embedding.preprocessTexts), [`apiKey`](gemini-embedding.ts.md#GeminiEmbeddingConfig.apiKey), [`outputDimensionality`](gemini-embedding.ts.md#GeminiEmbeddingConfig.outputDimensionality), [`GeminiEmbeddingConfig`](gemini-embedding.ts.md#GeminiEmbeddingConfig), [`contextLength`](gemini-embedding.ts.md#GeminiModelInfo.typeLiteral1.contextLength), [`dimension`](gemini-embedding.ts.md#GeminiModelInfo.typeLiteral1.dimension), [`supportedDimensions`](gemini-embedding.ts.md#GeminiModelInfo.typeLiteral1.supportedDimensions), [`baseURL`](gemini-embedding.ts.md#GeminiEmbeddingConfig.baseURL), [`description`](gemini-embedding.ts.md#GeminiModelInfo.typeLiteral1.description), [`GeminiModelInfo`](gemini-embedding.ts.md#GeminiModelInfo)
- used by: [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`Embedding`](base-embedding.ts.md#Embedding), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`EMBEDDING_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#EMBEDDING_PROVIDERS), [`gemini-embedding.test.ts`](gemini-embedding.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-embedding-gemini-embedding.test.ts), [`embed`](base-embedding.ts.md#Embedding.embed), [`embedBatch`](base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](base-embedding.ts.md#Embedding.getDimension)

### `GeminiEmbeddingConfig`
- def: [`packages/core/src/embedding/gemini-embedding.ts:11`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L11) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
- signature: `interface GeminiEmbeddingConfig`
- members:
  - `apiKey` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L13) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `baseURL` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L14) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `model` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L12) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `outputDimensionality` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L15) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`<constructor>`](gemini-embedding.ts.md#GeminiEmbedding.-constructor), [`gemini-embedding.test.ts`](gemini-embedding.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-embedding-gemini-embedding.test.ts), [`embedBatch`](gemini-embedding.ts.md#GeminiEmbedding.embedBatch), [`getSupportedDimensions`](gemini-embedding.ts.md#GeminiEmbedding.getSupportedDimensions), [`EmbeddingProviderConfig`](../../../vscode-extension/src/config/configManager.ts.md#EmbeddingProviderConfig), [`embedProcessedText`](gemini-embedding.ts.md#GeminiEmbedding.embedProcessedText), [`embed`](gemini-embedding.ts.md#GeminiEmbedding.embed), [`config`](gemini-embedding.ts.md#GeminiEmbedding.config), [`setModel`](gemini-embedding.ts.md#GeminiEmbedding.setModel), [`setOutputDimensionality`](gemini-embedding.ts.md#GeminiEmbedding.setOutputDimensionality)

### `GeminiModelInfo`
- def: [`packages/core/src/embedding/gemini-embedding.ts:4`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L4) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
- signature: `type GeminiModelInfo`
- members:
  - `contextLength` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L6) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `description` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L7) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `dimension` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L5) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
  - `supportedDimensions` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/gemini-embedding.ts#L8) — documented in [packages-core-src-embedding-gemini-embedding.ts](../../../../../concepts/packages-core-src-embedding-gemini-embedding.ts.md)
- used by: [`getSupportedDimensions`](gemini-embedding.ts.md#GeminiEmbedding.getSupportedDimensions), [`updateDimensionForModel`](gemini-embedding.ts.md#GeminiEmbedding.updateDimensionForModel), [`getSupportedModels`](gemini-embedding.ts.md#GeminiEmbedding.getSupportedModels)

