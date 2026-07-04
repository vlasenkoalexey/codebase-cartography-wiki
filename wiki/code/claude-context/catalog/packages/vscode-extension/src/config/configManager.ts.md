---
title: 'Module: packages/vscode-extension/src/config/configManager.ts'
type: catalog
provenance: extracted
module: packages/vscode-extension/src/config/configManager.ts
status: fresh
symbol_base: scip-typescript npm semanticcodesearch 0.1.11 src/config/`configManager.ts`/
symbols:
  EMBEDDING_PROVIDERS: EMBEDDING_PROVIDERS.
  SPLITTER_PROVIDERS: SPLITTER_PROVIDERS.
  FieldDefinition.typeLiteral27.name: FieldDefinition#typeLiteral27:name.
  ConfigManager.saveSplitterConfig: ConfigManager#saveSplitterConfig().
  ConfigManager: ConfigManager#
  FieldDefinition.typeLiteral27.type: FieldDefinition#typeLiteral27:type.
  FieldDefinition.typeLiteral27.description: FieldDefinition#typeLiteral27:description.
  FieldDefinition.typeLiteral27.inputType: FieldDefinition#typeLiteral27:inputType.
  ConfigManager.getSplitterConfig: ConfigManager#getSplitterConfig().
  EmbeddingProviderConfig: EmbeddingProviderConfig#
  FieldDefinition: FieldDefinition#
  ConfigManager.saveEmbeddingProviderConfig: ConfigManager#saveEmbeddingProviderConfig().
  ConfigManager.saveMilvusConfig: ConfigManager#saveMilvusConfig().
  ConfigManager.getEmbeddingProviderConfig: ConfigManager#getEmbeddingProviderConfig().
  ConfigManager.getMilvusFullConfig: ConfigManager#getMilvusFullConfig().
  FieldDefinition.typeLiteral27.placeholder: FieldDefinition#typeLiteral27:placeholder.
  ConfigManager.getMilvusConfig: ConfigManager#getMilvusConfig().
  ConfigManager.buildConfigObject: ConfigManager#buildConfigObject().
  ConfigManager.createEmbeddingInstance: ConfigManager#createEmbeddingInstance().
  FieldDefinition.typeLiteral27.required: FieldDefinition#typeLiteral27:required.
  ConfigManager.CONFIG_KEY: ConfigManager#CONFIG_KEY.
  ConfigManager.getProviderInfo: ConfigManager#getProviderInfo().
  MilvusWebConfig.address: MilvusWebConfig#address.
  ConfigManager.-constructor: ConfigManager#`<constructor>`().
  ConfigManager.getSupportedProviders: ConfigManager#getSupportedProviders().
  MilvusWebConfig: MilvusWebConfig#
  PluginConfig.embeddingProvider: PluginConfig#embeddingProvider.
  PluginConfig.splitterProvider: PluginConfig#splitterProvider.
  PluginConfig.milvusConfig: PluginConfig#milvusConfig.
  PluginConfig.splitterConfig: PluginConfig#splitterConfig.
  ConfigManager.getSplitterProviderInfo: ConfigManager#getSplitterProviderInfo().
  ConfigManager.getSupportedProviders.Record.typeLiteral82.requiredFields: ConfigManager#getSupportedProviders().Record:typeLiteral82:requiredFields.
  ConfigManager.getSupportedProviders.Record.typeLiteral82.optionalFields: ConfigManager#getSupportedProviders().Record:typeLiteral82:optionalFields.
  MilvusWebConfig.token: MilvusWebConfig#token.
  SplitterProviderConfig: SplitterProviderConfig#
  ConfigManager.context: ConfigManager#context.
  PluginConfig: PluginConfig#
  ConfigManager.getSupportedProviders.Record.typeLiteral82.name: ConfigManager#getSupportedProviders().Record:typeLiteral82:name.
  ConfigManager.getSupportedProviders.Record.typeLiteral82.models: ConfigManager#getSupportedProviders().Record:typeLiteral82:models.
  ConfigManager.getSupportedProviders.Record.typeLiteral82.defaultConfig: ConfigManager#getSupportedProviders().Record:typeLiteral82:defaultConfig.
