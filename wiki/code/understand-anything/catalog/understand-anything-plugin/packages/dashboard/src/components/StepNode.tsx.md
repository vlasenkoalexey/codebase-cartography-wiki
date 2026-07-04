---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`StepNode.tsx`/Step
symbols:
  StepNode: Node().
  StepFlowNode: FlowNode#
  StepNodeData: NodeData#
  StepNodeData.label: NodeData#label.
  StepNodeData.summary: NodeData#summary.
  StepNodeData.filePath: NodeData#filePath.
  StepNodeData.stepId: NodeData#stepId.
  StepNodeData.order: NodeData#order.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx)

## Classes
### `StepFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx:14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L14)
- signature: `type StepFlowNode`
- uses (calls/refs, reference-scoped): [`StepNodeData`](StepNode.tsx.md#StepNodeData)
- used by: [`DomainGraphView.tsx`](DomainGraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-DomainGraphView.tsx), [`buildDomainDetail`](DomainGraphView.tsx.md#buildDomainDetail), [`StepNode`](StepNode.tsx.md#StepNode)

### `StepNodeData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L6)
- signature: `interface StepNodeData`
- members:
  - `filePath` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L9)
  - `label` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L7)
  - `order` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L11)
  - `stepId` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L10)
  - `summary` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L8)
- used by: [`StepFlowNode`](StepNode.tsx.md#StepFlowNode)

## Functions
- `StepNode({ data }: NodeProps<Node<StepNodeData, "step-node">>)` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/StepNode.tsx#L16)

