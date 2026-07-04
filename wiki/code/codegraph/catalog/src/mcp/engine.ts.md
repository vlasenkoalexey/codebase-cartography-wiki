---
title: 'Module: src/mcp/engine.ts'
type: catalog
provenance: extracted
module: src/mcp/engine.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`engine.ts`/
symbols:
  MCPEngine.retryInitializeSync: MCPEngine#retryInitializeSync().
  MCPEngine.doInitialize: MCPEngine#doInitialize().
  MCPEngine.maybeStartPool: MCPEngine#maybeStartPool().
  MCPEngine.stop: MCPEngine#stop().
  MCPEngine.startWatching: MCPEngine#startWatching().
  MCPEngine.catchUpSync: MCPEngine#catchUpSync().
  MCPEngine.ensureInitialized: MCPEngine#ensureInitialized().
  MCPEngine.-constructor: MCPEngine#`<constructor>`().
  MCPEngine.toolHandler: MCPEngine#toolHandler.
  MCPEngine.cg: MCPEngine#cg.
  MCPEngine.queryPool: MCPEngine#queryPool.
  MCPEngine: MCPEngine#
  MCPEngine.setProjectPathHint: MCPEngine#setProjectPathHint().
  MCPEngine.getToolHandler: MCPEngine#getToolHandler().
  MCPEngine.hasDefaultCodeGraph: MCPEngine#hasDefaultCodeGraph().
  MCPEngine.projectPath: MCPEngine#projectPath.
  MCPEngine.opts: MCPEngine#opts.
  MCPEngine.initPromise: MCPEngine#initPromise.
  MCPEngine.closed: MCPEngine#closed.
  loadCodeGraph: loadCodeGraph.
  MCPEngine.getProjectPath: MCPEngine#getProjectPath().
  MCPEngineOptions.watch: MCPEngineOptions#watch.
  MCPEngineOptions.queryPool: MCPEngineOptions#queryPool.
  MCPEngine.watcherStarted: MCPEngine#watcherStarted.
  MCPEngineOptions: MCPEngineOptions#
  parseDebounceEnv: parseDebounceEnv().
---
# Module: [`src/mcp/engine.ts`](../../../../../../raw/code/codegraph/src/mcp/engine.ts)

