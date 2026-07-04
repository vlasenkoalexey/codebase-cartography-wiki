---
title: 'Module: understand-anything-plugin/packages/core/src/ignore-filter.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/ignore-filter.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`ignore-filter.ts`/
symbols:
  IgnoreFilter.isIgnored: IgnoreFilter#isIgnored().
  createIgnoreFilter: createIgnoreFilter().
  DEFAULT_IGNORE_PATTERNS: DEFAULT_IGNORE_PATTERNS.
  IgnoreFilter: IgnoreFilter#
---
# Module: [`understand-anything-plugin/packages/core/src/ignore-filter.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-filter.ts)

## Classes
### `IgnoreFilter`
- def: [`understand-anything-plugin/packages/core/src/ignore-filter.ts:72`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-filter.ts#L72)
- signature: `interface IgnoreFilter`
- members:
  - `isIgnored(method)` — [`L74`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-filter.ts#L74) — Returns true if the given relative path should be excluded from analysis.
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`createIgnoreFilter`](ignore-filter.ts.md#createIgnoreFilter), [`ignore-filter.test.ts`](__tests__/ignore-filter.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-ignore-filter.test.ts)

## Functions
- `createIgnoreFilter(projectRoot: string)` — [`L86`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-filter.ts#L86) — Creates an IgnoreFilter that merges hardcoded defaults with user-defined

## Module values
- `DEFAULT_IGNORE_PATTERNS` — [`L9`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-filter.ts#L9) — Hardcoded default ignore patterns matching the project-scanner agent's