---
# Module: [`packages/vscode-extension/src/config/configManager.ts`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts)

## Classes
### `ConfigManager`
- def: [`packages/vscode-extension/src/config/configManager.ts:139`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L139) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- signature: `class ConfigManager`
- members:
  - `<constructor>(context: vscode.ExtensionContext)` — [`L143`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L143)
  - `buildConfigObject(method)` — [`L170`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L170) — Build configuration object — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `createEmbeddingInstance(method)` — [`L256`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L256) — Create embedding instance
  - `getEmbeddingProviderConfig(method)` — [`L198`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L198) — Get embedding provider configuration
  - `getMilvusConfig(method)` — [`L296`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L296) — Get Milvus frontend configuration
  - `getMilvusFullConfig(method)` — [`L330`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L330) — Convert frontend configuration to complete MilvusConfig
  - `getProviderInfo(method)` — [`L150`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L150) — Get embedding provider configuration information — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `getSplitterConfig(method)` — [`L347`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L347) — Get splitter configuration
  - `getSplitterProviderInfo(method)` — [`L160`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L160) — Get splitter provider configuration information — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `getSupportedProviders(method)` — [`L267`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L267) — Get supported embedding providers — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `saveEmbeddingProviderConfig(method)` — [`L216`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L216) — Save embedding provider configuration — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `saveMilvusConfig(method)` — [`L312`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L312) — Save Milvus frontend configuration
  - `saveSplitterConfig(method)` — [`L372`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L372) — Save splitter configuration — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `CONFIG_KEY` — [`L140`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L140) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `context` — [`L141`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L141)
  - `defaultConfig` — [`L272`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L272)
  - `models` — [`L269`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L269)
  - `name` — [`L268`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L268)
  - `optionalFields` — [`L271`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L271)
  - `requiredFields` — [`L270`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L270)
