---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`FlowNode.tsx`/Flow
symbols:
  FlowNode: Node().
  FlowFlowNode: FlowNode#
  FlowNodeData: NodeData#
  FlowNodeData.label: NodeData#label.
  FlowNodeData.summary: NodeData#summary.
  FlowNodeData.entryPoint: NodeData#entryPoint.
  FlowNodeData.entryType: NodeData#entryType.
  FlowNodeData.stepCount: NodeData#stepCount.
  FlowNodeData.flowId: NodeData#flowId.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx)

## Classes
### `FlowFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx:15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L15)
- signature: `type FlowFlowNode`
- uses (calls/refs, reference-scoped): [`FlowNodeData`](FlowNode.tsx.md#FlowNodeData)
- used by: [`DomainGraphView.tsx`](DomainGraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-DomainGraphView.tsx), [`buildDomainDetail`](DomainGraphView.tsx.md#buildDomainDetail), [`FlowNode`](FlowNode.tsx.md#FlowNode)

### `FlowNodeData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L6)
- signature: `interface FlowNodeData`
- members:
  - `entryPoint` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L9)
  - `entryType` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L10)
  - `flowId` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L12)
  - `label` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L7)
  - `stepCount` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L11)
  - `summary` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L8)
- used by: [`FlowFlowNode`](FlowNode.tsx.md#FlowFlowNode)

## Functions
- `FlowNode({ data }: NodeProps<Node<FlowNodeData, "flow-node">>)` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FlowNode.tsx#L17)

