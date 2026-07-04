---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`makefile-parser.ts`/MakefileParser#
symbols:
  MakefileParser.analyzeFile: analyzeFile().
  MakefileParser: ''
  MakefileParser.extractTargets: extractTargets().
  MakefileParser.name: name.
  MakefileParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts)

## Classes
### `MakefileParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts#L8)
- doc: Parses Makefiles to extract build targets and their line ranges.
- signature: `class MakefileParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts#L12)
  - `extractTargets(method)` — [`L23`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts#L23)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/makefile-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`steps`](../../types.ts.md#StructuralAnalysis.steps), [`name`](../../types.ts.md#StepInfo.name), [`StepInfo`](../../types.ts.md#StepInfo), [`lineRange`](../../types.ts.md#StepInfo.lineRange)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

