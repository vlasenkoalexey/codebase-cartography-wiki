---
title: 'Module: extensions/vscode/src/webview/callGraphPanel.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/webview/callGraphPanel.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/webview/`callGraphPanel.ts`/CallGraphPanel#
symbols:
  CallGraphPanel._refreshData: _refreshData().
  CallGraphPanel.panel: panel.
  CallGraphPanel.show: show().
  CallGraphPanel.postEditorSelection: postEditorSelection().
  CallGraphPanel.-constructor: '`<constructor>`().'
  CallGraphPanel: ''
  CallGraphPanel.renderHtml: renderHtml().
---
# Module: [`extensions/vscode/src/webview/callGraphPanel.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts)

## Classes
### `CallGraphPanel`
- def: [`extensions/vscode/src/webview/callGraphPanel.ts:4`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L4)
- signature: `class CallGraphPanel`
- members:
  - `<constructor>(service: CgcService)` — [`L7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L7) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `postEditorSelection(method)` — [`L118`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L118)
  - `renderHtml(method)` — [`L124`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L124)
  - `show(method)` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L9)
  - `panel` — [`L5`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L5)
- protocol/private: `_refreshData`[`L44`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/callGraphPanel.ts#L44)
- uses (calls/refs, reference-scoped): [`CgcService`](../mcp/service.ts.md#CgcService), [`findCallers`](../mcp/service.ts.md#CgcService.findCallers), [`listCallees`](../mcp/service.ts.md#CgcService.listCallees), [`runCypher`](../mcp/service.ts.md#CgcService.runCypher)  (2 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

