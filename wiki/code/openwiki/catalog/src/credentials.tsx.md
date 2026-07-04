---
title: 'Module: src/credentials.tsx'
type: catalog
provenance: extracted
module: src/credentials.tsx
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/`credentials.tsx`/
symbols:
  InitSetup: InitSetup().
  Prompt: Prompt().
  getModelSelectionOptions: getModelSelectionOptions().
  SetupStep: SetupStep().
  SetupPanel: SetupPanel().
  getInitialStep: getInitialStep().
  needsCredentialSetup: needsCredentialSetup().
  getNextStepAfterProvider: getNextStepAfterProvider().
  getProviderSetupDetail: getProviderSetupDetail().
  getSelectedModelId: getSelectedModelId().
  getNextStepAfterApiKey: getNextStepAfterApiKey().
  getModelSetupDetail: getModelSetupDetail().
  getProviderSelectionIndex: getProviderSelectionIndex().
  getModelSelectionIndex: getModelSelectionIndex().
  InitSetupResult.typeLiteral7.provider: InitSetupResult#typeLiteral7:provider.
  SetupStepProps.typeLiteral174.label: SetupStepProps#typeLiteral174:label.
  SetupStepProps.typeLiteral174.state: SetupStepProps#typeLiteral174:state.
  SetupStepProps.typeLiteral174.detail: SetupStepProps#typeLiteral174:detail.
  SelectionMarker: SelectionMarker().
  PromptStep: PromptStep#
  InitSetupProps.typeLiteral8.onComplete: InitSetupProps#typeLiteral8:onComplete.
  PromptProps.typeLiteral176.provider: PromptProps#typeLiteral176:provider.
  PromptProps.typeLiteral176.step: PromptProps#typeLiteral176:step.
  InitSetupResult.typeLiteral7.modelId: InitSetupResult#typeLiteral7:modelId.
  SetupPanelProps.typeLiteral175.title: SetupPanelProps#typeLiteral175:title.
  SelectionMarker.-isSelected-.typeLiteral275.isSelected: SelectionMarker().(`{ isSelected
    }`)typeLiteral275:isSelected.
  getProviderArticle: getProviderArticle().
  InitSetupResult: InitSetupResult#
  InitSetupResult.typeLiteral7.savedApiKey: InitSetupResult#typeLiteral7:savedApiKey.
  InitSetupResult.typeLiteral7.savedLangSmithKey: InitSetupResult#typeLiteral7:savedLangSmithKey.
  InitSetupResult.typeLiteral7.savedModelId: InitSetupResult#typeLiteral7:savedModelId.
  InitSetupResult.typeLiteral7.savedProvider: InitSetupResult#typeLiteral7:savedProvider.
  InitSetupProps.typeLiteral8.modelIdOverride: InitSetupProps#typeLiteral8:modelIdOverride.
  InitSetupProps.typeLiteral8.onError: InitSetupProps#typeLiteral8:onError.
  PromptProps.typeLiteral176.input: PromptProps#typeLiteral176:input.
  PromptProps.typeLiteral176.isCustomModelInput: PromptProps#typeLiteral176:isCustomModelInput.
  PromptProps.typeLiteral176.modelSelectionIndex: PromptProps#typeLiteral176:modelSelectionIndex.
  PromptProps.typeLiteral176.providerSelectionIndex: PromptProps#typeLiteral176:providerSelectionIndex.
  moveSelectionIndex: moveSelectionIndex().
  mask: mask().
  InitSetupProps: InitSetupProps#
  SetupHeader: SetupHeader().
  SetupStepProps: SetupStepProps#
  SetupPanelProps: SetupPanelProps#
  SetupPanelProps.typeLiteral175.children: SetupPanelProps#typeLiteral175:children.
  PromptProps: PromptProps#
  ModelSelectionOption: ModelSelectionOption#
  sanitizeInputChunk: sanitizeInputChunk().
---
# Module: [`src/credentials.tsx`](../../../../../raw/code/openwiki/src/credentials.tsx)

