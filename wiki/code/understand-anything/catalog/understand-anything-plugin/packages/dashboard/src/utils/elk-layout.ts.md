---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`elk-layout.ts`/
symbols:
  repairElkInput: repairElkInput().
  applyElkLayout: applyElkLayout().
  ElkInput.children: ElkInput#children.
  ElkChild.id: ElkChild#id.
  ElkInput: ElkInput#
  ElkInput.edges: ElkInput#edges.
  ElkChild.width: ElkChild#width.
  ElkChild.height: ElkChild#height.
  ElkChild.children: ElkChild#children.
  ElkChild: ElkChild#
  ElkInput.id: ElkInput#id.
  RepairResult.input: RepairResult#input.
  ElkLayoutResult.positioned: ElkLayoutResult#positioned.
  RepairResult.issues: RepairResult#issues.
  ElkLayoutResult.issues: ElkLayoutResult#issues.
  ElkInput.layoutOptions: ElkInput#layoutOptions.
  makeIssue: makeIssue().
  maybeThrow: maybeThrow().
  ElkEdge: ElkEdge#
  DEFAULT_NODE_WIDTH: DEFAULT_NODE_WIDTH.
  DEFAULT_NODE_HEIGHT: DEFAULT_NODE_HEIGHT.
  ElkChild.x: ElkChild#x.
  ElkChild.y: ElkChild#y.
  ElkChild.parentId: ElkChild#parentId.
  ElkEdge.sources: ElkEdge#sources.
  ElkEdge.targets: ElkEdge#targets.
  ElkEdge.id: ElkEdge#id.
  RepairOptions: RepairOptions#
  RepairOptions.strict: RepairOptions#strict.
  RepairResult: RepairResult#
  elk: elk.
  ElkLayoutOptions: ElkLayoutOptions#
  ElkLayoutOptions.strict: ElkLayoutOptions#strict.
  ElkLayoutResult: ElkLayoutResult#
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts)

## Classes
### `ElkChild`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L5) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `interface ElkChild`
- members:
  - `children` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L12) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
  - `height` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L8) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `id` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L6) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `parentId` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L13) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
  - `width` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L7) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `x` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L10) — Set by ELK after layout; absent on input. Downstream consumers must default. — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
  - `y` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L11) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](../components/GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`repairElkInput`](elk-layout.ts.md#repairElkInput), [`elk-layout.test.ts`](__tests__/elk-layout.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-elk-layout.test.ts), [`children`](elk-layout.ts.md#ElkInput.children), [`mergeElkPositions`](layout.ts.md#mergeElkPositions)

### `ElkEdge`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L16) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `interface ElkEdge`
- members:
  - `id` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L17)
  - `sources` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L18) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
  - `targets` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L19) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](../components/GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`repairElkInput`](elk-layout.ts.md#repairElkInput), [`elk-layout.test.ts`](__tests__/elk-layout.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-elk-layout.test.ts), [`edges`](elk-layout.ts.md#ElkInput.edges)

### `ElkInput`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:22`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L22) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- signature: `interface ElkInput`
- members:
  - `children` — [`L24`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L24) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `edges` — [`L25`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L25) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `id` — [`L23`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L23) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `layoutOptions` — [`L26`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L26) — documented in [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md)
- uses (calls/refs, reference-scoped): [`ElkChild`](elk-layout.ts.md#ElkChild), [`ElkEdge`](elk-layout.ts.md#ElkEdge)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`GraphView.tsx`](../components/GraphView.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-GraphView.tsx), [`repairElkInput`](elk-layout.ts.md#repairElkInput), [`elk-layout.test.ts`](__tests__/elk-layout.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-elk-layout.test.ts), [`applyElkLayout`](elk-layout.ts.md#applyElkLayout), [`height`](layout.ts.md#nodesToElkInput.dims-Map.typeLiteral174.height), [`mergeElkPositions`](layout.ts.md#mergeElkPositions), [`layout.ts`](layout.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-layout.ts), [`input`](elk-layout.ts.md#RepairResult.input), [`positioned`](elk-layout.ts.md#ElkLayoutResult.positioned)

### `ElkLayoutOptions`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:216`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L216)
- signature: `interface ElkLayoutOptions`
- members:
  - `strict` — [`L217`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L217) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- used by: [`applyElkLayout`](elk-layout.ts.md#applyElkLayout)

### `ElkLayoutResult`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:220`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L220) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- signature: `interface ElkLayoutResult`
- members:
  - `issues` — [`L222`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L222) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
  - `positioned` — [`L221`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L221) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- uses (calls/refs, reference-scoped): [`ElkInput`](elk-layout.ts.md#ElkInput)
- used by: [`useLayerDetailTopology`](../components/GraphView.tsx.md#useLayerDetailTopology), [`elk-layout.test.ts`](__tests__/elk-layout.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-elk-layout.test.ts), [`useOverviewGraph`](../components/GraphView.tsx.md#useOverviewGraph), [`applyElkLayout`](elk-layout.ts.md#applyElkLayout), [`DomainGraphViewInner`](../components/DomainGraphView.tsx.md#DomainGraphViewInner)

### `RepairOptions`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:35`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L35)
- signature: `interface RepairOptions`
- members:
  - `strict` — [`L36`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L36) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- used by: [`repairElkInput`](elk-layout.ts.md#repairElkInput)

### `RepairResult`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts:39`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L39) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- signature: `interface RepairResult`
- members:
  - `input` — [`L40`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L40) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
  - `issues` — [`L41`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L41) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- uses (calls/refs, reference-scoped): [`ElkInput`](elk-layout.ts.md#ElkInput)
- used by: [`repairElkInput`](elk-layout.ts.md#repairElkInput), [`elk-layout.test.ts`](__tests__/elk-layout.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-elk-layout.test.ts), [`applyElkLayout`](elk-layout.ts.md#applyElkLayout)

## Functions
- `applyElkLayout(input: ElkInput, opts?: ElkLayoutOptions)` — [`L225`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L225) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)
- `makeIssue(level: GraphIssue, category: string, message: string)` — [`L44`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L44) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- `maybeThrow(strict: boolean | undefined, issue: GraphIssue)` — [`L52`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L52) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- `repairElkInput(input: ElkInput, opts?: RepairOptions)` — [`L56`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L56) — documented in [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md)

## Module values
- `DEFAULT_NODE_HEIGHT` — [`L33`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L33) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- `DEFAULT_NODE_WIDTH` — [`L32`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L32) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)
- `elk` — [`L214`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/elk-layout.ts#L214) — documented in [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md)

