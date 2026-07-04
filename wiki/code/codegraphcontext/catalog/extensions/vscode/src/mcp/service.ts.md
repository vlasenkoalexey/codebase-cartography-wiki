---
title: 'Module: extensions/vscode/src/mcp/service.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/mcp/service.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/mcp/`service.ts`/CgcService#
symbols:
  CgcService.getRepoStats: getRepoStats().
  CgcService.getComplexityHotspots: getComplexityHotspots().
  CgcService: ''
  CgcService.findCallers: findCallers().
  CgcService.getRepoPathOverride: getRepoPathOverride().
  CgcService.listRepositories: listRepositories().
  CgcService.findCallees: findCallees().
  CgcService.findDeadCode: findDeadCode().
  CgcService.listCallees: listCallees().
  CgcService.findClassHierarchy: findClassHierarchy().
  CgcService.variableImpactRadius: variableImpactRadius().
  CgcService.findCallChain: findCallChain().
  CgcService.findImporters: findImporters().
  CgcService.findModuleDeps: findModuleDeps().
  CgcService.findFunctionsByDecorator: findFunctionsByDecorator().
  CgcService.switchContext: switchContext().
  CgcService.checkJobStatus: checkJobStatus().
  CgcService.findCode: findCode().
  CgcService.listFunctions: listFunctions().
  CgcService.getComplexity: getComplexity().
  CgcService.discoverContexts: discoverContexts().
  CgcService.runCypher: runCypher().
  CgcService.indexWorkspace: indexWorkspace().
  CgcService.searchBundles: searchBundles().
  CgcService.listClasses: listClasses().
  CgcService.listImports: listImports().
  CgcService.watchWorkspace: watchWorkspace().
  CgcService.-constructor: '`<constructor>`().'
  CgcService.listWatches: listWatches().
  CgcService.generateReport: generateReport().
  CgcService.loadBundle: loadBundle().
---
# Module: [`extensions/vscode/src/mcp/service.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts)

