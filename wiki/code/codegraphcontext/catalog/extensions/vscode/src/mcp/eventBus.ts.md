---
title: 'Module: extensions/vscode/src/mcp/eventBus.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/mcp/eventBus.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/mcp/`eventBus.ts`/
symbols:
  cgcEvents: cgcEvents.
  CgcEventBus.emit: CgcEventBus#emit().
  CgcEventBus.on: CgcEventBus#on().
  CgcEventBus.listeners: CgcEventBus#listeners.
  CgcEventBus.off: CgcEventBus#off().
  Listener: Listener#
  CgcEventBus.dispose: CgcEventBus#dispose().
  CgcEventBus: CgcEventBus#
---
# Module: [`extensions/vscode/src/mcp/eventBus.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts)

## Classes
### `CgcEventBus`
- def: [`extensions/vscode/src/mcp/eventBus.ts:9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L9)
- doc: Lightweight pub/sub event bus for CGC extension events.
- signature: `class CgcEventBus`
- members:
  - `dispose(method)` — [`L35`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L35)
  - `emit(method)` — [`L24`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L24) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `off(method)` — [`L20`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L20) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `on(method)` — [`L12`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L12) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `listeners` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L10) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
- uses (calls/refs, reference-scoped): [`CgcEventType`](../types/cgc.ts.md#CgcEventType), [`Listener`](eventBus.ts.md#Listener), [`CgcEvent`](../types/cgc.ts.md#CgcEvent), [`payload`](../types/cgc.ts.md#CgcEvent.payload), [`type`](../types/cgc.ts.md#CgcEvent.type)
- used by: [`activate`](../extension.ts.md#activate), [`show`](../webview/dashboardPanel.ts.md#DashboardPanel.show), [`_subscribeEvents`](../views/statusBarItem.ts.md#CgcStatusBarItem._subscribeEvents), [`handleMessage`](../views/controlPanel.ts.md#SidebarControlPanel.handleMessage), [`startPolling`](jobPoller.ts.md#JobPoller.startPolling), [`<constructor>`](../views/controlPanel.ts.md#SidebarControlPanel.-constructor), [`<constructor>`](../webview/dashboardPanel.ts.md#DashboardPanel.-constructor), [`eventBus.ts`](eventBus.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-eventBus.ts), [`notifyOffline`](../views/statusBarItem.ts.md#CgcStatusBarItem.notifyOffline), [`notifyOnline`](../views/statusBarItem.ts.md#CgcStatusBarItem.notifyOnline)

### `Listener`
- def: [`extensions/vscode/src/mcp/eventBus.ts:3`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L3)
- signature: `type Listener`
- uses (calls/refs, reference-scoped): [`CgcEvent`](../types/cgc.ts.md#CgcEvent)
- used by: [`on`](eventBus.ts.md#CgcEventBus.on), [`listeners`](eventBus.ts.md#CgcEventBus.listeners), [`off`](eventBus.ts.md#CgcEventBus.off)

## Module values
- `cgcEvents` — [`L41`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/eventBus.ts#L41) — Singleton event bus shared across the extension.

