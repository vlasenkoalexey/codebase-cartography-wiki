---
title: 'Module: src/constants.ts'
type: catalog
provenance: extracted
module: src/constants.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/`constants.ts`/
symbols:
  OpenWikiProvider: OpenWikiProvider#
  PROVIDER_CONFIGS: PROVIDER_CONFIGS.
  OPENWIKI_MODEL_ID_ENV_KEY: OPENWIKI_MODEL_ID_ENV_KEY.
  OPEN_WIKI_DIR: OPEN_WIKI_DIR.
  getProviderApiKeyEnvKey: getProviderApiKeyEnvKey().
  getDefaultModelId: getDefaultModelId().
  resolveConfiguredProvider: resolveConfiguredProvider().
  ProviderModelOption.typeLiteral0.id: ProviderModelOption#typeLiteral0:id.
  getProviderLabel: getProviderLabel().
  OPENWIKI_PROVIDER_ENV_KEY: OPENWIKI_PROVIDER_ENV_KEY.
  ProviderModelOption.typeLiteral0.label: ProviderModelOption#typeLiteral0:label.
  getProviderModelOptions: getProviderModelOptions().
  UPDATE_METADATA_PATH: UPDATE_METADATA_PATH.
  SELECTABLE_OPENWIKI_PROVIDERS: SELECTABLE_OPENWIKI_PROVIDERS.
  getProviderConfig: getProviderConfig().
  isValidModelId: isValidModelId().
  DEFAULT_MODEL_ID: DEFAULT_MODEL_ID.
  ProviderConfig.typeLiteral1.modelOptions: ProviderConfig#typeLiteral1:modelOptions.
  OPENROUTER_API_KEY_ENV_KEY: OPENROUTER_API_KEY_ENV_KEY.
  SUGGESTED_MODEL_IDS: SUGGESTED_MODEL_IDS.
  normalizeProvider: normalizeProvider().
  normalizeModelId: normalizeModelId().
  BASETEN_API_KEY_ENV_KEY: BASETEN_API_KEY_ENV_KEY.
  FIREWORKS_API_KEY_ENV_KEY: FIREWORKS_API_KEY_ENV_KEY.
  OPENAI_API_KEY_ENV_KEY: OPENAI_API_KEY_ENV_KEY.
  ANTHROPIC_API_KEY_ENV_KEY: ANTHROPIC_API_KEY_ENV_KEY.
  DEFAULT_PROVIDER: DEFAULT_PROVIDER.
  ProviderConfig.typeLiteral1.baseURL: ProviderConfig#typeLiteral1:baseURL.
  ProviderConfig.typeLiteral1.apiKeyEnvKey: ProviderConfig#typeLiteral1:apiKeyEnvKey.
  ProviderConfig.typeLiteral1.label: ProviderConfig#typeLiteral1:label.
  isValidProvider: isValidProvider().
  OPENROUTER_BASE_URL: OPENROUTER_BASE_URL.
  SelectableOpenWikiProvider: SelectableOpenWikiProvider#
  OPENWIKI_VERSION: OPENWIKI_VERSION.
  ProviderModelOption: ProviderModelOption#
  ProviderConfig: ProviderConfig#
  OPENROUTER_FALLBACK_MODEL_IDS: OPENROUTER_FALLBACK_MODEL_IDS.
---
# Module: [`src/constants.ts`](../../../../../raw/code/openwiki/src/constants.ts)

