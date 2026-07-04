---
title: 'Module: understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/analyzer/`normalize-graph.ts`/
symbols:
  normalizeBatchOutput: normalizeBatchOutput().
  normalizeNodeId.node-typeLiteral16.type: normalizeNodeId().(node)typeLiteral16:type.
  normalizeNodeId: normalizeNodeId().
  normalizeComplexity: normalizeComplexity().
  normalizeNodeId.node-typeLiteral16.parentFlowSlug: normalizeNodeId().(node)typeLiteral16:parentFlowSlug.
  NormalizeBatchResult.stats: NormalizeBatchResult#stats.
  normalizeNodeId.node-typeLiteral16.filePath: normalizeNodeId().(node)typeLiteral16:filePath.
  NormalizeBatchResult.edges: NormalizeBatchResult#edges.
  normalizeNodeId.node-typeLiteral16.name: normalizeNodeId().(node)typeLiteral16:name.
  NormalizeBatchResult.nodes: NormalizeBatchResult#nodes.
  normalizeBatchOutput.data-typeLiteral53.nodes: normalizeBatchOutput().(data)typeLiteral53:nodes.
  normalizeBatchOutput.data-typeLiteral53.edges: normalizeBatchOutput().(data)typeLiteral53:edges.
  stripToValidPrefix: stripToValidPrefix().
  NormalizationStats.droppedEdges: NormalizationStats#droppedEdges.
  NormalizationStats.danglingEdgesDropped: NormalizationStats#danglingEdgesDropped.
  inferTypeFromId: inferTypeFromId().
  NormalizationStats.idsFixed: NormalizationStats#idsFixed.
  NormalizationStats.complexityFixed: NormalizationStats#complexityFixed.
  NormalizationStats.edgesRewritten: NormalizationStats#edgesRewritten.
  stripToValidPrefix.typeLiteral0.prefix: stripToValidPrefix().typeLiteral0:prefix.
  stripToValidPrefix.typeLiteral0.path: stripToValidPrefix().typeLiteral0:path.
  NormalizationStats: NormalizationStats#
  VALID_PREFIXES: VALID_PREFIXES.
  DroppedEdge: DroppedEdge#
  NormalizeBatchResult: NormalizeBatchResult#
  PREFIX_TO_TYPE: PREFIX_TO_TYPE.
  TYPE_TO_PREFIX: TYPE_TO_PREFIX.
  VALID_COMPLEXITIES: VALID_COMPLEXITIES.
  COMPLEXITY_STRING_MAP: COMPLEXITY_STRING_MAP.
  DroppedEdge.source: DroppedEdge#source.
  DroppedEdge.target: DroppedEdge#target.
  DroppedEdge.type: DroppedEdge#type.
  DroppedEdge.reason: DroppedEdge#reason.
  NormalizeBatchResult.idMap: NormalizeBatchResult#idMap.
---
# Module: [`understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts)

## Classes
### `DroppedEdge`
- def: [`understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts:154`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L154) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- signature: `interface DroppedEdge`
- members:
  - `reason` — [`L158`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L158) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `source` — [`L155`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L155) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `target` — [`L156`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L156) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `type` — [`L157`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L157) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`normalizeBatchOutput`](normalize-graph.ts.md#normalizeBatchOutput), [`droppedEdges`](normalize-graph.ts.md#NormalizationStats.droppedEdges)

### `NormalizationStats`
- def: [`understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts:161`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L161) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- signature: `interface NormalizationStats`
- members:
  - `complexityFixed` — [`L163`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L163) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `danglingEdgesDropped` — [`L165`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L165) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `droppedEdges` — [`L166`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L166) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `edgesRewritten` — [`L164`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L164) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `idsFixed` — [`L162`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L162) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- uses (calls/refs, reference-scoped): [`DroppedEdge`](normalize-graph.ts.md#DroppedEdge)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`normalizeBatchOutput`](normalize-graph.ts.md#normalizeBatchOutput), [`normalize-graph.test.ts`](../__tests__/normalize-graph.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-normalize-graph.test.ts), [`stats`](normalize-graph.ts.md#NormalizeBatchResult.stats)

### `NormalizeBatchResult`
- def: [`understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts:169`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L169) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- signature: `interface NormalizeBatchResult`
- members:
  - `edges` — [`L171`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L171) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `idMap` — [`L172`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L172) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `nodes` — [`L170`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L170) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
  - `stats` — [`L173`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L173) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- uses (calls/refs, reference-scoped): [`NormalizationStats`](normalize-graph.ts.md#NormalizationStats)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`normalizeBatchOutput`](normalize-graph.ts.md#normalizeBatchOutput), [`normalize-graph.test.ts`](../__tests__/normalize-graph.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-normalize-graph.test.ts)

## Functions
- `inferTypeFromId(id: string)` — [`L185`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L185) — Infer node type from an ID's prefix (e.g. "step:foo" → "step"). Falls back to "file". — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `normalizeBatchOutput(data: { nodes: Record<string, unknown>[]; edges: Record<string, unknown>[]; })` — [`L202`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L202) — Normalizes a merged batch output: fixes node IDs and numeric complexity, — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `normalizeComplexity(value: unknown)` — [`L134`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L134) — Normalizes a complexity value to one of "simple" | "moderate" | "complex". — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `normalizeNodeId(id: string, node: { type: string; filePath?: string | undefined; name?: string | undefined; parentFlowSlug?: string | undefined; })` — [`L64`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L64) — Normalizes a node ID to the canonical `type:path` format. — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `stripToValidPrefix(id: string)` — [`L31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L31) — Strips all non-valid prefixes from an ID, returning the bare path — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)

## Module values
- `COMPLEXITY_STRING_MAP` — [`L115`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L115) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `PREFIX_TO_TYPE` — [`L176`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L176) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `TYPE_TO_PREFIX` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L8) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `VALID_COMPLEXITIES` — [`L113`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L113) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `VALID_PREFIXES` — [`L1`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L1) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `edges` — [`L204`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L204) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `filePath` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L66) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `name` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L66) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `nodes` — [`L203`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L203) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `parentFlowSlug` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L66) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `path` — [`L31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L31) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `prefix` — [`L31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L31) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- `type` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts#L66) — documented in [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)

