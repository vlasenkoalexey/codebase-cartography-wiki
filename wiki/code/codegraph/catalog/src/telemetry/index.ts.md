---
title: 'Module: src/telemetry/index.ts'
type: catalog
provenance: extracted
module: src/telemetry/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/telemetry/`index.ts`/
symbols:
  Telemetry.send: Telemetry#send().
  Telemetry.recordUsage: Telemetry#recordUsage().
  Telemetry.-constructor: Telemetry#`<constructor>`().
  Telemetry.flushNow: Telemetry#flushNow().
  getTelemetry: getTelemetry().
  Telemetry.getStatus: Telemetry#getStatus().
  Telemetry.recordLifecycle: Telemetry#recordLifecycle().
  Telemetry.firstRunNotice: Telemetry#firstRunNotice().
  Telemetry.setEnabled: Telemetry#setEnabled().
  recordIndexEvent.result-typeLiteral6.durationMs: recordIndexEvent().(result)typeLiteral6:durationMs.
  Telemetry.readConfig: Telemetry#readConfig().
  Telemetry.claimQueue: Telemetry#claimQueue().
  BufferLine: BufferLine#
  Telemetry.persistSync: Telemetry#persistSync().
  Telemetry.writeConfig: Telemetry#writeConfig().
  Telemetry.appendLines: Telemetry#appendLines().
  registerForExit: registerForExit().
  Telemetry.recoverStaleClaims: Telemetry#recoverStaleClaims().
  TelemetryStatus.decidedBy: TelemetryStatus#decidedBy.
  Telemetry.isEnabled: Telemetry#isEnabled().
  Telemetry.ensureExitHook: Telemetry#ensureExitHook().
  Telemetry.env: Telemetry#env.
  Telemetry.configCache: Telemetry#configCache.
  Telemetry.-get-configPath: Telemetry#`<get>configPath`().
  Telemetry.startInterval: Telemetry#startInterval().
  Telemetry.dir: Telemetry#dir.
  Telemetry.counts: Telemetry#counts.
  Telemetry.-get-queuePath: Telemetry#`<get>queuePath`().
  TelemetryStatus.enabled: TelemetryStatus#enabled.
  Telemetry.now: Telemetry#now.
  Telemetry.debug: Telemetry#debug().
  Telemetry.events: Telemetry#events.
  ConfigFile.machine_id: ConfigFile#machine_id.
  Telemetry.intervalHandle: Telemetry#intervalHandle.
  Telemetry.maybeFlush: Telemetry#maybeFlush().
  singleton: singleton.
  TELEMETRY_DOCS: TELEMETRY_DOCS.
  ClientInfo: ClientInfo#
  TelemetryStatus.machineId: TelemetryStatus#machineId.
  TelemetryStatus.configPath: TelemetryStatus#configPath.
  CountLine.k: CountLine#k.
  EventLine.ev: EventLine#ev.
  exitInstances: exitInstances.
  Telemetry.utcDay: Telemetry#utcDay().
  SCHEMA_VERSION: SCHEMA_VERSION.
  ConfigFile: ConfigFile#
  ConfigFile.enabled: ConfigFile#enabled.
  ConfigFile.first_run_notice_shown: ConfigFile#first_run_notice_shown.
  Telemetry: Telemetry#
  Telemetry.hasStoredChoice: Telemetry#hasStoredChoice().
  ConfigFile.updated_at: ConfigFile#updated_at.
  CountLine: CountLine#
  CountLine.d: CountLine#d.
  CountLine.c: CountLine#c.
  CountLine.e: CountLine#e.
  CountLine.cn: CountLine#cn.
  CountLine.cv: CountLine#cv.
  Telemetry.writeStderr: Telemetry#writeStderr.
  Telemetry.stopInterval: Telemetry#stopInterval().
  MAX_BUFFER_BYTES: MAX_BUFFER_BYTES.
  MAX_EVENTS_PER_REQUEST: MAX_EVENTS_PER_REQUEST.
  UsageKind: UsageKind#
  LifecycleEvent: LifecycleEvent#
  recordIndexEvent: recordIndexEvent().
  ConfigFile.consent_source: ConfigFile#consent_source.
  CountLine.v: CountLine#v.
  CountLine.n: CountLine#n.
  EventLine: EventLine#
  EventLine.v: EventLine#v.
  EventLine.ts: EventLine#ts.
  EventLine.props: EventLine#props.
  exitListenerRegistered: exitListenerRegistered.
  Telemetry.fetchImpl: Telemetry#fetchImpl.
  Telemetry.installExitHook: Telemetry#installExitHook.
  Telemetry.exitHookInstalled: Telemetry#exitHookInstalled.
  TELEMETRY_ENDPOINT: TELEMETRY_ENDPOINT.
  DEFAULT_FLUSH_TIMEOUT_MS: DEFAULT_FLUSH_TIMEOUT_MS.
  STALE_CLAIM_MS: STALE_CLAIM_MS.
  bucketFileCount: bucketFileCount().
  bucketDuration: bucketDuration().
  recordIndexEvent.cg-typeLiteral4.getStats: recordIndexEvent().(cg)typeLiteral4:getStats().
  recordIndexEvent.cg-typeLiteral4.getStats.typeLiteral5.filesByLanguage: recordIndexEvent().(cg)typeLiteral4:getStats().typeLiteral5:filesByLanguage.
  recordIndexEvent.result-typeLiteral6.filesIndexed: recordIndexEvent().(result)typeLiteral6:filesIndexed.
  ClientInfo.name: ClientInfo#name.
  ClientInfo.version: ClientInfo#version.
  TelemetryStatus: TelemetryStatus#
  TelemetryOptions: TelemetryOptions#
  TelemetryOptions.dir: TelemetryOptions#dir.
  TelemetryOptions.fetchImpl: TelemetryOptions#fetchImpl.
  TelemetryOptions.now: TelemetryOptions#now.
  TelemetryOptions.env: TelemetryOptions#env.
  TelemetryOptions.stderr: TelemetryOptions#stderr.
  TelemetryOptions.installExitHook: TelemetryOptions#installExitHook.
  Telemetry.packageVersion: Telemetry#packageVersion().
