---
title: 'Module: src/mcp/session.ts'
type: catalog
provenance: extracted
module: src/mcp/session.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`session.ts`/
symbols:
  MCPSession.handleInitialize: MCPSession#handleInitialize().
  MCPSession.handleToolsCall: MCPSession#handleToolsCall().
  MCPSession.handleMessage: MCPSession#handleMessage().
  MCPSession.retryInitIfNeeded: MCPSession#retryInitIfNeeded().
  MCPSession.handleToolsList: MCPSession#handleToolsList().
  MCPSession.-constructor: MCPSession#`<constructor>`().
  MCPSession.initFromRoots: MCPSession#initFromRoots().
  MCPSession.resolvePromise: MCPSession#resolvePromise.
  MCPSession.start: MCPSession#start().
  MCPSession: MCPSession#
  SERVER_INFO: SERVER_INFO.
  MCPSession.stop: MCPSession#stop().
  MCPSession.clientInfo: MCPSession#clientInfo.
  MCPSession.explicitProjectPath: MCPSession#explicitProjectPath.
  firstRootPath: firstRootPath().
  PROTOCOL_VERSION: PROTOCOL_VERSION.
  fileUriToPath: fileUriToPath().
  MCPSession.getTransport: MCPSession#getTransport().
  MCPSession.clientSupportsRoots: MCPSession#clientSupportsRoots.
  MCPSession.rootsAttempted: MCPSession#rootsAttempted.
  ROOTS_LIST_TIMEOUT_MS: ROOTS_LIST_TIMEOUT_MS.
  MCPSessionOptions: MCPSessionOptions#
  MCPSessionOptions.explicitProjectPath: MCPSessionOptions#explicitProjectPath.
---
# Module: [`src/mcp/session.ts`](../../../../../../raw/code/codegraph/src/mcp/session.ts)

