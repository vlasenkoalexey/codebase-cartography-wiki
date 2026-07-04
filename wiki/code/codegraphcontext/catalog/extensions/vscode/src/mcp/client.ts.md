---
title: 'Module: extensions/vscode/src/mcp/client.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/mcp/client.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/mcp/`client.ts`/
symbols:
  CgcMcpClient.callTool: CgcMcpClient#callTool().
  CgcMcpClient.ensureStarted: CgcMcpClient#ensureStarted().
  CgcMcpClient.onStdout: CgcMcpClient#onStdout().
  CgcMcpClient.proc: CgcMcpClient#proc.
  CgcMcpClient.request: CgcMcpClient#request().
  CgcMcpClient.pending: CgcMcpClient#pending.
  CgcMcpClient: CgcMcpClient#
  CgcMcpClient.restart: CgcMcpClient#restart().
  CgcMcpClient.output: CgcMcpClient#output.
  CgcMcpClient.dispose: CgcMcpClient#dispose().
  CgcMcpClient.internalRequest: CgcMcpClient#internalRequest().
  CgcMcpClient.ensureProcessReady: CgcMcpClient#ensureProcessReady().
  JsonRpcResponse.error: JsonRpcResponse#error.
  CgcMcpClient.listTools: CgcMcpClient#listTools().
  CgcMcpClient.notify: CgcMcpClient#notify().
  JsonRpcResponse.id: JsonRpcResponse#id.
  JsonRpcResponse.error.typeLiteral4.data: JsonRpcResponse#error.typeLiteral4:data.
  CgcMcpClient.internalNotify: CgcMcpClient#internalNotify().
  JsonRpcResponse: JsonRpcResponse#
  JsonRpcResponse.result: JsonRpcResponse#result.
  JsonRpcResponse.error.typeLiteral4.message: JsonRpcResponse#error.typeLiteral4:message.
  PendingRequest: PendingRequest#
  CgcMcpClient.nextId: CgcMcpClient#nextId.
  CgcMcpClient.-constructor: CgcMcpClient#`<constructor>`().
  PendingRequest.typeLiteral5.resolve: PendingRequest#typeLiteral5:resolve.
  PendingRequest.typeLiteral5.reject: PendingRequest#typeLiteral5:reject.
---
# Module: [`extensions/vscode/src/mcp/client.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts)

