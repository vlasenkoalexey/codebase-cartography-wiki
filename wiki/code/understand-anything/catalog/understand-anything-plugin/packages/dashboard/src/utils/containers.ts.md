---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/containers.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/containers.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`containers.ts`/
symbols:
  deriveContainers: deriveContainers().
  DeriveResult.containers: DeriveResult#containers.
  DerivedContainer.nodeIds: DerivedContainer#nodeIds.
  groupByFolder.typeLiteral23.rooted: groupByFolder().typeLiteral23:rooted.
  DerivedContainer.name: DerivedContainer#name.
  DerivedContainer.id: DerivedContainer#id.
  DeriveResult.ungrouped: DeriveResult#ungrouped.
  DerivedContainer: DerivedContainer#
  shouldFallbackToCommunity: shouldFallbackToCommunity().
  DerivedContainer.strategy: DerivedContainer#strategy.
  MAX_CONCENTRATION: MAX_CONCENTRATION.
  ROOT_BUCKET: ROOT_BUCKET.
  groupByFolder.typeLiteral23.groups: groupByFolder().typeLiteral23:groups.
  DeriveResult: DeriveResult#
  MIN_BUCKET_COUNT: MIN_BUCKET_COUNT.
  MIN_NODES_FOR_SUPPRESSION: MIN_NODES_FOR_SUPPRESSION.
  commonPrefix: commonPrefix().
  firstSegment: firstSegment().
  groupByFolder: groupByFolder().
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/containers.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts)

## Classes
### `DeriveResult`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/containers.ts:14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L14) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- signature: `interface DeriveResult`
- members:
  - `containers` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L15) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
  - `ungrouped` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L16) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- uses (calls/refs, reference-scoped): [`DerivedContainer`](containers.ts.md#DerivedContainer)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`deriveContainers`](containers.ts.md#deriveContainers), [`containers.test.ts`](__tests__/containers.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-containers.test.ts)

### `DerivedContainer`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/containers.ts:7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L7) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `interface DerivedContainer`
- members:
  - `id` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L8) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `name` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L9) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `nodeIds` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L10) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `strategy` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L11) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](../components/GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`useLayerDetailGraph`](../components/GraphView.tsx.md#useLayerDetailGraph), [`deriveContainers`](containers.ts.md#deriveContainers), [`containers.test.ts`](__tests__/containers.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-containers.test.ts), [`containers`](containers.ts.md#DeriveResult.containers), [`containers`](../components/GraphView.tsx.md#LayerDetailTopology.containers)

## Functions
- `commonPrefix(paths: string[])` — [`L30`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L30) — Longest common prefix of the *directory* portion of paths, trimmed to a — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `deriveContainers(nodes: GraphNode[], edges: GraphEdge[])` — [`L91`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L91) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `firstSegment(path: string)` — [`L47`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L47) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `groupByFolder(nodes: GraphNode[])` — [`L52`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L52)
- `shouldFallbackToCommunity(groups: Map<string, string[]>, rooted: string[], totalNodes: number)` — [`L77`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L77) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)

## Module values
- `MAX_CONCENTRATION` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L20) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `MIN_BUCKET_COUNT` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L19) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `MIN_NODES_FOR_SUPPRESSION` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L21) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `ROOT_BUCKET` — [`L22`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L22) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `groups` — [`L54`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L54) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)
- `rooted` — [`L54`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/containers.ts#L54) — documented in [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md)

