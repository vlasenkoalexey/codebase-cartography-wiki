---
title: 'Module: src/resolution/workspace-packages.ts'
type: catalog
provenance: extracted
module: src/resolution/workspace-packages.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`workspace-packages.ts`/
symbols:
  loadWorkspacePackages: loadWorkspacePackages().
  resolveWorkspaceImport: resolveWorkspaceImport().
  WorkspacePackages: WorkspacePackages#
  readWorkspaceGlobs: readWorkspaceGlobs().
  WorkspacePackages.byName: WorkspacePackages#byName.
  parsePnpmPackages: parsePnpmPackages().
  expandWorkspaceGlob: expandWorkspaceGlob().
  readPackageName: readPackageName().
---
# Module: [`src/resolution/workspace-packages.ts`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts)

## Classes
### `WorkspacePackages`
- def: [`src/resolution/workspace-packages.ts:31`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L31)
- signature: `interface WorkspacePackages`
- members:
  - `byName` — [`L33`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L33) — Member package `name` → directory relative to projectRoot (posix).
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`loadWorkspacePackages`](workspace-packages.ts.md#loadWorkspacePackages), [`getWorkspacePackages`](types.ts.md#ResolutionContext.getWorkspacePackages), [`resolveWorkspaceImport`](workspace-packages.ts.md#resolveWorkspaceImport), [`workspacePackages`](index.ts.md#ReferenceResolver.workspacePackages)

## Functions
- `expandWorkspaceGlob(projectRoot: string, pattern: string)` — [`L151`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L151) — Expand one level of a `packages/*` / `apps/**` glob to member dirs.
- `loadWorkspacePackages(projectRoot: string)` — [`L45`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L45) — Load workspace member packages for `projectRoot`. Returns `null` when
- `parsePnpmPackages(yaml: string)` — [`L128`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L128) — Minimal pnpm-workspace.yaml `packages:` extractor. Handles the only shape
- `readPackageName(dirAbs: string)` — [`L173`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L173) — Read the `name` field from a member directory's package.json.
- `readWorkspaceGlobs(projectRoot: string)` — [`L89`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L89) — Read workspace glob patterns from package.json + pnpm-workspace.yaml.
- `resolveWorkspaceImport(importPath: string, ws: WorkspacePackages)` — [`L70`](../../../../../../raw/code/codegraph/src/resolution/workspace-packages.ts#L70) — Rewrite a bare workspace import to a path relative to projectRoot,

