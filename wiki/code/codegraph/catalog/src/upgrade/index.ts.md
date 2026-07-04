---
title: 'Module: src/upgrade/index.ts'
type: catalog
provenance: extracted
module: src/upgrade/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/upgrade/`index.ts`/
symbols:
  runUpgrade: runUpgrade().
  c: c.
  UpgradeDeps.log: UpgradeDeps#log.
  selfHealPromptHook: selfHealPromptHook().
  upgradeUnixBundle: upgradeUnixBundle().
  upgradeNpm: upgradeNpm().
  detectInstallMethod: detectInstallMethod().
  upgradeWindowsBundle: upgradeWindowsBundle().
  resolveLatestVersion: resolveLatestVersion().
  compareVersions: compareVersions().
  Semver.pre: Semver#pre.
  UpgradeDeps.error: UpgradeDeps#error.
  isUpdateAvailable: isUpdateAvailable().
  normalizeVersion: normalizeVersion().
  UpgradeOptions.version: UpgradeOptions#version.
  INSTALL_SH_URL: INSTALL_SH_URL.
  reindexAdvisory: reindexAdvisory().
  InstallMethod: InstallMethod#
  UpgradeDeps: UpgradeDeps#
  parseSemver: parseSemver().
  UpgradeDeps.method: UpgradeDeps#method.
  REPO: REPO.
  DetectInput.filename: DetectInput#filename.
  Semver.major: Semver#major.
  Semver.minor: Semver#minor.
  Semver.patch: Semver#patch.
  UpgradeDeps.run: UpgradeDeps#run.
  RAW_BASE: RAW_BASE.
  buildWindowsUpgradeScript: buildWindowsUpgradeScript().
  NPM_PACKAGE: NPM_PACKAGE.
  UpgradeDeps.hasCommand: UpgradeDeps#hasCommand.
  DetectInput.platform: DetectInput#platform.
  DetectInput.cwd: DetectInput#cwd.
  toPosix: toPosix().
  httpsGet: httpsGet().
  UpgradeOptions.check: UpgradeOptions#check.
  UpgradeOptions.force: UpgradeOptions#force.
  UpgradeDeps.currentVersion: UpgradeDeps#currentVersion.
  UpgradeDeps.resolveLatest: UpgradeDeps#resolveLatest.
  UpgradeDeps.warn: UpgradeDeps#warn.
  UpgradeDeps.platform: UpgradeDeps#platform.
  DetectInput: DetectInput#
  DetectInput.exists: DetectInput#exists.
  deriveInstallDir: deriveInstallDir().
  Semver: Semver#
  stripV: stripV().
  parseLatestTagFromLocation: parseLatestTagFromLocation().
  httpsGet.Promise.typeLiteral85.headers: httpsGet().Promise:typeLiteral85:headers.
  httpsGet.Promise.typeLiteral85.body: httpsGet().Promise:typeLiteral85:body.
  UpgradeOptions: UpgradeOptions#
  hasCommand: hasCommand().
  defaultRun: defaultRun().
  httpsGet.Promise.typeLiteral85.status: httpsGet().Promise:typeLiteral85:status.
  upgradeUnixBundle.method-Extract.typeLiteral173.kind: upgradeUnixBundle().(method)Extract:typeLiteral173:kind.
  upgradeWindowsBundle.method-Extract.typeLiteral189.kind: upgradeWindowsBundle().(method)Extract:typeLiteral189:kind.
  upgradeNpm.method-Extract.typeLiteral202.kind: upgradeNpm().(method)Extract:typeLiteral202:kind.
---
# Module: [`src/upgrade/index.ts`](../../../../../../raw/code/codegraph/src/upgrade/index.ts)

## Classes
### `DetectInput`
- def: [`src/upgrade/index.ts:48`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L48)
- signature: `interface DetectInput`
- members:
  - `cwd` — [`L52`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L52)
  - `exists` — [`L54`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L54) — Injectable existence probe (defaults to fs.existsSync) — for tests.
  - `filename` — [`L50`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L50) — `__filename` of the running CLI module — `<…>/dist/bin/codegraph.js`.
  - `platform` — [`L51`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L51)
