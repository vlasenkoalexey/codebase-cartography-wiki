---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`GraphView.tsx`/
symbols:
  useLayerDetailTopology: useLayerDetailTopology().
  useLayerDetailGraph: useLayerDetailGraph().
  useOverviewGraph: useOverviewGraph().
  EMPTY_TOPOLOGY: EMPTY_TOPOLOGY.
  GraphViewInner: GraphViewInner().
  LayerDetailTopology.nodeToContainer: LayerDetailTopology#nodeToContainer.
  buildCustomFlowNode: buildCustomFlowNode().
  nodeTypes: nodeTypes.
  LayerDetailTopology.filteredEdges: LayerDetailTopology#filteredEdges.
  LayerDetailTopology.containers: LayerDetailTopology#containers.
  GraphView: GraphView().
  LayerDetailTopology.edges: LayerDetailTopology#edges.
  buildCustomFlowNode.opts-typeLiteral756.diffMode: buildCustomFlowNode().(opts)typeLiteral756:diffMode.
  NODE_TYPE_TO_CATEGORY: NODE_TYPE_TO_CATEGORY.
  TourFitView: TourFitView().
  SelectedNodeFitView: SelectedNodeFitView().
  LayerDetailTopology.portalNodes: LayerDetailTopology#portalNodes.
  LayerDetailTopology: LayerDetailTopology#
  LayerDetailTopology.nodes: LayerDetailTopology#nodes.
  LayerDetailTopology.portalEdges: LayerDetailTopology#portalEdges.
  LayerDetailTopology.filteredNodes: LayerDetailTopology#filteredNodes.
  LayerDetailTopology.intraContainer: LayerDetailTopology#intraContainer.
  buildCustomFlowNode.opts-typeLiteral756.changedNodeIds: buildCustomFlowNode().(opts)typeLiteral756:changedNodeIds.
  buildCustomFlowNode.opts-typeLiteral756.affectedNodeIds: buildCustomFlowNode().(opts)typeLiteral756:affectedNodeIds.
  buildCustomFlowNode.opts-typeLiteral756.onNodeClick: buildCustomFlowNode().(opts)typeLiteral756:onNodeClick.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx)

## Classes
### `LayerDetailTopology`
- def: [`understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx:333`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L333)
- signature: `interface LayerDetailTopology`
- members:
  - `containers` — [`L340`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L340) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `edges` — [`L335`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L335) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `filteredEdges` — [`L338`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L338) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `filteredNodes` — [`L339`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L339)
  - `intraContainer` — [`L342`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L342)
  - `nodeToContainer` — [`L341`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L341) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `nodes` — [`L334`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L334)
  - `portalEdges` — [`L337`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L337)
  - `portalNodes` — [`L336`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L336)
- uses (calls/refs, reference-scoped): [`PortalFlowNode`](PortalNode.tsx.md#PortalFlowNode), [`DerivedContainer`](../utils/containers.ts.md#DerivedContainer)
- used by: [`useLayerDetailTopology`](GraphView.tsx.md#useLayerDetailTopology), [`useLayerDetailGraph`](GraphView.tsx.md#useLayerDetailGraph), [`EMPTY_TOPOLOGY`](GraphView.tsx.md#EMPTY_TOPOLOGY)

## Functions
- `GraphView()` — [`L1575`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L1575)
- `GraphViewInner()` — [`L1299`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L1299) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `SelectedNodeFitView()` — [`L182`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L182) — Centers the graph on the selected node (e.g. from search).
- `TourFitView()` — [`L95`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L95) — Pans/zooms to tour-highlighted nodes. Highlighted nodes are usually
- `buildCustomFlowNode(node: GraphNode, opts: { diffMode: boolean; changedNodeIds: Set<string>; affectedNodeIds: Set<string>; onNodeClick: (nodeId: string) => void; })` — [`L910`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L910) — Build a CustomFlowNode from a GraphNode. Mirrors the shape produced by — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `useLayerDetailGraph()` — [`L960`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L960) — Visual overlay: cheap O(n) pass that applies selection, search, and tour — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `useLayerDetailTopology()` — [`L365`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L365) — Topology hook: derives containers, aggregates inter-container edges, then — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `useOverviewGraph()` — [`L211`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L211) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)

## Module values
- `EMPTY_TOPOLOGY` — [`L345`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L345) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `NODE_TYPE_TO_CATEGORY` — [`L70`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L70) — Maps each NodeType to a filter category. Must be kept in sync with core NodeType.
- `affectedNodeIds` — [`L915`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L915)
- `changedNodeIds` — [`L914`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L914)
- `diffMode` — [`L913`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L913)
- `nodeTypes` — [`L57`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L57) — documented in [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md)
- `onNodeClick` — [`L916`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/GraphView.tsx#L916)

