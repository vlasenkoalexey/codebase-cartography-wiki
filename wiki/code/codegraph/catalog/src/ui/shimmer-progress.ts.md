---
title: 'Module: src/ui/shimmer-progress.ts'
type: catalog
provenance: extracted
module: src/ui/shimmer-progress.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/ui/`shimmer-progress.ts`/
symbols:
  createShimmerProgress: createShimmerProgress().
  ShimmerProgress.onProgress: ShimmerProgress#onProgress.
  IndexProgress.phase: IndexProgress#phase.
  ShimmerProgress.stop: ShimmerProgress#stop.
  IndexProgress.current: IndexProgress#current.
  IndexProgress: IndexProgress#
  IndexProgress.total: IndexProgress#total.
  PHASE_NAMES: PHASE_NAMES.
  ShimmerProgress: ShimmerProgress#
---
# Module: [`src/ui/shimmer-progress.ts`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts)

## Classes
### `IndexProgress`
- def: [`src/ui/shimmer-progress.ts:11`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L11)
- signature: `interface IndexProgress`
- members:
  - `current` — [`L13`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L13)
  - `phase` — [`L12`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L12)
  - `total` — [`L14`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L14)
- used by: [`createShimmerProgress`](shimmer-progress.ts.md#createShimmerProgress), [`onProgress`](shimmer-progress.ts.md#ShimmerProgress.onProgress)

### `ShimmerProgress`
- def: [`src/ui/shimmer-progress.ts:17`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L17)
- signature: `interface ShimmerProgress`
- members:
  - `onProgress` — [`L18`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L18)
  - `stop` — [`L19`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L19)
- uses (calls/refs, reference-scoped): [`IndexProgress`](shimmer-progress.ts.md#IndexProgress)
- used by: [`main`](../bin/codegraph.ts.md#main), [`createShimmerProgress`](shimmer-progress.ts.md#createShimmerProgress)

## Functions
- `createShimmerProgress()` — [`L22`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L22)

## Module values
- `PHASE_NAMES` — [`L4`](../../../../../../raw/code/codegraph/src/ui/shimmer-progress.ts#L4)

