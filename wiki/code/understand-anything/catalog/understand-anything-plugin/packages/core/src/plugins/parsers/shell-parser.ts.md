---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`shell-parser.ts`/ShellParser#
symbols:
  ShellParser.analyzeFile: analyzeFile().
  ShellParser.extractReferences: extractReferences().
  ShellParser: ''
  ShellParser.languages: languages.
  ShellParser.extractFunctions: extractFunctions().
  ShellParser.name: name.
  ShellParser.extractFunctions.Array.typeLiteral15.name: extractFunctions().Array:typeLiteral15:name.
  ShellParser.extractFunctions.Array.typeLiteral15.lineRange: extractFunctions().Array:typeLiteral15:lineRange.
  ShellParser.extractFunctions.Array.typeLiteral15.params: extractFunctions().Array:typeLiteral15:params.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts)

## Classes
### `ShellParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L8)
- doc: Parses shell scripts (.sh, .bash) to extract function definitions and source references.
- signature: `class ShellParser`
- members:
  - `analyzeFile(method)` — [`L14`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L14)
  - `extractFunctions(method)` — [`L42`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L42)
  - `extractReferences(method)` — [`L24`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L24)
  - `languages` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L12)
  - `lineRange` — [`L42`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L42)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L9)
  - `name` — [`L42`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L42)
  - `params` — [`L42`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/shell-parser.ts#L42)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`ReferenceResolution`](../../types.ts.md#ReferenceResolution), [`target`](../../types.ts.md#ReferenceResolution.target), [`line`](../../types.ts.md#ReferenceResolution.line), [`referenceType`](../../types.ts.md#ReferenceResolution.referenceType), [`source`](../../types.ts.md#ReferenceResolution.source)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages), [`extractReferences`](../../types.ts.md#AnalyzerPlugin.extractReferences)

