---
title: 'Module: src/mcp/index.ts'
type: catalog
provenance: extracted
module: src/mcp/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`index.ts`/
symbols:
  MCPServer.startDirect: MCPServer#startDirect().
  MCPServer.startDaemonProcess: MCPServer#startDaemonProcess().
  MCPServer.installPpidWatchdog: MCPServer#installPpidWatchdog().
  MCPServer.stop: MCPServer#stop().
  MCPServer.runProxyWithLocalHandshake: MCPServer#runProxyWithLocalHandshake().
  MCPServer.start: MCPServer#start().
  MCPServer.engine: MCPServer#engine.
  MCPServer.session: MCPServer#session.
  MCPServer.livenessWatchdog: MCPServer#livenessWatchdog.
  MCPServer.projectPath: MCPServer#projectPath.
  spawnDetachedDaemon: spawnDetachedDaemon().
  MCPServer.hostPpid: MCPServer#hostPpid.
  MCPServer.daemon: MCPServer#daemon.
  MCPServer.ppidWatchdog: MCPServer#ppidWatchdog.
  resolveDaemonRoot: resolveDaemonRoot().
  MCPServer.mode: MCPServer#mode.
  daemonInternalSet: daemonInternalSet().
  MCPServer.installSignalHandlers: MCPServer#installSignalHandlers().
  MCPServer.-constructor: MCPServer#`<constructor>`().
  DAEMON_INTERNAL_ENV: DAEMON_INTERNAL_ENV.
  MCPServer: MCPServer#
  MCPServer.stopped: MCPServer#stopped.
  sleep: sleep().
  TAKEOVER_MAX_RETRIES: TAKEOVER_MAX_RETRIES.
  TAKEOVER_RETRY_DELAY_MS: TAKEOVER_RETRY_DELAY_MS.
  DAEMON_CONNECT_MAX_RETRIES: DAEMON_CONNECT_MAX_RETRIES.
  DAEMON_CONNECT_RETRY_DELAY_MS: DAEMON_CONNECT_RETRY_DELAY_MS.
  daemonOptOutSet: daemonOptOutSet().
  MCPServer.originalPpid: MCPServer#originalPpid.
---
# Module: [`src/mcp/index.ts`](../../../../../../raw/code/codegraph/src/mcp/index.ts)

