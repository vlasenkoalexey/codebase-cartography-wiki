---
title: 'Module: extensions/vscode/src/webview/setupPanel.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/webview/setupPanel.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/webview/`setupPanel.ts`/SetupPanel#
symbols:
  SetupPanel: ''
  SetupPanel._panel: _panel.
  SetupPanel.createOrShow: createOrShow().
  SetupPanel._handleSave: _handleSave().
  SetupPanel.dispose: dispose().
  SetupPanel._update: _update().
  SetupPanel.currentPanel: currentPanel.
  SetupPanel._handleTest: _handleTest().
  SetupPanel._disposables: _disposables.
  SetupPanel.viewType: viewType.
  SetupPanel._getHtmlForWebview: _getHtmlForWebview().
---
# Module: [`extensions/vscode/src/webview/setupPanel.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts)

## Classes
### `SetupPanel`
- def: [`extensions/vscode/src/webview/setupPanel.ts:4`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L4)
- signature: `class SetupPanel`
- members:
  - `createOrShow(method)` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L10)
  - `dispose(method)` — [`L127`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L127)
  - `currentPanel` — [`L6`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L6)
  - `viewType` — [`L5`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L5)
- protocol/private: `_disposables`[`L8`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L8), `_getHtmlForWebview`[`L149`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L149), `_handleSave`[`L104`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L104), `_handleTest`[`L58`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L58), `_panel`[`L7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L7), `_update`[`L138`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/setupPanel.ts#L138)
- uses (calls/refs, reference-scoped): [`ensureStarted`](../mcp/client.ts.md#CgcMcpClient.ensureStarted), [`CgcMcpClient`](../mcp/client.ts.md#CgcMcpClient), [`dispose`](../mcp/client.ts.md#CgcMcpClient.dispose)

