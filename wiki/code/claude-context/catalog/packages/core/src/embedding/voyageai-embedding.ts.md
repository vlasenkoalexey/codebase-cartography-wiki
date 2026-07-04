---
title: 'Module: packages/core/src/embedding/voyageai-embedding.ts'
type: catalog
provenance: extracted
module: packages/core/src/embedding/voyageai-embedding.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/embedding/`voyageai-embedding.ts`/VoyageAIEmbedding
symbols:
  VoyageAIEmbedding.getSupportedModels.Record.typeLiteral7.dimension: '#getSupportedModels().Record:typeLiteral7:dimension.'
  VoyageAIEmbedding.getSupportedModels.Record.typeLiteral7.contextLength: '#getSupportedModels().Record:typeLiteral7:contextLength.'
  VoyageAIEmbedding.getSupportedModels.Record.typeLiteral7.description: '#getSupportedModels().Record:typeLiteral7:description.'
  VoyageAIEmbedding.embed: '#embed().'
  VoyageAIEmbedding.embedBatch: '#embedBatch().'
  VoyageAIEmbedding.-constructor: '#`<constructor>`().'
  VoyageAIEmbedding.updateModelSettings: '#updateModelSettings().'
  VoyageAIEmbedding.getSupportedModels: '#getSupportedModels().'
  VoyageAIEmbedding: '#'
  VoyageAIEmbeddingConfig.model: Config#model.
  VoyageAIEmbedding.setModel: '#setModel().'
  VoyageAIEmbedding.dimension: '#dimension.'
  VoyageAIEmbedding.config: '#config.'
  VoyageAIEmbedding.getDimension: '#getDimension().'
  VoyageAIEmbeddingConfig: Config#
  VoyageAIEmbedding.client: '#client.'
  VoyageAIEmbedding.detectDimension: '#detectDimension().'
  VoyageAIEmbeddingConfig.apiKey: Config#apiKey.
  VoyageAIEmbedding.inputType: '#inputType.'
  VoyageAIEmbedding.setInputType: '#setInputType().'
  VoyageAIEmbedding.getClient: '#getClient().'
  VoyageAIEmbedding.maxTokens: '#maxTokens.'
  VoyageAIEmbedding.getProvider: '#getProvider().'
---
# Module: [`packages/core/src/embedding/voyageai-embedding.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts)

## Classes
### `VoyageAIEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/embedding/voyageai-embedding.ts:9`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L9) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class VoyageAIEmbedding`
- members:
  - `<constructor>(config: VoyageAIEmbeddingConfig)` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L16)
  - `detectDimension(method)` — [`L48`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L48) — Detect embedding dimension
  - `embed(method)` — [`L53`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L53) — Generate text embedding vector — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embedBatch(method)` — [`L73`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L73) — Generate text embedding vectors in batch — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `getClient(method)` — [`L126`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L126) — Get client instance (for advanced usage)
  - `getDimension(method)` — [`L98`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L98) — Get embedding vector dimension
  - `getProvider(method)` — [`L102`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L102) — Get service provider name
  - `getSupportedModels(method)` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L133) — Get list of supported models — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `setInputType(method)` — [`L119`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L119) — Set input type (VoyageAI specific feature)
  - `setModel(method)` — [`L110`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L110) — Set model type
  - `updateModelSettings(method)` — [`L27`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L27) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `client` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L10) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `config` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L11) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `contextLength` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L133) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `description` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L133) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `dimension` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L12) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `dimension` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L133) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `inputType` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L13) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
  - `maxTokens` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L14) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](base-embedding.ts.md#Embedding), [`EmbeddingVector`](base-embedding.ts.md#EmbeddingVector), [`preprocessText`](base-embedding.ts.md#Embedding.preprocessText), [`model`](voyageai-embedding.ts.md#VoyageAIEmbeddingConfig.model), [`preprocessTexts`](base-embedding.ts.md#Embedding.preprocessTexts), [`VoyageAIEmbeddingConfig`](voyageai-embedding.ts.md#VoyageAIEmbeddingConfig), [`apiKey`](voyageai-embedding.ts.md#VoyageAIEmbeddingConfig.apiKey)
- used by: [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`Embedding`](base-embedding.ts.md#Embedding), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`EMBEDDING_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#EMBEDDING_PROVIDERS), [`embed`](base-embedding.ts.md#Embedding.embed), [`embedBatch`](base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](base-embedding.ts.md#Embedding.getProvider), [`voyageai-embedding.test.ts`](voyageai-embedding.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-embedding-voyageai-embedding.test.ts), [`detectDimension`](base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](base-embedding.ts.md#Embedding.getDimension)

### `VoyageAIEmbeddingConfig`
- def: [`packages/core/src/embedding/voyageai-embedding.ts:4`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L4) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
- signature: `interface VoyageAIEmbeddingConfig`
- members:
  - `apiKey` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L6)
  - `model` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/voyageai-embedding.ts#L5) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`voyageai-embedding.test.ts`](voyageai-embedding.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-embedding-voyageai-embedding.test.ts), [`embed`](voyageai-embedding.ts.md#VoyageAIEmbedding.embed), [`embedBatch`](voyageai-embedding.ts.md#VoyageAIEmbedding.embedBatch), [`<constructor>`](voyageai-embedding.ts.md#VoyageAIEmbedding.-constructor), [`EmbeddingProviderConfig`](../../../vscode-extension/src/config/configManager.ts.md#EmbeddingProviderConfig), [`setModel`](voyageai-embedding.ts.md#VoyageAIEmbedding.setModel), [`config`](voyageai-embedding.ts.md#VoyageAIEmbedding.config)

