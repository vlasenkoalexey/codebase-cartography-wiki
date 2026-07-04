---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`yaml-parser.ts`/YAMLConfigParser#
symbols:
  YAMLConfigParser.analyzeFile: analyzeFile().
  YAMLConfigParser.extractSections: extractSections().
  YAMLConfigParser: ''
  YAMLConfigParser.languages: languages.
  YAMLConfigParser.escapeRegex: escapeRegex().
  YAMLConfigParser.name: name.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts)

## Classes
### `YAMLConfigParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts:14`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L14) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
- doc: Parses YAML configuration files to extract top-level key sections.
- signature: `class YAMLConfigParser`
- members:
  - `analyzeFile(method)` — [`L24`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L24)
  - `escapeRegex(method)` — [`L103`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L103)
  - `extractSections(method)` — [`L35`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L35)
  - `languages` — [`L16`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L16)
  - `name` — [`L15`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/yaml-parser.ts#L15)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`sections`](../../types.ts.md#StructuralAnalysis.sections), [`name`](../../types.ts.md#SectionInfo.name), [`lineRange`](../../types.ts.md#SectionInfo.lineRange), [`SectionInfo`](../../types.ts.md#SectionInfo), [`level`](../../types.ts.md#SectionInfo.level)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

