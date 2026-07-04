---
title: 'Module: src/resolution/frameworks/react.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/react.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`react.ts`/
symbols:
  reactResolver: reactResolver.
  resolveComponent: resolveComponent().
  resolveHook: resolveHook().
  resolveContext: resolveContext().
  isBuiltInType: isBuiltInType().
  isPascalCase: isPascalCase().
  BUILT_IN_TYPES: BUILT_IN_TYPES.
  COMPONENT_KINDS: COMPONENT_KINDS.
  filePathToRoute: filePathToRoute().
---
# Module: [`src/resolution/frameworks/react.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts)

## Functions
- `filePathToRoute(filePath: string)` — [`L325`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L325) — Convert file path to Next.js route
- `isBuiltInType(name: string)` — [`L233`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L233) — Check if name is a built-in type
- `isPascalCase(str: string)` — [`L226`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L226) — Check if string is PascalCase
- `resolveComponent(name: string, fromFile: string, context: ResolutionContext)` — [`L248`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L248) — Resolve a component reference using name-based lookup
- `resolveContext(name: string, context: ResolutionContext)` — [`L300`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L300) — Resolve a context reference using name-based lookup
- `resolveHook(name: string, context: ResolutionContext)` — [`L280`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L280) — Resolve a custom hook reference using name-based lookup

## Module values
- `BUILT_IN_TYPES` — [`L237`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L237)
- `COMPONENT_KINDS` — [`L243`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L243)
- `reactResolver` — [`L10`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react.ts#L10) — documented in [types.ts](../../../../concepts/types.ts.md)

