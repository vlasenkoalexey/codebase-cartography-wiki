---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`csharp-extractor.ts`/
symbols:
  CSharpExtractor.extractStructure: CSharpExtractor#extractStructure().
  CSharpExtractor.extractClass: CSharpExtractor#extractClass().
  CSharpExtractor.extractInterface: CSharpExtractor#extractInterface().
  CSharpExtractor.extractMethod: CSharpExtractor#extractMethod().
  CSharpExtractor.extractConstructor: CSharpExtractor#extractConstructor().
  CSharpExtractor.walkTopLevel: CSharpExtractor#walkTopLevel().
  CSharpExtractor.extractCallGraph: CSharpExtractor#extractCallGraph().
  CSharpExtractor.walkNamespaceBody: CSharpExtractor#walkNamespaceBody().
  CSharpExtractor.extractUsing: CSharpExtractor#extractUsing().
  CSharpExtractor.extractClassBodyMembers: CSharpExtractor#extractClassBodyMembers().
  CSharpExtractor.extractField: CSharpExtractor#extractField().
  CSharpExtractor.extractProperty: CSharpExtractor#extractProperty().
  hasModifier: hasModifier().
  CSharpExtractor: CSharpExtractor#
  extractParams: extractParams().
  extractUsingSource: extractUsingSource().
  extractReturnType: extractReturnType().
  extractInvocationName: extractInvocationName().
  lastComponent: lastComponent().
  CSharpExtractor.languageIds: CSharpExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts)

## Classes
### `CSharpExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts:126`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L126)
- doc: C# extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class CSharpExtractor`
- members:
  - `extractCallGraph(method)` — [`L140`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L140) — Extract caller→callee relationships from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `extractClass(method)` — [`L299`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L299)
  - `extractClassBodyMembers(method)` — [`L389`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L389) — Extract methods, constructors, properties, and fields from a
  - `extractConstructor(method)` — [`L453`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L453)
  - `extractField(method)` — [`L503`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L503)
  - `extractInterface(method)` — [`L334`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L334)
  - `extractMethod(method)` — [`L420`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L420)
  - `extractProperty(method)` — [`L485`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L485)
  - `extractStructure(method)` — [`L129`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L129) — Extract functions, classes, imports, exports from the root AST node
  - `extractUsing(method)` — [`L285`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L285)
  - `walkNamespaceBody(method)` — [`L252`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L252) — Walk into a namespace_declaration's body (declaration_list) to find
  - `walkTopLevel(method)` — [`L209`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L209) — Walk the top-level nodes of a compilation_unit, recursing into
  - `languageIds` — [`L127`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L127) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`hasModifier`](csharp-extractor.ts.md#hasModifier), [`extractParams`](csharp-extractor.ts.md#extractParams), [`extractUsingSource`](csharp-extractor.ts.md#extractUsingSource), [`extractInvocationName`](csharp-extractor.ts.md#extractInvocationName), [`extractReturnType`](csharp-extractor.ts.md#extractReturnType), [`lastComponent`](csharp-extractor.ts.md#lastComponent)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`csharp-extractor.test.ts`](__tests__/csharp-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-csharp-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractInvocationName(node: any)` — [`L100`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L100) — Extract the callee name from an invocation_expression node.
- `extractParams(paramsNode: any)` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L10) — Extract parameter names from a C# `parameter_list` node.
- `extractReturnType(node: any)` — [`L32`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L32) — Extract the return type text from a method_declaration node.
- `extractUsingSource(node: any)` — [`L64`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L64) — Extract the namespace source text from a using_directive.
- `hasModifier(node: any, modifier: string)` — [`L46`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L46) — Check if a C# declaration node has a specific modifier.
- `lastComponent(path: string)` — [`L86`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/csharp-extractor.ts#L86) — Get the last component of a dotted namespace path.

