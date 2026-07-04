---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`layerStats.ts`/
symbols:
  computeLayerStats: computeLayerStats().
  LayerStats.aggregateComplexity: LayerStats#aggregateComplexity.
  LayerStats: LayerStats#
  Complexity: Complexity#
  LayerStats.resolvedCount: LayerStats#resolvedCount.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts)

## Classes
### `Complexity`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts:3`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts#L3)
- signature: `type Complexity`
- used by: [`computeLayerStats`](layerStats.ts.md#computeLayerStats), [`LayerStats`](layerStats.ts.md#LayerStats)

### `LayerStats`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts:5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts#L5)
- signature: `interface LayerStats`
- members:
  - `aggregateComplexity` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts#L9) — Aggregate label for the cluster card; matches the prior 30% threshold. — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `resolvedCount` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts#L7) — Number of layer.nodeIds that resolve to a node in the graph.
- uses (calls/refs, reference-scoped): [`Complexity`](layerStats.ts.md#Complexity)
- used by: [`useOverviewGraph`](../components/GraphView.tsx.md#useOverviewGraph), [`computeLayerStats`](layerStats.ts.md#computeLayerStats), [`layerStats.test.ts`](__tests__/layerStats.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-layerStats.test.ts)

## Functions
- `computeLayerStats(layer: Layer, nodesById: Map<string, GraphNode>)` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layerStats.ts#L20) — O(layer.nodeIds.length) summary of a layer's complexity composition. — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)