## Classes
### `OpenWikiProvider`
- def: [`src/constants.ts:13`](../../../../../raw/code/openwiki/src/constants.ts#L13) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- signature: `type OpenWikiProvider`
- used by: [`App`](cli.tsx.md#App), [`InitSetup`](credentials.tsx.md#InitSetup), [`cli.tsx`](cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`index.ts`](agent/index.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-index.ts), [`runOpenWikiAgentCore`](agent/index.ts.md#runOpenWikiAgentCore), [`credentials.tsx`](credentials.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-credentials.tsx), [`PROVIDER_CONFIGS`](constants.ts.md#PROVIDER_CONFIGS), [`runOpenWikiAgentWithModelFallbacks`](agent/index.ts.md#runOpenWikiAgentWithModelFallbacks), [`getProviderApiKeyEnvKey`](constants.ts.md#getProviderApiKeyEnvKey), [`getDefaultModelId`](constants.ts.md#getDefaultModelId), [`resolveConfiguredProvider`](constants.ts.md#resolveConfiguredProvider), [`syncMenuStateForInput`](cli.tsx.md#syncMenuStateForInput), [`getProviderLabel`](constants.ts.md#getProviderLabel), [`createModel`](agent/index.ts.md#createModel), [`resolveModelId`](agent/index.ts.md#resolveModelId), [`getModelMenuOptions`](cli.tsx.md#getModelMenuOptions), [`moveMenuSelection`](cli.tsx.md#moveMenuSelection), [`getModelSelectionOptions`](credentials.tsx.md#getModelSelectionOptions), [`getProviderModelOptions`](constants.ts.md#getProviderModelOptions), [`getInitialStep`](credentials.tsx.md#getInitialStep), [`getProviderConfig`](constants.ts.md#getProviderConfig), [`getNextStepAfterProvider`](credentials.tsx.md#getNextStepAfterProvider), [`getProviderSetupDetail`](credentials.tsx.md#getProviderSetupDetail), [`getSelectedModelId`](credentials.tsx.md#getSelectedModelId), [`normalizeProvider`](constants.ts.md#normalizeProvider), [`getNextStepAfterApiKey`](credentials.tsx.md#getNextStepAfterApiKey), [`ensureProviderKey`](agent/index.ts.md#ensureProviderKey), [`getModelSetupDetail`](credentials.tsx.md#getModelSetupDetail), [`createModelRoute`](agent/index.ts.md#createModelRoute), [`getModelSelectionIndex`](credentials.tsx.md#getModelSelectionIndex), [`getProviderSelectionIndex`](credentials.tsx.md#getProviderSelectionIndex), [`getCurrentModelOptionIndex`](cli.tsx.md#getCurrentModelOptionIndex), [`getCurrentProviderOptionIndex`](cli.tsx.md#getCurrentProviderOptionIndex), [`provider`](credentials.tsx.md#InitSetupResult.typeLiteral7.provider), [`isValidProvider`](constants.ts.md#isValidProvider), [`currentProvider`](cli.tsx.md#ChatInputProps.typeLiteral236.currentProvider), [`onProviderSelect`](cli.tsx.md#ChatInputProps.typeLiteral236.onProviderSelect), [`currentProvider`](cli.tsx.md#SlashMenu.-currentModelId-currentProvider-input-menuState-.typeLiteral1143.currentProvider), [`provider`](credentials.tsx.md#PromptProps.typeLiteral176.provider), [`SelectableOpenWikiProvider`](constants.ts.md#SelectableOpenWikiProvider)  (+1 more)

### `ProviderConfig`
- def: [`src/constants.ts:27`](../../../../../raw/code/openwiki/src/constants.ts#L27)
- signature: `type ProviderConfig`
- members:
  - `apiKeyEnvKey` — [`L28`](../../../../../raw/code/openwiki/src/constants.ts#L28)
  - `baseURL` — [`L29`](../../../../../raw/code/openwiki/src/constants.ts#L29)
  - `label` — [`L30`](../../../../../raw/code/openwiki/src/constants.ts#L30)
  - `modelOptions` — [`L31`](../../../../../raw/code/openwiki/src/constants.ts#L31) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- uses (calls/refs, reference-scoped): [`ProviderModelOption`](constants.ts.md#ProviderModelOption)
- used by: [`runOpenWikiAgent`](agent/index.ts.md#runOpenWikiAgent), [`PROVIDER_CONFIGS`](constants.ts.md#PROVIDER_CONFIGS), [`getProviderApiKeyEnvKey`](constants.ts.md#getProviderApiKeyEnvKey), [`getProviderLabel`](constants.ts.md#getProviderLabel), [`createModel`](agent/index.ts.md#createModel), [`getProviderModelOptions`](constants.ts.md#getProviderModelOptions), [`getProviderConfig`](constants.ts.md#getProviderConfig), [`DEFAULT_MODEL_ID`](constants.ts.md#DEFAULT_MODEL_ID), [`SUGGESTED_MODEL_IDS`](constants.ts.md#SUGGESTED_MODEL_IDS)

### `ProviderModelOption`
- def: [`src/constants.ts:22`](../../../../../raw/code/openwiki/src/constants.ts#L22)
- signature: `type ProviderModelOption`
- members:
  - `id` — [`L23`](../../../../../raw/code/openwiki/src/constants.ts#L23) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
  - `label` — [`L24`](../../../../../raw/code/openwiki/src/constants.ts#L24) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- used by: [`PROVIDER_CONFIGS`](constants.ts.md#PROVIDER_CONFIGS), [`getDefaultModelId`](constants.ts.md#getDefaultModelId), [`getModelMenuOptions`](cli.tsx.md#getModelMenuOptions), [`getModelSelectionOptions`](credentials.tsx.md#getModelSelectionOptions), [`getProviderModelOptions`](constants.ts.md#getProviderModelOptions), [`DEFAULT_MODEL_ID`](constants.ts.md#DEFAULT_MODEL_ID), [`modelOptions`](constants.ts.md#ProviderConfig.typeLiteral1.modelOptions), [`SUGGESTED_MODEL_IDS`](constants.ts.md#SUGGESTED_MODEL_IDS)

### `SelectableOpenWikiProvider`
- def: [`src/constants.ts:20`](../../../../../raw/code/openwiki/src/constants.ts#L20)
- signature: `type SelectableOpenWikiProvider`
- uses (calls/refs, reference-scoped): [`OpenWikiProvider`](constants.ts.md#OpenWikiProvider)
- used by: [`SELECTABLE_OPENWIKI_PROVIDERS`](constants.ts.md#SELECTABLE_OPENWIKI_PROVIDERS)

## Functions
- `getDefaultModelId(provider: OpenWikiProvider)` — [`L127`](../../../../../raw/code/openwiki/src/constants.ts#L127) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `getProviderApiKeyEnvKey(provider: OpenWikiProvider)` — [`L117`](../../../../../raw/code/openwiki/src/constants.ts#L117) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `getProviderConfig(provider: OpenWikiProvider)` — [`L109`](../../../../../raw/code/openwiki/src/constants.ts#L109) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `getProviderLabel(provider: OpenWikiProvider)` — [`L113`](../../../../../raw/code/openwiki/src/constants.ts#L113) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `getProviderModelOptions(provider: OpenWikiProvider)` — [`L121`](../../../../../raw/code/openwiki/src/constants.ts#L121) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `isValidModelId(value: string)` — [`L160`](../../../../../raw/code/openwiki/src/constants.ts#L160) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- `isValidProvider(value: string)` — [`L143`](../../../../../raw/code/openwiki/src/constants.ts#L143) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `normalizeModelId(value: string)` — [`L156`](../../../../../raw/code/openwiki/src/constants.ts#L156) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- `normalizeProvider(value: string | null | undefined)` — [`L131`](../../../../../raw/code/openwiki/src/constants.ts#L131) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `resolveConfiguredProvider(env?: NodeJS.ProcessEnv)` — [`L147`](../../../../../raw/code/openwiki/src/constants.ts#L147) — documented in [openwiki-agent-index.ts](../../concepts/openwiki-agent-index.ts.md)

## Module values
- `ANTHROPIC_API_KEY_ENV_KEY` — [`L6`](../../../../../raw/code/openwiki/src/constants.ts#L6) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `BASETEN_API_KEY_ENV_KEY` — [`L3`](../../../../../raw/code/openwiki/src/constants.ts#L3) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `DEFAULT_MODEL_ID` — [`L97`](../../../../../raw/code/openwiki/src/constants.ts#L97) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `DEFAULT_PROVIDER` — [`L10`](../../../../../raw/code/openwiki/src/constants.ts#L10)
- `FIREWORKS_API_KEY_ENV_KEY` — [`L4`](../../../../../raw/code/openwiki/src/constants.ts#L4) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `OPENAI_API_KEY_ENV_KEY` — [`L5`](../../../../../raw/code/openwiki/src/constants.ts#L5) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `OPENROUTER_API_KEY_ENV_KEY` — [`L7`](../../../../../raw/code/openwiki/src/constants.ts#L7) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `OPENROUTER_BASE_URL` — [`L11`](../../../../../raw/code/openwiki/src/constants.ts#L11)
- `OPENROUTER_FALLBACK_MODEL_IDS` — [`L100`](../../../../../raw/code/openwiki/src/constants.ts#L100)
- `OPENWIKI_MODEL_ID_ENV_KEY` — [`L9`](../../../../../raw/code/openwiki/src/constants.ts#L9) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `OPENWIKI_PROVIDER_ENV_KEY` — [`L8`](../../../../../raw/code/openwiki/src/constants.ts#L8) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `OPENWIKI_VERSION` — [`L171`](../../../../../raw/code/openwiki/src/constants.ts#L171)
- `OPEN_WIKI_DIR` — [`L1`](../../../../../raw/code/openwiki/src/constants.ts#L1) — documented in [openwiki-agent-index.ts](../../concepts/openwiki-agent-index.ts.md)
- `PROVIDER_CONFIGS` — [`L42`](../../../../../raw/code/openwiki/src/constants.ts#L42) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `SELECTABLE_OPENWIKI_PROVIDERS` — [`L34`](../../../../../raw/code/openwiki/src/constants.ts#L34) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `SUGGESTED_MODEL_IDS` — [`L105`](../../../../../raw/code/openwiki/src/constants.ts#L105) — documented in [openwiki-constants.ts](../../concepts/openwiki-constants.ts.md)
- `UPDATE_METADATA_PATH` — [`L2`](../../../../../raw/code/openwiki/src/constants.ts#L2) — documented in [openwiki-agent-index.ts](../../concepts/openwiki-agent-index.ts.md)

