---
title: 'Module: packages/core/src/embedding/ollama-embedding.ts'
type: catalog
provenance: extracted
module: packages/core/src/embedding/ollama-embedding.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/embedding/`ollama-embedding.ts`/OllamaEmbedding
symbols:
  OllamaEmbedding.config: '#config.'
  OllamaEmbedding.-constructor: '#`<constructor>`().'
  OllamaEmbedding.embed: '#embed().'
  OllamaEmbedding.embedBatch: '#embedBatch().'
  OllamaEmbedding.detectDimension: '#detectDimension().'
  OllamaEmbedding.setModel: '#setModel().'
  OllamaEmbeddingConfig.model: Config#model.
  OllamaEmbeddingConfig.keepAlive: Config#keepAlive.
  OllamaEmbedding.dimension: '#dimension.'
  OllamaEmbedding.setHost: '#setHost().'
  OllamaEmbedding.setMaxTokens: '#setMaxTokens().'
  OllamaEmbedding.dimensionDetected: '#dimensionDetected.'
  OllamaEmbedding.client: '#client.'
  OllamaEmbeddingConfig.dimension: Config#dimension.
  OllamaEmbedding.maxTokens: '#maxTokens.'
  OllamaEmbedding.setKeepAlive: '#setKeepAlive().'
  OllamaEmbedding.setOptions: '#setOptions().'
  OllamaEmbedding: '#'
  OllamaEmbedding.setDefaultMaxTokensForModel: '#setDefaultMaxTokensForModel().'
  OllamaEmbeddingConfig: Config#
  OllamaEmbeddingConfig.options: Config#options.
  OllamaEmbeddingConfig.maxTokens: Config#maxTokens.
  OllamaEmbedding.getDimension: '#getDimension().'
  OllamaEmbedding.getClient: '#getClient().'
  OllamaEmbeddingConfig.host: Config#host.
  OllamaEmbeddingConfig.fetch: Config#fetch.
  OllamaEmbedding.getProvider: '#getProvider().'
---
# Module: [`packages/core/src/embedding/ollama-embedding.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts)

## Classes
### `OllamaEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/embedding/ollama-embedding.ts:14`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L14) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class OllamaEmbedding`
- members:
  - `<constructor>(config: OllamaEmbeddingConfig)` — [`L21`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L21) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `detectDimension(method)` — [`L198`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L198) — Detect embedding dimension — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embed(method)` — [`L57`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L57) — Generate text embedding vector — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `embedBatch(method)` — [`L91`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L91) — Generate text embedding vectors in batch — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `getClient(method)` — [`L194`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L194) — Get client instance (for advanced usage)
  - `getDimension(method)` — [`L127`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L127) — Get embedding vector dimension
  - `getProvider(method)` — [`L131`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L131) — Get service provider name
  - `setDefaultMaxTokensForModel(method)` — [`L46`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L46) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `setHost(method)` — [`L158`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L158) — Set host URL — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `setKeepAlive(method)` — [`L170`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L170) — Set keep alive duration — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `setMaxTokens(method)` — [`L186`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L186) — Set max tokens manually — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `setModel(method)` — [`L139`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L139) — Set model type and detect its dimension — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `setOptions(method)` — [`L178`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L178) — Set additional options — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `client` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L15) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `config` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L16) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `dimension` — [`L17`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L17) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `dimensionDetected` — [`L18`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L18) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `maxTokens` — [`L19`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L19) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](base-embedding.ts.md#Embedding), [`EmbeddingVector`](base-embedding.ts.md#EmbeddingVector), [`model`](ollama-embedding.ts.md#OllamaEmbeddingConfig.model), [`keepAlive`](ollama-embedding.ts.md#OllamaEmbeddingConfig.keepAlive), [`preprocessText`](base-embedding.ts.md#Embedding.preprocessText), [`preprocessTexts`](base-embedding.ts.md#Embedding.preprocessTexts), [`dimension`](ollama-embedding.ts.md#OllamaEmbeddingConfig.dimension), [`OllamaEmbeddingConfig`](ollama-embedding.ts.md#OllamaEmbeddingConfig), [`options`](ollama-embedding.ts.md#OllamaEmbeddingConfig.options), [`maxTokens`](ollama-embedding.ts.md#OllamaEmbeddingConfig.maxTokens), [`fetch`](ollama-embedding.ts.md#OllamaEmbeddingConfig.fetch), [`host`](ollama-embedding.ts.md#OllamaEmbeddingConfig.host)
- used by: [`Embedding`](base-embedding.ts.md#Embedding), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`EMBEDDING_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#EMBEDDING_PROVIDERS), [`embed`](base-embedding.ts.md#Embedding.embed), [`embedBatch`](base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](base-embedding.ts.md#Embedding.getDimension)

### `OllamaEmbeddingConfig`
- def: [`packages/core/src/embedding/ollama-embedding.ts:4`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L4) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
- signature: `interface OllamaEmbeddingConfig`
- members:
  - `dimension` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L10) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `fetch` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L7) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `host` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L6) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `keepAlive` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L8) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
  - `maxTokens` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L11) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `model` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L5) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
  - `options` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/embedding/ollama-embedding.ts#L9) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`config`](ollama-embedding.ts.md#OllamaEmbedding.config), [`<constructor>`](ollama-embedding.ts.md#OllamaEmbedding.-constructor), [`embed`](ollama-embedding.ts.md#OllamaEmbedding.embed), [`embedBatch`](ollama-embedding.ts.md#OllamaEmbedding.embedBatch), [`detectDimension`](ollama-embedding.ts.md#OllamaEmbedding.detectDimension), [`setModel`](ollama-embedding.ts.md#OllamaEmbedding.setModel), [`EmbeddingProviderConfig`](../../../vscode-extension/src/config/configManager.ts.md#EmbeddingProviderConfig), [`setHost`](ollama-embedding.ts.md#OllamaEmbedding.setHost), [`setMaxTokens`](ollama-embedding.ts.md#OllamaEmbedding.setMaxTokens), [`setKeepAlive`](ollama-embedding.ts.md#OllamaEmbedding.setKeepAlive), [`setOptions`](ollama-embedding.ts.md#OllamaEmbedding.setOptions)

