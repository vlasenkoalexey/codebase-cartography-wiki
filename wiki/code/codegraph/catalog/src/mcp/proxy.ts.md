---
title: 'Module: src/mcp/proxy.ts'
type: catalog
provenance: extracted
module: src/mcp/proxy.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`proxy.ts`/
symbols:
  runLocalHandshakeProxy: runLocalHandshakeProxy().
  startPpidWatchdogNoSocket: startPpidWatchdogNoSocket().
  startPpidWatchdog: startPpidWatchdog().
  runProxy: runProxy().
  sendClientHello: sendClientHello().
  connectWithHello: connectWithHello().
  logAttachedDaemon: logAttachedDaemon().
  readHelloLine: readHelloLine().
  JsonRpc: JsonRpc#
  LocalHandshakeDeps.makeEngine: LocalHandshakeDeps#makeEngine().
  parsePollMs: parsePollMs().
  DEFAULT_PPID_POLL_MS: DEFAULT_PPID_POLL_MS.
  parseHostPpid: parseHostPpid().
  LocalHandshakeDeps.getDaemonSocket: LocalHandshakeDeps#getDaemonSocket().
  LocalHandshakeDeps.root: LocalHandshakeDeps#root.
  isProcessAliveLocal: isProcessAliveLocal().
  LOG_ATTACH_ENV: LOG_ATTACH_ENV.
  ProxyResult: ProxyResult#
  LocalHandshakeDeps: LocalHandshakeDeps#
  pipeUntilClose: pipeUntilClose().
  ProxyResult.outcome: ProxyResult#outcome.
  ProxyResult.reason: ProxyResult#reason.
---
# Module: [`src/mcp/proxy.ts`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts)

## Classes
### `JsonRpc`
- def: [`src/mcp/proxy.ts:186`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L186)
- signature: `type JsonRpc`
- used by: [`runLocalHandshakeProxy`](proxy.ts.md#runLocalHandshakeProxy)

### `LocalHandshakeDeps`
- def: [`src/mcp/proxy.ts:190`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L190)
- doc: Dependencies the local-handshake proxy needs, injected by MCPServer (which
- signature: `interface LocalHandshakeDeps`
- members:
  - `getDaemonSocket(method)` — [`L193`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L193) — Probe → spawn → retry → hello-verify; resolves a connected daemon socket,
  - `makeEngine(method)` — [`L196`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L196) — Lazily create an in-process engine — used ONLY if the daemon never comes up,
  - `root` — [`L198`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L198) — Project root for the fallback engine's lazy init.
- uses (calls/refs, reference-scoped): [`MCPEngine`](engine.ts.md#MCPEngine)
- used by: [`runLocalHandshakeProxy`](proxy.ts.md#runLocalHandshakeProxy), [`runProxyWithLocalHandshake`](index.ts.md#MCPServer.runProxyWithLocalHandshake)

### `ProxyResult`
- def: [`src/mcp/proxy.ts:57`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L57)
- signature: `interface ProxyResult`
- members:
  - `outcome` — [`L64`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L64) — `proxied` — successfully attached to a same-version daemon and piped
  - `reason` — [`L65`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L65)
- used by: [`runProxy`](proxy.ts.md#runProxy)

## Functions
- `connectWithHello(socketPath: string, expectedVersion?: string)` — [`L131`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L131) — Connect to a daemon at `socketPath` and verify its hello (exact version match).
- `isProcessAliveLocal(pid: number)` — [`L560`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L560)
- `logAttachedDaemon(socketPath: string, hello: DaemonHello)` — [`L50`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L50) — Log a successful daemon attach — gated behind {@link LOG_ATTACH_ENV} so it is
- `parseHostPpid(raw: string | undefined)` — [`L553`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L553)
- `parsePollMs(raw: string | undefined)` — [`L545`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L545)
- `pipeUntilClose(socket: net.Socket)` — [`L480`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L480) — Pipe stdin → socket and socket → stdout. Resolves once either end closes
- `readHelloLine(socket: net.Socket)` — [`L422`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L422) — Read one CRLF/LF-terminated JSON line from the socket, parse it as the
- `runLocalHandshakeProxy(deps: LocalHandshakeDeps)` — [`L214`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L214) — Local-handshake proxy (the cold-start fix). — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- `runProxy(socketPath: string, expectedVersion?: string)` — [`L83`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L83) — Attempt to connect to the daemon at `socketPath` and pipe stdio through it.
- `sendClientHello(socket: net.Socket)` — [`L177`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L177) — Tell the daemon our pids right after we verify its hello, so its liveness
- `startPpidWatchdog(socket: net.Socket)` — [`L524`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L524) — PPID watchdog mirroring the one in `MCPServer.start` — kills the proxy if
- `startPpidWatchdogNoSocket(onDeath: () => void)` — [`L396`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L396) — PPID watchdog for the local-handshake proxy — same #277 logic as

## Module values
- `DEFAULT_PPID_POLL_MS` — [`L35`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L35) — Default poll cadence for the PPID watchdog (same as the direct server).
- `LOG_ATTACH_ENV` — [`L44`](../../../../../../raw/code/codegraph/src/mcp/proxy.ts#L44) — Env var that opts INTO the "attached to shared daemon" log line. Off by

