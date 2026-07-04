---
title: 'Module: extensions/vscode/src/views/explorerViews.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/views/explorerViews.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/views/`explorerViews.ts`/
symbols:
  BundlesTreeProvider.getChildren: BundlesTreeProvider#getChildren().
  BundlesTreeProvider.emitter: BundlesTreeProvider#emitter.
  SimpleItem: SimpleItem#
  BundlesTreeProvider: BundlesTreeProvider#
  BundlesTreeProvider.-constructor: BundlesTreeProvider#`<constructor>`().
  SimpleItem.-constructor: SimpleItem#`<constructor>`().
  BundlesTreeProvider.onDidChangeTreeData: BundlesTreeProvider#onDidChangeTreeData.
  BundlesTreeProvider.refresh: BundlesTreeProvider#refresh().
  BundlesTreeProvider.getTreeItem: BundlesTreeProvider#getTreeItem().
---
# Module: [`extensions/vscode/src/views/explorerViews.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts)

## Classes
### `BundlesTreeProvider`
- def: [`extensions/vscode/src/views/explorerViews.ts:10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L10)
- signature: `class BundlesTreeProvider`
- members:
  - `<constructor>(service: CgcService)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L14) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `getChildren(method)` — [`L24`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L24)
  - `getTreeItem(method)` — [`L20`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L20)
  - `refresh(method)` — [`L16`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L16)
  - `emitter` — [`L11`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L11)
  - `onDidChangeTreeData` — [`L12`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L12)
- uses (calls/refs, reference-scoped): [`CgcService`](../mcp/service.ts.md#CgcService), [`searchBundles`](../mcp/service.ts.md#CgcService.searchBundles), [`SimpleItem`](explorerViews.ts.md#SimpleItem), [`<constructor>`](explorerViews.ts.md#SimpleItem.-constructor)  (1 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

### `SimpleItem`
- def: [`extensions/vscode/src/views/explorerViews.ts:4`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L4)
- signature: `class SimpleItem`
- members:
  - `<constructor>(label: string, collapsibleState?: vscode.TreeItemCollapsibleState)` — [`L5`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/explorerViews.ts#L5)
- used by: [`getChildren`](explorerViews.ts.md#BundlesTreeProvider.getChildren), [`emitter`](explorerViews.ts.md#BundlesTreeProvider.emitter), [`BundlesTreeProvider`](explorerViews.ts.md#BundlesTreeProvider), [`getTreeItem`](explorerViews.ts.md#BundlesTreeProvider.getTreeItem)

