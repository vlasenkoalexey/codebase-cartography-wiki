---
title: 'Module: src/extraction/liquid-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/liquid-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`liquid-extractor.ts`/LiquidExtractor#
symbols:
  LiquidExtractor.extractSnippetReferences: extractSnippetReferences().
  LiquidExtractor.extractSectionReferences: extractSectionReferences().
  LiquidExtractor.extractSchema: extractSchema().
  LiquidExtractor.extractAssignments: extractAssignments().
  LiquidExtractor.extract: extract().
  LiquidExtractor.createFileNode: createFileNode().
  LiquidExtractor.filePath: filePath.
  LiquidExtractor.extractShopifyJsonSections: extractShopifyJsonSections().
  LiquidExtractor.getLineStart: getLineStart().
  LiquidExtractor.nodes: nodes.
  LiquidExtractor.edges: edges.
  LiquidExtractor.source: source.
  LiquidExtractor.getLineNumber: getLineNumber().
  LiquidExtractor.unresolvedReferences: unresolvedReferences.
  LiquidExtractor.-constructor: '`<constructor>`().'
  LiquidExtractor.errors: errors.
  LiquidExtractor: ''
---
# Module: [`src/extraction/liquid-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts)

## Classes
### `LiquidExtractor`
- def: [`src/extraction/liquid-extractor.ts:13`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L13)
- doc: LiquidExtractor - Extracts relationships from Liquid template files
- signature: `class LiquidExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L21`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L21) — LiquidExtractor - Extracts relationships from Liquid template files
  - `createFileNode(method)` — [`L75`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L75) — Create a file node for the Liquid template
  - `extract(method)` — [`L29`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L29) — Extract from Liquid source
  - `extractAssignments(method)` — [`L337`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L337) — Extract {% assign var = value %} statements — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `extractSchema(method)` — [`L278`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L278) — Extract {% schema %}...{% endschema %} blocks — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `extractSectionReferences(method)` — [`L204`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L204) — Extract {% section 'name' %} references — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `extractShopifyJsonSections(method)` — [`L103`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L103) — Shopify OS 2.0 JSON template / section group. Both have a `sections` object
  - `extractSnippetReferences(method)` — [`L130`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L130) — Extract {% render 'snippet' %} and {% include 'snippet' %} references — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `getLineNumber(method)` — [`L377`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L377) — Get the line number for a character index
  - `getLineStart(method)` — [`L385`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L385) — Get the character index of the start of a line
  - `edges` — [`L17`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L17)
  - `errors` — [`L19`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L19)
  - `filePath` — [`L14`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L14)
  - `nodes` — [`L16`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L16)
  - `source` — [`L15`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L15)
  - `unresolvedReferences` — [`L18`](../../../../../../raw/code/codegraph/src/extraction/liquid-extractor.ts#L18)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`signature`](../types.ts.md#Node.signature), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`edges`](../types.ts.md#ExtractionResult.edges), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`code`](../types.ts.md#ExtractionError.code), [`durationMs`](../types.ts.md#ExtractionResult.durationMs)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

