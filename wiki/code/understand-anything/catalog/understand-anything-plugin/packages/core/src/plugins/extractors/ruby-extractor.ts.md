---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`ruby-extractor.ts`/
symbols:
  RubyExtractor.extractStructure: RubyExtractor#extractStructure().
  RubyExtractor.extractCallGraph: RubyExtractor#extractCallGraph().
  RubyExtractor.extractClass: RubyExtractor#extractClass().
  RubyExtractor.extractModule: RubyExtractor#extractModule().
  RubyExtractor.extractTopLevelCall: RubyExtractor#extractTopLevelCall().
  RubyExtractor.extractMethod: RubyExtractor#extractMethod().
  RubyExtractor.extractSingletonMethod: RubyExtractor#extractSingletonMethod().
  RubyExtractor.extractClassBody: RubyExtractor#extractClassBody().
  RubyExtractor: RubyExtractor#
  getStringContent: getStringContent().
  extractParams: extractParams().
  RubyExtractor.getClassName: RubyExtractor#getClassName().
  RubyExtractor.getModuleName: RubyExtractor#getModuleName().
  extractAttrProperties: extractAttrProperties().
  RubyExtractor.getMethodName: RubyExtractor#getMethodName().
  RubyExtractor.getSingletonMethodName: RubyExtractor#getSingletonMethodName().
  IMPORT_METHODS: IMPORT_METHODS.
  ATTR_METHODS: ATTR_METHODS.
  RubyExtractor.languageIds: RubyExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts)

## Classes
### `RubyExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts:111`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L111)
- doc: Ruby extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class RubyExtractor`
- members:
  - `extractCallGraph(method)` — [`L166`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L166) — Extract caller→callee relationships from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md)
  - `extractClass(method)` — [`L304`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L304)
  - `extractClassBody(method)` — [`L362`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L362) — Extract methods and properties from a class/module body_statement.
  - `extractMethod(method)` — [`L264`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L264)
  - `extractModule(method)` — [`L331`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L331)
  - `extractSingletonMethod(method)` — [`L284`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L284)
  - `extractStructure(method)` — [`L114`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L114) — Extract functions, classes, imports, exports from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `extractTopLevelCall(method)` — [`L397`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L397) — Handle top-level call nodes: extract require/require_relative as imports.
  - `getClassName(method)` — [`L252`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L252)
  - `getMethodName(method)` — [`L242`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L242)
  - `getModuleName(method)` — [`L259`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L259)
  - `getSingletonMethodName(method)` — [`L247`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L247)
  - `languageIds` — [`L112`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L112) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`getStringContent`](ruby-extractor.ts.md#getStringContent), [`extractParams`](ruby-extractor.ts.md#extractParams), [`extractAttrProperties`](ruby-extractor.ts.md#extractAttrProperties), [`ATTR_METHODS`](ruby-extractor.ts.md#ATTR_METHODS), [`IMPORT_METHODS`](ruby-extractor.ts.md#IMPORT_METHODS)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`ruby-extractor.test.ts`](__tests__/ruby-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-ruby-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractAttrProperties(callNode: any)` — [`L70`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L70) — Extract property names from attr_accessor/attr_reader/attr_writer calls.
- `extractParams(paramsNode: any)` — [`L24`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L24) — Extract parameter names from a Ruby `method_parameters` node.
- `getStringContent(node: any)` — [`L90`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L90) — Extract the string value from a Ruby string node.

## Module values
- `ATTR_METHODS` — [`L15`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L15) — Set of method names that define class properties (attr_* macros).
- `IMPORT_METHODS` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/ruby-extractor.ts#L9) — Set of method names that Ruby uses for imports.