## Classes
### `CgcMcpClient`
- def: [`extensions/vscode/src/mcp/client.ts:17`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L17)
- signature: `class CgcMcpClient`
- members:
  - `<constructor>(context: vscode.ExtensionContext)` — [`L23`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L23)
  - `callTool(method)` — [`L97`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L97) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `dispose(method)` — [`L106`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L106) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `ensureProcessReady(method)` — [`L212`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L212) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `ensureStarted(method)` — [`L25`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L25) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `internalNotify(method)` — [`L206`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L206) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `internalRequest(method)` — [`L180`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L180) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `listTools(method)` — [`L91`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L91)
  - `notify(method)` — [`L175`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L175)
  - `onStdout(method)` — [`L127`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L127) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `request(method)` — [`L151`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L151) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `restart(method)` — [`L112`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L112) — Kill the current MCP server process and re-start with a fresh DB connection. — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `nextId` — [`L19`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L19)
  - `output` — [`L21`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L21) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `pending` — [`L20`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L20) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `proc` — [`L18`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L18) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- uses (calls/refs, reference-scoped): [`error`](client.ts.md#JsonRpcResponse.error), [`CgcMcpToolResponse`](../types/cgc.ts.md#CgcMcpToolResponse), [`id`](client.ts.md#JsonRpcResponse.id), [`CgcTool`](../types/cgc.ts.md#CgcTool), [`data`](client.ts.md#JsonRpcResponse.error.typeLiteral4.data), [`JsonRpcResponse`](client.ts.md#JsonRpcResponse), [`PendingRequest`](client.ts.md#PendingRequest), [`content`](../types/cgc.ts.md#CgcMcpToolResponse.content), [`message`](client.ts.md#JsonRpcResponse.error.typeLiteral4.message), [`result`](client.ts.md#JsonRpcResponse.result)  (1 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts), [`service.ts`](service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`show`](../webview/dashboardPanel.ts.md#DashboardPanel.show), [`getRepoStats`](service.ts.md#CgcService.getRepoStats), [`getComplexityHotspots`](service.ts.md#CgcService.getComplexityHotspots), [`SetupPanel`](../webview/setupPanel.ts.md#SetupPanel), [`controlPanel.ts`](../views/controlPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-views-controlPanel.ts), [`dashboardPanel.ts`](../webview/dashboardPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-webview-dashboardPanel.ts), [`<constructor>`](../views/controlPanel.ts.md#SidebarControlPanel.-constructor), [`<constructor>`](../webview/dashboardPanel.ts.md#DashboardPanel.-constructor), [`findCallers`](service.ts.md#CgcService.findCallers), [`listRepositories`](service.ts.md#CgcService.listRepositories), [`<constructor>`](../views/statusBarItem.ts.md#CgcStatusBarItem.-constructor), [`createOrShow`](../webview/setupPanel.ts.md#SetupPanel.createOrShow), [`findCallees`](service.ts.md#CgcService.findCallees), [`_handleSave`](../webview/setupPanel.ts.md#SetupPanel._handleSave), [`statusBarItem.ts`](../views/statusBarItem.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-views-statusBarItem.ts), [`findClassHierarchy`](service.ts.md#CgcService.findClassHierarchy), [`findDeadCode`](service.ts.md#CgcService.findDeadCode), [`listCallees`](service.ts.md#CgcService.listCallees), [`variableImpactRadius`](service.ts.md#CgcService.variableImpactRadius), [`checkJobStatus`](service.ts.md#CgcService.checkJobStatus), [`findCallChain`](service.ts.md#CgcService.findCallChain), [`findCode`](service.ts.md#CgcService.findCode), [`findFunctionsByDecorator`](service.ts.md#CgcService.findFunctionsByDecorator), [`findImporters`](service.ts.md#CgcService.findImporters), [`findModuleDeps`](service.ts.md#CgcService.findModuleDeps), [`listFunctions`](service.ts.md#CgcService.listFunctions), [`saveConfig`](../views/controlPanel.ts.md#SidebarControlPanel.saveConfig), [`switchContext`](service.ts.md#CgcService.switchContext), [`getComplexity`](service.ts.md#CgcService.getComplexity), [`discoverContexts`](service.ts.md#CgcService.discoverContexts), [`runCypher`](service.ts.md#CgcService.runCypher), [`indexWorkspace`](service.ts.md#CgcService.indexWorkspace), [`_handleTest`](../webview/setupPanel.ts.md#SetupPanel._handleTest), [`listClasses`](service.ts.md#CgcService.listClasses), [`listImports`](service.ts.md#CgcService.listImports), [`searchBundles`](service.ts.md#CgcService.searchBundles), [`watchWorkspace`](service.ts.md#CgcService.watchWorkspace)  (+5 more)

### `JsonRpcResponse`
- def: [`extensions/vscode/src/mcp/client.ts:6`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L6) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- signature: `interface JsonRpcResponse`
- members:
  - `data` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L9) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `error` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L9) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `id` — [`L7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L7) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `message` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L9) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `result` — [`L8`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L8) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- used by: [`onStdout`](client.ts.md#CgcMcpClient.onStdout)

### `PendingRequest`
- def: [`extensions/vscode/src/mcp/client.ts:12`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L12) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- signature: `type PendingRequest`
- members:
  - `reject` — [`L14`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L14)
  - `resolve` — [`L13`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/client.ts#L13)
- used by: [`pending`](client.ts.md#CgcMcpClient.pending)

