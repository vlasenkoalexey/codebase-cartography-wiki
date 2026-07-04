---
title: 'Module: src/resolution/frameworks/rust.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/rust.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`rust.ts`/
symbols:
  rustResolver: rustResolver.
  resolveModule: resolveModule().
  resolveByNameAndKind: resolveByNameAndKind().
  getCachedCargoWorkspaceCrateMap: getCachedCargoWorkspaceCrateMap().
  cargoWorkspaceMapCache: cargoWorkspaceMapCache.
  HANDLER_DIRS: HANDLER_DIRS.
  SERVICE_DIRS: SERVICE_DIRS.
  MODEL_DIRS: MODEL_DIRS.
  FUNCTION_KINDS: FUNCTION_KINDS.
  SERVICE_KINDS: SERVICE_KINDS.
  STRUCT_KINDS: STRUCT_KINDS.
  findMatchingParen: findMatchingParen().
  ModuleResolution: ModuleResolution#
  ModuleResolution.targetId: ModuleResolution#targetId.
  ModuleResolution.fromWorkspace: ModuleResolution#fromWorkspace.
---
# Module: [`src/resolution/frameworks/rust.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts)

## Classes
### `ModuleResolution`
- def: [`src/resolution/frameworks/rust.ts:306`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L306)
- signature: `interface ModuleResolution`
- members:
  - `fromWorkspace` — [`L308`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L308)
  - `targetId` — [`L307`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L307)
- used by: [`rustResolver`](rust.ts.md#rustResolver), [`resolveModule`](rust.ts.md#resolveModule)

## Functions
- `findMatchingParen(s: string, openIdx: number)` — [`L268`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L268) — Index of the ')' that matches the '(' at openIdx, or -1 if unbalanced.
- `getCachedCargoWorkspaceCrateMap(context: ResolutionContext)` — [`L14`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L14)
- `resolveByNameAndKind(name: string, kinds: Set<string>, preferredDirPatterns: string[], context: ResolutionContext)` — [`L283`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L283) — Resolve a symbol by name using indexed queries instead of scanning all files.
- `resolveModule(name: string, context: ResolutionContext)` — [`L311`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L311)

## Module values
- `FUNCTION_KINDS` — [`L263`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L263)
- `HANDLER_DIRS` — [`L259`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L259)
- `MODEL_DIRS` — [`L261`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L261)
- `SERVICE_DIRS` — [`L260`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L260)
- `SERVICE_KINDS` — [`L264`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L264)
- `STRUCT_KINDS` — [`L265`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L265)
- `cargoWorkspaceMapCache` — [`L12`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L12)
- `rustResolver` — [`L22`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/rust.ts#L22) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

