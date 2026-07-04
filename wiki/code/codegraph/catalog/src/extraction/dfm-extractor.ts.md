---
title: 'Module: src/extraction/dfm-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/dfm-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`dfm-extractor.ts`/DfmExtractor#
symbols:
  DfmExtractor.parseComponents: parseComponents().
  DfmExtractor.extract: extract().
  DfmExtractor.createFileNode: createFileNode().
  DfmExtractor.filePath: filePath.
  DfmExtractor.-constructor: '`<constructor>`().'
  DfmExtractor.nodes: nodes.
  DfmExtractor.edges: edges.
  DfmExtractor.unresolvedReferences: unresolvedReferences.
  DfmExtractor.errors: errors.
  DfmExtractor.source: source.
  DfmExtractor: ''
---
# Module: [`src/extraction/dfm-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts)

## Classes
### `DfmExtractor`
- def: [`src/extraction/dfm-extractor.ts:16`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L16)
- doc: Custom extractor for Delphi DFM/FMX form files.
- signature: `class DfmExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L24`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L24) — Custom extractor for Delphi DFM/FMX form files.
  - `createFileNode(method)` — [`L56`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L56) — Create a file node for the DFM form file
  - `extract(method)` — [`L32`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L32) — Extract components and event handler references from DFM/FMX source
  - `parseComponents(method)` — [`L79`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L79) — Parse object/end blocks and extract components + event handlers — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `edges` — [`L20`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L20)
  - `errors` — [`L22`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L22)
  - `filePath` — [`L17`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L17)
  - `nodes` — [`L19`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L19)
  - `source` — [`L18`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L18)
  - `unresolvedReferences` — [`L21`](../../../../../../raw/code/codegraph/src/extraction/dfm-extractor.ts#L21)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`signature`](../types.ts.md#Node.signature), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`edges`](../types.ts.md#ExtractionResult.edges), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`code`](../types.ts.md#ExtractionError.code), [`durationMs`](../types.ts.md#ExtractionResult.durationMs)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