- used by: [`main`](../bin/codegraph.ts.md#main), [`detectInstallMethod`](index.ts.md#detectInstallMethod)

### `InstallMethod`
- def: [`src/upgrade/index.ts:41`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L41)
- signature: `type InstallMethod`
- used by: [`upgradeNpm`](index.ts.md#upgradeNpm), [`upgradeUnixBundle`](index.ts.md#upgradeUnixBundle), [`detectInstallMethod`](index.ts.md#detectInstallMethod), [`upgradeWindowsBundle`](index.ts.md#upgradeWindowsBundle), [`method`](index.ts.md#UpgradeDeps.method)

### `Semver`
- def: [`src/upgrade/index.ts:138`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L138)
- signature: `interface Semver`
- members:
  - `major` — [`L139`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L139)
  - `minor` — [`L140`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L140)
  - `patch` — [`L141`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L141)
  - `pre` — [`L142`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L142)
- used by: [`compareVersions`](index.ts.md#compareVersions), [`parseSemver`](index.ts.md#parseSemver)

### `UpgradeDeps`
- def: [`src/upgrade/index.ts:275`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L275)
- doc: Injectable side-effects so the orchestrator stays unit-testable.
- signature: `interface UpgradeDeps`
- members:
  - `currentVersion` — [`L276`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L276)
  - `error` — [`L284`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L284)
  - `hasCommand` — [`L281`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L281)
  - `log` — [`L282`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L282)
  - `method` — [`L277`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L277)
  - `platform` — [`L285`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L285)
  - `resolveLatest` — [`L278`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L278)
  - `run` — [`L280`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L280) — Run a command inheriting stdio; returns its exit code (-1 = spawn failed).
  - `warn` — [`L283`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L283)
- uses (calls/refs, reference-scoped): [`InstallMethod`](index.ts.md#InstallMethod)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runUpgrade`](index.ts.md#runUpgrade), [`selfHealPromptHook`](index.ts.md#selfHealPromptHook), [`upgradeNpm`](index.ts.md#upgradeNpm), [`upgradeUnixBundle`](index.ts.md#upgradeUnixBundle), [`upgradeWindowsBundle`](index.ts.md#upgradeWindowsBundle)

### `UpgradeOptions`
- def: [`src/upgrade/index.ts:265`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L265)
- signature: `interface UpgradeOptions`
- members:
  - `check` — [`L269`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L269) — Report current vs latest, don't change anything.
  - `force` — [`L271`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L271) — Reinstall even if already on the resolved version.
  - `version` — [`L267`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L267) — Pin a specific version (positional arg or CODEGRAPH_VERSION).
- used by: [`main`](../bin/codegraph.ts.md#main), [`runUpgrade`](index.ts.md#runUpgrade)

## Functions
- `buildWindowsUpgradeScript(bundleRoot: string, version: string, arch: string)` — [`L438`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L438) — Build the in-place Windows upgrade script (exported for unit-testing).
- `compareVersions(a: string, b: string)` — [`L157`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L157) — Returns >0 if a>b, <0 if a<b, 0 if equal. Throws on unparseable input.
- `defaultRun(cmd: string, args: string[], env?: any)` — [`L548`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L548)
- `deriveInstallDir(bundleRoot: string, os: "unix" | "windows", exists: (p: string) => boolean)` — [`L70`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L70) — Where the bundle installer keeps its install root, derived from the bundle
- `detectInstallMethod(input: DetectInput)` — [`L94`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L94)
- `hasCommand(cmd: string)` — [`L528`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L528) — True if `cmd` resolves to an executable on PATH. A pure-Node PATH scan — NOT
- `httpsGet(url: string, headers: Record<string, string>, timeoutMs: number)` — [`L207`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L207)
- `isUpdateAvailable(current: string, latest: string)` — [`L171`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L171)
- `normalizeVersion(v: string)` — [`L182`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L182) — `0.9.9` / `v0.9.9` → `v0.9.9` (release tags are v-prefixed).
- `parseLatestTagFromLocation(location: string | undefined)` — [`L197`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L197) — Parse the release tag out of the `Location` header GitHub returns for
- `parseSemver(version: string)` — [`L145`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L145)
- `reindexAdvisory()` — [`L297`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L297) — The honest, additive re-index reminder shown after a successful upgrade.
- `resolveLatestVersion(repo?: string, timeoutMs?: number)` — [`L232`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L232) — Resolve the latest release tag (e.g. `v0.9.9`).
- `runUpgrade(opts: UpgradeOptions, deps: UpgradeDeps)` — [`L310`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L310) — Returns the process exit code (0 = success / nothing to do, 1 = failure).
- `selfHealPromptHook(deps: UpgradeDeps)` — [`L393`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L393) — Wire the Claude `UserPromptSubmit` front-load hook on upgrade for an — documented in [installer-targets-types.ts](../../../concepts/installer-targets-types.ts.md)
- `stripV(v: string)` — [`L188`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L188) — Strip a leading `v`: `v0.9.9` → `0.9.9`.
- `toPosix(p: string)` — [`L57`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L57)
- `upgradeNpm(method: { kind: "npm"; scope: "local" | "global"; }, versionSpec: string, deps: UpgradeDeps)` — [`L492`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L492)
- `upgradeUnixBundle(method: { kind: "bundle"; os: "unix" | "windows"; bundleRoot: string; installDir: string | null; }, pinned: string | undefined, deps: UpgradeDeps)` — [`L405`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L405)
- `upgradeWindowsBundle(method: { kind: "bundle"; os: "unix" | "windows"; bundleRoot: string; installDir: string | null; }, latest: string, deps: UpgradeDeps)` — [`L469`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L469)

## Module values
- `INSTALL_SH_URL` — [`L35`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L35)
- `NPM_PACKAGE` — [`L33`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L33)
- `RAW_BASE` — [`L34`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L34)
- `REPO` — [`L32`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L32)
- `body` — [`L211`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L211)
- `c` — [`L288`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L288)
- `headers` — [`L211`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L211)
- `kind` — [`L406`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L406)
- `kind` — [`L470`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L470)
- `kind` — [`L493`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L493)
- `status` — [`L211`](../../../../../../raw/code/codegraph/src/upgrade/index.ts#L211)

