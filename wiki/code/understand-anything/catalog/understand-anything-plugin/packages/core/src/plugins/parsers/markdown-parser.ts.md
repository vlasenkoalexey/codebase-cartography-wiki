---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`markdown-parser.ts`/MarkdownParser#
symbols:
  MarkdownParser.analyzeFile: analyzeFile().
  MarkdownParser.extractReferences: extractReferences().
  MarkdownParser.extractSections: extractSections().
  MarkdownParser: ''
  MarkdownParser.name: name.
  MarkdownParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts)

## Classes
### `MarkdownParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L8) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
- doc: Parses Markdown files to extract heading sections and local file/image references.
- signature: `class MarkdownParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L12)
  - `extractReferences(method)` — [`L23`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L23)
  - `extractSections(method)` — [`L41`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L41)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/markdown-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`sections`](../../types.ts.md#StructuralAnalysis.sections), [`name`](../../types.ts.md#SectionInfo.name), [`lineRange`](../../types.ts.md#SectionInfo.lineRange), [`SectionInfo`](../../types.ts.md#SectionInfo), [`ReferenceResolution`](../../types.ts.md#ReferenceResolution), [`level`](../../types.ts.md#SectionInfo.level), [`target`](../../types.ts.md#ReferenceResolution.target), [`line`](../../types.ts.md#ReferenceResolution.line), [`referenceType`](../../types.ts.md#ReferenceResolution.referenceType), [`source`](../../types.ts.md#ReferenceResolution.source)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages), [`extractReferences`](../../types.ts.md#AnalyzerPlugin.extractReferences)

