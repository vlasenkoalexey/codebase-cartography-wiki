---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`rust-extractor.ts`/
symbols:
  RustExtractor.extractStructure: RustExtractor#extractStructure().
  RustExtractor.extractImpl: RustExtractor#extractImpl().
  RustExtractor.extractFunction: RustExtractor#extractFunction().
  RustExtractor.extractStruct: RustExtractor#extractStruct().
  RustExtractor.extractTrait: RustExtractor#extractTrait().
  RustExtractor.extractEnum: RustExtractor#extractEnum().
  RustExtractor.extractUseDeclaration: RustExtractor#extractUseDeclaration().
  RustExtractor.extractCallGraph: RustExtractor#extractCallGraph().
  isPublic: isPublic().
  extractScopedPath: extractScopedPath().
  RustExtractor: RustExtractor#
  extractParams: extractParams().
  extractReturnType: extractReturnType().
  RustExtractor.extractCalleeName: RustExtractor#extractCalleeName().
  extractScopedPath.typeLiteral18.path: extractScopedPath().typeLiteral18:path.
  extractScopedPath.typeLiteral18.name: extractScopedPath().typeLiteral18:name.
  RustExtractor.languageIds: RustExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts)

## Classes
### `RustExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts:92`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L92)
- doc: Rust extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class RustExtractor`
- members:
  - `extractCallGraph(method)` — [`L146`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L146) — Extract caller→callee relationships from the root AST node
  - `extractCalleeName(method)` — [`L201`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L201) — Extract the callee name from a call_expression.
  - `extractEnum(method)` — [`L295`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L295)
  - `extractFunction(method)` — [`L227`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L227)
  - `extractImpl(method)` — [`L380`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L380) — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
  - `extractStruct(method)` — [`L257`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L257)
  - `extractStructure(method)` — [`L95`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L95) — Extract functions, classes, imports, exports from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `extractTrait(method)` — [`L333`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L333)
  - `extractUseDeclaration(method)` — [`L429`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L429)
  - `languageIds` — [`L93`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L93) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`isPublic`](rust-extractor.ts.md#isPublic), [`extractScopedPath`](rust-extractor.ts.md#extractScopedPath), [`extractParams`](rust-extractor.ts.md#extractParams), [`extractReturnType`](rust-extractor.ts.md#extractReturnType), [`name`](rust-extractor.ts.md#extractScopedPath.typeLiteral18.name), [`path`](rust-extractor.ts.md#extractScopedPath.typeLiteral18.path)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`rust-extractor.test.ts`](__tests__/rust-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-rust-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractParams(paramsNode: any)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L12) — Extract parameter names from a Rust `parameters` node.
- `extractReturnType(node: any)` — [`L39`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L39) — Extract the return type from a function_item node.
- `extractScopedPath(node: any)` — [`L65`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L65) — Recursively extract the path portion of a scoped_identifier.
- `isPublic(node: any)` — [`L51`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L51) — Check if a node has a `visibility_modifier` child whose text starts with "pub".

## Module values
- `name` — [`L65`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L65)
- `path` — [`L65`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/rust-extractor.ts#L65)

