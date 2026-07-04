---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/`tree-sitter-plugin.ts`/
symbols:
  TreeSitterPlugin.analyzeFile: TreeSitterPlugin#analyzeFile().
  TreeSitterPlugin.-constructor: TreeSitterPlugin#`<constructor>`().
  TreeSitterPlugin.init: TreeSitterPlugin#init().
  TreeSitterPlugin.extractCallGraph: TreeSitterPlugin#extractCallGraph().
  TreeSitterPlugin.getParser: TreeSitterPlugin#getParser().
  TreeSitterPlugin.resolveImports: TreeSitterPlugin#resolveImports().
  TreeSitterPlugin.registerExtractor: TreeSitterPlugin#registerExtractor().
  TreeSitterPlugin._languages: TreeSitterPlugin#_languages.
  TreeSitterPlugin._extensionToLang: TreeSitterPlugin#_extensionToLang.
  TreeSitterPlugin.configs: TreeSitterPlugin#configs.
  TreeSitterPlugin.getExtractor: TreeSitterPlugin#getExtractor().
  TreeSitterPlugin: TreeSitterPlugin#
  TreeSitterPlugin._ParserClass: TreeSitterPlugin#_ParserClass.
  TreeSitterPlugin.languageKeyFromPath: TreeSitterPlugin#languageKeyFromPath().
  require: require.
  TreeSitterPlugin.extractors: TreeSitterPlugin#extractors.
  TreeSitterParser: TreeSitterParser#
  TreeSitterPlugin.languages: TreeSitterPlugin#languages.
  TreeSitterPlugin._initialized: TreeSitterPlugin#_initialized.
  TreeSitterLanguage: TreeSitterLanguage#
  TreeSitterPlugin.name: TreeSitterPlugin#name.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts)

## Classes
### `TreeSitterLanguage`
- def: [`understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts:17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L17)
- signature: `type TreeSitterLanguage`
- used by: [`_languages`](tree-sitter-plugin.ts.md#TreeSitterPlugin._languages)

### `TreeSitterParser`
- def: [`understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts:16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L16)
- signature: `type TreeSitterParser`
- used by: [`init`](tree-sitter-plugin.ts.md#TreeSitterPlugin.init), [`getParser`](tree-sitter-plugin.ts.md#TreeSitterPlugin.getParser), [`_ParserClass`](tree-sitter-plugin.ts.md#TreeSitterPlugin._ParserClass)

### `TreeSitterPlugin`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts:31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L31) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
- doc: Config-driven tree-sitter plugin.
- signature: `class TreeSitterPlugin`
- members:
  - `<constructor>(configs?: z.infer<any>[] | undefined, extractors?: LanguageExtractor[] | undefined)` — [`L56`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L56) — Config-driven tree-sitter plugin. — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `analyzeFile(method)` — [`L221`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L221) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `extractCallGraph(method)` — [`L277`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L277) — documented in [understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md)
  - `getExtractor(method)` — [`L105`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L105)
  - `getParser(method)` — [`L203`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L203) — Create a parser set to the appropriate language for the given file.
  - `init(method)` — [`L124`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L124) — Initialize the plugin by loading the WASM module and all language grammars. — documented in [understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md)
  - `languageKeyFromPath(method)` — [`L111`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L111)
  - `registerExtractor(method)` — [`L99`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L99)
  - `resolveImports(method)` — [`L252`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L252)
  - `configs` — [`L35`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L35) — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
  - `extractors` — [`L46`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L46)
  - `languages` — [`L33`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L33)
  - `name` — [`L32`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L32)
- protocol/private: `_ParserClass`[`L38`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L38), `_extensionToLang`[`L42`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L42), `_initialized`[`L43`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L43), `_languages`[`L41`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L41)
- uses (calls/refs, reference-scoped): [`functions`](../types.ts.md#StructuralAnalysis.functions), [`classes`](../types.ts.md#StructuralAnalysis.classes), [`imports`](../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../types.ts.md#StructuralAnalysis), [`exports`](../types.ts.md#StructuralAnalysis.exports), [`LanguageConfig`](../languages/types.ts.md#LanguageConfig), [`source`](../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`specifiers`](../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`AnalyzerPlugin`](../types.ts.md#AnalyzerPlugin), [`LanguageExtractor`](extractors/types.ts.md#LanguageExtractor), [`CallGraphEntry`](../types.ts.md#CallGraphEntry), [`extractStructure`](extractors/types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](extractors/types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](extractors/types.ts.md#LanguageExtractor.languageIds), [`ImportResolution`](../types.ts.md#ImportResolution), [`require`](tree-sitter-plugin.ts.md#require), [`TreeSitterParser`](tree-sitter-plugin.ts.md#TreeSitterParser), [`builtinExtractors`](extractors/index.ts.md#builtinExtractors), [`TreeSitterLanguage`](tree-sitter-plugin.ts.md#TreeSitterLanguage)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`tree-sitter-plugin.test.ts`](tree-sitter-plugin.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-tree-sitter-plugin.test.ts), [`AnalyzerPlugin`](../types.ts.md#AnalyzerPlugin), [`swift-extractor.test.ts`](extractors/__tests__/swift-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-swift-extractor.test.ts), [`analyzeFile`](../types.ts.md#AnalyzerPlugin.analyzeFile), [`name`](../types.ts.md#AnalyzerPlugin.name), [`languages`](../types.ts.md#AnalyzerPlugin.languages), [`resolveImports`](../types.ts.md#AnalyzerPlugin.resolveImports), [`extractCallGraph`](../types.ts.md#AnalyzerPlugin.extractCallGraph)

## Module values
- `require` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts#L14)

