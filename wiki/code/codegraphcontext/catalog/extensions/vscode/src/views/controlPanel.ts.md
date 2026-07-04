---
title: 'Module: extensions/vscode/src/views/controlPanel.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/views/controlPanel.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/views/`controlPanel.ts`/
symbols:
  SidebarControlPanel.buildHtml.data-typeLiteral60.discoveredContexts.Array.typeLiteral170.path: SidebarControlPanel#buildHtml().(data)typeLiteral60:discoveredContexts.Array:typeLiteral170:path.
  SidebarControlPanel.render: SidebarControlPanel#render().
  SidebarControlPanel.runSmartQuery: SidebarControlPanel#runSmartQuery().
  SidebarControlPanel.handleMessage: SidebarControlPanel#handleMessage().
  SidebarControlPanel.-constructor: SidebarControlPanel#`<constructor>`().
  SidebarControlPanel.refresh: SidebarControlPanel#refresh().
  SidebarControlPanel.resolveWebviewView: SidebarControlPanel#resolveWebviewView().
  esc: esc().
  SidebarControlPanel.saveConfig: SidebarControlPanel#saveConfig().
  SidebarControlPanel.view: SidebarControlPanel#view.
  SidebarControlPanel.buildHtml.data-typeLiteral60.repos: SidebarControlPanel#buildHtml().(data)typeLiteral60:repos.
  SidebarControlPanel.buildHtml.data-typeLiteral60.hotspots: SidebarControlPanel#buildHtml().(data)typeLiteral60:hotspots.
  SidebarControlPanel.buildHtml.data-typeLiteral60.stats: SidebarControlPanel#buildHtml().(data)typeLiteral60:stats.
  SidebarControlPanel.buildHtml.data-typeLiteral60.discoveredContexts: SidebarControlPanel#buildHtml().(data)typeLiteral60:discoveredContexts.
  SidebarControlPanel: SidebarControlPanel#
  SidebarControlPanel.eventDisposables: SidebarControlPanel#eventDisposables.
  SidebarControlPanel.launchVizServer: SidebarControlPanel#launchVizServer().
  SidebarControlPanel.buildHtml.data-typeLiteral60.watches: SidebarControlPanel#buildHtml().(data)typeLiteral60:watches.
  SidebarControlPanel.buildHtml.data-typeLiteral60.selectedRepo: SidebarControlPanel#buildHtml().(data)typeLiteral60:selectedRepo.
  SidebarControlPanel.buildHtml.data-typeLiteral60.contextMode: SidebarControlPanel#buildHtml().(data)typeLiteral60:contextMode.
  SidebarControlPanel.buildHtml.data-typeLiteral60.workspacePath: SidebarControlPanel#buildHtml().(data)typeLiteral60:workspacePath.
  SidebarControlPanel.buildHtml.data-typeLiteral60.cfg: SidebarControlPanel#buildHtml().(data)typeLiteral60:cfg.
  SidebarControlPanel.viewType: SidebarControlPanel#viewType.
  SidebarControlPanel.buildHtml: SidebarControlPanel#buildHtml().
  SidebarControlPanel.buildHtml.data-typeLiteral60.repos.Array.typeLiteral168.repo_name: SidebarControlPanel#buildHtml().(data)typeLiteral60:repos.Array:typeLiteral168:repo_name.
  SidebarControlPanel.buildHtml.data-typeLiteral60.repos.Array.typeLiteral168.path: SidebarControlPanel#buildHtml().(data)typeLiteral60:repos.Array:typeLiteral168:path.
  SidebarControlPanel.buildHtml.data-typeLiteral60.hotspots.Array.typeLiteral169.function_name: SidebarControlPanel#buildHtml().(data)typeLiteral60:hotspots.Array:typeLiteral169:function_name.
  SidebarControlPanel.buildHtml.data-typeLiteral60.hotspots.Array.typeLiteral169.cyclomatic_complexity: SidebarControlPanel#buildHtml().(data)typeLiteral60:hotspots.Array:typeLiteral169:cyclomatic_complexity.
  SidebarControlPanel.buildHtml.data-typeLiteral60.hotspots.Array.typeLiteral169.path: SidebarControlPanel#buildHtml().(data)typeLiteral60:hotspots.Array:typeLiteral169:path.
  SidebarControlPanel.buildHtml.data-typeLiteral60.discoveredContexts.Array.typeLiteral170.name: SidebarControlPanel#buildHtml().(data)typeLiteral60:discoveredContexts.Array:typeLiteral170:name.
---
# Module: [`extensions/vscode/src/views/controlPanel.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts)

