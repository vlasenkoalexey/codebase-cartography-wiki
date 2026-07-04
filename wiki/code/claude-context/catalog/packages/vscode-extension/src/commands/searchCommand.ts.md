---
title: 'Module: packages/vscode-extension/src/commands/searchCommand.ts'
type: catalog
provenance: extracted
module: packages/vscode-extension/src/commands/searchCommand.ts
status: fresh
symbol_base: scip-typescript npm semanticcodesearch 0.1.11 src/commands/`searchCommand.ts`/SearchCommand#
symbols:
  SearchCommand.execute: execute().
  SearchCommand.executeForWebview: executeForWebview().
  SearchCommand.context: context.
  SearchCommand.openResult: openResult().
  SearchCommand.generateQuickPickItems: generateQuickPickItems().
  SearchCommand: ''
  SearchCommand.-constructor: '`<constructor>`().'
  SearchCommand.updateContext: updateContext().
  SearchCommand.hasIndex: hasIndex().
---
# Module: [`packages/vscode-extension/src/commands/searchCommand.ts`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts)

## Classes
### `SearchCommand`
- def: [`packages/vscode-extension/src/commands/searchCommand.ts:5`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L5)
- signature: `class SearchCommand`
- members:
  - `<constructor>(context: Context)` — [`L8`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L8)
  - `execute(method)` — [`L19`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L19) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `executeForWebview(method)` — [`L169`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L169) — Execute search for webview (without UI prompts)
  - `generateQuickPickItems(method)` — [`L221`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L221) — Generate quick pick items for VS Code
  - `hasIndex(method)` — [`L209`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L209) — Check if index exists for the given codebase path
  - `openResult(method)` — [`L135`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L135)
  - `updateContext(method)` — [`L15`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L15) — Update the Context instance (used when configuration changes)
  - `context` — [`L6`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/commands/searchCommand.ts#L6)
- uses (calls/refs, reference-scoped): [`semanticSearch`](../../../core/src/context.ts.md#Context.semanticSearch), [`Context`](../../../core/src/context.ts.md#Context), [`SemanticSearchResult`](../../../core/src/types.ts.md#SemanticSearchResult), [`hasIndex`](../../../core/src/context.ts.md#Context.hasIndex), [`relativePath`](../../../core/src/types.ts.md#SemanticSearchResult.relativePath), [`startLine`](../../../core/src/types.ts.md#SemanticSearchResult.startLine), [`content`](../../../core/src/types.ts.md#SemanticSearchResult.content), [`SearchQuery`](../../../core/src/types.ts.md#SearchQuery), [`limit`](../../../core/src/types.ts.md#SearchQuery.limit), [`term`](../../../core/src/types.ts.md#SearchQuery.term), [`includeContent`](../../../core/src/types.ts.md#SearchQuery.includeContent)
- used by: [`reloadContextConfiguration`](../extension.ts.md#reloadContextConfiguration), [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`semanticSearchProvider.ts`](../webview/semanticSearchProvider.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-webview-semanticSearchProvider.ts), [`resolveWebviewView`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.resolveWebviewView), [`<constructor>`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.-constructor), [`updateCommands`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.updateCommands), [`checkIndexStatusAndUpdateWebview`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.checkIndexStatusAndUpdateWebview), [`searchCommand`](../extension.ts.md#searchCommand), [`searchCommand`](../webview/semanticSearchProvider.ts.md#SemanticSearchViewProvider.searchCommand)

