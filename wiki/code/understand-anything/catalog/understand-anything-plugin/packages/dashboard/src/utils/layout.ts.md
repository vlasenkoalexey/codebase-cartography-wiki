---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/layout.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/layout.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`layout.ts`/
symbols:
  nodesToElkInput.dims-Map.typeLiteral174.height: nodesToElkInput().(dims)Map:typeLiteral174:height.
  mergeElkPositions: mergeElkPositions().
  applyForceLayout: applyForceLayout().
  applyDagreLayout.typeLiteral14.edges: applyDagreLayout().typeLiteral14:edges.
  NODE_WIDTH: NODE_WIDTH.
  NODE_HEIGHT: NODE_HEIGHT.
  ForceNode: ForceNode#
  ELK_DEFAULT_LAYOUT_OPTIONS: ELK_DEFAULT_LAYOUT_OPTIONS.
  nodesToElkInput: nodesToElkInput().
  applyForceLayout.typeLiteral57.nodes: applyForceLayout().typeLiteral57:nodes.
  LAYER_CLUSTER_WIDTH: LAYER_CLUSTER_WIDTH.
  LAYER_CLUSTER_HEIGHT: LAYER_CLUSTER_HEIGHT.
  PORTAL_NODE_WIDTH: PORTAL_NODE_WIDTH.
  PORTAL_NODE_HEIGHT: PORTAL_NODE_HEIGHT.
  applyDagreLayout.nodeDimensions-Map.typeLiteral12.width: applyDagreLayout().(nodeDimensions)Map:typeLiteral12:width.
  applyDagreLayout.nodeDimensions-Map.typeLiteral12.height: applyDagreLayout().(nodeDimensions)Map:typeLiteral12:height.
  ForceNode.id: ForceNode#id.
  applyForceLayout.nodeDimensions-Map.typeLiteral56.width: applyForceLayout().(nodeDimensions)Map:typeLiteral56:width.
  applyForceLayout.typeLiteral57.edges: applyForceLayout().typeLiteral57:edges.
  applyDagreLayout.spacingOverrides-typeLiteral13.nodesep: applyDagreLayout().(spacingOverrides)typeLiteral13:nodesep.
  applyDagreLayout.spacingOverrides-typeLiteral13.ranksep: applyDagreLayout().(spacingOverrides)typeLiteral13:ranksep.
  applyDagreLayout.typeLiteral14.nodes: applyDagreLayout().typeLiteral14:nodes.
  applyForceLayout.nodeDimensions-Map.typeLiteral56.height: applyForceLayout().(nodeDimensions)Map:typeLiteral56:height.
  nodesToElkInput.dims-Map.typeLiteral174.width: nodesToElkInput().(dims)Map:typeLiteral174:width.
  applyDagreLayout: applyDagreLayout().
  ForceNode.community: ForceNode#community.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/layout.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts)

## Classes
### `ForceNode`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/layout.ts:85`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L85) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- signature: `interface ForceNode`
- members:
  - `community` — [`L87`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L87)
  - `id` — [`L86`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L86)
- used by: [`applyForceLayout`](layout.ts.md#applyForceLayout)

## Functions
- `applyDagreLayout(nodes: Node[], edges: Edge[], direction?: "TB" | "LR", nodeDimensions?: Map<string, { width: number; height: number; }> | undefined, spacingOverrides?: { nodesep?: number | undefined; ranksep?: number | undefined; } | undefined)` — [`L30`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L30) — Synchronous dagre layout — used for small graphs.
- `applyForceLayout(nodes: Node[], edges: Edge[], nodeDimensions?: Map<string, { width: number; height: number; }> | undefined, communityMap?: Map<string, number> | undefined)` — [`L94`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L94) — Force-directed layout using d3-force — used for knowledge graphs. — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- `mergeElkPositions(nodes: T[], positioned: ElkInput)` — [`L231`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L231) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `nodesToElkInput(nodes: Node[], edges: Edge[], dims: Map<string, { width: number; height: number; }>, layoutOptionsOverride?: Record<string, string> | undefined)` — [`L206`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L206) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)

## Module values
- `ELK_DEFAULT_LAYOUT_OPTIONS` — [`L195`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L195) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `LAYER_CLUSTER_HEIGHT` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L18)
- `LAYER_CLUSTER_WIDTH` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L17)
- `NODE_HEIGHT` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L16) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `NODE_WIDTH` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L15) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `PORTAL_NODE_HEIGHT` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L20)
- `PORTAL_NODE_WIDTH` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L19)
- `edges` — [`L36`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L36) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- `edges` — [`L99`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L99)
- `height` — [`L34`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L34)
- `height` — [`L97`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L97)
- `height` — [`L209`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L209)
- `nodes` — [`L36`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L36)
- `nodes` — [`L99`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L99)
- `nodesep` — [`L35`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L35) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- `ranksep` — [`L35`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L35) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- `width` — [`L34`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L34)
- `width` — [`L97`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L97)
- `width` — [`L209`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.ts#L209)