## Classes
### `SidebarControlPanel`
- def: [`extensions/vscode/src/views/controlPanel.ts:8`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L8)
- signature: `class SidebarControlPanel`
- members:
  - `<constructor>(service: CgcService, client: CgcMcpClient, context: vscode.ExtensionContext)` — [`L13`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L13) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `buildHtml(method)` — [`L326`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L326)
  - `handleMessage(method)` — [`L109`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L109)
  - `launchVizServer(method)` — [`L229`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L229)
  - `refresh(method)` — [`L57`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L57)
  - `render(method)` — [`L62`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L62) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `resolveWebviewView(method)` — [`L39`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L39)
  - `runSmartQuery(method)` — [`L255`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L255) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `saveConfig(method)` — [`L205`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L205) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `cfg` — [`L334`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L334)
  - `contextMode` — [`L332`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L332)
  - `cyclomatic_complexity` — [`L329`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L329)
  - `discoveredContexts` — [`L335`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L335)
  - `eventDisposables` — [`L11`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L11)
  - `function_name` — [`L329`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L329)
  - `hotspots` — [`L329`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L329)
  - `name` — [`L335`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L335)
  - `path` — [`L327`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L327)
  - `path` — [`L329`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L329)
  - `path` — [`L335`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L335)
  - `repo_name` — [`L327`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L327)
  - `repos` — [`L327`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L327)
  - `selectedRepo` — [`L331`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L331)
  - `stats` — [`L330`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L330) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `view` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L10)
  - `viewType` — [`L9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L9)
  - `watches` — [`L328`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L328)
  - `workspacePath` — [`L333`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L333)
- uses (calls/refs, reference-scoped): [`cgcEvents`](../mcp/eventBus.ts.md#cgcEvents), [`emit`](../mcp/eventBus.ts.md#CgcEventBus.emit), [`on`](../mcp/eventBus.ts.md#CgcEventBus.on), [`getRepoStats`](../mcp/service.ts.md#CgcService.getRepoStats), [`ensureStarted`](../mcp/client.ts.md#CgcMcpClient.ensureStarted), [`getComplexityHotspots`](../mcp/service.ts.md#CgcService.getComplexityHotspots), [`CgcService`](../mcp/service.ts.md#CgcService), [`findCallers`](../mcp/service.ts.md#CgcService.findCallers), [`listRepositories`](../mcp/service.ts.md#CgcService.listRepositories), [`CgcMcpClient`](../mcp/client.ts.md#CgcMcpClient), [`esc`](controlPanel.ts.md#esc), [`findClassHierarchy`](../mcp/service.ts.md#CgcService.findClassHierarchy), [`findDeadCode`](../mcp/service.ts.md#CgcService.findDeadCode), [`listCallees`](../mcp/service.ts.md#CgcService.listCallees), [`variableImpactRadius`](../mcp/service.ts.md#CgcService.variableImpactRadius), [`findCallChain`](../mcp/service.ts.md#CgcService.findCallChain), [`findFunctionsByDecorator`](../mcp/service.ts.md#CgcService.findFunctionsByDecorator), [`findImporters`](../mcp/service.ts.md#CgcService.findImporters), [`findModuleDeps`](../mcp/service.ts.md#CgcService.findModuleDeps), [`listFunctions`](../mcp/service.ts.md#CgcService.listFunctions), [`switchContext`](../mcp/service.ts.md#CgcService.switchContext), [`RepoStats`](../types/cgc.ts.md#RepoStats), [`discoverContexts`](../mcp/service.ts.md#CgcService.discoverContexts), [`dispose`](../mcp/client.ts.md#CgcMcpClient.dispose), [`indexWorkspace`](../mcp/service.ts.md#CgcService.indexWorkspace), [`listClasses`](../mcp/service.ts.md#CgcService.listClasses), [`listImports`](../mcp/service.ts.md#CgcService.listImports), [`payload`](../types/cgc.ts.md#CgcEvent.payload), [`listWatches`](../mcp/service.ts.md#CgcService.listWatches), [`class_count`](../types/cgc.ts.md#RepoStats.class_count), [`file_count`](../types/cgc.ts.md#RepoStats.file_count), [`function_count`](../types/cgc.ts.md#RepoStats.function_count), [`total_classes`](../types/cgc.ts.md#RepoStats.total_classes), [`total_files`](../types/cgc.ts.md#RepoStats.total_files), [`total_functions`](../types/cgc.ts.md#RepoStats.total_functions)  (2 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts), [`contextManager.ts`](../mcp/contextManager.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-contextManager.ts), [`handlePerRepoMode`](../mcp/contextManager.ts.md#ContextManager.handlePerRepoMode), [`<constructor>`](../mcp/contextManager.ts.md#ContextManager.-constructor), [`handleGlobalMode`](../mcp/contextManager.ts.md#ContextManager.handleGlobalMode), [`handleSharedMode`](../mcp/contextManager.ts.md#ContextManager.handleSharedMode)

## Functions
- `esc(v: string)` — [`L803`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/views/controlPanel.ts#L803)

