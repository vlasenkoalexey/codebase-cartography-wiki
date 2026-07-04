---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`LayerClusterNode.tsx`/
symbols:
  LayerClusterNode: LayerClusterNode().
  LayerClusterFlowNode: LayerClusterFlowNode#
  complexityColors: complexityColors.
  LayerClusterData: LayerClusterData#
  LayerClusterData.layerId: LayerClusterData#layerId.
  LayerClusterData.layerName: LayerClusterData#layerName.
  LayerClusterData.layerDescription: LayerClusterData#layerDescription.
  LayerClusterData.fileCount: LayerClusterData#fileCount.
  LayerClusterData.aggregateComplexity: LayerClusterData#aggregateComplexity.
  LayerClusterData.layerColorIndex: LayerClusterData#layerColorIndex.
  LayerClusterData.searchMatchCount: LayerClusterData#searchMatchCount.
  LayerClusterData.onDrillIn: LayerClusterData#onDrillIn.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx)

## Classes
### `LayerClusterData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx:12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L12)
- signature: `interface LayerClusterData`
- members:
  - `aggregateComplexity` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L17)
  - `fileCount` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L16)
  - `layerColorIndex` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L18)
  - `layerDescription` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L15)
  - `layerId` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L13)
  - `layerName` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L14)
  - `onDrillIn` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L20)
  - `searchMatchCount` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L19)
- used by: [`LayerClusterFlowNode`](LayerClusterNode.tsx.md#LayerClusterFlowNode)

### `LayerClusterFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx:23`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L23) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `type LayerClusterFlowNode`
- uses (calls/refs, reference-scoped): [`LayerClusterData`](LayerClusterNode.tsx.md#LayerClusterData)
- used by: [`GraphView.tsx`](GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`useOverviewGraph`](GraphView.tsx.md#useOverviewGraph), [`LayerClusterNode`](LayerClusterNode.tsx.md#LayerClusterNode)

## Functions
- `LayerClusterNode({ data, }: NodeProps<Node<LayerClusterData, "layer-cluster">>)` — [`L25`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L25)

## Module values
- `complexityColors` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/LayerClusterNode.tsx#L6)

