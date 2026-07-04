---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`edgeAggregation.ts`/
symbols:
  aggregateContainerEdges: aggregateContainerEdges().
  computePortals: computePortals().
  ContainerEdgeBuckets.interContainerAggregated: ContainerEdgeBuckets#interContainerAggregated.
  aggregateLayerEdges: aggregateLayerEdges().
  PortalInfo.layerId: PortalInfo#layerId.
  ContainerEdgeBuckets.intraContainer: ContainerEdgeBuckets#intraContainer.
  LayerEdgeAggregation.sourceLayerId: LayerEdgeAggregation#sourceLayerId.
  LayerEdgeAggregation.targetLayerId: LayerEdgeAggregation#targetLayerId.
  LayerEdgeAggregation.count: LayerEdgeAggregation#count.
  ContainerEdgeBuckets: ContainerEdgeBuckets#
  AggregatedContainerEdge.sourceContainerId: AggregatedContainerEdge#sourceContainerId.
  AggregatedContainerEdge.targetContainerId: AggregatedContainerEdge#targetContainerId.
  AggregatedContainerEdge.count: AggregatedContainerEdge#count.
  LayerEdgeAggregation: LayerEdgeAggregation#
  findCrossLayerFileNodes: findCrossLayerFileNodes().
  AggregatedContainerEdge: AggregatedContainerEdge#
  PortalInfo: PortalInfo#
  PortalInfo.layerName: PortalInfo#layerName.
  PortalInfo.connectionCount: PortalInfo#connectionCount.
  AggregatedContainerEdge.edgeTypes: AggregatedContainerEdge#edgeTypes.
  LayerEdgeAggregation.edgeTypes: LayerEdgeAggregation#edgeTypes.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts)

## Classes
### `AggregatedContainerEdge`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts:137`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L137) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
- signature: `interface AggregatedContainerEdge`
- members:
  - `count` — [`L140`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L140)
  - `edgeTypes` — [`L141`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L141)
  - `sourceContainerId` — [`L138`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L138)
  - `targetContainerId` — [`L139`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L139)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`edgeAggregation.test.ts`](__tests__/edgeAggregation.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-edgeAggregation.test.ts), [`aggregateContainerEdges`](edgeAggregation.ts.md#aggregateContainerEdges), [`ContainerEdgeBuckets`](edgeAggregation.ts.md#ContainerEdgeBuckets)

### `ContainerEdgeBuckets`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts:144`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L144) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
- signature: `interface ContainerEdgeBuckets`
- members:
  - `interContainerAggregated` — [`L146`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L146) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `intraContainer` — [`L145`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L145) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- uses (calls/refs, reference-scoped): [`AggregatedContainerEdge`](edgeAggregation.ts.md#AggregatedContainerEdge)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`edgeAggregation.test.ts`](__tests__/edgeAggregation.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-edgeAggregation.test.ts), [`aggregateContainerEdges`](edgeAggregation.ts.md#aggregateContainerEdges)

### `LayerEdgeAggregation`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts:3`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L3) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
- signature: `interface LayerEdgeAggregation`
- members:
  - `count` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L6) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `edgeTypes` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L7)
  - `sourceLayerId` — [`L4`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L4) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
  - `targetLayerId` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L5) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
- used by: [`useOverviewGraph`](../components/GraphView.tsx.md#useOverviewGraph), [`computePortals`](edgeAggregation.ts.md#computePortals), [`aggregateLayerEdges`](edgeAggregation.ts.md#aggregateLayerEdges)

### `PortalInfo`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts:10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L10) — documented in [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md)
- signature: `interface PortalInfo`
- members:
  - `connectionCount` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L13)
  - `layerId` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L11) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `layerName` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L12)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`computePortals`](edgeAggregation.ts.md#computePortals)

## Functions
- `aggregateContainerEdges(edges: GraphEdge[], nodeToContainer: Map<string, string>)` — [`L158`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L158) — Bucket edges into intra-container (preserved) and inter-container — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `aggregateLayerEdges(graph: KnowledgeGraph)` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L21) — Aggregate edges between layers. Counts how many graph edges cross — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `computePortals(graph: KnowledgeGraph, activeLayerId: string, precomputed?: LayerEdgeAggregation[] | undefined)` — [`L77`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L77) — Compute portal info for a given layer: which other layers are connected — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `findCrossLayerFileNodes(graph: KnowledgeGraph, activeLayerId: string, targetLayerId: string)` — [`L113`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/edgeAggregation.ts#L113) — For a given layer, find which file nodes in that layer connect to a

