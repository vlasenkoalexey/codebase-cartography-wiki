---
title: 'Module: packages/core/src/utils/env-manager.ts'
type: catalog
provenance: extracted
module: packages/core/src/utils/env-manager.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/utils/`env-manager.ts`/
symbols:
  envManager: envManager.
  EnvManager.get: EnvManager#get().
  EnvManager.envFilePath: EnvManager#envFilePath.
  EnvManager.-constructor: EnvManager#`<constructor>`().
  EnvManager.set: EnvManager#set().
  EnvManager.getEnvFilePath: EnvManager#getEnvFilePath().
  EnvManager: EnvManager#
---
# Module: [`packages/core/src/utils/env-manager.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts)

## Classes
### `EnvManager`
- def: [`packages/core/src/utils/env-manager.ts:5`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L5)
- signature: `class EnvManager`
- members:
  - `<constructor>()` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L8)
  - `get(method)` — [`L17`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L17) — Get environment variable by name — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `getEnvFilePath(method)` — [`L95`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L95) — Get the path to the .env file
  - `set(method)` — [`L46`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L46) — Set environment variable to the .env file
  - `envFilePath` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L6) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- used by: [`<constructor>`](../context.ts.md#Context.-constructor), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`getCollectionName`](../context.ts.md#Context.getCollectionName), [`status`](../context.ts.md#Context.processFileList.Promise.typeLiteral113.status), [`<constructor>`](../vectordb/zilliz-utils.ts.md#ClusterManager.-constructor), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-utils-index.ts), [`getIsHybrid`](../context.ts.md#Context.getIsHybrid), [`getCustomExtensionsFromEnv`](../context.ts.md#Context.getCustomExtensionsFromEnv), [`getCustomIgnorePatternsFromEnv`](../context.ts.md#Context.getCustomIgnorePatternsFromEnv), [`env-manager.ts`](env-manager.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-utils-env-manager.ts)

## Module values
- `envManager` — [`L101`](../../../../../../../../raw/code/claude-context/packages/core/src/utils/env-manager.ts#L101) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)

