---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/parsers/`protobuf-parser.ts`/ProtobufParser#
symbols:
  ProtobufParser.analyzeFile: analyzeFile().
  ProtobufParser.extractDefinitions: extractDefinitions().
  ProtobufParser.extractServiceMethods: extractServiceMethods().
  ProtobufParser: ''
  ProtobufParser.findClosingBrace: findClosingBrace().
  ProtobufParser.extractMessageFields: extractMessageFields().
  ProtobufParser.extractEnumValues: extractEnumValues().
  ProtobufParser.name: name.
  ProtobufParser.languages: languages.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts)

## Classes
### `ProtobufParser`  ·  implements/extends AnalyzerPlugin
- def: [`understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts:8`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L8)
- doc: Parses Protocol Buffer (.proto) files to extract message, enum, and service definitions.
- signature: `class ProtobufParser`
- members:
  - `analyzeFile(method)` — [`L12`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L12)
  - `extractDefinitions(method)` — [`L25`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L25)
  - `extractEnumValues(method)` — [`L109`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L109)
  - `extractMessageFields(method)` — [`L91`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L91)
  - `extractServiceMethods(method)` — [`L66`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L66)
  - `findClosingBrace(method)` — [`L127`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L127)
  - `languages` — [`L10`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L10)
  - `name` — [`L9`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/parsers/protobuf-parser.ts#L9)
- uses (calls/refs, reference-scoped): [`functions`](../../types.ts.md#StructuralAnalysis.functions), [`classes`](../../types.ts.md#StructuralAnalysis.classes), [`imports`](../../types.ts.md#StructuralAnalysis.imports), [`StructuralAnalysis`](../../types.ts.md#StructuralAnalysis), [`exports`](../../types.ts.md#StructuralAnalysis.exports), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`definitions`](../../types.ts.md#StructuralAnalysis.definitions), [`fields`](../../types.ts.md#DefinitionInfo.fields), [`name`](../../types.ts.md#DefinitionInfo.name), [`kind`](../../types.ts.md#DefinitionInfo.kind), [`DefinitionInfo`](../../types.ts.md#DefinitionInfo), [`lineRange`](../../types.ts.md#DefinitionInfo.lineRange), [`endpoints`](../../types.ts.md#StructuralAnalysis.endpoints), [`EndpointInfo`](../../types.ts.md#EndpointInfo), [`path`](../../types.ts.md#EndpointInfo.path), [`method`](../../types.ts.md#EndpointInfo.method), [`lineRange`](../../types.ts.md#EndpointInfo.lineRange)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsers.test.ts`](../../__tests__/parsers.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-parsers.test.ts), [`AnalyzerPlugin`](../../types.ts.md#AnalyzerPlugin), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-plugins-parsers-index.ts), [`analyzeFile`](../../types.ts.md#AnalyzerPlugin.analyzeFile), [`registerAllParsers`](index.ts.md#registerAllParsers), [`name`](../../types.ts.md#AnalyzerPlugin.name), [`languages`](../../types.ts.md#AnalyzerPlugin.languages)

