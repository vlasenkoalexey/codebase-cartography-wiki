---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`dockerfile-parser.ts`/DockerfileParser#
symbols:
  DockerfileParser.analyzeFile: analyzeFile().
  DockerfileParser.extractStages: extractStages().
  DockerfileParser: ''
  DockerfileParser.extractSteps: extractSteps().
  DockerfileParser.name: name.
  DockerfileParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts)

## Classes
### `DockerfileParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L8)
- doc: Parses Dockerfiles to extract multi-stage build stages, EXPOSE ports, and instruction steps.
- signature: `class DockerfileParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L12) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `extractStages(method)` — [`L25`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L25)
  - `extractSteps(method)` — [`L72`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L72)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/dockerfile-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`services`](../../types.ts.md#StructuralAnalysis.services), [`steps`](../../types.ts.md#StructuralAnalysis.steps), [`ports`](../../types.ts.md#ServiceInfo.ports), [`name`](../../types.ts.md#StepInfo.name), [`lineRange`](../../types.ts.md#ServiceInfo.lineRange), [`name`](../../types.ts.md#ServiceInfo.name), [`StepInfo`](../../types.ts.md#StepInfo), [`ServiceInfo`](../../types.ts.md#ServiceInfo), [`image`](../../types.ts.md#ServiceInfo.image), [`lineRange`](../../types.ts.md#StepInfo.lineRange)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

