---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`go-extractor.ts`/
symbols:
  GoExtractor.extractStructure: GoExtractor#extractStructure().
  GoExtractor.extractMethod: GoExtractor#extractMethod().
  GoExtractor.extractFunction: GoExtractor#extractFunction().
  GoExtractor.extractStruct: GoExtractor#extractStruct().
  GoExtractor.extractInterface: GoExtractor#extractInterface().
  GoExtractor.extractImportSpec: GoExtractor#extractImportSpec().
  GoExtractor.extractCallGraph: GoExtractor#extractCallGraph().
  GoExtractor.extractTypeDeclaration: GoExtractor#extractTypeDeclaration().
  GoExtractor.extractImportDeclaration: GoExtractor#extractImportDeclaration().
  GoExtractor: GoExtractor#
  extractParams: extractParams().
  extractReceiverType: extractReceiverType().
  extractResultType: extractResultType().
  isExported: isExported().
  GoExtractor.languageIds: GoExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts)

## Classes
### `GoExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts:89`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L89)
- doc: Go extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class GoExtractor`
- members:
  - `extractCallGraph(method)` — [`L135`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L135) — Extract caller→callee relationships from the root AST node
  - `extractFunction(method)` — [`L186`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L186)
  - `extractImportDeclaration(method)` — [`L354`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L354)
  - `extractImportSpec(method)` — [`L374`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L374)
  - `extractInterface(method)` — [`L319`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L319)
  - `extractMethod(method)` — [`L216`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L216) — documented in [understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md)
  - `extractStruct(method)` — [`L278`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L278)
  - `extractStructure(method)` — [`L92`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L92) — Extract functions, classes, imports, exports from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `extractTypeDeclaration(method)` — [`L259`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L259)
  - `languageIds` — [`L90`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L90) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`extractParams`](go-extractor.ts.md#extractParams), [`extractReceiverType`](go-extractor.ts.md#extractReceiverType), [`extractResultType`](go-extractor.ts.md#extractResultType), [`isExported`](go-extractor.ts.md#isExported)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`go-extractor.test.ts`](__tests__/go-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-go-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractParams(paramsNode: any)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L12) — Extract parameter names from a Go `parameter_list` node.
- `extractReceiverType(receiverNode: any)` — [`L49`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L49) — Extract the receiver type name from a method_declaration's receiver parameter_list.
- `extractResultType(node: any)` — [`L39`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L39) — Extract the return type text from a function/method declaration's `result` field.
- `isExported(name: string)` — [`L71`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/go-extractor.ts#L71) — Check if a name is exported in Go (starts with an uppercase letter).