## Classes
### `InitSetupProps`
- def: [`src/credentials.tsx:28`](../../../../../raw/code/openwiki/src/credentials.tsx#L28)
- signature: `type InitSetupProps`
- members:
  - `modelIdOverride` — [`L29`](../../../../../raw/code/openwiki/src/credentials.tsx#L29)
  - `onComplete` — [`L30`](../../../../../raw/code/openwiki/src/credentials.tsx#L30)
  - `onError` — [`L31`](../../../../../raw/code/openwiki/src/credentials.tsx#L31)
- uses (calls/refs, reference-scoped): [`InitSetupResult`](credentials.tsx.md#InitSetupResult)
- used by: [`App`](cli.tsx.md#App), [`InitSetup`](credentials.tsx.md#InitSetup)

### `InitSetupResult`
- def: [`src/credentials.tsx:19`](../../../../../raw/code/openwiki/src/credentials.tsx#L19)
- signature: `type InitSetupResult`
- members:
  - `modelId` — [`L20`](../../../../../raw/code/openwiki/src/credentials.tsx#L20)
  - `provider` — [`L21`](../../../../../raw/code/openwiki/src/credentials.tsx#L21)
  - `savedApiKey` — [`L22`](../../../../../raw/code/openwiki/src/credentials.tsx#L22)
  - `savedLangSmithKey` — [`L23`](../../../../../raw/code/openwiki/src/credentials.tsx#L23)
  - `savedModelId` — [`L24`](../../../../../raw/code/openwiki/src/credentials.tsx#L24)
  - `savedProvider` — [`L25`](../../../../../raw/code/openwiki/src/credentials.tsx#L25)
- uses (calls/refs, reference-scoped): [`OpenWikiProvider`](constants.ts.md#OpenWikiProvider)
- used by: [`App`](cli.tsx.md#App), [`InitSetup`](credentials.tsx.md#InitSetup), [`cli.tsx`](cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`RunState`](cli.tsx.md#RunState), [`onComplete`](credentials.tsx.md#InitSetupProps.typeLiteral8.onComplete)

### `ModelSelectionOption`
- def: [`src/credentials.tsx:703`](../../../../../raw/code/openwiki/src/credentials.tsx#L703)
- signature: `type ModelSelectionOption`
- used by: [`getModelSelectionOptions`](credentials.tsx.md#getModelSelectionOptions)

### `PromptProps`
- def: [`src/credentials.tsx:513`](../../../../../raw/code/openwiki/src/credentials.tsx#L513)
- signature: `type PromptProps`
- members:
  - `input` — [`L514`](../../../../../raw/code/openwiki/src/credentials.tsx#L514)
  - `isCustomModelInput` — [`L515`](../../../../../raw/code/openwiki/src/credentials.tsx#L515)
  - `modelSelectionIndex` — [`L516`](../../../../../raw/code/openwiki/src/credentials.tsx#L516)
  - `provider` — [`L517`](../../../../../raw/code/openwiki/src/credentials.tsx#L517)
  - `providerSelectionIndex` — [`L518`](../../../../../raw/code/openwiki/src/credentials.tsx#L518)
  - `step` — [`L519`](../../../../../raw/code/openwiki/src/credentials.tsx#L519)
- uses (calls/refs, reference-scoped): [`OpenWikiProvider`](constants.ts.md#OpenWikiProvider), [`PromptStep`](credentials.tsx.md#PromptStep)
- used by: [`InitSetup`](credentials.tsx.md#InitSetup), [`Prompt`](credentials.tsx.md#Prompt)

### `PromptStep`
- def: [`src/credentials.tsx:34`](../../../../../raw/code/openwiki/src/credentials.tsx#L34)
- signature: `type PromptStep`
- used by: [`InitSetup`](credentials.tsx.md#InitSetup), [`getInitialStep`](credentials.tsx.md#getInitialStep), [`getNextStepAfterProvider`](credentials.tsx.md#getNextStepAfterProvider), [`getNextStepAfterApiKey`](credentials.tsx.md#getNextStepAfterApiKey), [`step`](credentials.tsx.md#PromptProps.typeLiteral176.step)

### `SetupPanelProps`
- def: [`src/credentials.tsx:491`](../../../../../raw/code/openwiki/src/credentials.tsx#L491)
- signature: `type SetupPanelProps`
- members:
  - `children` — [`L493`](../../../../../raw/code/openwiki/src/credentials.tsx#L493)
  - `title` — [`L492`](../../../../../raw/code/openwiki/src/credentials.tsx#L492)
- used by: [`InitSetup`](credentials.tsx.md#InitSetup), [`SetupPanel`](credentials.tsx.md#SetupPanel)

### `SetupStepProps`
- def: [`src/credentials.tsx:467`](../../../../../raw/code/openwiki/src/credentials.tsx#L467)
- signature: `type SetupStepProps`
- members:
  - `detail` — [`L470`](../../../../../raw/code/openwiki/src/credentials.tsx#L470)
  - `label` — [`L468`](../../../../../raw/code/openwiki/src/credentials.tsx#L468)
  - `state` — [`L469`](../../../../../raw/code/openwiki/src/credentials.tsx#L469)
- used by: [`InitSetup`](credentials.tsx.md#InitSetup), [`SetupStep`](credentials.tsx.md#SetupStep)

## Functions
- `InitSetup({ modelIdOverride, onComplete, onError, }: InitSetupProps)` — [`L51`](../../../../../raw/code/openwiki/src/credentials.tsx#L51) — documented in [openwiki-cli.tsx](../../concepts/openwiki-cli.tsx.md)
- `Prompt({ input, isCustomModelInput, modelSelectionIndex, provider, providerSelectionIndex, step, }: PromptProps)` — [`L522`](../../../../../raw/code/openwiki/src/credentials.tsx#L522) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `SelectionMarker({ isSelected }: { isSelected: boolean; })` — [`L619`](../../../../../raw/code/openwiki/src/credentials.tsx#L619)
- `SetupHeader()` — [`L447`](../../../../../raw/code/openwiki/src/credentials.tsx#L447)
- `SetupPanel({ title, children }: SetupPanelProps)` — [`L496`](../../../../../raw/code/openwiki/src/credentials.tsx#L496)
- `SetupStep({ label, state, detail }: SetupStepProps)` — [`L473`](../../../../../raw/code/openwiki/src/credentials.tsx#L473) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getInitialStep(modelIdOverride: string | null, provider: OpenWikiProvider)` — [`L625`](../../../../../raw/code/openwiki/src/credentials.tsx#L625) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getModelSelectionIndex(provider: OpenWikiProvider, selectedModelId: string)` — [`L755`](../../../../../raw/code/openwiki/src/credentials.tsx#L755) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getModelSelectionOptions(provider: OpenWikiProvider)` — [`L713`](../../../../../raw/code/openwiki/src/credentials.tsx#L713) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getModelSetupDetail(modelIdOverride: string | null, provider: OpenWikiProvider)` — [`L688`](../../../../../raw/code/openwiki/src/credentials.tsx#L688) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getNextStepAfterApiKey(provider: OpenWikiProvider, modelIdOverride: string | null)` — [`L662`](../../../../../raw/code/openwiki/src/credentials.tsx#L662) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getNextStepAfterProvider(provider: OpenWikiProvider, modelIdOverride: string | null)` — [`L651`](../../../../../raw/code/openwiki/src/credentials.tsx#L651) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getProviderArticle(provider: OpenWikiProvider)` — [`L778`](../../../../../raw/code/openwiki/src/credentials.tsx#L778)
- `getProviderSelectionIndex(provider: OpenWikiProvider)` — [`L747`](../../../../../raw/code/openwiki/src/credentials.tsx#L747)
- `getProviderSetupDetail(provider: OpenWikiProvider)` — [`L680`](../../../../../raw/code/openwiki/src/credentials.tsx#L680) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `getSelectedModelId(provider: OpenWikiProvider, selectedIndex: number, input: string, isCustomInput: boolean)` — [`L726`](../../../../../raw/code/openwiki/src/credentials.tsx#L726) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `mask(value: string)` — [`L786`](../../../../../raw/code/openwiki/src/credentials.tsx#L786)
- `moveSelectionIndex(currentIndex: number, offset: number, itemCount: number)` — [`L766`](../../../../../raw/code/openwiki/src/credentials.tsx#L766)
- `needsCredentialSetup(modelIdOverride?: string | null)` — [`L36`](../../../../../raw/code/openwiki/src/credentials.tsx#L36) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)
- `sanitizeInputChunk(value: string)` — [`L782`](../../../../../raw/code/openwiki/src/credentials.tsx#L782)

## Module values
- `isSelected` — [`L619`](../../../../../raw/code/openwiki/src/credentials.tsx#L619)

