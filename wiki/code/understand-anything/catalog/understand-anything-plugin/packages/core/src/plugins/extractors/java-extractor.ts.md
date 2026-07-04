---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`java-extractor.ts`/
symbols:
  JavaExtractor.extractStructure: JavaExtractor#extractStructure().
  JavaExtractor.extractClass: JavaExtractor#extractClass().
  JavaExtractor.extractInterface: JavaExtractor#extractInterface().
  JavaExtractor.extractMethod: JavaExtractor#extractMethod().
  JavaExtractor.extractConstructor: JavaExtractor#extractConstructor().
  JavaExtractor.extractImport: JavaExtractor#extractImport().
  JavaExtractor.extractCallGraph: JavaExtractor#extractCallGraph().
  JavaExtractor.extractClassBodyMembers: JavaExtractor#extractClassBodyMembers().
  JavaExtractor.extractField: JavaExtractor#extractField().
  hasModifier: hasModifier().
  JavaExtractor: JavaExtractor#
  extractParams: extractParams().
  extractReturnType: extractReturnType().
  extractScopedIdentifierPath: extractScopedIdentifierPath().
  JavaExtractor.extractMethodInvocationName: JavaExtractor#extractMethodInvocationName().
  lastComponent: lastComponent().
  JavaExtractor.languageIds: JavaExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts)

## Classes
### `JavaExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts:96`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L96)
- doc: Java extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class JavaExtractor`
- members:
  - `extractCallGraph(method)` — [`L129`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L129) — Extract caller→callee relationships from the root AST node
  - `extractClass(method)` — [`L241`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L241)
  - `extractClassBodyMembers(method)` — [`L339`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L339) — Extract methods, constructors, and fields from a class_body node.
  - `extractConstructor(method)` — [`L411`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L411)
  - `extractField(method)` — [`L443`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L443)
  - `extractImport(method)` — [`L212`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L212)
  - `extractInterface(method)` — [`L282`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L282)
  - `extractMethod(method)` — [`L378`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L378)
  - `extractMethodInvocationName(method)` — [`L200`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L200) — Extract the callee name from a method_invocation node.
  - `extractStructure(method)` — [`L99`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L99) — Extract functions, classes, imports, exports from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `languageIds` — [`L97`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L97) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`hasModifier`](java-extractor.ts.md#hasModifier), [`extractParams`](java-extractor.ts.md#extractParams), [`extractReturnType`](java-extractor.ts.md#extractReturnType), [`extractScopedIdentifierPath`](java-extractor.ts.md#extractScopedIdentifierPath), [`lastComponent`](java-extractor.ts.md#lastComponent)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`java-extractor.test.ts`](__tests__/java-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-java-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractParams(paramsNode: any)` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L10) — Extract parameter names from a Java `formal_parameters` node.
- `extractReturnType(node: any)` — [`L40`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L40) — Extract the return type text from a method_declaration node.
- `extractScopedIdentifierPath(node: any)` — [`L68`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L68) — Extract the full dotted path from a scoped_identifier node.
- `hasModifier(node: any, modifier: string)` — [`L49`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L49) — Check if a node has a `modifiers` child containing a specific modifier keyword.
- `lastComponent(path: string)` — [`L76`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/java-extractor.ts#L76) — Get the last component of a dotted import path.

