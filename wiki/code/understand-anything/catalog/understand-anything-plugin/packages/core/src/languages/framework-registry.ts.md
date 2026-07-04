---
title: 'Module: understand-anything-plugin/packages/core/src/languages/framework-registry.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/languages/framework-registry.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/languages/`framework-registry.ts`/FrameworkRegistry#
symbols:
  FrameworkRegistry.register: register().
  FrameworkRegistry: ''
  FrameworkRegistry.getForLanguage: getForLanguage().
  FrameworkRegistry.detectFrameworks: detectFrameworks().
  FrameworkRegistry.createDefault: createDefault().
  FrameworkRegistry.byId: byId.
  FrameworkRegistry.getById: getById().
  FrameworkRegistry.getAllFrameworks: getAllFrameworks().
  FrameworkRegistry.byLanguage: byLanguage.
---
# Module: [`understand-anything-plugin/packages/core/src/languages/framework-registry.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts)

## Classes
### `FrameworkRegistry`
- def: [`understand-anything-plugin/packages/core/src/languages/framework-registry.ts:9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L9)
- doc: Registry for framework configurations. Provides detection of frameworks
- signature: `class FrameworkRegistry`
- members:
  - `createDefault(method)` — [`L79`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L79) — Create a registry pre-populated with all built-in framework configs.
  - `detectFrameworks(method)` — [`L45`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L45) — Detect frameworks from manifest file contents. — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `getAllFrameworks(method)` — [`L36`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L36)
  - `getById(method)` — [`L28`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L28)
  - `getForLanguage(method)` — [`L32`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L32) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `register(method)` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L13) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `byId` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L10) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `byLanguage` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/framework-registry.ts#L11)
- uses (calls/refs, reference-scoped): [`FrameworkConfig`](types.ts.md#FrameworkConfig), [`FrameworkConfigSchema`](types.ts.md#FrameworkConfigSchema), [`builtinFrameworkConfigs`](frameworks/index.ts.md#builtinFrameworkConfigs)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-languages-index.ts), [`framework-registry.test.ts`](../__tests__/framework-registry.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-framework-registry.test.ts)

