---
title: 'Module: src/mcp/daemon.ts'
type: catalog
provenance: extracted
module: src/mcp/daemon.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`daemon.ts`/
symbols:
  Daemon.start: Daemon#start().
  Daemon.handleConnection: Daemon#handleConnection().
  Daemon.stop: Daemon#stop().
  Daemon.-constructor: Daemon#`<constructor>`().
  tryAcquireDaemonLock: tryAcquireDaemonLock().
  Daemon.startLivenessTimers: Daemon#startLivenessTimers().
  Daemon.armIdleTimer: Daemon#armIdleTimer().
  Daemon.clients: Daemon#clients.
  Daemon.reapDeadClients: Daemon#reapDeadClients().
  Daemon.dropClient: Daemon#dropClient().
  Daemon.idleTimer: Daemon#idleTimer.
  Daemon.cleanupLockfile: Daemon#cleanupLockfile().
  clearStaleDaemonLock: clearStaleDaemonLock().
  Daemon.socketPath: Daemon#socketPath.
  readClientHello: readClientHello().
  Daemon.engine: Daemon#engine.
  DaemonHello.codegraph: DaemonHello#codegraph.
  Daemon.pidPath: Daemon#pidPath.
  acquireLockViaExclusiveOpen: acquireLockViaExclusiveOpen().
  peerIsDead: peerIsDead().
  Daemon.clientPeers: Daemon#clientPeers.
  DaemonHello: DaemonHello#
  Daemon.maxIdleTimer: Daemon#maxIdleTimer.
  Daemon.clientSweepTimer: Daemon#clientSweepTimer.
  isProcessAlive: isProcessAlive().
  bindFirstUsableSocket.Promise.typeLiteral160.socketPath: bindFirstUsableSocket().Promise:typeLiteral160:socketPath.
  MAX_HELLO_LINE_BYTES: MAX_HELLO_LINE_BYTES.
  Daemon.server: Daemon#server.
  Daemon.idleTimeoutMs: Daemon#idleTimeoutMs.
  Daemon.maxIdleMs: Daemon#maxIdleMs.
  Daemon.stopping: Daemon#stopping.
  finalizeDaemonExit: finalizeDaemonExit().
  DaemonStartResult: DaemonStartResult#
  Daemon.disarmIdleTimer: Daemon#disarmIdleTimer().
  AcquireResult: AcquireResult#
  resolveIdleTimeoutMs: resolveIdleTimeoutMs().
  resolveMaxIdleMs: resolveMaxIdleMs().
  resolveClientSweepMs: resolveClientSweepMs().
  DaemonHello.pid: DaemonHello#pid.
  Daemon: Daemon#
  Daemon.getClientCount: Daemon#getClientCount().
  Daemon.getSocketPath: Daemon#getSocketPath().
  DEFAULT_IDLE_TIMEOUT_MS: DEFAULT_IDLE_TIMEOUT_MS.
  DEFAULT_MAX_IDLE_MS: DEFAULT_MAX_IDLE_MS.
  DEFAULT_CLIENT_SWEEP_MS: DEFAULT_CLIENT_SWEEP_MS.
  DaemonClientHello: DaemonClientHello#
  Daemon.lastActivityAt: Daemon#lastActivityAt.
  peerIsDead.peers-typeLiteral210.pid: peerIsDead().(peers)typeLiteral210:pid.
  peerIsDead.peers-typeLiteral210.hostPid: peerIsDead().(peers)typeLiteral210:hostPid.
  DAEMON_SHUTDOWN_BACKSTOP_MS: DAEMON_SHUTDOWN_BACKSTOP_MS.
  CLIENT_HELLO_TIMEOUT_MS: CLIENT_HELLO_TIMEOUT_MS.
  DaemonHello.socketPath: DaemonHello#socketPath.
  DaemonHello.protocol: DaemonHello#protocol.
  DaemonClientHello.codegraph_client: DaemonClientHello#codegraph_client.
  DaemonClientHello.pid: DaemonClientHello#pid.
  DaemonClientHello.hostPid: DaemonClientHello#hostPid.
  Daemon.-constructor-.opts-typeLiteral12.idleTimeoutMs: Daemon#`<constructor>`().(opts)typeLiteral12:idleTimeoutMs.
  Daemon.-constructor-.opts-typeLiteral12.maxIdleMs: Daemon#`<constructor>`().(opts)typeLiteral12:maxIdleMs.
  SOCKET_BIND_CONFLICT_CODE: SOCKET_BIND_CONFLICT_CODE.
  bindFirstUsableSocket: bindFirstUsableSocket().
  bindFirstUsableSocket.opts-typeLiteral155.onRelocate: bindFirstUsableSocket().(opts)typeLiteral155:onRelocate.
  parseClientHelloLine: parseClientHelloLine().
  DaemonStartResult.socketPath: DaemonStartResult#socketPath.
  DaemonStartResult.lock: DaemonStartResult#lock.
  bindFirstUsableSocket.Promise.typeLiteral160.server: bindFirstUsableSocket().Promise:typeLiteral160:server.
  readClientHello.Promise.typeLiteral213.pid: readClientHello().Promise:typeLiteral213:pid.
  readClientHello.Promise.typeLiteral213.hostPid: readClientHello().Promise:typeLiteral213:hostPid.