## Classes
### `MCPSession`
- def: [`src/mcp/session.ts:84`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L84)
- doc: One MCP client's view of the server. Created fresh per stdio launch
- signature: `class MCPSession`
- members:
  - `<constructor>(transport: JsonRpcTransport, engine: MCPEngine, opts?: MCPSessionOptions)` — [`L92`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L92) — One MCP client's view of the server. Created fresh per stdio launch — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `getTransport(method)` — [`L117`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L117) — Underlying transport — exposed for daemon-side close hooks.
  - `handleInitialize(method)` — [`L163`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L163) — documented in [directory.ts](../../../concepts/directory.ts.md)
  - `handleMessage(method)` — [`L121`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L121) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `handleToolsCall(method)` — [`L239`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L239) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `handleToolsList(method)` — [`L221`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L221) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `initFromRoots(method)` — [`L309`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L309) — Ask the client for its workspace root via `roots/list` and open the
  - `retryInitIfNeeded(method)` — [`L280`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L280) — Lazy default-project resolution. Three layers: — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `start(method)` — [`L104`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L104) — Start handling messages from the transport. Returns immediately — the
  - `stop(method)` — [`L112`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L112) — Tear down the session. Does NOT touch the engine (the engine may serve
  - `clientInfo` — [`L87`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L87) — From the initialize handshake — attributes usage rollups to the agent host.
  - `clientSupportsRoots` — [`L85`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L85)
  - `explicitProjectPath` — [`L90`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L90)
  - `resolvePromise` — [`L89`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L89)
  - `rootsAttempted` — [`L88`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L88)
- uses (calls/refs, reference-scoped): [`recordUsage`](../telemetry/index.ts.md#Telemetry.recordUsage), [`execute`](tools.ts.md#ToolHandler.execute), [`tools`](tools.ts.md#tools), [`retryInitializeSync`](engine.ts.md#MCPEngine.retryInitializeSync), [`getTelemetry`](../telemetry/index.ts.md#getTelemetry), [`getTools`](tools.ts.md#ToolHandler.getTools), [`ensureInitialized`](engine.ts.md#MCPEngine.ensureInitialized), [`JsonRpcRequest`](transport.ts.md#JsonRpcRequest), [`name`](tools.ts.md#ToolDefinition.name), [`findNearestCodeGraphRoot`](../directory.ts.md#findNearestCodeGraphRoot), [`JsonRpcTransport`](transport.ts.md#JsonRpcTransport), [`id`](transport.ts.md#JsonRpcRequest.id), [`isError`](tools.ts.md#ToolResult.isError), [`start`](transport.ts.md#JsonRpcTransport.start), [`sendResult`](transport.ts.md#JsonRpcTransport.sendResult), [`MCPEngine`](engine.ts.md#MCPEngine), [`stop`](transport.ts.md#JsonRpcTransport.stop), [`getToolHandler`](engine.ts.md#MCPEngine.getToolHandler), [`ErrorCodes`](transport.ts.md#ErrorCodes), [`hasDefaultCodeGraph`](engine.ts.md#MCPEngine.hasDefaultCodeGraph), [`SERVER_INFO`](session.ts.md#SERVER_INFO), [`sendError`](transport.ts.md#JsonRpcTransport.sendError), [`ClientInfo`](../telemetry/index.ts.md#ClientInfo), [`JsonRpcNotification`](transport.ts.md#JsonRpcNotification), [`SERVER_INSTRUCTIONS`](server-instructions.ts.md#SERVER_INSTRUCTIONS), [`firstRootPath`](session.ts.md#firstRootPath), [`getProjectPath`](engine.ts.md#MCPEngine.getProjectPath), [`request`](transport.ts.md#JsonRpcTransport.request), [`PROTOCOL_VERSION`](session.ts.md#PROTOCOL_VERSION), [`fileUriToPath`](session.ts.md#fileUriToPath), [`SERVER_INSTRUCTIONS_NO_ROOT_INDEX`](server-instructions.ts.md#SERVER_INSTRUCTIONS_NO_ROOT_INDEX), [`method`](transport.ts.md#JsonRpcNotification.method), [`method`](transport.ts.md#JsonRpcRequest.method), [`params`](transport.ts.md#JsonRpcRequest.params), [`MCPSessionOptions`](session.ts.md#MCPSessionOptions), [`ROOTS_LIST_TIMEOUT_MS`](session.ts.md#ROOTS_LIST_TIMEOUT_MS), [`explicitProjectPath`](session.ts.md#MCPSessionOptions.explicitProjectPath)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-index.ts), [`daemon.ts`](daemon.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon.ts), [`handleConnection`](daemon.ts.md#Daemon.handleConnection), [`startDirect`](index.ts.md#MCPServer.startDirect), [`stop`](daemon.ts.md#Daemon.stop), [`stop`](index.ts.md#MCPServer.stop), [`clients`](daemon.ts.md#Daemon.clients), [`reapDeadClients`](daemon.ts.md#Daemon.reapDeadClients), [`dropClient`](daemon.ts.md#Daemon.dropClient), [`session`](index.ts.md#MCPServer.session), [`clientPeers`](daemon.ts.md#Daemon.clientPeers)

### `MCPSessionOptions`
- def: [`src/mcp/session.ts:71`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L71)
- signature: `interface MCPSessionOptions`
- members:
  - `explicitProjectPath` — [`L77`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L77) — Explicit project path from the `--path` CLI flag. When set, the session
- used by: [`<constructor>`](session.ts.md#MCPSession.-constructor)

## Functions
- `fileUriToPath(uri: string)` — [`L48`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L48) — Convert a file:// URI to a filesystem path. Handles URL encoding and
- `firstRootPath(result: unknown)` — [`L62`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L62) — First usable filesystem path from a `roots/list` result, or null.

## Module values
- `PROTOCOL_VERSION` — [`L36`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L36) — MCP Protocol Version (latest the server claims).
- `ROOTS_LIST_TIMEOUT_MS` — [`L42`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L42) — How long to wait for the client's `roots/list` response before giving up
- `SERVER_INFO` — [`L30`](../../../../../../raw/code/codegraph/src/mcp/session.ts#L30) — MCP Server Info — kept on the session because some clients log it. The

