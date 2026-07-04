---
title: 'Module: packages/vscode-extension/src/webview/semanticSearchProvider.ts'
type: catalog
provenance: extracted
module: packages/vscode-extension/src/webview/semanticSearchProvider.ts
status: fresh
symbol_base: scip-typescript npm semanticcodesearch 0.1.11 src/webview/`semanticSearchProvider.ts`/SemanticSearchViewProvider#
symbols:
  SemanticSearchViewProvider.resolveWebviewView: resolveWebviewView().
  SemanticSearchViewProvider.-constructor: '`<constructor>`().'
  SemanticSearchViewProvider.sendCurrentConfig: sendCurrentConfig().
  SemanticSearchViewProvider.updateCommands: updateCommands().
  SemanticSearchViewProvider.saveConfig: saveConfig().
  SemanticSearchViewProvider.configManager: configManager.
  SemanticSearchViewProvider.checkIndexStatusAndUpdateWebview: checkIndexStatusAndUpdateWebview().
  SemanticSearchViewProvider.searchCommand: searchCommand.
  SemanticSearchViewProvider.testEmbedding: testEmbedding().
  SemanticSearchViewProvider.indexCommand: indexCommand.
  SemanticSearchViewProvider.syncCommand: syncCommand.
  SemanticSearchViewProvider: ''
  SemanticSearchViewProvider.viewType: viewType.
  SemanticSearchViewProvider.convertSearchResultsToWebviewFormat: convertSearchResultsToWebviewFormat().
---
# Module: [`packages/vscode-extension/src/webview/semanticSearchProvider.ts`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts)

## Classes
### `SemanticSearchViewProvider`
- def: [`packages/vscode-extension/src/webview/semanticSearchProvider.ts:9`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L9)
- signature: `class SemanticSearchViewProvider`
- members:
  - `<constructor>(_extensionUri: vscode.Uri, searchCommand: SearchCommand, indexCommand: IndexCommand, syncCommand: SyncCommand, configManager: ConfigManager)` — [`L16`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L16)
  - `checkIndexStatusAndUpdateWebview(method)` — [`L199`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L199) — Check index status and update webview accordingly
  - `convertSearchResultsToWebviewFormat(method)` — [`L165`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L165) — Convert SemanticSearchResult[] from core to webview format
  - `resolveWebviewView(method)` — [`L32`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L32)
  - `saveConfig(method)` — [`L241`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L241) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
  - `sendCurrentConfig(method)` — [`L226`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L226)
  - `testEmbedding(method)` — [`L282`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L282)
  - `updateCommands(method)` — [`L26`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L26) — Update the command instances (used when configuration changes)
  - `configManager` — [`L14`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L14)
  - `indexCommand` — [`L12`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L12)
  - `searchCommand` — [`L11`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L11)
  - `syncCommand` — [`L13`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L13)
  - `viewType` — [`L10`](../../../../../../../../raw/code/claude-context/packages/vscode-extension/src/webview/semanticSearchProvider.ts#L10)
- uses (calls/refs, reference-scoped): [`execute`](../commands/indexCommand.ts.md#IndexCommand.execute), [`saveSplitterConfig`](../config/configManager.ts.md#ConfigManager.saveSplitterConfig), [`ConfigManager`](../config/configManager.ts.md#ConfigManager), [`getSplitterConfig`](../config/configManager.ts.md#ConfigManager.getSplitterConfig), [`EmbeddingProviderConfig`](../config/configManager.ts.md#EmbeddingProviderConfig), [`saveEmbeddingProviderConfig`](../config/configManager.ts.md#ConfigManager.saveEmbeddingProviderConfig), [`saveMilvusConfig`](../config/configManager.ts.md#ConfigManager.saveMilvusConfig), [`getEmbeddingProviderConfig`](../config/configManager.ts.md#ConfigManager.getEmbeddingProviderConfig), [`executeForWebview`](../commands/searchCommand.ts.md#SearchCommand.executeForWebview), [`getMilvusConfig`](../config/configManager.ts.md#ConfigManager.getMilvusConfig), [`createEmbeddingInstance`](../config/configManager.ts.md#ConfigManager.createEmbeddingInstance), [`IndexCommand`](../commands/indexCommand.ts.md#IndexCommand), [`SearchCommand`](../commands/searchCommand.ts.md#SearchCommand), [`SyncCommand`](../commands/syncCommand.ts.md#SyncCommand), [`hasIndex`](../commands/searchCommand.ts.md#SearchCommand.hasIndex), [`getHtmlContent`](webviewHelper.ts.md#WebviewHelper.getHtmlContent), [`getSupportedProviders`](../config/configManager.ts.md#ConfigManager.getSupportedProviders), [`WebviewHelper`](webviewHelper.ts.md#WebviewHelper)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`semanticSearchProvider`](../extension.ts.md#semanticSearchProvider)

