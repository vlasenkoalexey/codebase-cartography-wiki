---
title: 'Module: extensions/vscode/src/webview/dashboardTemplate.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/webview/dashboardTemplate.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/webview/`dashboardTemplate.ts`/
symbols:
  renderDashboardHtml: renderDashboardHtml().
  DashboardPayload.typeLiteral0.repos: DashboardPayload#typeLiteral0:repos.
  DashboardPayload.typeLiteral0.hotspots: DashboardPayload#typeLiteral0:hotspots.
  DashboardPayload.typeLiteral0.selectedRepo: DashboardPayload#typeLiteral0:selectedRepo.
  escapeHtml: escapeHtml().
  DashboardPayload: DashboardPayload#
---
# Module: [`extensions/vscode/src/webview/dashboardTemplate.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts)

## Classes
### `DashboardPayload`
- def: [`extensions/vscode/src/webview/dashboardTemplate.ts:3`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L3)
- signature: `type DashboardPayload`
- members:
  - `hotspots` — [`L5`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L5)
  - `repos` — [`L4`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L4) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `selectedRepo` — [`L6`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L6)
- uses (calls/refs, reference-scoped): [`ComplexityEntry`](../types/cgc.ts.md#ComplexityEntry), [`IndexedRepository`](../types/cgc.ts.md#IndexedRepository)
- used by: [`refresh`](dashboardPanel.ts.md#DashboardPanel.refresh), [`renderDashboardHtml`](dashboardTemplate.ts.md#renderDashboardHtml)  (1 test-only)

## Functions
- `escapeHtml(v: string)` — [`L102`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L102)
- `renderDashboardHtml(payload: DashboardPayload)` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/webview/dashboardTemplate.ts#L9)