---
# Module: [`src/mcp/daemon.ts`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts)

## Classes
### `AcquireResult`
- def: [`src/mcp/daemon.ts:490`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L490)
- doc: Result of `tryAcquireDaemonLock`. Either we got the lockfile (caller becomes
- signature: `type AcquireResult`
- uses (calls/refs, reference-scoped): [`DaemonLockInfo`](daemon-paths.ts.md#DaemonLockInfo)
- used by: [`tryAcquireDaemonLock`](daemon.ts.md#tryAcquireDaemonLock)

### `Daemon`
- def: [`src/mcp/daemon.ts:167`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L167)
- doc: Run as the shared daemon for `projectRoot`. Resolves once the socket is
- signature: `class Daemon`
- members:
  - `<constructor>(projectRoot: string, opts?: { idleTimeoutMs?: number | undefined; maxIdleMs?: number | undefined; })` — [`L183`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L183) — Run as the shared daemon for `projectRoot`. Resolves once the socket is — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `armIdleTimer(method)` — [`L392`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L392) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `cleanupLockfile(method)` — [`L470`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L470) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `disarmIdleTimer(method)` — [`L412`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L412)
  - `dropClient(method)` — [`L386`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L386) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `getClientCount(method)` — [`L308`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L308) — Currently-connected client count. Exposed for tests / status output.
  - `getSocketPath(method)` — [`L313`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L313) — The socket path the daemon is (or will be) listening on.
  - `handleConnection(method)` — [`L354`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L354) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `reapDeadClients(method)` — [`L454`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L454) — Drop every connected client whose peer process is gone. Returns the count — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `start(method)` — [`L206`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L206) — Bind the socket, kick off engine init, and register signal handlers. The — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `startLivenessTimers(method)` — [`L431`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L431) — Defense-in-depth against a daemon that outlives its clients (#692), for the — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `stop(method)` — [`L318`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L318) — Graceful shutdown: close all sessions, the engine, and clean up the lock. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `clientPeers` — [`L171`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L171) — Per-client peer pids from the optional client-hello, for the liveness sweep.
  - `clientSweepTimer` — [`L177`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L177)
  - `clients` — [`L169`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L169) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `engine` — [`L178`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L178)
  - `idleTimeoutMs` — [`L173`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L173)
  - `idleTimeoutMs` — [`L185`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L185)
  - `idleTimer` — [`L172`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L172) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `lastActivityAt` — [`L175`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L175)
  - `maxIdleMs` — [`L174`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L174)
  - `maxIdleMs` — [`L185`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L185)
  - `maxIdleTimer` — [`L176`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L176)
  - `pidPath` — [`L181`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L181)
  - `server` — [`L168`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L168)
  - `socketPath` — [`L180`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L180) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `stopping` — [`L179`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L179)
- uses (calls/refs, reference-scoped): [`stop`](engine.ts.md#MCPEngine.stop), [`ensureInitialized`](engine.ts.md#MCPEngine.ensureInitialized), [`<constructor>`](engine.ts.md#MCPEngine.-constructor), [`getDaemonSocketCandidates`](daemon-paths.ts.md#getDaemonSocketCandidates), [`<constructor>`](session.ts.md#MCPSession.-constructor), [`CodeGraphPackageVersion`](version.ts.md#CodeGraphPackageVersion), [`registerDaemon`](daemon-registry.ts.md#registerDaemon), [`root`](daemon-registry.ts.md#DaemonRecord.root), [`DaemonLockInfo`](daemon-paths.ts.md#DaemonLockInfo), [`pid`](daemon-paths.ts.md#DaemonLockInfo.pid), [`MCPEngine`](engine.ts.md#MCPEngine), [`decodeLockInfo`](daemon-paths.ts.md#decodeLockInfo), [`getDaemonPidPath`](daemon-paths.ts.md#getDaemonPidPath), [`readClientHello`](daemon.ts.md#readClientHello), [`setProjectPathHint`](engine.ts.md#MCPEngine.setProjectPathHint), [`codegraph`](daemon.ts.md#DaemonHello.codegraph), [`start`](session.ts.md#MCPSession.start), [`encodeLockInfo`](daemon-paths.ts.md#encodeLockInfo), [`MCPSession`](session.ts.md#MCPSession), [`peerIsDead`](daemon.ts.md#peerIsDead), [`deregisterDaemon`](daemon-registry.ts.md#deregisterDaemon), [`getDaemonSocketPath`](daemon-paths.ts.md#getDaemonSocketPath), [`stop`](session.ts.md#MCPSession.stop), [`DaemonHello`](daemon.ts.md#DaemonHello), [`isProcessAlive`](daemon.ts.md#isProcessAlive), [`DaemonStartResult`](daemon.ts.md#DaemonStartResult), [`finalizeDaemonExit`](daemon.ts.md#finalizeDaemonExit), [`onClose`](transport.ts.md#SocketTransport.onClose), [`resolveClientSweepMs`](daemon.ts.md#resolveClientSweepMs), [`resolveIdleTimeoutMs`](daemon.ts.md#resolveIdleTimeoutMs), [`resolveMaxIdleMs`](daemon.ts.md#resolveMaxIdleMs), [`pid`](daemon.ts.md#DaemonHello.pid), [`socketPath`](daemon-paths.ts.md#DaemonLockInfo.socketPath), [`startedAt`](daemon-paths.ts.md#DaemonLockInfo.startedAt), [`version`](daemon-paths.ts.md#DaemonLockInfo.version), [`<constructor>`](transport.ts.md#SocketTransport.-constructor), [`bindFirstUsableSocket`](daemon.ts.md#bindFirstUsableSocket), [`protocol`](daemon.ts.md#DaemonHello.protocol), [`socketPath`](daemon.ts.md#DaemonHello.socketPath)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-index.ts), [`startDaemonProcess`](index.ts.md#MCPServer.startDaemonProcess), [`stop`](index.ts.md#MCPServer.stop), [`daemon`](index.ts.md#MCPServer.daemon)

### `DaemonClientHello`
- def: [`src/mcp/daemon.ts:143`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L143)
- doc: Optional reverse-handshake line a proxy sends right after it verifies the
- signature: `interface DaemonClientHello`
- members:
  - `codegraph_client` — [`L144`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L144)
  - `hostPid` — [`L146`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L146)
  - `pid` — [`L145`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L145)
- used by: [`proxy.ts`](proxy.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-proxy.ts), [`sendClientHello`](proxy.ts.md#sendClientHello)

### `DaemonHello`
- def: [`src/mcp/daemon.ts:127`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L127)
- doc: Wire format for the one-shot hello line the daemon emits on every new
- signature: `interface DaemonHello`
- members:
  - `codegraph` — [`L128`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L128)
  - `pid` — [`L129`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L129)
  - `protocol` — [`L131`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L131)
  - `socketPath` — [`L130`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L130)
- used by: [`proxy.ts`](proxy.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-proxy.ts), [`handleConnection`](daemon.ts.md#Daemon.handleConnection), [`runProxy`](proxy.ts.md#runProxy), [`connectWithHello`](proxy.ts.md#connectWithHello), [`logAttachedDaemon`](proxy.ts.md#logAttachedDaemon), [`readHelloLine`](proxy.ts.md#readHelloLine)

### `DaemonStartResult`
- def: [`src/mcp/daemon.ts:149`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L149)
- signature: `interface DaemonStartResult`
- members:
  - `lock` — [`L153`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L153) — Lockfile contents as written.
  - `socketPath` — [`L151`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L151) — Always-non-null for a successfully-started daemon.
- uses (calls/refs, reference-scoped): [`DaemonLockInfo`](daemon-paths.ts.md#DaemonLockInfo)
- used by: [`start`](daemon.ts.md#Daemon.start)

## Functions
- `acquireLockViaExclusiveOpen(pidPath: string, info: DaemonLockInfo)` — [`L585`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L585) — Exclusive-create the pidfile (O_CREAT|O_EXCL via the `wx` flag) and write the
- `bindFirstUsableSocket(candidates: string[], listen: (socketPath: string) => Promise<net.Server>, opts?: { onRelocate?: ((from: string, to: string, code: string) => void) | undefined; })` — [`L673`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L673) — Bind the first usable socket from an ordered candidate list, relocating past
- `clearStaleDaemonLock(pidPath: string, expectedDeadPid?: number | undefined)` — [`L612`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L612) — Remove a stale pidfile, but only if it still names a dead process. Re-reads
- `finalizeDaemonExit(platform: NodeJS.Platform, exit: (code: number) => void)` — [`L95`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L95) — Finalize daemon shutdown. On POSIX, exit immediately — it's clean and fast.
- `isProcessAlive(pid: number)` — [`L636`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L636) — Probe whether `pid` is currently alive (signal-0). Treats EPERM as alive on
- `parseClientHelloLine(line: string)` — [`L728`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L728) — Parse one client-hello line. Returns the peer pids if `line` is a well-formed
- `peerIsDead(peers: { pid: number | null; hostPid: number | null; }, isAlive: (pid: number) => boolean)` — [`L744`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L744) — A client's peer is dead when its proxy process is gone, or when its known
- `readClientHello(socket: net.Socket)` — [`L763`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L763) — Read the optional client-hello line a proxy sends after the daemon hello. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
- `resolveClientSweepMs()` — [`L715`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L715)
- `resolveIdleTimeoutMs()` — [`L699`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L699)
- `resolveMaxIdleMs()` — [`L707`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L707)
- `tryAcquireDaemonLock(projectRoot: string)` — [`L525`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L525) — Atomically create the daemon pidfile with its full record already in place.

## Module values
- `CLIENT_HELLO_TIMEOUT_MS` — [`L116`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L116) — How long the daemon waits for the optional client-hello before proceeding without it.
- `DAEMON_SHUTDOWN_BACKSTOP_MS` — [`L84`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L84) — Windows-only shutdown backstop. On Windows, calling `process.exit()` while a
- `DEFAULT_CLIENT_SWEEP_MS` — [`L113`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L113) — How often the daemon sweeps connected clients for a dead peer process (#692).
- `DEFAULT_IDLE_TIMEOUT_MS` — [`L61`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L61) — Default idle linger after the last client disconnects.
- `DEFAULT_MAX_IDLE_MS` — [`L71`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L71) — Hard ceiling on how long the daemon stays up with clients connected but no
- `MAX_HELLO_LINE_BYTES` — [`L119`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L119) — Bytes/parse-window for an oversized hello line — bounded against a malicious peer.
- `SOCKET_BIND_CONFLICT_CODE` — [`L661`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L661) — The one `listen()` error we must NOT relocate past. EADDRINUSE means the path
- `hostPid` — [`L745`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L745)
- `hostPid` — [`L765`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L765)
- `onRelocate` — [`L676`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L676)
- `pid` — [`L745`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L745)
- `pid` — [`L765`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L765)
- `server` — [`L677`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L677)
- `socketPath` — [`L677`](../../../../../../raw/code/codegraph/src/mcp/daemon.ts#L677)

