---
title: 'Module: understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/utils/`layout.worker.ts`/Layout
symbols:
  LayoutMessage: Message#
  LayoutResult: Result#
  LayoutResult.requestId: Result#requestId.
  LayoutResult.positions: Result#positions.
  LayoutMessage.requestId: Message#requestId.
  LayoutMessage.nodes: Message#nodes.
  LayoutMessage.nodes.Array.typeLiteral1.id: Message#nodes.Array:typeLiteral1:id.
  LayoutMessage.nodes.Array.typeLiteral1.width: Message#nodes.Array:typeLiteral1:width.
  LayoutMessage.nodes.Array.typeLiteral1.height: Message#nodes.Array:typeLiteral1:height.
  LayoutMessage.edges: Message#edges.
  LayoutMessage.edges.Array.typeLiteral2.source: Message#edges.Array:typeLiteral2:source.
  LayoutMessage.edges.Array.typeLiteral2.target: Message#edges.Array:typeLiteral2:target.
  LayoutMessage.direction: Message#direction.
  LayoutResult.positions.Record.typeLiteral3.x: Result#positions.Record:typeLiteral3:x.
  LayoutResult.positions.Record.typeLiteral3.y: Result#positions.Record:typeLiteral3:y.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts)

## Classes
### `LayoutMessage`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts:3`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L3)
- signature: `interface LayoutMessage`
- members:
  - `direction` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L7)
  - `edges` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L6)
  - `height` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L5)
  - `id` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L5)
  - `nodes` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L5)
  - `requestId` — [`L4`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L4)
  - `source` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L6)
  - `target` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L6)
  - `width` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L5)
- used by: [`layout.worker.ts`](layout.worker.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-layout.worker.ts)

### `LayoutResult`
- def: [`understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts:10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L10)
- signature: `interface LayoutResult`
- members:
  - `positions` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L12)
  - `requestId` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L11)
  - `x` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L12)
  - `y` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/utils/layout.worker.ts#L12)
- used by: [`layout.worker.ts`](layout.worker.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-layout.worker.ts)

