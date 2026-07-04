---
title: 'Module: src/resolution/cooperative-yield.ts'
type: catalog
provenance: extracted
module: src/resolution/cooperative-yield.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`cooperative-yield.ts`/
symbols:
  createYielder: createYielder().
  MaybeYield: MaybeYield#
  DEFAULT_YIELD_BUDGET_MS: DEFAULT_YIELD_BUDGET_MS.
---
# Module: [`src/resolution/cooperative-yield.ts`](../../../../../../raw/code/codegraph/src/resolution/cooperative-yield.ts)

## Classes
### `MaybeYield`
- def: [`src/resolution/cooperative-yield.ts:28`](../../../../../../raw/code/codegraph/src/resolution/cooperative-yield.ts#L28)
- doc: Yield when more than `budgetMs` of wall-clock has passed since the last yield.
- signature: `type MaybeYield`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`fieldChannelEdges`](callback-synthesizer.ts.md#fieldChannelEdges), [`resolveBatchYielding`](index.ts.md#ReferenceResolver.resolveBatchYielding), [`objectRegistryEdges`](callback-synthesizer.ts.md#objectRegistryEdges), [`closureCollectionEdges`](callback-synthesizer.ts.md#closureCollectionEdges), [`reactJsxChildEdges`](callback-synthesizer.ts.md#reactJsxChildEdges), [`callback-synthesizer.ts`](callback-synthesizer.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-callback-synthesizer.ts), [`eventEmitterEdges`](callback-synthesizer.ts.md#eventEmitterEdges), [`createYielder`](cooperative-yield.ts.md#createYielder)

## Functions
- `createYielder(budgetMs?: number)` — [`L34`](../../../../../../raw/code/codegraph/src/resolution/cooperative-yield.ts#L34)

## Module values
- `DEFAULT_YIELD_BUDGET_MS` — [`L32`](../../../../../../raw/code/codegraph/src/resolution/cooperative-yield.ts#L32) — Default budget: well under the watchdog's minimum heartbeat cadence (~1s), so

