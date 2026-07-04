---
title: 'Module: packages/chrome-extension/src/config/milvusConfig.ts'
type: catalog
provenance: extracted
module: packages/chrome-extension/src/config/milvusConfig.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-chrome-extension 0.1.4 src/config/`milvusConfig.ts`/
symbols:
  MilvusConfigManager.getMilvusConfig: MilvusConfigManager#getMilvusConfig().
  MilvusConfigManager.saveMilvusConfig: MilvusConfigManager#saveMilvusConfig().
  MilvusConfigManager: MilvusConfigManager#
  MilvusConfigManager.validateMilvusConfig: MilvusConfigManager#validateMilvusConfig().
  MilvusConfig.address: MilvusConfig#address.
  MilvusConfigManager.getOpenAIConfig: MilvusConfigManager#getOpenAIConfig().
  MilvusConfig: MilvusConfig#
  MilvusConfig.token: MilvusConfig#token.
  MilvusConfig.username: MilvusConfig#username.
  MilvusConfig.database: MilvusConfig#database.
  MilvusConfig.password: MilvusConfig#password.
  ChromeStorageConfig: ChromeStorageConfig#
  ChromeStorageConfig.openaiToken: ChromeStorageConfig#openaiToken.
  ChromeStorageConfig.milvusAddress: ChromeStorageConfig#milvusAddress.
  ChromeStorageConfig.milvusToken: ChromeStorageConfig#milvusToken.
  ChromeStorageConfig.milvusUsername: ChromeStorageConfig#milvusUsername.
  ChromeStorageConfig.milvusPassword: ChromeStorageConfig#milvusPassword.
  ChromeStorageConfig.milvusDatabase: ChromeStorageConfig#milvusDatabase.
  ChromeStorageConfig.githubToken: ChromeStorageConfig#githubToken.
---
# Module: [`packages/chrome-extension/src/config/milvusConfig.ts`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts)

## Classes
### `ChromeStorageConfig`
- def: [`packages/chrome-extension/src/config/milvusConfig.ts:9`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L9) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
- signature: `interface ChromeStorageConfig`
- members:
  - `githubToken` — [`L10`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L10)
  - `milvusAddress` — [`L12`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L12) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `milvusDatabase` — [`L16`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L16) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `milvusPassword` — [`L15`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L15) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `milvusToken` — [`L13`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L13) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `milvusUsername` — [`L14`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L14) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `openaiToken` — [`L11`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L11)
- used by: [`getMilvusConfig`](milvusConfig.ts.md#MilvusConfigManager.getMilvusConfig), [`getOpenAIConfig`](milvusConfig.ts.md#MilvusConfigManager.getOpenAIConfig)

### `MilvusConfig`
- def: [`packages/chrome-extension/src/config/milvusConfig.ts:1`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L1) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
- signature: `interface MilvusConfig`
- members:
  - `address` — [`L2`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L2) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `database` — [`L6`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L6) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `password` — [`L5`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L5) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `token` — [`L3`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L3) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `username` — [`L4`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L4) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- used by: [`getMilvusConfig`](milvusConfig.ts.md#MilvusConfigManager.getMilvusConfig), [`initialize`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.initialize), [`testConnection`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.testConnection), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`saveMilvusConfig`](milvusConfig.ts.md#MilvusConfigManager.saveMilvusConfig), [`validateMilvusConfig`](milvusConfig.ts.md#MilvusConfigManager.validateMilvusConfig)

### `MilvusConfigManager`
- def: [`packages/chrome-extension/src/config/milvusConfig.ts:19`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L19) — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
- signature: `class MilvusConfigManager`
- members:
  - `getMilvusConfig(method)` — [`L23`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L23) — Get Milvus configuration from Chrome storage — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `getOpenAIConfig(method)` — [`L80`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L80) — Get OpenAI configuration — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `saveMilvusConfig(method)` — [`L59`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L59) — Save Milvus configuration to Chrome storage — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `validateMilvusConfig(method)` — [`L99`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/config/milvusConfig.ts#L99) — Validate Milvus configuration — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- uses (calls/refs, reference-scoped): [`address`](milvusConfig.ts.md#MilvusConfig.address), [`MilvusConfig`](milvusConfig.ts.md#MilvusConfig), [`database`](milvusConfig.ts.md#MilvusConfig.database), [`token`](milvusConfig.ts.md#MilvusConfig.token), [`username`](milvusConfig.ts.md#MilvusConfig.username), [`password`](milvusConfig.ts.md#MilvusConfig.password), [`ChromeStorageConfig`](milvusConfig.ts.md#ChromeStorageConfig), [`milvusAddress`](milvusConfig.ts.md#ChromeStorageConfig.milvusAddress), [`openaiToken`](milvusConfig.ts.md#ChromeStorageConfig.openaiToken), [`milvusDatabase`](milvusConfig.ts.md#ChromeStorageConfig.milvusDatabase), [`milvusPassword`](milvusConfig.ts.md#ChromeStorageConfig.milvusPassword), [`milvusToken`](milvusConfig.ts.md#ChromeStorageConfig.milvusToken), [`milvusUsername`](milvusConfig.ts.md#ChromeStorageConfig.milvusUsername)
- used by: [`background.ts`](../background.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-background.ts), [`initialize`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.initialize), [`testConnection`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.testConnection), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`getConfig`](../background.ts.md#EmbeddingModel.getConfig)

