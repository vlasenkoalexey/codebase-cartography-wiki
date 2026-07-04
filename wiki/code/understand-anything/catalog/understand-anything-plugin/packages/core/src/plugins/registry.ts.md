---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/registry.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/registry.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/`registry.ts`/PluginRegistry#
symbols:
  PluginRegistry.register: register().
  PluginRegistry.-constructor: '`<constructor>`().'
  PluginRegistry.getPluginForFile: getPluginForFile().
  PluginRegistry.getSupportedLanguages: getSupportedLanguages().
  PluginRegistry.getPluginForLanguage: getPluginForLanguage().
  PluginRegistry.unregister: unregister().
  PluginRegistry.analyzeFile: analyzeFile().
  PluginRegistry.getPlugins: getPlugins().
  PluginRegistry.resolveImports: resolveImports().
  PluginRegistry.plugins: plugins.
  PluginRegistry: ''
  PluginRegistry.getLanguageForFile: getLanguageForFile().
  PluginRegistry.languageMap: languageMap.
  PluginRegistry.extractCallGraph: extractCallGraph().
  PluginRegistry.languageRegistry: languageRegistry.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/registry.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts)

## Classes
### `PluginRegistry`
- def: [`understand-anything-plugin/packages/core/src/plugins/registry.ts:11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L11)
- doc: Registry for analyzer plugins. Maps languages to plugins and provides
- signature: `class PluginRegistry`
- members:
  - `<constructor>(languageRegistry?: LanguageRegistry | undefined)` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L16) — Registry for analyzer plugins. Maps languages to plugins and provides — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `analyzeFile(method)` — [`L56`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L56) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `extractCallGraph(method)` — [`L68`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L68) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `getLanguageForFile(method)` — [`L52`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L52) — Get the language id for a file path using the language registry.
  - `getPluginForFile(method)` — [`L43`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L43) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `getPluginForLanguage(method)` — [`L39`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L39) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `getPlugins(method)` — [`L74`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L74)
  - `getSupportedLanguages(method)` — [`L78`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L78) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `register(method)` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L20) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `resolveImports(method)` — [`L62`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L62) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `unregister(method)` — [`L27`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L27)
  - `languageMap` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L13) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
  - `languageRegistry` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L14)
  - `plugins` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/registry.ts#L12) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
- uses (calls/refs, reference-scoped): [`StructuralAnalysis`](../types.ts.md#StructuralAnalysis), [`AnalyzerPlugin`](../types.ts.md#AnalyzerPlugin), [`CallGraphEntry`](../types.ts.md#CallGraphEntry), [`analyzeFile`](../types.ts.md#AnalyzerPlugin.analyzeFile), [`name`](../types.ts.md#AnalyzerPlugin.name), [`languages`](../types.ts.md#AnalyzerPlugin.languages), [`LanguageRegistry`](../languages/language-registry.ts.md#LanguageRegistry), [`getForFile`](../languages/language-registry.ts.md#LanguageRegistry.getForFile), [`createDefault`](../languages/language-registry.ts.md#LanguageRegistry.createDefault), [`resolveImports`](../types.ts.md#AnalyzerPlugin.resolveImports), [`ImportResolution`](../types.ts.md#ImportResolution), [`extractCallGraph`](../types.ts.md#AnalyzerPlugin.extractCallGraph)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`plugin-registry.test.ts`](../__tests__/plugin-registry.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-plugin-registry.test.ts), [`analyzeChanges`](../fingerprint.ts.md#analyzeChanges), [`index.ts`](parsers/index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`buildFingerprintStore`](../fingerprint.ts.md#buildFingerprintStore), [`registerAllParsers`](parsers/index.ts.md#registerAllParsers), [`fingerprint.ts`](../fingerprint.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-fingerprint.ts)

