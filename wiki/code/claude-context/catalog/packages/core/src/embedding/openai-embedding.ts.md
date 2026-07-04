---
title: 'Module: packages/core/src/embedding/openai-embedding.ts'
type: catalog
provenance: extracted
module: packages/core/src/embedding/openai-embedding.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/embedding/`openai-embedding.ts`/OpenAIEmbedding
symbols:
  OpenAIEmbedding.embed: '#embed().'
  OpenAIEmbedding.embedBatch: '#embedBatch().'
  OpenAIEmbedding.detectDimension: '#detectDimension().'
  OpenAIEmbedding.setModel: '#setModel().'
  OpenAIEmbedding.getDimension: '#getDimension().'
  OpenAIEmbedding.dimension: '#dimension.'
  OpenAIEmbedding.-constructor: '#`<constructor>`().'
  OpenAIEmbedding: '#'
  OpenAIEmbedding.getSupportedModels: '#getSupportedModels().'
  OpenAIEmbedding.getSupportedModels.Record.typeLiteral7.dimension: '#getSupportedModels().Record:typeLiteral7:dimension.'
  OpenAIEmbedding.config: '#config.'
  OpenAIEmbeddingConfig.model: Config#model.
  OpenAIEmbedding.client: '#client.'
  OpenAIEmbeddingConfig: Config#
  OpenAIEmbedding.getSupportedModels.Record.typeLiteral7.description: '#getSupportedModels().Record:typeLiteral7:description.'
  OpenAIEmbedding.getClient: '#getClient().'
  OpenAIEmbeddingConfig.apiKey: Config#apiKey.
  OpenAIEmbeddingConfig.baseURL: Config#baseURL.
  OpenAIEmbedding.maxTokens: '#maxTokens.'
  OpenAIEmbedding.getProvider: '#getProvider().'
---
# Module: [`packages/core/src/embedding/openai-embedding.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts)

## Classes
### `OpenAIEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/embedding/openai-embedding.ts:10`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L10) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class OpenAIEmbedding`
- members:
  - `<constructor>(config: OpenAIEmbeddingConfig)` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L16)
  - `detectDimension(method)` — [`L25`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L25) — Detect embedding dimension — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embed(method)` — [`L56`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L56) — Generate text embedding vector — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embedBatch(method)` — [`L87`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L87) — Generate text embedding vectors in batch — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `getClient(method)` — [`L154`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L154) — Get client instance (for advanced usage)
  - `getDimension(method)` — [`L117`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L117) — Get embedding vector dimension
  - `getProvider(method)` — [`L133`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L133) — Get service provider name
  - `getSupportedModels(method)` — [`L161`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L161) — Get list of supported models — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `setModel(method)` — [`L141`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L141) — Set model type — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `client` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L11) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `config` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L12) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `description` — [`L161`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L161) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `dimension` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L13) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `dimension` — [`L161`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L161) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
  - `maxTokens` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L14) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](base-embedding.ts.md#Embedding), [`EmbeddingVector`](base-embedding.ts.md#EmbeddingVector), [`preprocessText`](base-embedding.ts.md#Embedding.preprocessText), [`model`](openai-embedding.ts.md#OpenAIEmbeddingConfig.model), [`preprocessTexts`](base-embedding.ts.md#Embedding.preprocessTexts), [`OpenAIEmbeddingConfig`](openai-embedding.ts.md#OpenAIEmbeddingConfig), [`apiKey`](openai-embedding.ts.md#OpenAIEmbeddingConfig.apiKey), [`baseURL`](openai-embedding.ts.md#OpenAIEmbeddingConfig.baseURL)
- used by: [`<constructor>`](../context.ts.md#Context.-constructor), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`Embedding`](base-embedding.ts.md#Embedding), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`EMBEDDING_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#EMBEDDING_PROVIDERS), [`embed`](base-embedding.ts.md#Embedding.embed), [`embedBatch`](base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](base-embedding.ts.md#Embedding.getDimension)

### `OpenAIEmbeddingConfig`
- def: [`packages/core/src/embedding/openai-embedding.ts:4`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L4) — documented in [packages-core-src-embedding-openai-embedding.ts](../../../../../concepts/packages-core-src-embedding-openai-embedding.ts.md)
- signature: `interface OpenAIEmbeddingConfig`
- members:
  - `apiKey` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L6)
  - `baseURL` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L7)
  - `model` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/openai-embedding.ts#L5) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- used by: [`<constructor>`](../context.ts.md#Context.-constructor), [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`embed`](openai-embedding.ts.md#OpenAIEmbedding.embed), [`embedBatch`](openai-embedding.ts.md#OpenAIEmbedding.embedBatch), [`detectDimension`](openai-embedding.ts.md#OpenAIEmbedding.detectDimension), [`setModel`](openai-embedding.ts.md#OpenAIEmbedding.setModel), [`EmbeddingProviderConfig`](../../../vscode-extension/src/config/configManager.ts.md#EmbeddingProviderConfig), [`getDimension`](openai-embedding.ts.md#OpenAIEmbedding.getDimension), [`<constructor>`](openai-embedding.ts.md#OpenAIEmbedding.-constructor), [`config`](openai-embedding.ts.md#OpenAIEmbedding.config)

