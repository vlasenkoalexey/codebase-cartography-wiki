---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`python-extractor.ts`/
symbols:
  PythonExtractor.extractStructure: PythonExtractor#extractStructure().
  PythonExtractor.extractFunction: PythonExtractor#extractFunction().
  PythonExtractor.extractClass: PythonExtractor#extractClass().
  PythonExtractor.extractImport: PythonExtractor#extractImport().
  PythonExtractor.extractFromImport: PythonExtractor#extractFromImport().
  PythonExtractor.extractCallGraph: PythonExtractor#extractCallGraph().
  PythonExtractor.addExport: PythonExtractor#addExport().
  PythonExtractor: PythonExtractor#
  unwrapDecorated: unwrapDecorated().
  extractParams: extractParams().
  extractReturnType: extractReturnType().
  PythonExtractor.languageIds: PythonExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts)

## Classes
### `PythonExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts:102`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L102)
- doc: Python extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class PythonExtractor`
- members:
  - `addExport(method)` — [`L340`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L340)
  - `extractCallGraph(method)` — [`L144`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L144) — Extract caller→callee relationships from the root AST node
  - `extractClass(method)` — [`L215`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L215)
  - `extractFromImport(method)` — [`L297`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L297)
  - `extractFunction(method)` — [`L193`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L193)
  - `extractImport(method)` — [`L265`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L265)
  - `extractStructure(method)` — [`L105`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L105) — Extract functions, classes, imports, exports from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `languageIds` — [`L103`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L103) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`unwrapDecorated`](python-extractor.ts.md#unwrapDecorated), [`extractParams`](python-extractor.ts.md#extractParams), [`extractReturnType`](python-extractor.ts.md#extractReturnType)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`python-extractor.test.ts`](__tests__/python-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-python-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractParams(paramsNode: any)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L12) — Extract parameter names from a Python `parameters` node.
- `extractReturnType(node: any)` — [`L73`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L73) — Extract the return type annotation from a function_definition node.
- `unwrapDecorated(node: any)` — [`L85`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/python-extractor.ts#L85) — Unwrap a `decorated_definition` to get the inner definition.

