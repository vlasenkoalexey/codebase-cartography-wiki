---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`typescript-extractor.ts`/
symbols:
  TypeScriptExtractor.processExportStatement: TypeScriptExtractor#processExportStatement().
  TypeScriptExtractor.processTopLevelNode: TypeScriptExtractor#processTopLevelNode().
  TypeScriptExtractor.extractFunction: TypeScriptExtractor#extractFunction().
  TypeScriptExtractor.extractVariableDeclarations: TypeScriptExtractor#extractVariableDeclarations().
  TypeScriptExtractor.extractImport: TypeScriptExtractor#extractImport().
  TypeScriptExtractor.extractStructure: TypeScriptExtractor#extractStructure().
  TypeScriptExtractor.extractClass: TypeScriptExtractor#extractClass().
  TypeScriptExtractor.extractCallGraph: TypeScriptExtractor#extractCallGraph().
  TypeScriptExtractor: TypeScriptExtractor#
  extractParams: extractParams().
  extractReturnType: extractReturnType().
  extractImportSpecifiers: extractImportSpecifiers().
  TypeScriptExtractor.languageIds: TypeScriptExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts)

## Classes
### `TypeScriptExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts:106`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L106)
- doc: TypeScript/JavaScript extractor.
- signature: `class TypeScriptExtractor`
- members:
  - `extractCallGraph(method)` — [`L132`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L132) — Extract caller→callee relationships from the root AST node
  - `extractClass(method)` — [`L267`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L267)
  - `extractFunction(method)` — [`L238`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L238)
  - `extractImport(method)` — [`L359`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L359)
  - `extractStructure(method)` — [`L109`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L109) — Extract functions, classes, imports, exports from the root AST node
  - `extractVariableDeclarations(method)` — [`L319`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L319)
  - `processExportStatement(method)` — [`L385`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L385)
  - `processTopLevelNode(method)` — [`L198`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L198)
  - `languageIds` — [`L107`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L107) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`getStringValue`](base-extractor.ts.md#getStringValue), [`extractParams`](typescript-extractor.ts.md#extractParams), [`extractReturnType`](typescript-extractor.ts.md#extractReturnType), [`isDefault`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.isDefault), [`extractImportSpecifiers`](typescript-extractor.ts.md#extractImportSpecifiers)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds), [`typescript-extractor.test.ts`](__tests__/typescript-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-typescript-extractor.test.ts)

## Functions
- `extractImportSpecifiers(importClause: any)` — [`L66`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L66) — Extract import specifiers from an import_clause node.
- `extractParams(paramsNode: any)` — [`L8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L8) — Extract parameter names from a formal_parameters node.
- `extractReturnType(node: any)` — [`L52`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/typescript-extractor.ts#L52) — Extract return type annotation from a function-like node.

