---
title: 'Module: src/mcp/liveness-watchdog.ts'
type: catalog
provenance: extracted
module: src/mcp/liveness-watchdog.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`liveness-watchdog.ts`/
symbols:
  installMainThreadWatchdog: installMainThreadWatchdog().
  debug: debug().
  parseWatchdogTimeoutMs: parseWatchdogTimeoutMs().
  WatchdogHandle: WatchdogHandle#
  WatchdogHandle.stop: WatchdogHandle#stop().
  DEFAULT_WATCHDOG_TIMEOUT_MS: DEFAULT_WATCHDOG_TIMEOUT_MS.
  isEnvTruthy: isEnvTruthy().
  deriveCheckIntervalMs: deriveCheckIntervalMs().
  CHILD_SOURCE: CHILD_SOURCE.
---
# Module: [`src/mcp/liveness-watchdog.ts`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts)

## Classes
### `WatchdogHandle`
- def: [`src/mcp/liveness-watchdog.ts:72`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L72)
- signature: `interface WatchdogHandle`
- members:
  - `stop(method)` — [`L74`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L74) — Stop heartbeating and shut the watchdog child down. Idempotent.
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-index.ts), [`installCommandSupervision`](../bin/command-supervision.ts.md#installCommandSupervision), [`stop`](index.ts.md#MCPServer.stop), [`installMainThreadWatchdog`](liveness-watchdog.ts.md#installMainThreadWatchdog), [`livenessWatchdog`](index.ts.md#MCPServer.livenessWatchdog)

## Functions
- `debug(msg: string)` — [`L66`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L66) — Arming/teardown diagnostics, gated on the existing MCP debug switch.
- `deriveCheckIntervalMs(timeoutMs: number)` — [`L61`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L61) — Derive a heartbeat cadence that emits several beats inside the timeout window.
- `installMainThreadWatchdog()` — [`L108`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L108) — Install the main-thread liveness watchdog for a long-lived process. Returns a
- `isEnvTruthy(raw: string | undefined)` — [`L45`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L45) — `true` for `1/true/yes/on` (case-insensitive); `false` otherwise.
- `parseWatchdogTimeoutMs(raw: string | undefined, fallback?: number)` — [`L51`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L51) — Parse the timeout env, falling back to the default for missing/invalid values.

## Module values
- `CHILD_SOURCE` — [`L84`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L84) — The watchdog child body, run via `node -e`. Inlined as a string (not a
- `DEFAULT_WATCHDOG_TIMEOUT_MS` — [`L42`](../../../../../../raw/code/codegraph/src/mcp/liveness-watchdog.ts#L42) — Default: 60s — ~300× shorter than the 5h #850 wedge, far longer than any real main-thread block.

