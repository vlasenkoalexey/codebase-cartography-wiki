---
title: 'Module: src/resolution/frameworks/laravel.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/laravel.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`laravel.ts`/
symbols:
  laravelResolver: laravelResolver.
  resolveControllerMethod: resolveControllerMethod().
  resolveModelCall: resolveModelCall().
  extractLaravelHandler: extractLaravelHandler().
  FACADE_MAPPINGS: FACADE_MAPPINGS.
---
# Module: [`src/resolution/frameworks/laravel.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts)

## Functions
- `extractLaravelHandler(expr: string)` — [`L193`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts#L193) — Parse a Laravel route handler expression and return the symbol to link.
- `resolveControllerMethod(controller: string, method: string, context: ResolutionContext)` — [`L266`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts#L266) — Resolve a Controller@method reference
- `resolveModelCall(className: string, methodName: string, context: ResolutionContext)` — [`L217`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts#L217) — Resolve a Model::method() call

## Module values
- `FACADE_MAPPINGS` — [`L15`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts#L15) — Laravel facade mappings to underlying classes
- `laravelResolver` — [`L38`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/laravel.ts#L38) — documented in [types.ts](../../../../concepts/types.ts.md)

