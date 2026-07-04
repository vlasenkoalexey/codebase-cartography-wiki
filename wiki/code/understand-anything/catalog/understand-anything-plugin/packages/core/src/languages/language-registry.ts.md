---
title: 'Module: understand-anything-plugin/packages/core/src/languages/language-registry.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/languages/language-registry.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/languages/`language-registry.ts`/LanguageRegistry#
symbols:
  LanguageRegistry: ''
  LanguageRegistry.getForFile: getForFile().
  LanguageRegistry.getByExtension: getByExtension().
  LanguageRegistry.register: register().
  LanguageRegistry.createDefault: createDefault().
  LanguageRegistry.getAllLanguages: getAllLanguages().
  LanguageRegistry.getById: getById().
  LanguageRegistry.byId: byId.
  LanguageRegistry.byExtension: byExtension.
  LanguageRegistry.byFilename: byFilename.
---
# Module: [`understand-anything-plugin/packages/core/src/languages/language-registry.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts)

## Classes
### `LanguageRegistry`
- def: [`understand-anything-plugin/packages/core/src/languages/language-registry.ts:9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L9) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- doc: Registry for language configurations. Maps language ids and file extensions
- signature: `class LanguageRegistry`
- members:
  - `createDefault(method)` — [`L57`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L57) — Create a registry pre-populated with all built-in language configs. — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `getAllLanguages(method)` — [`L50`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L50)
  - `getByExtension(method)` — [`L33`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L33) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `getById(method)` — [`L29`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L29) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `getForFile(method)` — [`L38`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L38) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `register(method)` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L14) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `byExtension` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L11)
  - `byFilename` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L12)
  - `byId` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/languages/language-registry.ts#L10)
- uses (calls/refs, reference-scoped): [`LanguageConfig`](types.ts.md#LanguageConfig), [`LanguageConfigSchema`](types.ts.md#LanguageConfigSchema), [`builtinLanguageConfigs`](configs/index.ts.md#builtinLanguageConfigs)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-languages-index.ts), [`language-registry.test.ts`](../__tests__/language-registry.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-language-registry.test.ts), [`graph-builder.ts`](../analyzer/graph-builder.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.ts), [`<constructor>`](../analyzer/graph-builder.ts.md#GraphBuilder.-constructor), [`<constructor>`](../plugins/registry.ts.md#PluginRegistry.-constructor), [`registry.ts`](../plugins/registry.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-registry.ts), [`getPluginForFile`](../plugins/registry.ts.md#PluginRegistry.getPluginForFile), [`detectLanguage`](../analyzer/graph-builder.ts.md#GraphBuilder.detectLanguage), [`getLanguageForFile`](../plugins/registry.ts.md#PluginRegistry.getLanguageForFile), [`languageRegistry`](../plugins/registry.ts.md#PluginRegistry.languageRegistry), [`languageRegistry`](../analyzer/graph-builder.ts.md#GraphBuilder.languageRegistry)

