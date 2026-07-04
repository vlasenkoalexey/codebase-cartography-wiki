---
title: 'Module: src/resolution/go-module.ts'
type: catalog
provenance: extracted
module: src/resolution/go-module.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`go-module.ts`/
symbols:
  GoModule.modulePath: GoModule#modulePath.
  loadGoModule: loadGoModule().
  GoModule: GoModule#
  GoModule.rootDir: GoModule#rootDir.
---
# Module: [`src/resolution/go-module.ts`](../../../../../../raw/code/codegraph/src/resolution/go-module.ts)

## Classes
### `GoModule`
- def: [`src/resolution/go-module.ts:15`](../../../../../../raw/code/codegraph/src/resolution/go-module.ts#L15)
- signature: `interface GoModule`
- members:
  - `modulePath` — [`L17`](../../../../../../raw/code/codegraph/src/resolution/go-module.ts#L17) — The module path declared in `go.mod`, e.g. `github.com/example/myproject`
  - `rootDir` — [`L19`](../../../../../../raw/code/codegraph/src/resolution/go-module.ts#L19) — Absolute path to the directory containing the `go.mod` file.
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`resolveGoCrossPackageReference`](import-resolver.ts.md#resolveGoCrossPackageReference), [`isExternalImport`](import-resolver.ts.md#isExternalImport), [`getGoModule`](types.ts.md#ResolutionContext.getGoModule), [`goModule`](index.ts.md#ReferenceResolver.goModule), [`loadGoModule`](go-module.ts.md#loadGoModule)

## Functions
- `loadGoModule(projectRoot: string)` — [`L30`](../../../../../../raw/code/codegraph/src/resolution/go-module.ts#L30) — Read the `go.mod` file at the project root and extract the module path.

