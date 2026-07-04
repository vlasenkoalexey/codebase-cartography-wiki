---
title: 'Module: packages/vscode-extension/src/commands/syncCommand.ts'
type: catalog
provenance: extracted
module: packages/vscode-extension/src/commands/syncCommand.ts
status: fresh
symbol_base: scip-typescript npm semanticcodesearch 0.1.11 src/commands/`syncCommand.ts`/SyncCommand#
symbols:
  SyncCommand.executeSilent: executeSilent().
  SyncCommand.execute: execute().
  SyncCommand.isSyncing: isSyncing.
  SyncCommand.context: context.
  SyncCommand: ''
  SyncCommand.-constructor: '`<constructor>`().'
  SyncCommand.updateContext: updateContext().
  SyncCommand.startAutoSync: startAutoSync().
  SyncCommand.getIsSyncing: getIsSyncing().
---
# Module: [`packages/vscode-extension/src/commands/syncCommand.ts`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts)

## Classes
### `SyncCommand`
- def: [`packages/vscode-extension/src/commands/syncCommand.ts:5`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L5)
- signature: `class SyncCommand`
- members:
  - `<constructor>(context: Context)` — [`L9`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L9)
  - `execute(method)` — [`L23`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L23) — Sync the current workspace folder - check for changes and update index
  - `executeSilent(method)` — [`L127`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L127) — Silent sync - runs without progress notifications, used for auto-sync
  - `getIsSyncing(method)` — [`L178`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L178) — Check if sync is currently in progress
  - `startAutoSync(method)` — [`L102`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L102) — Auto-sync functionality - periodically check for changes
  - `updateContext(method)` — [`L16`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L16) — Update the Context instance (used when configuration changes)
  - `context` — [`L6`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L6)
  - `isSyncing` — [`L7`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/syncCommand.ts#L7)
- uses (calls/refs, reference-scoped): [`Context`](../../../core/src/context.ts.md#Context), [`reindexByChange`](../../../core/src/context.ts.md#Context.reindexByChange)
- used by: [`reloadContextConfiguration`](../extension.ts.md#reloadContextConfiguration), [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`semanticSearchProvider.ts`](../webview/semanticSearchProvider.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-webview-semanticSearchProvider.ts), [`<constructor>`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.-constructor), [`updateCommands`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.updateCommands), [`setupAutoSync`](../extension.ts.md#setupAutoSync), [`syncCommand`](../extension.ts.md#syncCommand), [`runInitialSync`](../extension.ts.md#runInitialSync), [`syncCommand`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.syncCommand)

