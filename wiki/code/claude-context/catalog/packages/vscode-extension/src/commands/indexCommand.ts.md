---
title: 'Module: packages/vscode-extension/src/commands/indexCommand.ts'
type: catalog
provenance: extracted
module: packages/vscode-extension/src/commands/indexCommand.ts
status: fresh
symbol_base: scip-typescript npm semanticcodesearch 0.1.11 src/commands/`indexCommand.ts`/IndexCommand#
symbols:
  IndexCommand.execute: execute().
  IndexCommand.context: context.
  IndexCommand: ''
  IndexCommand.-constructor: '`<constructor>`().'
  IndexCommand.updateContext: updateContext().
  IndexCommand.clearIndex: clearIndex().
---
# Module: [`packages/vscode-extension/src/commands/indexCommand.ts`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts)

## Classes
### `IndexCommand`
- def: [`packages/vscode-extension/src/commands/indexCommand.ts:5`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L5)
- signature: `class IndexCommand`
- members:
  - `<constructor>(context: Context)` — [`L8`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L8)
  - `clearIndex(method)` — [`L138`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L138)
  - `execute(method)` — [`L19`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L19) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `updateContext(method)` — [`L15`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L15) — Update the Context instance (used when configuration changes)
  - `context` — [`L6`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/indexCommand.ts#L6)
- uses (calls/refs, reference-scoped): [`getCollectionName`](../../../core/src/context.ts.md#Context.getCollectionName), [`index.ts`](../../../core/src/index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-index.ts), [`Context`](../../../core/src/context.ts.md#Context), [`indexCodebase`](../../../core/src/context.ts.md#Context.indexCodebase), [`clearIndex`](../../../core/src/context.ts.md#Context.clearIndex), [`initialize`](../../../core/src/sync/synchronizer.ts.md#FileSynchronizer.initialize), [`FileSynchronizer`](../../../core/src/sync/synchronizer.ts.md#FileSynchronizer), [`setSynchronizer`](../../../core/src/context.ts.md#Context.setSynchronizer), [`getSupportedExtensions`](../../../core/src/context.ts.md#Context.getSupportedExtensions), [`getIgnorePatterns`](../../../core/src/context.ts.md#Context.getIgnorePatterns), [`getPreparedCollection`](../../../core/src/context.ts.md#Context.getPreparedCollection)
- used by: [`reloadContextConfiguration`](../extension.ts.md#reloadContextConfiguration), [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`semanticSearchProvider.ts`](../webview/semanticSearchProvider.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-webview-semanticSearchProvider.ts), [`resolveWebviewView`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.resolveWebviewView), [`<constructor>`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.-constructor), [`updateCommands`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.updateCommands), [`indexCommand`](../extension.ts.md#indexCommand), [`indexCommand`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.indexCommand)

