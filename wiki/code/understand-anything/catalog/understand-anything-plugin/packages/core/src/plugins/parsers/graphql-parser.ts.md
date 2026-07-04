---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`graphql-parser.ts`/GraphQLParser#
symbols:
  GraphQLParser.analyzeFile: analyzeFile().
  GraphQLParser.extractDefinitions: extractDefinitions().
  GraphQLParser.extractEndpoints: extractEndpoints().
  GraphQLParser: ''
  GraphQLParser.extractFields: extractFields().
  GraphQLParser.name: name.
  GraphQLParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts)

## Classes
### `GraphQLParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L8)
- doc: Parses GraphQL schema files to extract type, input, enum, interface, union, and scalar definitions.
- signature: `class GraphQLParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L12)
  - `extractDefinitions(method)` — [`L25`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L25)
  - `extractEndpoints(method)` — [`L58`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L58)
  - `extractFields(method)` — [`L97`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L97)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/graphql-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`definitions`](../../types.ts.md#StructuralAnalysis.definitions), [`fields`](../../types.ts.md#DefinitionInfo.fields), [`name`](../../types.ts.md#DefinitionInfo.name), [`kind`](../../types.ts.md#DefinitionInfo.kind), [`DefinitionInfo`](../../types.ts.md#DefinitionInfo), [`lineRange`](../../types.ts.md#DefinitionInfo.lineRange), [`endpoints`](../../types.ts.md#StructuralAnalysis.endpoints), [`EndpointInfo`](../../types.ts.md#EndpointInfo), [`path`](../../types.ts.md#EndpointInfo.path), [`method`](../../types.ts.md#EndpointInfo.method), [`lineRange`](../../types.ts.md#EndpointInfo.lineRange)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

