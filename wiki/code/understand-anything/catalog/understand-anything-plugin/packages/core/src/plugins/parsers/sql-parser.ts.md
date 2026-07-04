---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`sql-parser.ts`/SQLParser#
symbols:
  SQLParser.analyzeFile: analyzeFile().
  SQLParser.extractDefinitions: extractDefinitions().
  SQLParser: ''
  SQLParser.extractColumns: extractColumns().
  SQLParser.name: name.
  SQLParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts)

## Classes
### `SQLParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L8) — documented in [understand-anything-plugin-packages-core-src-plugins-registry.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md)
- doc: Parses SQL files to extract table, view, and index definitions.
- signature: `class SQLParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L12)
  - `extractColumns(method)` — [`L78`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L78)
  - `extractDefinitions(method)` — [`L23`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L23)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/sql-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`definitions`](../../types.ts.md#StructuralAnalysis.definitions), [`fields`](../../types.ts.md#DefinitionInfo.fields), [`name`](../../types.ts.md#DefinitionInfo.name), [`kind`](../../types.ts.md#DefinitionInfo.kind), [`DefinitionInfo`](../../types.ts.md#DefinitionInfo), [`lineRange`](../../types.ts.md#DefinitionInfo.lineRange)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