## Classes
### `CgcService`
- def: [`extensions/vscode/src/mcp/service.ts:14`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L14) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- signature: `class CgcService`
- members:
  - `<constructor>(client: CgcMcpClient)` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L15)
  - `checkJobStatus(method)` — [`L282`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L282)
  - `discoverContexts(method)` — [`L249`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L249)
  - `findCallChain(method)` — [`L122`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L122) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findCallees(method)` — [`L86`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L86) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findCallers(method)` — [`L66`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L66) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findClassHierarchy(method)` — [`L168`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L168) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findCode(method)` — [`L315`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L315) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findDeadCode(method)` — [`L24`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L24) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `findFunctionsByDecorator(method)` — [`L183`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L183)
  - `findImporters(method)` — [`L138`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L138) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `findModuleDeps(method)` — [`L153`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L153) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `generateReport(method)` — [`L369`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L369)
  - `getComplexity(method)` — [`L36`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L36) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `getComplexityHotspots(method)` — [`L45`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L45) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `getRepoPathOverride(method)` — [`L17`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L17) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `getRepoStats(method)` — [`L224`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L224) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `indexWorkspace(method)` — [`L275`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L275) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `listCallees(method)` — [`L105`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L105)
  - `listClasses(method)` — [`L338`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L338)
  - `listFunctions(method)` — [`L330`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L330)
  - `listImports(method)` — [`L348`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L348)
  - `listRepositories(method)` — [`L214`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L214) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `listWatches(method)` — [`L266`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L266)
  - `loadBundle(method)` — [`L309`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L309)
  - `runCypher(method)` — [`L360`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L360) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `searchBundles(method)` — [`L301`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L301)
  - `switchContext(method)` — [`L260`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L260)
  - `variableImpactRadius(method)` — [`L197`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L197) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
  - `watchWorkspace(method)` — [`L271`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/service.ts#L271)
- uses (calls/refs, reference-scoped): [`callTool`](client.ts.md#CgcMcpClient.callTool), [`CgcMcpClient`](client.ts.md#CgcMcpClient), [`RepoStats`](../types/cgc.ts.md#RepoStats), [`ComplexityEntry`](../types/cgc.ts.md#ComplexityEntry), [`DeadCodeEntry`](../types/cgc.ts.md#DeadCodeEntry), [`IndexedRepository`](../types/cgc.ts.md#IndexedRepository), [`status`](../types/cgc.ts.md#JobStatus.status), [`DiscoveredContext`](../types/cgc.ts.md#DiscoveredContext), [`cyclomatic_complexity`](../types/cgc.ts.md#ComplexityEntry.cyclomatic_complexity), [`CalleeEntry`](../types/cgc.ts.md#CalleeEntry), [`CallerEntry`](../types/cgc.ts.md#CallerEntry), [`JobStatus`](../types/cgc.ts.md#JobStatus), [`function_name`](../types/cgc.ts.md#ComplexityEntry.function_name), [`path`](../types/cgc.ts.md#IndexedRepository.path), [`repo_name`](../types/cgc.ts.md#IndexedRepository.repo_name), [`class_count`](../types/cgc.ts.md#RepoStats.class_count), [`complexity`](../types/cgc.ts.md#ComplexityEntry.complexity), [`file_count`](../types/cgc.ts.md#RepoStats.file_count), [`function_count`](../types/cgc.ts.md#RepoStats.function_count), [`path`](../types/cgc.ts.md#ComplexityEntry.path), [`total_classes`](../types/cgc.ts.md#RepoStats.total_classes), [`total_files`](../types/cgc.ts.md#RepoStats.total_files), [`total_functions`](../types/cgc.ts.md#RepoStats.total_functions), [`file_count`](../types/cgc.ts.md#IndexedRepository.file_count), [`line_number`](../types/cgc.ts.md#ComplexityEntry.line_number), [`module_count`](../types/cgc.ts.md#RepoStats.module_count)  (1 test-only)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts), [`render`](../views/controlPanel.ts.md#SidebarControlPanel.render), [`runSmartQuery`](../views/controlPanel.ts.md#SidebarControlPanel.runSmartQuery), [`refresh`](../webview/dashboardPanel.ts.md#DashboardPanel.refresh), [`show`](../webview/dashboardPanel.ts.md#DashboardPanel.show), [`handleMessage`](../views/controlPanel.ts.md#SidebarControlPanel.handleMessage), [`startPolling`](jobPoller.ts.md#JobPoller.startPolling), [`controlPanel.ts`](../views/controlPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-views-controlPanel.ts), [`_fetchAll`](../providers/editorProviders.ts.md#CgcCodeLensProvider._fetchAll), [`dashboardPanel.ts`](../webview/dashboardPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-webview-dashboardPanel.ts), [`refreshForDocument`](../providers/editorProviders.ts.md#CgcDeadCodeDiagnostics.refreshForDocument), [`<constructor>`](../views/controlPanel.ts.md#SidebarControlPanel.-constructor), [`<constructor>`](../webview/dashboardPanel.ts.md#DashboardPanel.-constructor), [`_refreshData`](../webview/callGraphPanel.ts.md#CallGraphPanel._refreshData), [`contextManager.ts`](contextManager.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-contextManager.ts), [`editorProviders.ts`](../providers/editorProviders.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-providers-editorProviders.ts), [`jobPoller.ts`](jobPoller.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-jobPoller.ts), [`getChildren`](../views/explorerViews.ts.md#BundlesTreeProvider.getChildren), [`provideHover`](../providers/editorProviders.ts.md#CgcHoverProvider.provideHover), [`handlePerRepoMode`](contextManager.ts.md#ContextManager.handlePerRepoMode), [`<constructor>`](contextManager.ts.md#ContextManager.-constructor), [`callGraphPanel.ts`](../webview/callGraphPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-webview-callGraphPanel.ts), [`explorerViews.ts`](../views/explorerViews.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-views-explorerViews.ts), [`handleGlobalMode`](contextManager.ts.md#ContextManager.handleGlobalMode), [`handleSharedMode`](contextManager.ts.md#ContextManager.handleSharedMode), [`<constructor>`](jobPoller.ts.md#JobPoller.-constructor), [`<constructor>`](../providers/editorProviders.ts.md#CgcCodeLensProvider.-constructor), [`<constructor>`](../providers/editorProviders.ts.md#CgcDeadCodeDiagnostics.-constructor), [`<constructor>`](../providers/editorProviders.ts.md#CgcHoverProvider.-constructor), [`<constructor>`](../views/explorerViews.ts.md#BundlesTreeProvider.-constructor), [`<constructor>`](../webview/callGraphPanel.ts.md#CallGraphPanel.-constructor)