---
# Module: [`src/telemetry/index.ts`](../../../../../../raw/code/codegraph/src/telemetry/index.ts)

## Classes
### `BufferLine`
- def: [`src/telemetry/index.ts:122`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L122) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- signature: `type BufferLine`
- uses (calls/refs, reference-scoped): [`CountLine`](index.ts.md#CountLine), [`EventLine`](index.ts.md#EventLine)
- used by: [`send`](index.ts.md#Telemetry.send), [`flushNow`](index.ts.md#Telemetry.flushNow), [`claimQueue`](index.ts.md#Telemetry.claimQueue), [`persistSync`](index.ts.md#Telemetry.persistSync), [`appendLines`](index.ts.md#Telemetry.appendLines)

### `ClientInfo`
- def: [`src/telemetry/index.ts:84`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L84) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- signature: `interface ClientInfo`
- members:
  - `name` — [`L85`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L85)
  - `version` — [`L86`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L86)
- used by: [`proxy.ts`](../mcp/proxy.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-proxy.ts), [`runLocalHandshakeProxy`](../mcp/proxy.ts.md#runLocalHandshakeProxy), [`session.ts`](../mcp/session.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-session.ts), [`recordUsage`](index.ts.md#Telemetry.recordUsage), [`clientInfo`](../mcp/session.ts.md#MCPSession.clientInfo)

### `ConfigFile`
- def: [`src/telemetry/index.ts:89`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L89) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- signature: `interface ConfigFile`
- members:
  - `consent_source` — [`L92`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L92)
  - `enabled` — [`L90`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L90) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `first_run_notice_shown` — [`L93`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L93) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `machine_id` — [`L91`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L91) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `updated_at` — [`L94`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L94) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- used by: [`send`](index.ts.md#Telemetry.send), [`getStatus`](index.ts.md#Telemetry.getStatus), [`firstRunNotice`](index.ts.md#Telemetry.firstRunNotice), [`setEnabled`](index.ts.md#Telemetry.setEnabled), [`readConfig`](index.ts.md#Telemetry.readConfig), [`writeConfig`](index.ts.md#Telemetry.writeConfig), [`configCache`](index.ts.md#Telemetry.configCache)

### `CountLine`
- def: [`src/telemetry/index.ts:106`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L106) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- doc: One buffered line: either a usage-count delta or a lifecycle event.
- signature: `interface CountLine`
- members:
  - `c` — [`L111`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L111) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `cn` — [`L113`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L113) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `cv` — [`L114`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L114) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `d` — [`L108`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L108) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `e` — [`L112`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L112) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `k` — [`L109`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L109) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `n` — [`L110`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L110) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `v` — [`L107`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L107) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- uses (calls/refs, reference-scoped): [`UsageKind`](index.ts.md#UsageKind)
- used by: [`send`](index.ts.md#Telemetry.send), [`recordUsage`](index.ts.md#Telemetry.recordUsage), [`flushNow`](index.ts.md#Telemetry.flushNow), [`claimQueue`](index.ts.md#Telemetry.claimQueue), [`BufferLine`](index.ts.md#BufferLine), [`counts`](index.ts.md#Telemetry.counts)

### `EventLine`
- def: [`src/telemetry/index.ts:116`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L116)
- signature: `interface EventLine`
- members:
  - `ev` — [`L118`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L118) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `props` — [`L120`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L120) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `ts` — [`L119`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L119) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `v` — [`L117`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L117)
- uses (calls/refs, reference-scoped): [`LifecycleEvent`](index.ts.md#LifecycleEvent)
- used by: [`send`](index.ts.md#Telemetry.send), [`recordLifecycle`](index.ts.md#Telemetry.recordLifecycle), [`claimQueue`](index.ts.md#Telemetry.claimQueue), [`BufferLine`](index.ts.md#BufferLine), [`events`](index.ts.md#Telemetry.events)

### `LifecycleEvent`
- def: [`src/telemetry/index.ts:44`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L44)
- signature: `type LifecycleEvent`
- used by: [`recordLifecycle`](index.ts.md#Telemetry.recordLifecycle), [`ev`](index.ts.md#EventLine.ev)

### `Telemetry`
- def: [`src/telemetry/index.ts:151`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L151)
- signature: `class Telemetry`
- members:
  - `<constructor>(opts?: TelemetryOptions)` — [`L165`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L165) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `<get>configPath` — [`L176`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L176)
  - `<get>queuePath` — [`L179`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L179) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `appendLines(method)` — [`L398`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L398) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `claimQueue(method)` — [`L422`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L422) — Atomically claim the queue for sending (rename). Concurrent processes — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `debug(method)` — [`L533`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L533)
  - `ensureExitHook(method)` — [`L527`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L527) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `firstRunNotice(method)` — [`L363`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L363) — Default-on consent is gated by a one-time stderr notice (interactive — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `flushNow(method)` — [`L277`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L277) — Drain in-memory state to the buffer, then send completed-day rollups and — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `getStatus(method)` — [`L187`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L187) — Resolution order (first match wins) — keep in sync with TELEMETRY.md: — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `hasStoredChoice(method)` — [`L229`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L229) — True once any consent decision (or the first-run notice) is on disk.
  - `isEnabled(method)` — [`L205`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L205) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `maybeFlush(method)` — [`L268`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L268) — Fire-and-forget send of everything sendable. Never throws, never logs — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `packageVersion(method)` — [`L517`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L517)
  - `persistSync(method)` — [`L387`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L387) — Synchronous, tiny, exit-safe: drain in-memory deltas to the JSONL queue. — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `readConfig(method)` — [`L338`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L338) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `recordLifecycle(method)` — [`L256`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L256) — install / index / uninstall — buffered like everything else.
  - `recordUsage(method)` — [`L236`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L236) — In-memory increment — safe on the MCP tool-call hot path. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `recoverStaleClaims(method)` — [`L446`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L446) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `send(method)` — [`L468`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L468) — Returns the lines that did NOT make it out (to be re-queued). — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `setEnabled(method)` — [`L214`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L214) — Persist an explicit user choice (installer toggle or `codegraph
  - `startInterval(method)` — [`L318`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L318) — Periodic flush for long-lived processes (MCP daemon / serve). Unref'd so
  - `stopInterval(method)` — [`L325`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L325)
  - `utcDay(method)` — [`L334`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L334) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `writeConfig(method)` — [`L349`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L349) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `configCache` — [`L162`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L162) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `counts` — [`L158`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L158) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `dir` — [`L152`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L152) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `env` — [`L155`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L155)
  - `events` — [`L159`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L159) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `exitHookInstalled` — [`L161`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L161)
  - `fetchImpl` — [`L153`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L153)
  - `installExitHook` — [`L160`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L160)
  - `intervalHandle` — [`L163`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L163)
  - `now` — [`L154`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L154)
  - `writeStderr` — [`L156`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L156) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- uses (calls/refs, reference-scoped): [`BufferLine`](index.ts.md#BufferLine), [`registerForExit`](index.ts.md#registerForExit), [`decidedBy`](index.ts.md#TelemetryStatus.decidedBy), [`enabled`](index.ts.md#TelemetryStatus.enabled), [`machine_id`](index.ts.md#ConfigFile.machine_id), [`ClientInfo`](index.ts.md#ClientInfo), [`TELEMETRY_DOCS`](index.ts.md#TELEMETRY_DOCS), [`configPath`](index.ts.md#TelemetryStatus.configPath), [`machineId`](index.ts.md#TelemetryStatus.machineId), [`ev`](index.ts.md#EventLine.ev), [`k`](index.ts.md#CountLine.k), [`ConfigFile`](index.ts.md#ConfigFile), [`SCHEMA_VERSION`](index.ts.md#SCHEMA_VERSION), [`enabled`](index.ts.md#ConfigFile.enabled), [`first_run_notice_shown`](index.ts.md#ConfigFile.first_run_notice_shown), [`CountLine`](index.ts.md#CountLine), [`c`](index.ts.md#CountLine.c), [`cn`](index.ts.md#CountLine.cn), [`cv`](index.ts.md#CountLine.cv), [`d`](index.ts.md#CountLine.d), [`e`](index.ts.md#CountLine.e), [`updated_at`](index.ts.md#ConfigFile.updated_at), [`EventLine`](index.ts.md#EventLine), [`LifecycleEvent`](index.ts.md#LifecycleEvent), [`UsageKind`](index.ts.md#UsageKind), [`MAX_BUFFER_BYTES`](index.ts.md#MAX_BUFFER_BYTES), [`MAX_EVENTS_PER_REQUEST`](index.ts.md#MAX_EVENTS_PER_REQUEST), [`consent_source`](index.ts.md#ConfigFile.consent_source), [`n`](index.ts.md#CountLine.n), [`props`](index.ts.md#EventLine.props), [`ts`](index.ts.md#EventLine.ts), [`v`](index.ts.md#CountLine.v), [`v`](index.ts.md#EventLine.v), [`TelemetryOptions`](index.ts.md#TelemetryOptions), [`TelemetryStatus`](index.ts.md#TelemetryStatus), [`DEFAULT_FLUSH_TIMEOUT_MS`](index.ts.md#DEFAULT_FLUSH_TIMEOUT_MS), [`STALE_CLAIM_MS`](index.ts.md#STALE_CLAIM_MS), [`TELEMETRY_ENDPOINT`](index.ts.md#TELEMETRY_ENDPOINT), [`dir`](index.ts.md#TelemetryOptions.dir), [`env`](index.ts.md#TelemetryOptions.env)  (+6 more)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runInstallerWithOptions`](../installer/index.ts.md#runInstallerWithOptions), [`runUninstaller`](../installer/index.ts.md#runUninstaller), [`runLocalHandshakeProxy`](../mcp/proxy.ts.md#runLocalHandshakeProxy), [`handleToolsCall`](../mcp/session.ts.md#MCPSession.handleToolsCall), [`getTelemetry`](index.ts.md#getTelemetry), [`start`](../mcp/index.ts.md#MCPServer.start), [`durationMs`](index.ts.md#recordIndexEvent.result-typeLiteral6.durationMs), [`registerForExit`](index.ts.md#registerForExit), [`singleton`](index.ts.md#singleton), [`exitInstances`](index.ts.md#exitInstances)

### `TelemetryOptions`
- def: [`src/telemetry/index.ts:124`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L124)
- signature: `interface TelemetryOptions`
- members:
  - `dir` — [`L126`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L126) — Global state dir; defaults to ~/.codegraph. Tests inject a temp dir.
  - `env` — [`L129`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L129)
  - `fetchImpl` — [`L127`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L127)
  - `installExitHook` — [`L132`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L132) — Tests opt out so short-lived instances don't pile onto process 'exit'.
  - `now` — [`L128`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L128)
  - `stderr` — [`L130`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L130)
- used by: [`<constructor>`](index.ts.md#Telemetry.-constructor)

### `TelemetryStatus`
- def: [`src/telemetry/index.ts:97`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L97)
- signature: `interface TelemetryStatus`
- members:
  - `configPath` — [`L102`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L102) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `decidedBy` — [`L100`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L100) — What decided the current state — mirrors the precedence order. — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `enabled` — [`L98`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L98) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
  - `machineId` — [`L101`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L101) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runInstallerWithOptions`](../installer/index.ts.md#runInstallerWithOptions), [`getStatus`](index.ts.md#Telemetry.getStatus), [`isEnabled`](index.ts.md#Telemetry.isEnabled)

### `UsageKind`
- def: [`src/telemetry/index.ts:43`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L43)
- signature: `type UsageKind`
- used by: [`recordUsage`](index.ts.md#Telemetry.recordUsage), [`k`](index.ts.md#CountLine.k)

## Functions
- `bucketDuration(ms: number)` — [`L54`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L54)
- `bucketFileCount(n: number)` — [`L47`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L47) — Coarse buckets — exact counts are deliberately not collected.
- `getStats(method)` — [`L67`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L67)
- `getTelemetry()` — [`L543`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L543) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
- `recordIndexEvent(cg: { getStats(): { filesByLanguage: Record<string, number>; }; }, result: { filesIndexed: number; durationMs: number; })` — [`L66`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L66) — Shared "a full index completed" event (CLI init/index + installer local
- `registerForExit(instance: Telemetry)` — [`L139`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L139) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)

## Module values
- `DEFAULT_FLUSH_TIMEOUT_MS` — [`L39`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L39)
- `MAX_BUFFER_BYTES` — [`L37`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L37)
- `MAX_EVENTS_PER_REQUEST` — [`L38`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L38) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- `SCHEMA_VERSION` — [`L36`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L36) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- `STALE_CLAIM_MS` — [`L41`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L41) — A crashed sender's claimed file is merged back after this long.
- `TELEMETRY_DOCS` — [`L31`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L31)
- `TELEMETRY_ENDPOINT` — [`L30`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L30)
- `durationMs` — [`L68`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L68)
- `exitInstances` — [`L137`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L137) — documented in [telemetry-index.ts](../../../concepts/telemetry-index.ts.md)
- `exitListenerRegistered` — [`L138`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L138)
- `filesByLanguage` — [`L67`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L67)
- `filesIndexed` — [`L68`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L68)
- `singleton` — [`L541`](../../../../../../raw/code/codegraph/src/telemetry/index.ts#L541)

