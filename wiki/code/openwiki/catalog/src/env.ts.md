---
title: 'Module: src/env.ts'
type: catalog
provenance: extracted
module: src/env.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/`env.ts`/
symbols:
  createCredentialDiagnostic: createCredentialDiagnostic().
  getCredentialDiagnostics: getCredentialDiagnostics().
  saveOpenWikiEnv: saveOpenWikiEnv().
  managedEnvKeys: managedEnvKeys.
  CredentialDiagnostic: CredentialDiagnostic#
  readOpenWikiEnv: readOpenWikiEnv().
  loadOpenWikiEnv: loadOpenWikiEnv().
  formatEnv: formatEnv().
  openWikiEnvPath: openWikiEnvPath.
  openWikiEnvDir: openWikiEnvDir.
  EnvMap: EnvMap#
  getCredentialSource: getCredentialSource().
  parseEnv: parseEnv().
  CredentialDiagnostic.typeLiteral6.key: CredentialDiagnostic#typeLiteral6:key.
  CredentialDiagnostic.typeLiteral6.warnings: CredentialDiagnostic#typeLiteral6:warnings.
  CredentialDiagnostic.typeLiteral6.source: CredentialDiagnostic#typeLiteral6:source.
  getModelWarnings: getModelWarnings().
  getProviderWarnings: getProviderWarnings().
  CredentialDiagnostic.typeLiteral6.length: CredentialDiagnostic#typeLiteral6:length.
  CredentialDiagnostic.typeLiteral6.preview: CredentialDiagnostic#typeLiteral6:preview.
  deprecatedEnvKeys: deprecatedEnvKeys.
  createCredentialPreview: createCredentialPreview().
  getCredentialWarnings: getCredentialWarnings().
  parseEnvValue: parseEnvValue().
  formatEnvValue: formatEnvValue().
  isFileNotFoundError: isFileNotFoundError().
---
# Module: [`src/env.ts`](../../../../../raw/code/openwiki/src/env.ts)

## Classes
### `CredentialDiagnostic`
- def: [`src/env.ts:21`](../../../../../raw/code/openwiki/src/env.ts#L21) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- signature: `type CredentialDiagnostic`
- members:
  - `key` — [`L22`](../../../../../raw/code/openwiki/src/env.ts#L22)
  - `length` — [`L28`](../../../../../raw/code/openwiki/src/env.ts#L28) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
  - `preview` — [`L29`](../../../../../raw/code/openwiki/src/env.ts#L29) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
  - `source` — [`L23`](../../../../../raw/code/openwiki/src/env.ts#L23) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
  - `warnings` — [`L30`](../../../../../raw/code/openwiki/src/env.ts#L30) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- used by: [`App`](cli.tsx.md#App), [`cli.tsx`](cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`createCredentialDiagnostic`](env.ts.md#createCredentialDiagnostic), [`getCredentialDiagnostics`](env.ts.md#getCredentialDiagnostics), [`diagnostics`](cli.tsx.md#CredentialDiagnosticsPanel.-diagnostics-.typeLiteral250.diagnostics), [`RunState`](cli.tsx.md#RunState), [`getCredentialSource`](env.ts.md#getCredentialSource), [`updateRunningCredentialDiagnostics`](cli.tsx.md#updateRunningCredentialDiagnostics), [`credentialDiagnostics`](cli.tsx.md#RunViewProps.typeLiteral229.credentialDiagnostics), [`credentialDiagnostics`](cli.tsx.md#CompletedRun.typeLiteral35.credentialDiagnostics)

### `EnvMap`
- def: [`src/env.ts:19`](../../../../../raw/code/openwiki/src/env.ts#L19) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- signature: `type EnvMap`
- used by: [`createCredentialDiagnostic`](env.ts.md#createCredentialDiagnostic), [`saveOpenWikiEnv`](env.ts.md#saveOpenWikiEnv), [`readOpenWikiEnv`](env.ts.md#readOpenWikiEnv), [`loadOpenWikiEnv`](env.ts.md#loadOpenWikiEnv), [`formatEnv`](env.ts.md#formatEnv), [`parseEnv`](env.ts.md#parseEnv)

## Functions
- `createCredentialDiagnostic(key: string, fileEnv: EnvMap)` — [`L113`](../../../../../raw/code/openwiki/src/env.ts#L113) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `createCredentialPreview(value: string)` — [`L168`](../../../../../raw/code/openwiki/src/env.ts#L168) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `formatEnv(env: EnvMap)` — [`L259`](../../../../../raw/code/openwiki/src/env.ts#L259) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `formatEnvValue(value: string)` — [`L270`](../../../../../raw/code/openwiki/src/env.ts#L270) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `getCredentialDiagnostics()` — [`L68`](../../../../../raw/code/openwiki/src/env.ts#L68) — documented in [openwiki-cli.tsx](../../concepts/openwiki-cli.tsx.md)
- `getCredentialSource(processValue: string | undefined, fileValue: string | undefined)` — [`L149`](../../../../../raw/code/openwiki/src/env.ts#L149) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `getCredentialWarnings(value: string)` — [`L176`](../../../../../raw/code/openwiki/src/env.ts#L176) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `getModelWarnings(value: string)` — [`L198`](../../../../../raw/code/openwiki/src/env.ts#L198) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `getProviderWarnings(value: string)` — [`L202`](../../../../../raw/code/openwiki/src/env.ts#L202) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `isFileNotFoundError(error: unknown)` — [`L277`](../../../../../raw/code/openwiki/src/env.ts#L277) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `loadOpenWikiEnv()` — [`L52`](../../../../../raw/code/openwiki/src/env.ts#L52) — documented in [openwiki-agent-index.ts](../../concepts/openwiki-agent-index.ts.md)
- `parseEnv(content: string)` — [`L218`](../../../../../raw/code/openwiki/src/env.ts#L218) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `parseEnvValue(value: string)` — [`L247`](../../../../../raw/code/openwiki/src/env.ts#L247) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `readOpenWikiEnv()` — [`L206`](../../../../../raw/code/openwiki/src/env.ts#L206) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `saveOpenWikiEnv(updates: EnvMap)` — [`L85`](../../../../../raw/code/openwiki/src/env.ts#L85) — documented in [openwiki-credentials.tsx](../../concepts/openwiki-credentials.tsx.md)

## Module values
- `deprecatedEnvKeys` — [`L46`](../../../../../raw/code/openwiki/src/env.ts#L46) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `managedEnvKeys` — [`L33`](../../../../../raw/code/openwiki/src/env.ts#L33) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)
- `openWikiEnvDir` — [`L16`](../../../../../raw/code/openwiki/src/env.ts#L16)
- `openWikiEnvPath` — [`L17`](../../../../../raw/code/openwiki/src/env.ts#L17) — documented in [openwiki-env.ts](../../concepts/openwiki-env.ts.md)

