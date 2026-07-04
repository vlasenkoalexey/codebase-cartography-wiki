---
title: 'Module: src/resolution/frameworks/svelte.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/svelte.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`svelte.ts`/
symbols:
  svelteResolver: svelteResolver.
  resolveComponent: resolveComponent().
  isRuneReference: isRuneReference().
  getSvelteKitRouteInfo: getSvelteKitRouteInfo().
  SVELTE_RUNES: SVELTE_RUNES.
  SVELTEKIT_MODULE_PREFIXES: SVELTEKIT_MODULE_PREFIXES.
  isPascalCase: isPascalCase().
  SVELTEKIT_ROUTE_FILES: SVELTEKIT_ROUTE_FILES.
  filePathToSvelteKitRoute: filePathToSvelteKitRoute().
---
# Module: [`src/resolution/frameworks/svelte.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts)

## Functions
- `filePathToSvelteKitRoute(filePath: string)` — [`L259`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L259) — Convert a file path to a SvelteKit route path
- `getSvelteKitRouteInfo(fileName: string)` — [`L252`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L252) — Check if filename is a SvelteKit route file
- `isPascalCase(str: string)` — [`L200`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L200) — Check if string is PascalCase
- `isRuneReference(name: string)` — [`L185`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L185) — Check if a reference name is a Svelte rune
- `resolveComponent(name: string, fromFile: string, context: ResolutionContext)` — [`L207`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L207) — Resolve a Svelte component reference using name-based lookup

## Module values
- `SVELTEKIT_MODULE_PREFIXES` — [`L33`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L33) — SvelteKit framework-provided module prefixes
- `SVELTEKIT_ROUTE_FILES` — [`L233`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L233) — SvelteKit route file patterns
- `SVELTE_RUNES` — [`L14`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L14) — Svelte 5 runes — compiler-provided, not user code
- `svelteResolver` — [`L45`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/svelte.ts#L45) — documented in [types.ts](../../../../concepts/types.ts.md)

