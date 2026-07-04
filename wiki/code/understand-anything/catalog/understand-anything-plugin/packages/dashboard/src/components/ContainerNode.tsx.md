---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`ContainerNode.tsx`/Container
symbols:
  ContainerNodeComponent: NodeComponent().
  ContainerFlowNode: FlowNode#
  ContainerNode: Node.
  ContainerNodeData: NodeData#
  ContainerNodeData.isExpanded: NodeData#isExpanded.
  ContainerNodeData.hasSearchHits: NodeData#hasSearchHits.
  ContainerNodeData.searchHitCount: NodeData#searchHitCount.
  ContainerNodeData.isDiffAffected: NodeData#isDiffAffected.
  ContainerNodeData.isFocusedViaChild: NodeData#isFocusedViaChild.
  ContainerNodeData.containerId: NodeData#containerId.
  ContainerNodeData.name: NodeData#name.
  ContainerNodeData.childCount: NodeData#childCount.
  ContainerNodeData.strategy: NodeData#strategy.
  ContainerNodeData.colorIndex: NodeData#colorIndex.
  ContainerNodeData.onToggle: NodeData#onToggle.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx)

## Classes
### `ContainerFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx:19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L19) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `type ContainerFlowNode`
- uses (calls/refs, reference-scoped): [`ContainerNodeData`](ContainerNode.tsx.md#ContainerNodeData)
- used by: [`useLayerDetailTopology`](GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`ContainerNodeComponent`](ContainerNode.tsx.md#ContainerNodeComponent)

### `ContainerNodeData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx:5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L5)
- signature: `interface ContainerNodeData`
- members:
  - `childCount` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L8)
  - `colorIndex` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L10)
  - `containerId` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L6)
  - `hasSearchHits` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L12)
  - `isDiffAffected` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L14)
  - `isExpanded` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L11)
  - `isFocusedViaChild` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L15)
  - `name` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L7)
  - `onToggle` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L16)
  - `searchHitCount` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L13)
  - `strategy` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L9)
- used by: [`GraphView.tsx`](GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`useLayerDetailGraph`](GraphView.tsx.md#useLayerDetailGraph), [`ContainerFlowNode`](ContainerNode.tsx.md#ContainerFlowNode)

## Functions
- `ContainerNodeComponent({ data, width, height }: NodeProps<Node<ContainerNodeData, "container">>)` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L21)

## Module values
- `ContainerNode` — [`L98`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/ContainerNode.tsx#L98)

