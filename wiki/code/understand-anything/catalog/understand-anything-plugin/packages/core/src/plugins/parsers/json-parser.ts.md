---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`json-parser.ts`/
symbols:
  JSONConfigParser.analyzeFile: JSONConfigParser#analyzeFile().
  JSONConfigParser.extractReferences: JSONConfigParser#extractReferences().
  JSONConfigParser.extractSections: JSONConfigParser#extractSections().
  stripJsoncSyntax: stripJsoncSyntax().
  JSONConfigParser: JSONConfigParser#
  JSONConfigParser.languages: JSONConfigParser#languages.
  JSONConfigParser.name: JSONConfigParser#name.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts)

## Classes
### `JSONConfigParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts:69`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L69)
- doc: Parses JSON / JSONC configuration files to extract top-level key sections and $ref references.
- signature: `class JSONConfigParser`
- members:
  - `analyzeFile(method)` — [`L76`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L76)
  - `extractReferences(method)` — [`L87`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L87)
  - `extractSections(method)` — [`L106`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L106)
  - `languages` — [`L74`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L74)
  - `name` — [`L70`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L70)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`sections`](../../types.ts.md#StructuralAnalysis.sections), [`name`](../../types.ts.md#SectionInfo.name), [`lineRange`](../../types.ts.md#SectionInfo.lineRange), [`SectionInfo`](../../types.ts.md#SectionInfo), [`ReferenceResolution`](../../types.ts.md#ReferenceResolution), [`stripJsoncSyntax`](json-parser.ts.md#stripJsoncSyntax), [`level`](../../types.ts.md#SectionInfo.level), [`target`](../../types.ts.md#ReferenceResolution.target), [`line`](../../types.ts.md#ReferenceResolution.line), [`referenceType`](../../types.ts.md#ReferenceResolution.referenceType), [`source`](../../types.ts.md#ReferenceResolution.source)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages), [`extractReferences`](../../types.ts.md#AnalyzerPlugin.extractReferences)

## Functions
- `stripJsoncSyntax(content: string)` — [`L11`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/json-parser.ts#L11) — Strip JSONC syntax (line comments, block comments, trailing commas) so the

