---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`kotlin-extractor.ts`/
symbols:
  KotlinExtractor.extractStructure: KotlinExtractor#extractStructure().
  KotlinExtractor.extractClassDeclaration: KotlinExtractor#extractClassDeclaration().
  collectClassBody: collectClassBody().
  KotlinExtractor.extractObjectDeclaration: KotlinExtractor#extractObjectDeclaration().
  KotlinExtractor.extractTopLevelFunction: KotlinExtractor#extractTopLevelFunction().
  KotlinExtractor.extractImport: KotlinExtractor#extractImport().
  KotlinExtractor.extractCallGraph: KotlinExtractor#extractCallGraph().
  isExported: isExported().
  extractParams: extractParams().
  extractDeclarationName: extractDeclarationName().
  collectPrimaryConstructorProperties: collectPrimaryConstructorProperties().
  KotlinExtractor: KotlinExtractor#
  extractVisibility: extractVisibility().
  extractPropertyName: extractPropertyName().
  extractReturnType: extractReturnType().
  KotlinExtractor.extractCalleeName: KotlinExtractor#extractCalleeName().
  KotlinExtractor.languageIds: KotlinExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts)

## Classes
### `KotlinExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts:183`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L183)
- doc: Kotlin extractor for tree-sitter structural analysis and call graph
- signature: `class KotlinExtractor`
- members:
  - `extractCallGraph(method)` — [`L222`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L222) — Extract caller→callee relationships from the root AST node
  - `extractCalleeName(method)` — [`L404`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L404) — Extract the callee name from a Kotlin `call_expression`. Two shapes:
  - `extractClassDeclaration(method)` — [`L280`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L280)
  - `extractImport(method)` — [`L357`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L357) — Extract a Kotlin import.
  - `extractObjectDeclaration(method)` — [`L314`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L314)
  - `extractStructure(method)` — [`L186`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L186) — Extract functions, classes, imports, exports from the root AST node
  - `extractTopLevelFunction(method)` — [`L262`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L262)
  - `languageIds` — [`L184`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L184) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`collectClassBody`](kotlin-extractor.ts.md#collectClassBody), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`isExported`](kotlin-extractor.ts.md#isExported), [`extractParams`](kotlin-extractor.ts.md#extractParams), [`collectPrimaryConstructorProperties`](kotlin-extractor.ts.md#collectPrimaryConstructorProperties), [`extractDeclarationName`](kotlin-extractor.ts.md#extractDeclarationName), [`extractReturnType`](kotlin-extractor.ts.md#extractReturnType)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`kotlin-extractor.test.ts`](__tests__/kotlin-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-kotlin-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `collectClassBody(body: any, methods: string[], properties: string[], functions: { name: string; lineRange: [number, number]; params: string[]; returnType?: string | undefined; }[], exports: { name: string; lineNumber: number; isDefault?: boolean | undefined; }[])` — [`L97`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L97) — Walk a `class_body` and collect functions + properties. Function entries
- `collectPrimaryConstructorProperties(declNode: any, properties: string[])` — [`L154`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L154) — Walk a `primary_constructor`'s `class_parameters` and surface every
- `extractDeclarationName(declNode: any)` — [`L40`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L40) — Get the identifier-text name of a Kotlin declaration. Works for
- `extractParams(declNode: any)` — [`L53`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L53) — Extract parameter names from a `function_value_parameters` node. Each
- `extractPropertyName(propNode: any)` — [`L141`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L141) — Extract the property name from a `property_declaration`. The name lives
- `extractReturnType(declNode: any)` — [`L70`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L70) — Extract the return type text from a `function_declaration` by looking for
- `extractVisibility(declNode: any)` — [`L13`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L13) — Extract the visibility keyword text (e.g., "public", "private") from a
- `isExported(declNode: any)` — [`L30`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/kotlin-extractor.ts#L30) — Whether a Kotlin declaration is visible to other files.

