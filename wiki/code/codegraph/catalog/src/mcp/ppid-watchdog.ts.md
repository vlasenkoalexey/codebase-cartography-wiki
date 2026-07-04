---
title: 'Module: src/mcp/ppid-watchdog.ts'
type: catalog
provenance: extracted
module: src/mcp/ppid-watchdog.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`ppid-watchdog.ts`/
symbols:
  supervisionLostReason: supervisionLostReason().
  parsePpidPollMs: parsePpidPollMs().
  SupervisionState.originalPpid: SupervisionState#originalPpid.
  SupervisionState.currentPpid: SupervisionState#currentPpid.
  SupervisionState.hostPpid: SupervisionState#hostPpid.
  SupervisionState.isAlive: SupervisionState#isAlive.
  parseHostPpid: parseHostPpid().
  DEFAULT_PPID_POLL_MS: DEFAULT_PPID_POLL_MS.
  SupervisionState: SupervisionState#
  SupervisionState.platform: SupervisionState#platform.
---
# Module: [`src/mcp/ppid-watchdog.ts`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts)

## Classes
### `SupervisionState`
- def: [`src/mcp/ppid-watchdog.ts:23`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L23)
- doc: Shared decision logic for the PPID watchdog (#277, #692).
- signature: `interface SupervisionState`
- members:
  - `currentPpid` — [`L27`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L27) — `process.ppid` right now.
  - `hostPpid` — [`L33`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L33) — The MCP host pid threaded past an intermediate launcher
  - `isAlive` — [`L35`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L35) — Liveness probe — `process.kill(pid, 0)` in production, stubbed in tests.
  - `originalPpid` — [`L25`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L25) — `process.ppid` captured at startup.
  - `platform` — [`L37`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L37) — Defaults to `process.platform`.
- used by: [`installCommandSupervision`](../bin/command-supervision.ts.md#installCommandSupervision), [`installPpidWatchdog`](index.ts.md#MCPServer.installPpidWatchdog), [`startPpidWatchdog`](proxy.ts.md#startPpidWatchdog), [`startPpidWatchdogNoSocket`](proxy.ts.md#startPpidWatchdogNoSocket), [`supervisionLostReason`](ppid-watchdog.ts.md#supervisionLostReason)

## Functions
- `parseHostPpid(raw: string | undefined)` — [`L90`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L90) — Parse the host PID propagated across the `--liftoff-only` re-exec
- `parsePpidPollMs(raw: string | undefined)` — [`L75`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L75) — Resolve the PPID watchdog poll interval from an env override
- `supervisionLostReason(state: SupervisionState)` — [`L44`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L44) — Returns a human-readable reason string when the process has lost its

## Module values
- `DEFAULT_PPID_POLL_MS` — [`L66`](../../../../../../raw/code/codegraph/src/mcp/ppid-watchdog.ts#L66) — Default PPID poll cadence (ms). Shared by the MCP server and CLI commands.

