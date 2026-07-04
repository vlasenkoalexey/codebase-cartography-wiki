---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`php-extractor.ts`/
symbols:
  PhpExtractor.walkStatements: PhpExtractor#walkStatements().
  PhpExtractor.extractStructure: PhpExtractor#extractStructure().
  PhpExtractor.extractClass: PhpExtractor#extractClass().
  PhpExtractor.extractFunction: PhpExtractor#extractFunction().
  PhpExtractor.extractInterface: PhpExtractor#extractInterface().
  PhpExtractor.extractDeclarationList: PhpExtractor#extractDeclarationList().
  PhpExtractor.extractUseDeclaration: PhpExtractor#extractUseDeclaration().
  PhpExtractor.extractCallGraph: PhpExtractor#extractCallGraph().
  extractParams: extractParams().
  PhpExtractor: PhpExtractor#
  extractUseName: extractUseName().
  PhpExtractor.getClassName: PhpExtractor#getClassName().
  PhpExtractor.getInterfaceName: PhpExtractor#getInterfaceName().
  PhpExtractor.getFunctionName: PhpExtractor#getFunctionName().
  extractReturnType: extractReturnType().
  lastSegment: lastSegment().
  PhpExtractor.languageIds: PhpExtractor#languageIds.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts)

## Classes
### `PhpExtractor`  ·  implements/extends LanguageExtractor
- def: [`understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts:115`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L115)
- doc: PHP extractor for tree-sitter structural analysis and call graph extraction.
- signature: `class PhpExtractor`
- members:
  - `extractCallGraph(method)` — [`L191`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L191) — Extract caller→callee relationships from the root AST node
  - `extractClass(method)` — [`L305`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L305)
  - `extractDeclarationList(method)` — [`L363`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L363) — Extract methods and properties from a class `declaration_list`.
  - `extractFunction(method)` — [`L286`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L286)
  - `extractInterface(method)` — [`L329`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L329)
  - `extractStructure(method)` — [`L118`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L118) — Extract functions, classes, imports, exports from the root AST node
  - `extractUseDeclaration(method)` — [`L418`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L418) — Extract imports from a `namespace_use_declaration` node.
  - `getClassName(method)` — [`L276`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L276)
  - `getFunctionName(method)` — [`L271`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L271)
  - `getInterfaceName(method)` — [`L281`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L281)
  - `walkStatements(method)` — [`L137`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L137) — Walk top-level statements, extracting functions, classes, interfaces, and imports. — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
  - `languageIds` — [`L116`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L116) — Language IDs this extractor handles (must match LanguageConfig.id)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`TreeSitterNode`](types.ts.md#TreeSitterNode), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`name`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`methods`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.methods), [`findChild`](base-extractor.ts.md#findChild), [`name`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.name), [`name`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`params`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.params), [`source`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.source), [`callee`](../../types.ts.md#CallGraphEntry.callee), [`properties`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.properties), [`returnType`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.returnType), [`caller`](../../types.ts.md#CallGraphEntry.caller), [`specifiers`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.specifiers), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`lineNumber`](../../types.ts.md#StructuralAnalysis.exports.Array.typeLiteral3.lineNumber), [`lineRange`](../../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`findChildren`](base-extractor.ts.md#findChildren), [`lineNumber`](../../types.ts.md#StructuralAnalysis.imports.Array.typeLiteral2.lineNumber), [`CallGraphEntry`](../../types.ts.md#CallGraphEntry), [`lineRange`](../../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`lineNumber`](../../types.ts.md#CallGraphEntry.lineNumber), [`extractParams`](php-extractor.ts.md#extractParams), [`extractUseName`](php-extractor.ts.md#extractUseName), [`extractReturnType`](php-extractor.ts.md#extractReturnType), [`lastSegment`](php-extractor.ts.md#lastSegment)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-index.ts), [`LanguageExtractor`](types.ts.md#LanguageExtractor), [`php-extractor.test.ts`](__tests__/php-extractor.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-extractors-__tests__-php-extractor.test.ts), [`extractStructure`](types.ts.md#LanguageExtractor.extractStructure), [`extractCallGraph`](types.ts.md#LanguageExtractor.extractCallGraph), [`languageIds`](types.ts.md#LanguageExtractor.languageIds)

## Functions
- `extractParams(paramsNode: any)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L12) — Extract parameter names from a PHP `formal_parameters` node.
- `extractReturnType(node: any)` — [`L37`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L37) — Extract a return type string from the siblings following the `formal_parameters`
- `extractUseName(clause: any, prefix: string)` — [`L74`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L74) — Reconstruct a fully-qualified name from a `namespace_use_clause`.
- `lastSegment(fqn: string)` — [`L94`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/php-extractor.ts#L94) — Extract the last segment (class/interface name) from a fully-qualified name.

