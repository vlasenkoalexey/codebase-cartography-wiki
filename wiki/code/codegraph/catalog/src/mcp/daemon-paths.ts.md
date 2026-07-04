---
title: 'Module: src/mcp/daemon-paths.ts'
type: catalog
provenance: extracted
module: src/mcp/daemon-paths.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`daemon-paths.ts`/
symbols:
  getDaemonSocketCandidates: getDaemonSocketCandidates().
  DaemonLockInfo: DaemonLockInfo#
  DaemonLockInfo.pid: DaemonLockInfo#pid.
  getDaemonPidPath: getDaemonPidPath().
  decodeLockInfo: decodeLockInfo().
  encodeLockInfo: encodeLockInfo().
  getDaemonSocketPath: getDaemonSocketPath().
  tmpdirSocketPath: tmpdirSocketPath().
  projectHash: projectHash().
  DaemonLockInfo.version: DaemonLockInfo#version.
  DaemonLockInfo.socketPath: DaemonLockInfo#socketPath.
  DaemonLockInfo.startedAt: DaemonLockInfo#startedAt.
  POSIX_SOCKET_PATH_LIMIT: POSIX_SOCKET_PATH_LIMIT.
---
# Module: [`src/mcp/daemon-paths.ts`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts)

## Classes
### `DaemonLockInfo`
- def: [`src/mcp/daemon-paths.ts:97`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L97) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
- doc: Structured contents of the pid lockfile.
- signature: `interface DaemonLockInfo`
- members:
  - `pid` — [`L98`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L98) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `socketPath` — [`L100`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L100)
  - `startedAt` — [`L101`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L101)
  - `version` — [`L99`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L99)
- used by: [`start`](daemon.ts.md#Daemon.start), [`daemon.ts`](daemon.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon.ts), [`startDaemonProcess`](index.ts.md#MCPServer.startDaemonProcess), [`tryAcquireDaemonLock`](daemon.ts.md#tryAcquireDaemonLock), [`stopDaemonAt`](daemon-registry.ts.md#stopDaemonAt), [`cleanupLockfile`](daemon.ts.md#Daemon.cleanupLockfile), [`clearStaleDaemonLock`](daemon.ts.md#clearStaleDaemonLock), [`decodeLockInfo`](daemon-paths.ts.md#decodeLockInfo), [`encodeLockInfo`](daemon-paths.ts.md#encodeLockInfo), [`acquireLockViaExclusiveOpen`](daemon.ts.md#acquireLockViaExclusiveOpen), [`AcquireResult`](daemon.ts.md#AcquireResult), [`DaemonStartResult`](daemon.ts.md#DaemonStartResult)

## Functions
- `decodeLockInfo(raw: string)` — [`L117`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L117) — Parse a pidfile body. Tolerant of old-format pidfiles (plain decimal pid) so
- `encodeLockInfo(info: DaemonLockInfo)` — [`L108`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L108) — Serialize a {@link DaemonLockInfo} for writing to the pidfile. JSON for
- `getDaemonPidPath(projectRoot: string)` — [`L92`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L92) — Absolute path to the daemon pid lockfile for `projectRoot`. — documented in [directory.ts](../../../concepts/directory.ts.md)
- `getDaemonSocketCandidates(projectRoot: string)` — [`L69`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L69) — Ordered socket / named-pipe path candidates the daemon should try to bind (and — documented in [directory.ts](../../../concepts/directory.ts.md)
- `getDaemonSocketPath(projectRoot: string)` — [`L86`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L86) — The PREFERRED (primary) socket path — candidate 0. Use this only where a
- `projectHash(projectRoot: string)` — [`L40`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L40) — Short stable identifier for a project root — used in tmpdir/pipe names.
- `tmpdirSocketPath(projectRoot: string)` — [`L51`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L51) — The deterministic tmpdir socket path for `projectRoot` — the fallback used

## Module values
- `POSIX_SOCKET_PATH_LIMIT` — [`L37`](../../../../../../raw/code/codegraph/src/mcp/daemon-paths.ts#L37) — Soft upper bound for in-project socket paths.