- uses (calls/refs, reference-scoped): [`EMBEDDING_PROVIDERS`](configManager.ts.md#EMBEDDING_PROVIDERS), [`SPLITTER_PROVIDERS`](configManager.ts.md#SPLITTER_PROVIDERS), [`name`](configManager.ts.md#FieldDefinition.typeLiteral27.name), [`EmbeddingProviderConfig`](configManager.ts.md#EmbeddingProviderConfig), [`FieldDefinition`](configManager.ts.md#FieldDefinition), [`SplitterType`](../../../core/src/splitter/index.ts.md#SplitterType), [`type`](../../../core/src/splitter/index.ts.md#SplitterConfig.type), [`chunkOverlap`](../../../core/src/splitter/index.ts.md#SplitterConfig.chunkOverlap), [`chunkSize`](../../../core/src/splitter/index.ts.md#SplitterConfig.chunkSize), [`MilvusConfig`](../../../core/src/vectordb/milvus-vectordb.ts.md#MilvusConfig), [`SplitterConfig`](../../../core/src/splitter/index.ts.md#SplitterConfig), [`address`](configManager.ts.md#MilvusWebConfig.address), [`MilvusWebConfig`](configManager.ts.md#MilvusWebConfig), [`AST`](../../../core/src/splitter/index.ts.md#SplitterType.AST), [`token`](configManager.ts.md#MilvusWebConfig.token)
- used by: [`reloadContextConfiguration`](../extension.ts.md#reloadContextConfiguration), [`createContextWithConfig`](../extension.ts.md#createContextWithConfig), [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`semanticSearchProvider.ts`](../webview/semanticSearchProvider.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-webview-semanticSearchProvider.ts), [`<constructor>`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.-constructor), [`sendCurrentConfig`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.sendCurrentConfig), [`saveConfig`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.saveConfig), [`configManager`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.configManager), [`configManager`](../extension.ts.md#configManager), [`testEmbedding`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.testEmbedding)

### `EmbeddingProviderConfig`
- def: [`packages/vscode-extension/src/config/configManager.ts:10`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L10)
- signature: `type EmbeddingProviderConfig`
- uses (calls/refs, reference-scoped): [`GeminiEmbeddingConfig`](../../../core/src/embedding/gemini-embedding.ts.md#GeminiEmbeddingConfig), [`OllamaEmbeddingConfig`](../../../core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig), [`OpenAIEmbeddingConfig`](../../../core/src/embedding/openai-embedding.ts.md#OpenAIEmbeddingConfig), [`VoyageAIEmbeddingConfig`](../../../core/src/embedding/voyageai-embedding.ts.md#VoyageAIEmbeddingConfig)
- used by: [`semanticSearchProvider.ts`](../webview/semanticSearchProvider.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-webview-semanticSearchProvider.ts), [`saveConfig`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.saveConfig), [`saveEmbeddingProviderConfig`](configManager.ts.md#ConfigManager.saveEmbeddingProviderConfig), [`getEmbeddingProviderConfig`](configManager.ts.md#ConfigManager.getEmbeddingProviderConfig), [`embeddingProvider`](configManager.ts.md#PluginConfig.embeddingProvider)

### `FieldDefinition`
- def: [`packages/vscode-extension/src/config/configManager.ts:39`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L39) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- signature: `type FieldDefinition`
- members:
  - `description` — [`L42`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L42) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `inputType` — [`L43`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L43) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `name` — [`L40`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L40) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `placeholder` — [`L44`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L44) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `required` — [`L45`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L45) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `type` — [`L41`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L41) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- used by: [`EMBEDDING_PROVIDERS`](configManager.ts.md#EMBEDDING_PROVIDERS), [`SPLITTER_PROVIDERS`](configManager.ts.md#SPLITTER_PROVIDERS), [`saveEmbeddingProviderConfig`](configManager.ts.md#ConfigManager.saveEmbeddingProviderConfig), [`buildConfigObject`](configManager.ts.md#ConfigManager.buildConfigObject), [`optionalFields`](configManager.ts.md#ConfigManager.getSupportedProviders.Record.typeLiteral82.optionalFields), [`requiredFields`](configManager.ts.md#ConfigManager.getSupportedProviders.Record.typeLiteral82.requiredFields)

### `MilvusWebConfig`
- def: [`packages/vscode-extension/src/config/configManager.ts:5`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L5)
- signature: `interface MilvusWebConfig`
- members:
  - `address` — [`L6`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L6)
  - `token` — [`L7`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L7)
- used by: [`saveMilvusConfig`](configManager.ts.md#ConfigManager.saveMilvusConfig), [`getMilvusFullConfig`](configManager.ts.md#ConfigManager.getMilvusFullConfig), [`getMilvusConfig`](configManager.ts.md#ConfigManager.getMilvusConfig), [`milvusConfig`](configManager.ts.md#PluginConfig.milvusConfig)

### `PluginConfig`
- def: [`packages/vscode-extension/src/config/configManager.ts:32`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L32)
- signature: `interface PluginConfig`
- members:
  - `embeddingProvider` — [`L33`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L33)
  - `milvusConfig` — [`L35`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L35)
  - `splitterConfig` — [`L36`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L36)
  - `splitterProvider` — [`L34`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L34)
- uses (calls/refs, reference-scoped): [`EmbeddingProviderConfig`](configManager.ts.md#EmbeddingProviderConfig), [`SplitterConfig`](../../../core/src/splitter/index.ts.md#SplitterConfig), [`MilvusWebConfig`](configManager.ts.md#MilvusWebConfig), [`SplitterProviderConfig`](configManager.ts.md#SplitterProviderConfig)

### `SplitterProviderConfig`
- def: [`packages/vscode-extension/src/config/configManager.ts:24`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L24)
- signature: `type SplitterProviderConfig`
- used by: [`splitterProvider`](configManager.ts.md#PluginConfig.splitterProvider)

## Module values
- `EMBEDDING_PROVIDERS` — [`L49`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L49) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- `SPLITTER_PROVIDERS` — [`L110`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/config/configManager.ts#L110) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)

