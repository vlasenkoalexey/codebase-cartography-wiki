---
title: 'Module: src/resolution/path-aliases.ts'
type: catalog
provenance: extracted
module: src/resolution/path-aliases.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`path-aliases.ts`/
symbols:
  loadProjectAliases: loadProjectAliases().
  applyAliases: applyAliases().
  AliasPattern.prefix: AliasPattern#prefix.
  readTsconfigLike: readTsconfigLike().
  splitWildcard: splitWildcard().
  AliasMap: AliasMap#
  AliasPattern.hasWildcard: AliasPattern#hasWildcard.
  AliasPattern.suffix: AliasPattern#suffix.
  RawTsconfig: RawTsconfig#
  splitWildcard.typeLiteral24.prefix: splitWildcard().typeLiteral24:prefix.
  splitWildcard.typeLiteral24.suffix: splitWildcard().typeLiteral24:suffix.
  splitWildcard.typeLiteral24.hasWildcard: splitWildcard().typeLiteral24:hasWildcard.
  AliasPattern: AliasPattern#
  AliasPattern.replacements: AliasPattern#replacements.
  AliasMap.patterns: AliasMap#patterns.
  AliasMap.baseUrl: AliasMap#baseUrl.
  stripJsonc: stripJsonc().
  RawTsconfig.compilerOptions: RawTsconfig#compilerOptions.
  RawTsconfig.compilerOptions.typeLiteral14.baseUrl: RawTsconfig#compilerOptions.typeLiteral14:baseUrl.
  RawTsconfig.compilerOptions.typeLiteral14.paths: RawTsconfig#compilerOptions.typeLiteral14:paths.
---
# Module: [`src/resolution/path-aliases.ts`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts)

## Classes
### `AliasMap`
- def: [`src/resolution/path-aliases.ts:47`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L47)
- signature: `interface AliasMap`
- members:
  - `baseUrl` — [`L49`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L49) — Absolute path. The directory `compilerOptions.paths` is rooted at.
  - `patterns` — [`L54`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L54) — Patterns ordered by specificity: longer prefix first, then literal-
- uses (calls/refs, reference-scoped): [`AliasPattern`](path-aliases.ts.md#AliasPattern)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`loadProjectAliases`](path-aliases.ts.md#loadProjectAliases), [`isExternalImport`](import-resolver.ts.md#isExternalImport), [`applyAliases`](path-aliases.ts.md#applyAliases), [`getProjectAliases`](types.ts.md#ResolutionContext.getProjectAliases), [`projectAliases`](index.ts.md#ReferenceResolver.projectAliases)

### `AliasPattern`
- def: [`src/resolution/path-aliases.ts:31`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L31)
- doc: A single alias pattern from `compilerOptions.paths`.
- signature: `interface AliasPattern`
- members:
  - `hasWildcard` — [`L37`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L37) — Whether the pattern contains a `*` wildcard.
  - `prefix` — [`L33`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L33) — The literal prefix before `*` (or the whole pattern if no `*`).
  - `replacements` — [`L44`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L44) — Replacement templates. When `hasWildcard` is true, `*` in the
  - `suffix` — [`L35`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L35) — The literal suffix after `*` (almost always empty).
- used by: [`loadProjectAliases`](path-aliases.ts.md#loadProjectAliases), [`isExternalImport`](import-resolver.ts.md#isExternalImport), [`applyAliases`](path-aliases.ts.md#applyAliases), [`AliasMap`](path-aliases.ts.md#AliasMap)

### `RawTsconfig`
- def: [`src/resolution/path-aliases.ts:106`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L106)
- signature: `interface RawTsconfig`
- members:
  - `baseUrl` — [`L108`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L108)
  - `compilerOptions` — [`L107`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L107)
  - `paths` — [`L109`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L109)
- used by: [`loadProjectAliases`](path-aliases.ts.md#loadProjectAliases), [`readTsconfigLike`](path-aliases.ts.md#readTsconfigLike)

## Functions
- `applyAliases(importPath: string, aliases: AliasMap, projectRoot: string)` — [`L211`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L211) — Resolve an import path through an {@link AliasMap}. Returns the list
- `loadProjectAliases(projectRoot: string)` — [`L145`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L145) — Load aliases for `projectRoot`. Returns `null` when no tsconfig /
- `readTsconfigLike(filePath: string)` — [`L113`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L113)
- `splitWildcard(pattern: string)` — [`L124`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L124)
- `stripJsonc(src: string)` — [`L65`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L65) — Strip JSONC comments + trailing commas so a tsconfig with the usual

## Module values
- `hasWildcard` — [`L127`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L127)
- `prefix` — [`L125`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L125)
- `suffix` — [`L126`](../../../../../../raw/code/codegraph/src/resolution/path-aliases.ts#L126)

