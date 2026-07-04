---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`DomainClusterNode.tsx`/DomainCluster
symbols:
  DomainClusterNode: Node().
  DomainClusterFlowNode: FlowNode#
  DomainClusterData: Data#
  DomainClusterData.label: Data#label.
  DomainClusterData.summary: Data#summary.
  DomainClusterData.entities: Data#entities.
  DomainClusterData.flowCount: Data#flowCount.
  DomainClusterData.businessRules: Data#businessRules.
  DomainClusterData.domainId: Data#domainId.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx)

## Classes
### `DomainClusterData`
- def: [`understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L6)
- signature: `interface DomainClusterData`
- members:
  - `businessRules` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L11)
  - `domainId` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L12)
  - `entities` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L9)
  - `flowCount` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L10)
  - `label` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L7)
  - `summary` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L8)
- used by: [`DomainClusterFlowNode`](DomainClusterNode.tsx.md#DomainClusterFlowNode)

### `DomainClusterFlowNode`
- def: [`understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx:15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L15)
- signature: `type DomainClusterFlowNode`
- uses (calls/refs, reference-scoped): [`DomainClusterData`](DomainClusterNode.tsx.md#DomainClusterData)
- used by: [`DomainGraphView.tsx`](DomainGraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-DomainGraphView.tsx), [`buildDomainOverview`](DomainGraphView.tsx.md#buildDomainOverview), [`DomainClusterNode`](DomainClusterNode.tsx.md#DomainClusterNode)

## Functions
- `DomainClusterNode({ data }: NodeProps<Node<DomainClusterData, "domain-cluster">>)` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/DomainClusterNode.tsx#L17)