## Classes
### `MCPEngine`
- def: [`src/mcp/engine.ts:53`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L53)
- doc: Shared MCP engine. Thread-safe in the sense that multiple sessions can
- signature: `class MCPEngine`
- members:
  - `<constructor>(opts?: MCPEngineOptions)` — [`L69`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L69) — Shared MCP engine. Thread-safe in the sense that multiple sessions can — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `catchUpSync(method)` — [`L296`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L296) — Reconcile the index with the current filesystem once, right after open —
  - `doInitialize(method)` — [`L201`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L201) — documented in [directory.ts](../../../concepts/directory.ts.md)
  - `ensureInitialized(method)` — [`L133`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L133) — Walk up from `searchFrom` to find the nearest `.codegraph/` and open it. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `getProjectPath(method)` — [`L110`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L110) — Project root that the engine resolved on first init (null if none).
  - `getToolHandler(method)` — [`L115`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L115) — Shared ToolHandler — sessions delegate tool dispatch through this.
  - `hasDefaultCodeGraph(method)` — [`L120`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L120) — Whether the default project's CodeGraph is open.
  - `maybeStartPool(method)` — [`L80`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L80) — Start the worker-thread query pool once a default project is open (daemon — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `retryInitializeSync(method)` — [`L157`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L157) — Synchronous last-resort init used by the per-session retry loop when the — documented in [directory.ts](../../../concepts/directory.ts.md)
  - `setProjectPathHint(method)` — [`L104`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L104) — Convenience for {@link MCPServer } compatibility: pre-seed an explicit — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `startWatching(method)` — [`L231`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L231) — Start file watching on the active CodeGraph instance. Idempotent — the
  - `stop(method)` — [`L184`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L184) — Close everything. Used on graceful daemon shutdown (SIGTERM/idle timeout) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `cg` — [`L54`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L54) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `closed` — [`L64`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L64)
  - `initPromise` — [`L61`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L61)
  - `opts` — [`L63`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L63)
  - `projectPath` — [`L59`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L59)
  - `queryPool` — [`L67`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L67)
  - `toolHandler` — [`L55`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L55) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `watcherStarted` — [`L62`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L62)
- uses (calls/refs, reference-scoped): [`sync`](../index.ts.md#CodeGraph.sync), [`open`](../index.ts.md#CodeGraph.open), [`CodeGraph`](../index.ts.md#CodeGraph), [`<constructor>`](query-pool.ts.md#QueryPool.-constructor), [`watch`](../index.ts.md#CodeGraph.watch), [`destroy`](query-pool.ts.md#QueryPool.destroy), [`openSync`](../index.ts.md#CodeGraph.openSync), [`watchDisabledReason`](../sync/watch-policy.ts.md#watchDisabledReason), [`close`](../index.ts.md#CodeGraph.close), [`findNearestCodeGraphRoot`](../directory.ts.md#findNearestCodeGraphRoot), [`ToolHandler`](tools.ts.md#ToolHandler), [`closeAll`](tools.ts.md#ToolHandler.closeAll), [`filesAdded`](../extraction/index.ts.md#SyncResult.filesAdded), [`filesModified`](../extraction/index.ts.md#SyncResult.filesModified), [`setQueryPool`](tools.ts.md#ToolHandler.setQueryPool), [`filesRemoved`](../extraction/index.ts.md#SyncResult.filesRemoved), [`setDefaultProjectHint`](tools.ts.md#ToolHandler.setDefaultProjectHint), [`QueryPool`](query-pool.ts.md#QueryPool), [`loadCodeGraph`](engine.ts.md#loadCodeGraph), [`resolvePoolSize`](query-pool.ts.md#resolvePoolSize), [`setDefaultCodeGraph`](tools.ts.md#ToolHandler.setDefaultCodeGraph), [`<constructor>`](tools.ts.md#ToolHandler.-constructor), [`setCatchUpGate`](tools.ts.md#ToolHandler.setCatchUpGate), [`hasDefaultCodeGraph`](tools.ts.md#ToolHandler.hasDefaultCodeGraph), [`queryPool`](engine.ts.md#MCPEngineOptions.queryPool), [`watch`](engine.ts.md#MCPEngineOptions.watch), [`MCPEngineOptions`](engine.ts.md#MCPEngineOptions), [`root`](query-pool.ts.md#QueryPoolOptions.root), [`size`](query-pool.ts.md#QueryPoolOptions.size), [`parseDebounceEnv`](engine.ts.md#parseDebounceEnv)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-index.ts), [`proxy.ts`](proxy.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-proxy.ts), [`start`](daemon.ts.md#Daemon.start), [`runLocalHandshakeProxy`](proxy.ts.md#runLocalHandshakeProxy), [`daemon.ts`](daemon.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon.ts), [`session.ts`](session.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-session.ts), [`startDirect`](index.ts.md#MCPServer.startDirect), [`handleInitialize`](session.ts.md#MCPSession.handleInitialize), [`handleToolsCall`](session.ts.md#MCPSession.handleToolsCall), [`stop`](daemon.ts.md#Daemon.stop), [`<constructor>`](daemon.ts.md#Daemon.-constructor), [`stop`](index.ts.md#MCPServer.stop), [`runProxyWithLocalHandshake`](index.ts.md#MCPServer.runProxyWithLocalHandshake), [`retryInitIfNeeded`](session.ts.md#MCPSession.retryInitIfNeeded), [`handleToolsList`](session.ts.md#MCPSession.handleToolsList), [`<constructor>`](session.ts.md#MCPSession.-constructor), [`initFromRoots`](session.ts.md#MCPSession.initFromRoots), [`engine`](index.ts.md#MCPServer.engine), [`engine`](daemon.ts.md#Daemon.engine), [`makeEngine`](proxy.ts.md#LocalHandshakeDeps.makeEngine)

### `MCPEngineOptions`
- def: [`src/mcp/engine.ts:29`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L29)
- signature: `interface MCPEngineOptions`
- members:
  - `queryPool` — [`L44`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L44) — Whether to off-load read-tool dispatch to a worker-thread pool. Only the
  - `watch` — [`L35`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L35) — Whether to start the file watcher when initializing. Daemon and direct
- used by: [`maybeStartPool`](engine.ts.md#MCPEngine.maybeStartPool), [`startWatching`](engine.ts.md#MCPEngine.startWatching), [`<constructor>`](engine.ts.md#MCPEngine.-constructor), [`opts`](engine.ts.md#MCPEngine.opts)

## Functions
- `parseDebounceEnv(raw: string | undefined)` — [`L328`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L328) — Parse and clamp the CODEGRAPH_WATCH_DEBOUNCE_MS env override.

## Module values
- `loadCodeGraph` — [`L26`](../../../../../../raw/code/codegraph/src/mcp/engine.ts#L26)

