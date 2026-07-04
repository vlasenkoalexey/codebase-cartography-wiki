---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`PortalNode.tsx`/Portal
symbols:
  PortalFlowNode: FlowNode#
  PortalNode: Node().
  PortalNodeData: NodeData#
  PortalNodeData.targetLayerId: NodeData#targetLayerId.
  PortalNodeData.targetLayerName: NodeData#targetLayerName.
  PortalNodeData.connectionCount: NodeData#connectionCount.
  PortalNodeData.layerColorIndex: NodeData#layerColorIndex.
  PortalNodeData.onNavigate: NodeData#onNavigate.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx)

## Classes
### `PortalFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx:14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L14) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `type PortalFlowNode`
- uses (calls/refs, reference-scoped): [`PortalNodeData`](PortalNode.tsx.md#PortalNodeData)
- used by: [`useLayerDetailTopology`](GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`PortalNode`](PortalNode.tsx.md#PortalNode), [`portalNodes`](GraphView.tsx.md#LayerDetailTopology.portalNodes)

### `PortalNodeData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L6)
- signature: `interface PortalNodeData`
- members:
  - `connectionCount` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L9)
  - `layerColorIndex` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L10)
  - `onNavigate` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L11)
  - `targetLayerId` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L7)
  - `targetLayerName` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L8)
- used by: [`PortalFlowNode`](PortalNode.tsx.md#PortalFlowNode)

## Functions
- `PortalNode({ data, }: NodeProps<Node<PortalNodeData, "portal">>)` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/PortalNode.tsx#L16)

