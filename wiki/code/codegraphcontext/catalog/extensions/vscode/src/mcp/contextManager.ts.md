---
title: 'Module: extensions/vscode/src/mcp/contextManager.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/mcp/contextManager.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/mcp/`contextManager.ts`/ContextManager#
symbols:
  ContextManager.initializeContext: initializeContext().
  ContextManager.handlePerRepoMode: handlePerRepoMode().
  ContextManager.-constructor: '`<constructor>`().'
  ContextManager.handleGlobalMode: handleGlobalMode().
  ContextManager.handleSharedMode: handleSharedMode().
  ContextManager.getRecommendedPath: getRecommendedPath().
  ContextManager.lastRecommendedPath: lastRecommendedPath.
  ContextManager: ''
---
# Module: [`extensions/vscode/src/mcp/contextManager.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts)

## Classes
### `ContextManager`
- def: [`extensions/vscode/src/mcp/contextManager.ts:7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L7)
- signature: `class ContextManager`
- members:
  - `<constructor>(service: CgcService, sidebar: SidebarControlPanel)` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L10) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `getRecommendedPath(method)` — [`L87`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L87)
  - `handleGlobalMode(method)` — [`L32`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L32)
  - `handlePerRepoMode(method)` — [`L50`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L50)
  - `handleSharedMode(method)` — [`L40`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L40)
  - `initializeContext(method)` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L15)
  - `lastRecommendedPath` — [`L8`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/contextManager.ts#L8)
- uses (calls/refs, reference-scoped): [`CgcService`](service.ts.md#CgcService), [`refresh`](../views/controlPanel.ts.md#SidebarControlPanel.refresh), [`switchContext`](service.ts.md#CgcService.switchContext), [`SidebarControlPanel`](../views/controlPanel.ts.md#SidebarControlPanel)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

