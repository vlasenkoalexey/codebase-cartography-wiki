---
title: 'Module: src/installer/index.ts'
type: catalog
provenance: extracted
module: src/installer/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/`index.ts`/
symbols:
  runInstallerWithOptions: runInstallerWithOptions().
  runUninstaller: runUninstaller().
  resolveTargets: resolveTargets().
  offerWatchFallback: offerWatchFallback().
  uninstallTargets: uninstallTargets().
  RunInstallerOptions.location: RunInstallerOptions#location.
  RunUninstallerOptions.location: RunUninstallerOptions#location.
  UninstallReport.status: UninstallReport#status.
  importESM: importESM.
  UninstallReport.displayName: UninstallReport#displayName.
  runInstaller: runInstaller().
  UninstallReport.id: UninstallReport#id.
  RunInstallerOptions.target: RunInstallerOptions#target.
  RunInstallerOptions.autoAllow: RunInstallerOptions#autoAllow.
  RunUninstallerOptions.target: RunUninstallerOptions#target.
  getVersion: getVersion().
  RunInstallerOptions: RunInstallerOptions#
  RunInstallerOptions.yes: RunInstallerOptions#yes.
  RunUninstallerOptions.yes: RunUninstallerOptions#yes.
  tildify: tildify().
  RunUninstallerOptions: RunUninstallerOptions#
  UninstallStatus: UninstallStatus#
  UninstallReport: UninstallReport#
  UninstallReport.removedPaths: UninstallReport#removedPaths.
  UninstallReport.notes: UninstallReport#notes.
  offerWatchFallback.opts-typeLiteral218.yes: offerWatchFallback().(opts)typeLiteral218:yes.
---
# Module: [`src/installer/index.ts`](../../../../../../raw/code/codegraph/src/installer/index.ts)

## Classes
### `RunInstallerOptions`
- def: [`src/installer/index.ts:61`](../../../../../../raw/code/codegraph/src/installer/index.ts#L61)
- signature: `interface RunInstallerOptions`
- members:
  - `autoAllow` — [`L67`](../../../../../../raw/code/codegraph/src/installer/index.ts#L67) — Skip the auto-allow prompt; use this value directly.
  - `location` — [`L65`](../../../../../../raw/code/codegraph/src/installer/index.ts#L65) — Skip the location prompt; use this value directly.
  - `target` — [`L63`](../../../../../../raw/code/codegraph/src/installer/index.ts#L63) — Comma-separated target list, or `auto` / `all` / `none`.
  - `yes` — [`L72`](../../../../../../raw/code/codegraph/src/installer/index.ts#L72) — Skip every confirm and use defaults: location=global,
- uses (calls/refs, reference-scoped): [`Location`](targets/types.ts.md#Location)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runInstallerWithOptions`](index.ts.md#runInstallerWithOptions), [`resolveTargets`](index.ts.md#resolveTargets)

### `RunUninstallerOptions`
- def: [`src/installer/index.ts:291`](../../../../../../raw/code/codegraph/src/installer/index.ts#L291)
- signature: `interface RunUninstallerOptions`
- members:
  - `location` — [`L300`](../../../../../../raw/code/codegraph/src/installer/index.ts#L300) — Skip the location prompt; use this value directly.
  - `target` — [`L298`](../../../../../../raw/code/codegraph/src/installer/index.ts#L298) — Comma-separated target list, or `auto` / `all` / `none`. Defaults
  - `yes` — [`L302`](../../../../../../raw/code/codegraph/src/installer/index.ts#L302) — Non-interactive: location=global, target=all, no prompts.
- uses (calls/refs, reference-scoped): [`Location`](targets/types.ts.md#Location)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runUninstaller`](index.ts.md#runUninstaller)

### `UninstallReport`
- def: [`src/installer/index.ts:314`](../../../../../../raw/code/codegraph/src/installer/index.ts#L314)
- doc: Per-target outcome of an uninstall sweep. `removed` means we deleted
- signature: `interface UninstallReport`
- members:
  - `displayName` — [`L316`](../../../../../../raw/code/codegraph/src/installer/index.ts#L316)
  - `id` — [`L315`](../../../../../../raw/code/codegraph/src/installer/index.ts#L315)
  - `notes` — [`L321`](../../../../../../raw/code/codegraph/src/installer/index.ts#L321) — Verbatim notes from the target (rare for uninstall).
  - `removedPaths` — [`L319`](../../../../../../raw/code/codegraph/src/installer/index.ts#L319) — Absolute paths we actually edited/removed (action === 'removed').
  - `status` — [`L317`](../../../../../../raw/code/codegraph/src/installer/index.ts#L317)
- uses (calls/refs, reference-scoped): [`TargetId`](targets/types.ts.md#TargetId), [`UninstallStatus`](index.ts.md#UninstallStatus)
- used by: [`runUninstaller`](index.ts.md#runUninstaller), [`uninstallTargets`](index.ts.md#uninstallTargets)

### `UninstallStatus`
- def: [`src/installer/index.ts:305`](../../../../../../raw/code/codegraph/src/installer/index.ts#L305)
- signature: `type UninstallStatus`
- used by: [`status`](index.ts.md#UninstallReport.status)

## Functions
- `getVersion()` — [`L51`](../../../../../../raw/code/codegraph/src/installer/index.ts#L51)
- `offerWatchFallback(clack: typeof import("@clack/prompts"), projectPath: string, opts?: { yes?: boolean | undefined; })` — [`L529`](../../../../../../raw/code/codegraph/src/installer/index.ts#L529) — When the live file watcher will be disabled for this project (e.g. WSL2
- `resolveTargets(clack: typeof import("@clack/prompts"), opts: RunInstallerOptions, location: Location, useDefaults: boolean)` — [`L469`](../../../../../../raw/code/codegraph/src/installer/index.ts#L469) — documented in [installer-targets-types.ts](../../../concepts/installer-targets-types.ts.md)
- `runInstaller()` — [`L80`](../../../../../../raw/code/codegraph/src/installer/index.ts#L80) — Interactive entry point — preserves the historical UX (`codegraph
- `runInstallerWithOptions(opts: RunInstallerOptions)` — [`L84`](../../../../../../raw/code/codegraph/src/installer/index.ts#L84) — documented in [installer-targets-types.ts](../../../concepts/installer-targets-types.ts.md)
- `runUninstaller(opts: RunUninstallerOptions)` — [`L372`](../../../../../../raw/code/codegraph/src/installer/index.ts#L372) — Interactive uninstaller — the inverse of `runInstallerWithOptions`. — documented in [directory.ts](../../../concepts/directory.ts.md)
- `tildify(p: string)` — [`L463`](../../../../../../raw/code/codegraph/src/installer/index.ts#L463) — Replace home-directory prefix in a path with `~/` for cleaner log
- `uninstallTargets(targets: readonly AgentTarget[], location: Location)` — [`L333`](../../../../../../raw/code/codegraph/src/installer/index.ts#L333) — Pure uninstall sweep — no prompts, no I/O beyond the targets' own — documented in [installer-targets-types.ts](../../../concepts/installer-targets-types.ts.md)

## Module values
- `importESM` — [`L47`](../../../../../../raw/code/codegraph/src/installer/index.ts#L47)
- `yes` — [`L532`](../../../../../../raw/code/codegraph/src/installer/index.ts#L532)