## Classes
### `MCPServer`
- def: [`src/mcp/index.ts:181`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L181)
- doc: MCP Server for CodeGraph
- signature: `class MCPServer`
- members:
  - `<constructor>(projectPath?: string | undefined)` — [`L200`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L200) — MCP Server for CodeGraph
  - `installPpidWatchdog(method)` — [`L426`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L426) — PPID watchdog (#277) — direct mode only. Daemon mode is detached on purpose
  - `installSignalHandlers(method)` — [`L416`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L416) — Standard SIGINT/SIGTERM handlers that route to our `stop()` (direct mode).
  - `runProxyWithLocalHandshake(method)` — [`L378`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L378) — Proxy mode (the common case). Serve the MCP handshake LOCALLY for instant
  - `start(method)` — [`L217`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L217) — Start the MCP server.
  - `startDaemonProcess(method)` — [`L333`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L333) — Run as the detached shared daemon (process spawned with — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `startDirect(method)` — [`L293`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L293) — Single-process stdio MCP session — the pre-issue-#411 code path.
  - `stop(method)` — [`L265`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L265) — Stop the server. In daemon mode this triggers graceful shutdown of every — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `daemon` — [`L187`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L187)
  - `engine` — [`L186`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L186)
  - `hostPpid` — [`L195`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L195)
  - `livenessWatchdog` — [`L191`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L191)
  - `mode` — [`L198`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L198)
  - `originalPpid` — [`L194`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L194)
  - `ppidWatchdog` — [`L188`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L188)
  - `projectPath` — [`L182`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L182)
  - `session` — [`L185`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L185)
  - `stopped` — [`L197`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L197)
- uses (calls/refs, reference-scoped): [`start`](daemon.ts.md#Daemon.start), [`runLocalHandshakeProxy`](proxy.ts.md#runLocalHandshakeProxy), [`stop`](daemon.ts.md#Daemon.stop), [`<constructor>`](daemon.ts.md#Daemon.-constructor), [`tryAcquireDaemonLock`](daemon.ts.md#tryAcquireDaemonLock), [`getTelemetry`](../telemetry/index.ts.md#getTelemetry), [`stop`](engine.ts.md#MCPEngine.stop), [`supervisionLostReason`](ppid-watchdog.ts.md#supervisionLostReason), [`installMainThreadWatchdog`](liveness-watchdog.ts.md#installMainThreadWatchdog), [`ensureInitialized`](engine.ts.md#MCPEngine.ensureInitialized), [`<constructor>`](engine.ts.md#MCPEngine.-constructor), [`getDaemonSocketCandidates`](daemon-paths.ts.md#getDaemonSocketCandidates), [`connectWithHello`](proxy.ts.md#connectWithHello), [`<constructor>`](session.ts.md#MCPSession.-constructor), [`<constructor>`](transport.ts.md#StdioTransport.-constructor), [`pid`](daemon-paths.ts.md#DaemonLockInfo.pid), [`clearStaleDaemonLock`](daemon.ts.md#clearStaleDaemonLock), [`MCPEngine`](engine.ts.md#MCPEngine), [`HOST_PPID_ENV`](../extraction/wasm-runtime-flags.ts.md#HOST_PPID_ENV), [`startInterval`](../telemetry/index.ts.md#Telemetry.startInterval), [`start`](session.ts.md#MCPSession.start), [`parsePpidPollMs`](ppid-watchdog.ts.md#parsePpidPollMs), [`MCPSession`](session.ts.md#MCPSession), [`spawnDetachedDaemon`](index.ts.md#spawnDetachedDaemon), [`stop`](session.ts.md#MCPSession.stop), [`currentPpid`](ppid-watchdog.ts.md#SupervisionState.currentPpid), [`hostPpid`](ppid-watchdog.ts.md#SupervisionState.hostPpid), [`isAlive`](ppid-watchdog.ts.md#SupervisionState.isAlive), [`isProcessAlive`](daemon.ts.md#isProcessAlive), [`originalPpid`](ppid-watchdog.ts.md#SupervisionState.originalPpid), [`makeEngine`](proxy.ts.md#LocalHandshakeDeps.makeEngine), [`resolveDaemonRoot`](index.ts.md#resolveDaemonRoot), [`parseHostPpid`](ppid-watchdog.ts.md#parseHostPpid), [`treatStdinFailureAsShutdown`](stdin-teardown.ts.md#treatStdinFailureAsShutdown), [`daemonInternalSet`](index.ts.md#daemonInternalSet), [`Daemon`](daemon.ts.md#Daemon), [`WatchdogHandle`](liveness-watchdog.ts.md#WatchdogHandle), [`getDaemonSocket`](proxy.ts.md#LocalHandshakeDeps.getDaemonSocket), [`root`](proxy.ts.md#LocalHandshakeDeps.root), [`sleep`](index.ts.md#sleep)  (+6 more)
- used by: [`main`](../bin/codegraph.ts.md#main), [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts)

## Functions
- `daemonInternalSet()` — [`L98`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L98) — Whether this process was spawned to BE the detached daemon.
- `daemonOptOutSet()` — [`L91`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L91) — Whether `CODEGRAPH_NO_DAEMON` was set to a truthy value.
- `resolveDaemonRoot(explicitPath: string | null)` — [`L116`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L116) — Resolve the project root the daemon machinery should key on. Returns
- `sleep(ms: number)` — [`L448`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L448)
- `spawnDetachedDaemon(root: string)` — [`L134`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L134) — Spawn the shared daemon as a fully detached background process: its own

## Module values
- `DAEMON_CONNECT_MAX_RETRIES` — [`L87`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L87) — How long a launcher waits for a freshly-spawned daemon to bind its socket
- `DAEMON_CONNECT_RETRY_DELAY_MS` — [`L88`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L88)
- `DAEMON_INTERNAL_ENV` — [`L64`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L64) — Env var that marks a process as the *detached daemon* itself (set by
- `TAKEOVER_MAX_RETRIES` — [`L71`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L71) — Retries for the detached daemon arbitrating the O_EXCL lock against a racing
- `TAKEOVER_RETRY_DELAY_MS` — [`L72`](../../../../../../raw/code/codegraph/src/mcp/index.ts#L72)

