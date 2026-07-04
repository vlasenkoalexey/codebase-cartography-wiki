---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`cpp-extractor.ts`/
symbols:
  CppExtractor.extractClassOrStruct: CppExtractor#extractClassOrStruct().
  CppExtractor.extractStructure: CppExtractor#extractStructure().
  CppExtractor.extractFunctionDef: CppExtractor#extractFunctionDef().
  CppExtractor.walkTopLevel: CppExtractor#walkTopLevel().
  CppExtractor.extractCallGraph: CppExtractor#extractCallGraph().
  CppExtractor.extractInclude: CppExtractor#extractInclude().
  unwrapDeclaratorName: unwrapDeclaratorName().
  extractParams: extractParams().
  extractFuncDeclName: extractFuncDeclName().
  CppExtractor: CppExtractor#
  isStatic: isStatic().
  CppExtractor.extractFunctionName: CppExtractor#extractFunctionName().
  extractReturnType: extractReturnType().
  CppExtractor.extractCalleeName: CppExtractor#extractCalleeName().
  CppExtractor.languageIds: CppExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts)

## Classes
### `CppExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts:124`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L124)
- doc: C/C++ extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class CppExtractor`
- members:
  - `extractCallGraph(method)` — [`L153`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L153) — Extract caller→callee relationships from the root AST node — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md)
  - `extractCalleeName(method)` — [`L482`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L482) — Extract the callee name from a call_expression.
  - `extractClassOrStruct(method)` — [`L317`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L317) — Extract class_specifier or struct_specifier into the classes array.
  - `extractFunctionDef(method)` — [`L431`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L431) — Extract a free function or out-of-class method definition.
  - `extractFunctionName(method)` — [`L264`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L264) — Extract the simple function name from a function_definition.
  - `extractInclude(method)` — [`L279`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L279) — Extract #include directives and map them to the imports array.
  - `extractStructure(method)` — [`L127`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L127) — Extract functions, classes, imports, exports from the root AST node
  - `walkTopLevel(method)` — [`L204`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L204) — Walk top-level declarations. Recurses into namespace_definition bodies — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
  - `languageIds` — [`L125`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L125) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`unwrapDeclaratorName`](cpp-extractor.ts.md#unwrapDeclaratorName), [`extractParams`](cpp-extractor.ts.md#extractParams), [`extractFuncDeclName`](cpp-extractor.ts.md#extractFuncDeclName), [`isStatic`](cpp-extractor.ts.md#isStatic), [`extractReturnType`](cpp-extractor.ts.md#extractReturnType)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`cpp-extractor.test.ts`](__tests__/cpp-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-cpp-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractFuncDeclName(funcDecl: any)` — [`L39`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L39) — Extract the function/method name from a function_declarator node.
- `extractParams(paramsNode: any)` — [`L69`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L69) — Extract parameter names from a parameter_list node.
- `extractReturnType(node: any)` — [`L93`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L93) — Extract the return type text from a function_definition node.
- `isStatic(node: any)` — [`L104`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L104) — Check if a function_definition has a `storage_class_specifier` child with "static".
- `unwrapDeclaratorName(node: any)` — [`L14`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/cpp-extractor.ts#L14) — Recursively unwrap nested declarators (pointer_declarator, reference_declarator,

