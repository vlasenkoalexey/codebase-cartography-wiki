---
title: 'Module: src/extraction/mybatis-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/mybatis-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`mybatis-extractor.ts`/MyBatisExtractor#
symbols:
  MyBatisExtractor.extractMapper: extractMapper().
  MyBatisExtractor.extract: extract().
  MyBatisExtractor.createFileNode: createFileNode().
  MyBatisExtractor.filePath: filePath.
  MyBatisExtractor.-constructor: '`<constructor>`().'
  MyBatisExtractor.source: source.
  MyBatisExtractor.computeLineStarts: computeLineStarts().
  MyBatisExtractor.nodes: nodes.
  MyBatisExtractor.getLineNumber: getLineNumber().
  MyBatisExtractor.edges: edges.
  MyBatisExtractor.unresolvedReferences: unresolvedReferences.
  MyBatisExtractor.errors: errors.
  MyBatisExtractor.lineStarts: lineStarts.
  MyBatisExtractor.findMapperRoot: findMapperRoot().
  MyBatisExtractor: ''
  MyBatisExtractor.buildSignature: buildSignature().
  MyBatisExtractor.previewSql: previewSql().
---
# Module: [`src/extraction/mybatis-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts)

## Classes
### `MyBatisExtractor`
- def: [`src/extraction/mybatis-extractor.ts:27`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L27)
- doc: MyBatisExtractor — parses MyBatis mapper XML files.
- signature: `class MyBatisExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L36`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L36) — MyBatisExtractor — parses MyBatis mapper XML files.
  - `buildSignature(method)` — [`L165`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L165)
  - `computeLineStarts(method)` — [`L180`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L180)
  - `createFileNode(method)` — [`L69`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L69)
  - `extract(method)` — [`L42`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L42)
  - `extractMapper(method)` — [`L106`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L106) — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `findMapperRoot(method)` — [`L94`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L94) — Find the `<mapper namespace="X">` opening tag. Returns the namespace and
  - `getLineNumber(method)` — [`L187`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L187)
  - `previewSql(method)` — [`L176`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L176)
  - `edges` — [`L31`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L31)
  - `errors` — [`L33`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L33)
  - `filePath` — [`L28`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L28)
  - `lineStarts` — [`L34`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L34)
  - `nodes` — [`L30`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L30)
  - `source` — [`L29`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L29)
  - `unresolvedReferences` — [`L32`](../../../../../../raw/code/codegraph/src/extraction/mybatis-extractor.ts#L32)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`signature`](../types.ts.md#Node.signature), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`edges`](../types.ts.md#ExtractionResult.edges), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`code`](../types.ts.md#ExtractionError.code), [`docstring`](../types.ts.md#Node.docstring), [`durationMs`](../types.ts.md#ExtractionResult.durationMs)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

