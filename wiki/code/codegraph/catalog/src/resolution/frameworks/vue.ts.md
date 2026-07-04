---
title: 'Module: src/resolution/frameworks/vue.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/vue.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`vue.ts`/
symbols:
  vueResolver: vueResolver.
  resolveComponent: resolveComponent().
  VUE_COMPILER_MACROS: VUE_COMPILER_MACROS.
  NUXT_AUTO_IMPORTS: NUXT_AUTO_IMPORTS.
  NUXT_VIRTUAL_MODULES: NUXT_VIRTUAL_MODULES.
  isPascalCase: isPascalCase().
  filePathToNuxtRoute: filePathToNuxtRoute().
---
# Module: [`src/resolution/frameworks/vue.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts)

## Functions
- `filePathToNuxtRoute(normalized: string, afterPagesStart: number)` — [`L313`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L313) — Convert a file path to a Nuxt route path
- `isPascalCase(str: string)` — [`L270`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L270) — Check if string is PascalCase
- `resolveComponent(name: string, fromFile: string, context: ResolutionContext)` — [`L277`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L277) — Resolve a Vue component reference to its .vue file

## Module values
- `NUXT_AUTO_IMPORTS` — [`L27`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L27) — Nuxt auto-imported composables and utilities
- `NUXT_VIRTUAL_MODULES` — [`L72`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L72) — Nuxt virtual module prefixes (auto-import namespaces)
- `VUE_COMPILER_MACROS` — [`L14`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L14) — Vue 3 compiler macros — compiler-provided, not user code
- `vueResolver` — [`L80`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/vue.ts#L80) — documented in [types.ts](../../../../concepts/types.ts.md)

