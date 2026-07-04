---
title: 'Module: extensions/vscode/src/webview/dashboardPanel.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/webview/dashboardPanel.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/webview/`dashboardPanel.ts`/DashboardPanel#
symbols:
  DashboardPanel.refresh: refresh().
  DashboardPanel.show: show().
  DashboardPanel.-constructor: '`<constructor>`().'
  DashboardPanel.panel: panel.
  DashboardPanel.dispose: dispose().
  DashboardPanel.notifyRefresh: notifyRefresh().
  DashboardPanel.getSelectedRepo: getSelectedRepo().
  DashboardPanel.disposables: disposables.
  DashboardPanel.disposables.Array.typeLiteral1.dispose: disposables.Array:typeLiteral1:dispose().
  DashboardPanel: ''
  DashboardPanel.getSelectedRepo.repos-Array.typeLiteral2.path: getSelectedRepo().(repos)Array:typeLiteral2:path.
---
# Module: [`extensions/vscode/src/webview/dashboardPanel.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts)

## Classes
### `DashboardPanel`
- def: [`extensions/vscode/src/webview/dashboardPanel.ts:7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L7)
- signature: `class DashboardPanel`
- members:
  - `<constructor>(service: CgcService, client: CgcMcpClient)` — [`L11`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L11) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `dispose(method)` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L9)
  - `dispose(method)` — [`L108`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L108)
  - `getSelectedRepo(method)` — [`L25`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L25) — Read selected repo from the VS Code config — single source of truth.
  - `notifyRefresh(method)` — [`L104`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L104)
  - `refresh(method)` — [`L94`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L94) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `show(method)` — [`L31`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L31)
  - `disposables` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L9)
  - `panel` — [`L8`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L8)
  - `path` — [`L25`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardPanel.ts#L25)
- uses (calls/refs, reference-scoped): [`cgcEvents`](../mcp/eventBus.ts.md#cgcEvents), [`emit`](../mcp/eventBus.ts.md#CgcEventBus.emit), [`on`](../mcp/eventBus.ts.md#CgcEventBus.on), [`renderDashboardHtml`](dashboardTemplate.ts.md#renderDashboardHtml), [`getComplexityHotspots`](../mcp/service.ts.md#CgcService.getComplexityHotspots), [`CgcService`](../mcp/service.ts.md#CgcService), [`listRepositories`](../mcp/service.ts.md#CgcService.listRepositories), [`CgcMcpClient`](../mcp/client.ts.md#CgcMcpClient), [`restart`](../mcp/client.ts.md#CgcMcpClient.restart), [`findCode`](../mcp/service.ts.md#CgcService.findCode), [`runCypher`](../mcp/service.ts.md#CgcService.runCypher), [`hotspots`](dashboardTemplate.ts.md#DashboardPayload.typeLiteral0.hotspots), [`indexWorkspace`](../mcp/service.ts.md#CgcService.indexWorkspace), [`repos`](dashboardTemplate.ts.md#DashboardPayload.typeLiteral0.repos), [`watchWorkspace`](../mcp/service.ts.md#CgcService.watchWorkspace), [`selectedRepo`](dashboardTemplate.ts.md#DashboardPayload.typeLiteral0.selectedRepo)  (2 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

