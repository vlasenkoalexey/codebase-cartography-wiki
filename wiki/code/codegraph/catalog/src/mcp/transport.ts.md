---
title: 'Module: src/mcp/transport.ts'
type: catalog
provenance: extracted
module: src/mcp/transport.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`transport.ts`/
symbols:
  LineBasedJsonRpcTransport.handleLine: LineBasedJsonRpcTransport#handleLine().
  StdioTransport.start: StdioTransport#start().
  JsonRpcRequest: JsonRpcRequest#
  LineBasedJsonRpcTransport.sendError: LineBasedJsonRpcTransport#sendError().
  LineBasedJsonRpcTransport.notify: LineBasedJsonRpcTransport#notify().
  SocketTransport.start: SocketTransport#start().
  JsonRpcTransport: JsonRpcTransport#
  JsonRpcRequest.id: JsonRpcRequest#id.
  JsonRpcTransport.start: JsonRpcTransport#start().
  StdioTransport.-constructor: StdioTransport#`<constructor>`().
  MessageHandler: MessageHandler#
  LineBasedJsonRpcTransport.request: LineBasedJsonRpcTransport#request().
  LineBasedJsonRpcTransport.sendResult: LineBasedJsonRpcTransport#sendResult().
  JsonRpcTransport.sendResult: JsonRpcTransport#sendResult().
  LineBasedJsonRpcTransport: LineBasedJsonRpcTransport#
  SocketTransport.handleSocketClose: SocketTransport#handleSocketClose().
  JsonRpcTransport.stop: JsonRpcTransport#stop().
  LineBasedJsonRpcTransport.write: LineBasedJsonRpcTransport#write().
  LineBasedJsonRpcTransport.start: LineBasedJsonRpcTransport#start().
  StdioTransport.stop: StdioTransport#stop().
  ErrorCodes: ErrorCodes.
  LineBasedJsonRpcTransport.send: LineBasedJsonRpcTransport#send().
  LineBasedJsonRpcTransport.messageHandler: LineBasedJsonRpcTransport#messageHandler.
  LineBasedJsonRpcTransport.pending: LineBasedJsonRpcTransport#pending.
  LineBasedJsonRpcTransport.stopped: LineBasedJsonRpcTransport#stopped.
  LineBasedJsonRpcTransport.idPrefix: LineBasedJsonRpcTransport#idPrefix().
  StdioTransport.rl: StdioTransport#rl.
  JsonRpcTransport.sendError: JsonRpcTransport#sendError().
  LineBasedJsonRpcTransport.rejectPending: LineBasedJsonRpcTransport#rejectPending().
  StdioTransport.opts: StdioTransport#opts.
  JsonRpcNotification: JsonRpcNotification#
  JsonRpcTransport.send: JsonRpcTransport#send().
  LineBasedJsonRpcTransport.stop: LineBasedJsonRpcTransport#stop().
  SocketTransport.buffer: SocketTransport#buffer.
  SocketTransport.stop: SocketTransport#stop().
  JsonRpcResponse: JsonRpcResponse#
  StdioTransport: StdioTransport#
  JsonRpcTransport.request: JsonRpcTransport#request().
  LineBasedJsonRpcTransport.handleResponse: LineBasedJsonRpcTransport#handleResponse().
  SocketTransport: SocketTransport#
  SocketTransport.onClose: SocketTransport#onClose().
  StdioTransportOptions.exitOnClose: StdioTransportOptions#exitOnClose.
  StdioTransportOptions.onClose: StdioTransportOptions#onClose.
  SocketTransport.closeHandlers: SocketTransport#closeHandlers.
  JsonRpcTransport.notify: JsonRpcTransport#notify().
  JsonRpcRequest.method: JsonRpcRequest#method.
  JsonRpcRequest.params: JsonRpcRequest#params.
  JsonRpcResponse.jsonrpc: JsonRpcResponse#jsonrpc.
  JsonRpcResponse.id: JsonRpcResponse#id.
  JsonRpcNotification.method: JsonRpcNotification#method.
  StdioTransportOptions: StdioTransportOptions#
  JsonRpcResponse.result: JsonRpcResponse#result.
  JsonRpcResponse.error: JsonRpcResponse#error.
  JsonRpcError: JsonRpcError#
  JsonRpcNotification.jsonrpc: JsonRpcNotification#jsonrpc.
  JsonRpcNotification.params: JsonRpcNotification#params.
  LineBasedJsonRpcTransport.nextRequestId: LineBasedJsonRpcTransport#nextRequestId.
  LineBasedJsonRpcTransport.isValidMessage: LineBasedJsonRpcTransport#isValidMessage().
  SocketTransport.-constructor: SocketTransport#`<constructor>`().
  JsonRpcRequest.jsonrpc: JsonRpcRequest#jsonrpc.
  JsonRpcError.code: JsonRpcError#code.
  JsonRpcError.message: JsonRpcError#message.
  JsonRpcError.data: JsonRpcError#data.
  StdioTransport.write: StdioTransport#write().
  StdioTransport.idPrefix: StdioTransport#idPrefix().
  SocketTransport.writeRaw: SocketTransport#writeRaw().
  SocketTransport.write: SocketTransport#write().
  SocketTransport.idPrefix: SocketTransport#idPrefix().
