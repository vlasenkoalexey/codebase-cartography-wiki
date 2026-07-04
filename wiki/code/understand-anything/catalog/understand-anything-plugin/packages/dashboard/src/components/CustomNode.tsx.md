---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`CustomNode.tsx`/
symbols:
  CustomNodeComponent: CustomNodeComponent().
  CustomFlowNode: CustomFlowNode#
  CustomNodeData: CustomNodeData#
  CustomNodeData.summary: CustomNodeData#summary.
  CustomNode: CustomNode.
  typeColors: typeColors.
  CustomNodeData.nodeType: CustomNodeData#nodeType.
  CustomNodeData.complexity: CustomNodeData#complexity.
  typeTextColors: typeTextColors.
  complexityColors: complexityColors.
  CustomNodeData.label: CustomNodeData#label.
  CustomNodeData.isHighlighted: CustomNodeData#isHighlighted.
  CustomNodeData.searchScore: CustomNodeData#searchScore.
  CustomNodeData.isSelected: CustomNodeData#isSelected.
  CustomNodeData.isTourHighlighted: CustomNodeData#isTourHighlighted.
  CustomNodeData.isDiffChanged: CustomNodeData#isDiffChanged.
  CustomNodeData.isDiffAffected: CustomNodeData#isDiffAffected.
  CustomNodeData.isDiffFaded: CustomNodeData#isDiffFaded.
  CustomNodeData.isNeighbor: CustomNodeData#isNeighbor.
  CustomNodeData.isSelectionFaded: CustomNodeData#isSelectionFaded.
  CustomNodeData.onNodeClick: CustomNodeData#onNodeClick.
  CustomNodeData.incomingCount: CustomNodeData#incomingCount.
  CustomNodeData.tags: CustomNodeData#tags.
  CustomNodeData.outgoingCount: CustomNodeData#outgoingCount.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx)

## Classes
### `CustomFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx:82`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L82) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- signature: `type CustomFlowNode`
- uses (calls/refs, reference-scoped): [`CustomNodeData`](CustomNode.tsx.md#CustomNodeData)
- used by: [`useLayerDetailTopology`](GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`useLayerDetailGraph`](GraphView.tsx.md#useLayerDetailGraph), [`CustomNodeComponent`](CustomNode.tsx.md#CustomNodeComponent), [`buildCustomFlowNode`](GraphView.tsx.md#buildCustomFlowNode)

### `CustomNodeData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx:62`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L62) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- signature: `interface CustomNodeData`
- members:
  - `complexity` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L66)
  - `incomingCount` — [`L77`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L77)
  - `isDiffAffected` — [`L72`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L72)
  - `isDiffChanged` — [`L71`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L71)
  - `isDiffFaded` — [`L73`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L73)
  - `isHighlighted` — [`L67`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L67)
  - `isNeighbor` — [`L74`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L74)
  - `isSelected` — [`L69`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L69)
  - `isSelectionFaded` — [`L75`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L75)
  - `isTourHighlighted` — [`L70`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L70)
  - `label` — [`L63`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L63)
  - `nodeType` — [`L64`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L64)
  - `onNodeClick` — [`L76`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L76)
  - `outgoingCount` — [`L78`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L78)
  - `searchScore` — [`L68`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L68)
  - `summary` — [`L65`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L65)
  - `tags` — [`L79`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L79)
- used by: [`KnowledgeGraphViewInner`](KnowledgeGraphView.tsx.md#KnowledgeGraphViewInner), [`NodeTooltip`](NodeTooltip.tsx.md#NodeTooltip), [`KnowledgeGraphView.tsx`](KnowledgeGraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-KnowledgeGraphView.tsx), [`CustomFlowNode`](CustomNode.tsx.md#CustomFlowNode), [`NodeTooltip.tsx`](NodeTooltip.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-NodeTooltip.tsx), [`data`](NodeTooltip.tsx.md#NodeTooltipProps.data)

## Functions
- `CustomNodeComponent({ id, data, }: NodeProps<Node<CustomNodeData, "custom">>)` — [`L84`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L84) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)

## Module values
- `CustomNode` — [`L189`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L189) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `complexityColors` — [`L56`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L56) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `typeColors` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L8) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `typeTextColors` — [`L32`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CustomNode.tsx#L32) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)

