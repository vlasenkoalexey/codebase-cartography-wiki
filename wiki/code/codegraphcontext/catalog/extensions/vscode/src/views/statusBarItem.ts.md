---
title: 'Module: extensions/vscode/src/views/statusBarItem.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/views/statusBarItem.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/views/`statusBarItem.ts`/
symbols:
  CgcStatusBarItem._subscribeEvents: CgcStatusBarItem#_subscribeEvents().
  CgcStatusBarItem.item: CgcStatusBarItem#item.
  CgcStatusBarItem.-constructor: CgcStatusBarItem#`<constructor>`().
  CgcStatusBarItem._startSpin: CgcStatusBarItem#_startSpin().
  CgcStatusBarItem._render: CgcStatusBarItem#_render().
  CgcStatusBarItem.state: CgcStatusBarItem#state.
  CgcStatusBarItem.indexingCount: CgcStatusBarItem#indexingCount.
  CgcStatusBarItem._stopSpin: CgcStatusBarItem#_stopSpin().
  CgcStatusBarItem.notifyOnline: CgcStatusBarItem#notifyOnline().
  CgcStatusBarItem.notifyOffline: CgcStatusBarItem#notifyOffline().
  CgcStatusBarItem.dispose: CgcStatusBarItem#dispose().
  CgcStatusBarItem.spinTimer: CgcStatusBarItem#spinTimer.
  CgcStatusBarItem.spinFrame: CgcStatusBarItem#spinFrame.
  StatusState: StatusState#
  DEFAULT_STATUS_BAR_PRIORITY: DEFAULT_STATUS_BAR_PRIORITY.
  CgcStatusBarItem: CgcStatusBarItem#
---
# Module: [`extensions/vscode/src/views/statusBarItem.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts)

## Classes
### `CgcStatusBarItem`
- def: [`extensions/vscode/src/views/statusBarItem.ts:27`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L27)
- doc: Persistent status bar item showing CGC health.
- signature: `class CgcStatusBarItem`
- members:
  - `<constructor>(client: CgcMcpClient)` — [`L34`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L34) — Persistent status bar item showing CGC health.
  - `dispose(method)` — [`L150`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L150)
  - `notifyOffline(method)` — [`L146`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L146) — Called by extension.ts if MCP start fails or process dies.
  - `notifyOnline(method)` — [`L141`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L141) — Called by extension.ts after MCP start succeeds.
  - `indexingCount` — [`L30`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L30)
  - `item` — [`L28`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L28)
  - `spinFrame` — [`L31`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L31)
  - `spinTimer` — [`L32`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L32)
  - `state` — [`L29`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L29)
- protocol/private: `_render`[`L120`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L120), `_startSpin`[`L103`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L103), `_stopSpin`[`L113`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L113), `_subscribeEvents`[`L59`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L59)
- uses (calls/refs, reference-scoped): [`cgcEvents`](../mcp/eventBus.ts.md#cgcEvents), [`emit`](../mcp/eventBus.ts.md#CgcEventBus.emit), [`on`](../mcp/eventBus.ts.md#CgcEventBus.on), [`CgcMcpClient`](../mcp/client.ts.md#CgcMcpClient), [`cgc.ts`](../types/cgc.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-types-cgc.ts), [`CgcEvent`](../types/cgc.ts.md#CgcEvent), [`payload`](../types/cgc.ts.md#CgcEvent.payload), [`StatusState`](statusBarItem.ts.md#StatusState), [`DEFAULT_STATUS_BAR_PRIORITY`](statusBarItem.ts.md#DEFAULT_STATUS_BAR_PRIORITY)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

### `StatusState`
- def: [`extensions/vscode/src/views/statusBarItem.ts:5`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L5)
- signature: `type StatusState`
- used by: [`state`](statusBarItem.ts.md#CgcStatusBarItem.state)

## Module values
- `DEFAULT_STATUS_BAR_PRIORITY` — [`L17`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/statusBarItem.ts#L17) — Default priority for the CGC status bar item.