---
# Module: [`src/mcp/transport.ts`](../../../../../../raw/code/codegraph/src/mcp/transport.ts)

## Classes
### `JsonRpcError`
- def: [`src/mcp/transport.ts:43`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L43) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- doc: JSON-RPC 2.0 Error
- signature: `interface JsonRpcError`
- members:
  - `code` — [`L44`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L44)
  - `data` — [`L46`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L46)
  - `message` — [`L45`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L45)
- used by: [`JsonRpcResponse`](transport.ts.md#JsonRpcResponse)

### `JsonRpcNotification`
- def: [`src/mcp/transport.ts:52`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L52) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- doc: JSON-RPC 2.0 Notification (no id, no response expected)
- signature: `interface JsonRpcNotification`
- members:
  - `jsonrpc` — [`L53`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L53)
  - `method` — [`L54`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L54)
  - `params` — [`L55`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L55)
- used by: [`session.ts`](session.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-session.ts), [`handleMessage`](session.ts.md#MCPSession.handleMessage), [`handleLine`](transport.ts.md#LineBasedJsonRpcTransport.handleLine), [`notify`](transport.ts.md#LineBasedJsonRpcTransport.notify), [`MessageHandler`](transport.ts.md#MessageHandler)

### `JsonRpcRequest`
- def: [`src/mcp/transport.ts:23`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L23) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- doc: JSON-RPC 2.0 Request
- signature: `interface JsonRpcRequest`
- members:
  - `id` — [`L25`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L25) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `jsonrpc` — [`L24`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L24)
  - `method` — [`L26`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L26)
  - `params` — [`L27`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L27)
- used by: [`session.ts`](session.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-session.ts), [`handleInitialize`](session.ts.md#MCPSession.handleInitialize), [`handleToolsCall`](session.ts.md#MCPSession.handleToolsCall), [`handleMessage`](session.ts.md#MCPSession.handleMessage), [`handleLine`](transport.ts.md#LineBasedJsonRpcTransport.handleLine), [`handleToolsList`](session.ts.md#MCPSession.handleToolsList), [`MessageHandler`](transport.ts.md#MessageHandler)

### `JsonRpcResponse`
- def: [`src/mcp/transport.ts:33`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L33) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- doc: JSON-RPC 2.0 Response
- signature: `interface JsonRpcResponse`
- members:
  - `error` — [`L37`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L37) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `id` — [`L35`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L35) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `jsonrpc` — [`L34`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L34) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `result` — [`L36`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L36)
- uses (calls/refs, reference-scoped): [`JsonRpcError`](transport.ts.md#JsonRpcError)
- used by: [`sendError`](transport.ts.md#LineBasedJsonRpcTransport.sendError), [`sendResult`](transport.ts.md#LineBasedJsonRpcTransport.sendResult), [`send`](transport.ts.md#LineBasedJsonRpcTransport.send), [`send`](transport.ts.md#JsonRpcTransport.send)

### `JsonRpcTransport`
- def: [`src/mcp/transport.ts:74`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L74)
- doc: Generic JSON-RPC transport interface — common surface for stdio and socket
- signature: `interface JsonRpcTransport`
- members:
  - `notify(method)` — [`L78`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L78)
  - `request(method)` — [`L79`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L79)
  - `send(method)` — [`L77`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L77)
  - `sendError(method)` — [`L81`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L81) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `sendResult(method)` — [`L80`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L80)
  - `start(method)` — [`L75`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L75) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `stop(method)` — [`L76`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L76)
- uses (calls/refs, reference-scoped): [`start`](transport.ts.md#StdioTransport.start), [`sendError`](transport.ts.md#LineBasedJsonRpcTransport.sendError), [`notify`](transport.ts.md#LineBasedJsonRpcTransport.notify), [`start`](transport.ts.md#SocketTransport.start), [`MessageHandler`](transport.ts.md#MessageHandler), [`request`](transport.ts.md#LineBasedJsonRpcTransport.request), [`sendResult`](transport.ts.md#LineBasedJsonRpcTransport.sendResult), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`start`](transport.ts.md#LineBasedJsonRpcTransport.start), [`stop`](transport.ts.md#StdioTransport.stop), [`send`](transport.ts.md#LineBasedJsonRpcTransport.send), [`stop`](transport.ts.md#LineBasedJsonRpcTransport.stop), [`stop`](transport.ts.md#SocketTransport.stop), [`JsonRpcResponse`](transport.ts.md#JsonRpcResponse), [`StdioTransport`](transport.ts.md#StdioTransport), [`SocketTransport`](transport.ts.md#SocketTransport)
- used by: [`session.ts`](session.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-session.ts), [`handleInitialize`](session.ts.md#MCPSession.handleInitialize), [`handleToolsCall`](session.ts.md#MCPSession.handleToolsCall), [`handleMessage`](session.ts.md#MCPSession.handleMessage), [`handleToolsList`](session.ts.md#MCPSession.handleToolsList), [`<constructor>`](session.ts.md#MCPSession.-constructor), [`initFromRoots`](session.ts.md#MCPSession.initFromRoots), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`start`](session.ts.md#MCPSession.start), [`stop`](session.ts.md#MCPSession.stop), [`getTransport`](session.ts.md#MCPSession.getTransport)

### `LineBasedJsonRpcTransport`  ·  implements/extends JsonRpcTransport
- def: [`src/mcp/transport.ts:90`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L90)
- doc: Shared implementation of newline-delimited JSON-RPC 2.0 over any
- signature: `class LineBasedJsonRpcTransport`
- members:
  - `handleLine(method)` — [`L162`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L162) — Handle an incoming line of JSON. Both transports feed lines here. — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `handleResponse(method)` — [`L215`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L215) — Resolve (or reject) the pending server-initiated request matching this — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `idPrefix(method)` — [`L103`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L103)
  - `isValidMessage(method)` — [`L231`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L231) — Check if message is a valid JSON-RPC 2.0 message — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `notify(method)` — [`L135`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L135)
  - `rejectPending(method)` — [`L152`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L152) — Fail any in-flight server-initiated requests so their awaiters don't hang.
  - `request(method)` — [`L114`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L114) — Send a server-initiated request to the client and await its response.
  - `send(method)` — [`L131`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L131) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `sendError(method)` — [`L144`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L144) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `sendResult(method)` — [`L140`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L140)
  - `start(method)` — [`L101`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L101)
  - `stop(method)` — [`L104`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L104)
  - `write(method)` — [`L102`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L102) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `messageHandler` — [`L91`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L91) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `nextRequestId` — [`L98`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L98)
  - `pending` — [`L94`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L94) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `stopped` — [`L99`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L99)
- uses (calls/refs, reference-scoped): [`start`](transport.ts.md#StdioTransport.start), [`JsonRpcRequest`](transport.ts.md#JsonRpcRequest), [`start`](transport.ts.md#SocketTransport.start), [`JsonRpcTransport`](transport.ts.md#JsonRpcTransport), [`id`](transport.ts.md#JsonRpcRequest.id), [`MessageHandler`](transport.ts.md#MessageHandler), [`stop`](transport.ts.md#StdioTransport.stop), [`ErrorCodes`](transport.ts.md#ErrorCodes), [`JsonRpcNotification`](transport.ts.md#JsonRpcNotification), [`stop`](transport.ts.md#SocketTransport.stop), [`JsonRpcResponse`](transport.ts.md#JsonRpcResponse), [`StdioTransport`](transport.ts.md#StdioTransport), [`SocketTransport`](transport.ts.md#SocketTransport), [`id`](transport.ts.md#JsonRpcResponse.id), [`jsonrpc`](transport.ts.md#JsonRpcResponse.jsonrpc), [`method`](transport.ts.md#JsonRpcNotification.method), [`error`](transport.ts.md#JsonRpcResponse.error), [`jsonrpc`](transport.ts.md#JsonRpcNotification.jsonrpc), [`params`](transport.ts.md#JsonRpcNotification.params), [`result`](transport.ts.md#JsonRpcResponse.result), [`idPrefix`](transport.ts.md#SocketTransport.idPrefix), [`idPrefix`](transport.ts.md#StdioTransport.idPrefix), [`write`](transport.ts.md#SocketTransport.write), [`write`](transport.ts.md#StdioTransport.write)
- used by: [`start`](transport.ts.md#StdioTransport.start), [`start`](transport.ts.md#SocketTransport.start), [`JsonRpcTransport`](transport.ts.md#JsonRpcTransport), [`start`](transport.ts.md#JsonRpcTransport.start), [`handleSocketClose`](transport.ts.md#SocketTransport.handleSocketClose), [`sendResult`](transport.ts.md#JsonRpcTransport.sendResult), [`stop`](transport.ts.md#JsonRpcTransport.stop), [`stop`](transport.ts.md#StdioTransport.stop), [`sendError`](transport.ts.md#JsonRpcTransport.sendError), [`send`](transport.ts.md#JsonRpcTransport.send), [`stop`](transport.ts.md#SocketTransport.stop), [`StdioTransport`](transport.ts.md#StdioTransport), [`SocketTransport`](transport.ts.md#SocketTransport), [`request`](transport.ts.md#JsonRpcTransport.request), [`notify`](transport.ts.md#JsonRpcTransport.notify)

### `MessageHandler`
- def: [`src/mcp/transport.ts:67`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L67) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- signature: `type MessageHandler`
- uses (calls/refs, reference-scoped): [`JsonRpcRequest`](transport.ts.md#JsonRpcRequest), [`JsonRpcNotification`](transport.ts.md#JsonRpcNotification)
- used by: [`start`](transport.ts.md#StdioTransport.start), [`start`](transport.ts.md#SocketTransport.start), [`start`](transport.ts.md#JsonRpcTransport.start), [`start`](transport.ts.md#LineBasedJsonRpcTransport.start), [`messageHandler`](transport.ts.md#LineBasedJsonRpcTransport.messageHandler)

### `SocketTransport`  ·  implements/extends JsonRpcTransport, LineBasedJsonRpcTransport
- def: [`src/mcp/transport.ts:336`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L336)
- doc: Socket Transport for MCP daemon sessions.
- signature: `class SocketTransport`
- members:
  - `<constructor>(socket: Socket, prefix?: string)` — [`L340`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L340) — Socket Transport for MCP daemon sessions.
  - `handleSocketClose(method)` — [`L410`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L410)
  - `idPrefix(method)` — [`L406`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L406)
  - `onClose(method)` — [`L348`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L348) — Register a callback fired exactly once when the socket closes (from either
  - `start(method)` — [`L352`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L352) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `stop(method)` — [`L379`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L379)
  - `write(method)` — [`L400`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L400) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `writeRaw(method)` — [`L394`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L394) — Write a one-shot line directly to the socket (no JSON-RPC framing applied
  - `buffer` — [`L337`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L337)
  - `closeHandlers` — [`L338`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L338)
- uses (calls/refs, reference-scoped): [`handleLine`](transport.ts.md#LineBasedJsonRpcTransport.handleLine), [`MessageHandler`](transport.ts.md#MessageHandler), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`messageHandler`](transport.ts.md#LineBasedJsonRpcTransport.messageHandler), [`stopped`](transport.ts.md#LineBasedJsonRpcTransport.stopped), [`rejectPending`](transport.ts.md#LineBasedJsonRpcTransport.rejectPending)
- used by: [`daemon.ts`](daemon.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-daemon.ts), [`handleConnection`](daemon.ts.md#Daemon.handleConnection), [`JsonRpcTransport`](transport.ts.md#JsonRpcTransport), [`start`](transport.ts.md#JsonRpcTransport.start), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`stop`](transport.ts.md#JsonRpcTransport.stop), [`write`](transport.ts.md#LineBasedJsonRpcTransport.write), [`start`](transport.ts.md#LineBasedJsonRpcTransport.start), [`idPrefix`](transport.ts.md#LineBasedJsonRpcTransport.idPrefix), [`stop`](transport.ts.md#LineBasedJsonRpcTransport.stop)

### `StdioTransport`  ·  implements/extends JsonRpcTransport, LineBasedJsonRpcTransport
- def: [`src/mcp/transport.ts:264`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L264)
- doc: Stdio Transport for MCP
- signature: `class StdioTransport`
- members:
  - `<constructor>(opts?: StdioTransportOptions)` — [`L268`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L268) — Stdio Transport for MCP
  - `idPrefix(method)` — [`L323`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L323)
  - `start(method)` — [`L276`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L276) — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `stop(method)` — [`L309`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L309)
  - `write(method)` — [`L319`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L319) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `opts` — [`L266`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L266) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `rl` — [`L265`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L265) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- uses (calls/refs, reference-scoped): [`handleLine`](transport.ts.md#LineBasedJsonRpcTransport.handleLine), [`MessageHandler`](transport.ts.md#MessageHandler), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`messageHandler`](transport.ts.md#LineBasedJsonRpcTransport.messageHandler), [`stopped`](transport.ts.md#LineBasedJsonRpcTransport.stopped), [`rejectPending`](transport.ts.md#LineBasedJsonRpcTransport.rejectPending), [`exitOnClose`](transport.ts.md#StdioTransportOptions.exitOnClose), [`onClose`](transport.ts.md#StdioTransportOptions.onClose), [`StdioTransportOptions`](transport.ts.md#StdioTransportOptions)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-index.ts), [`startDirect`](index.ts.md#MCPServer.startDirect), [`JsonRpcTransport`](transport.ts.md#JsonRpcTransport), [`start`](transport.ts.md#JsonRpcTransport.start), [`LineBasedJsonRpcTransport`](transport.ts.md#LineBasedJsonRpcTransport), [`stop`](transport.ts.md#JsonRpcTransport.stop), [`write`](transport.ts.md#LineBasedJsonRpcTransport.write), [`start`](transport.ts.md#LineBasedJsonRpcTransport.start), [`idPrefix`](transport.ts.md#LineBasedJsonRpcTransport.idPrefix), [`stop`](transport.ts.md#LineBasedJsonRpcTransport.stop)

### `StdioTransportOptions`
- def: [`src/mcp/transport.ts:240`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L240) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- signature: `interface StdioTransportOptions`
- members:
  - `exitOnClose` — [`L247`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L247) — If true, the transport calls `process.exit(0)` when stdin closes. Set to — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
  - `onClose` — [`L252`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L252) — Optional callback fired when the stdin stream closes. The daemon uses — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)
- used by: [`start`](transport.ts.md#StdioTransport.start), [`<constructor>`](transport.ts.md#StdioTransport.-constructor), [`opts`](transport.ts.md#StdioTransport.opts)

## Module values
- `ErrorCodes` — [`L59`](../../../../../../raw/code/codegraph/src/mcp/transport.ts#L59) — documented in [mcp-transport.ts](../../../concepts/mcp-transport.ts.md)

