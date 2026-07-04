---
title: 'Module: src/mcp/daemon-registry.ts'
type: catalog
provenance: extracted
module: src/mcp/daemon-registry.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`daemon-registry.ts`/
symbols:
  stopDaemonAt: stopDaemonAt().
  listDaemons: listDaemons().
  DaemonRecord.root: DaemonRecord#root.
  registerDaemon: registerDaemon().
  stopAllDaemons: stopAllDaemons().
  cleanupDaemonArtifacts: cleanupDaemonArtifacts().
  DaemonRecord: DaemonRecord#
  waitForDeath: waitForDeath().
  StopResult: StopResult#
  DaemonRecord.startedAt: DaemonRecord#startedAt.
  isProcessAlive: isProcessAlive().
  deregisterDaemon: deregisterDaemon().
  DaemonRecord.pid: DaemonRecord#pid.
  recordPath: recordPath().
  StopResult.outcome: StopResult#outcome.
  getRegistryDir: getRegistryDir().
  DaemonRecord.version: DaemonRecord#version.
  listDaemons.opts-typeLiteral10.prune: listDaemons().(opts)typeLiteral10:prune.
  sleep: sleep.
  StopResult.pid: StopResult#pid.
  DaemonRecord.socketPath: DaemonRecord#socketPath.
  StopResult.root: StopResult#root.
---
# Module: [`src/mcp/daemon-registry.ts`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts)

## Classes
### `DaemonRecord`
- def: [`src/mcp/daemon-registry.ts:27`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L27)
- signature: `interface DaemonRecord`
- members:
  - `pid` — [`L30`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L30)
  - `root` — [`L29`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L29) — Realpath'd project root the daemon serves. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `socketPath` — [`L32`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L32)
  - `startedAt` — [`L34`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L34) — Epoch ms when the daemon bound its socket.
  - `version` — [`L31`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L31)
- used by: [`main`](../bin/codegraph.ts.md#main), [`start`](daemon.ts.md#Daemon.start), [`stopDaemonAt`](daemon-registry.ts.md#stopDaemonAt), [`buildPickItems`](daemon-manager.ts.md#buildPickItems), [`listDaemons`](daemon-registry.ts.md#listDaemons), [`registerDaemon`](daemon-registry.ts.md#registerDaemon), [`stopAllDaemons`](daemon-registry.ts.md#stopAllDaemons), [`daemon-manager.ts`](daemon-manager.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon-manager.ts), [`list`](daemon-manager.ts.md#PickerDeps.list)

### `StopResult`
- def: [`src/mcp/daemon-registry.ts:142`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L142)
- signature: `interface StopResult`
- members:
  - `outcome` — [`L146`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L146) — 'term' graceful, 'kill' force, 'not-running' stale lock, 'no-daemon' none found.
  - `pid` — [`L144`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L144)
  - `root` — [`L143`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L143)
- used by: [`runDaemonPicker`](daemon-manager.ts.md#runDaemonPicker), [`stopDaemonAt`](daemon-registry.ts.md#stopDaemonAt), [`stopAllDaemons`](daemon-registry.ts.md#stopAllDaemons), [`daemon-manager.ts`](daemon-manager.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon-manager.ts), [`stop`](daemon-manager.ts.md#PickerDeps.stop), [`stopAll`](daemon-manager.ts.md#PickerDeps.stopAll)

## Functions
- `cleanupDaemonArtifacts(root: string)` — [`L118`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L118) — Remove a stopped daemon's leftover lockfile + socket + registry record.
- `deregisterDaemon(root: string)` — [`L76`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L76) — Best-effort: drop this daemon's record on graceful shutdown.
- `getRegistryDir()` — [`L41`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L41) — `~/.codegraph/daemons` — GLOBAL, keyed off the home install dir. (The
- `isProcessAlive(pid: number)` — [`L55`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L55) — Is `pid` a live process? `kill(pid, 0)` sends no signal — it just probes:
- `listDaemons(opts?: { prune?: boolean | undefined; })` — [`L88`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L88) — All registered daemons whose process is still alive, newest first. Dead/garbage
- `recordPath(root: string)` — [`L45`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L45)
- `registerDaemon(rec: DaemonRecord)` — [`L66`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L66) — Best-effort: record this daemon so `list`/`stop --all` can find it. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
- `stopAllDaemons()` — [`L193`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L193) — Stop every registered, live daemon.
- `stopDaemonAt(root: string)` — [`L155`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L155) — Stop the daemon serving `root`: SIGTERM, wait, then SIGKILL if it won't go,
- `waitForDeath(pid: number, timeoutMs: number)` — [`L133`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L133)

## Module values
- `prune` — [`L88`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L88)
- `sleep` — [`L131`](../../../../../../raw/code/codegraph/src/mcp/daemon-registry.ts#L131)

