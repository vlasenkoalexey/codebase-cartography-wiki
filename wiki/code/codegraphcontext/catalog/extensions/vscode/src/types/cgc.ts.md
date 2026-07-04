---
title: 'Module: extensions/vscode/src/types/cgc.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/types/cgc.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/types/`cgc.ts`/
symbols:
  RepoStats: RepoStats#
  IndexedRepository: IndexedRepository#
  DeadCodeEntry: DeadCodeEntry#
  ComplexityEntry: ComplexityEntry#
  CgcEventType: CgcEventType#
  JobStatus.status: JobStatus#status.
  CgcMcpToolResponse: CgcMcpToolResponse#
  ComplexityEntry.cyclomatic_complexity: ComplexityEntry#cyclomatic_complexity.
  DiscoveredContext: DiscoveredContext#
  CgcEvent: CgcEvent#
  CgcEvent.payload: CgcEvent#payload.
  CgcEvent.type: CgcEvent#type.
  CgcTool: CgcTool#
  IndexedRepository.repo_name: IndexedRepository#repo_name.
  IndexedRepository.path: IndexedRepository#path.
  DeadCodeEntry.line_number: DeadCodeEntry#line_number.
  CallerEntry: CallerEntry#
  CalleeEntry: CalleeEntry#
  ComplexityEntry.function_name: ComplexityEntry#function_name.
  JobStatus: JobStatus#
  DeadCodeEntry.function_name: DeadCodeEntry#function_name.
  DeadCodeEntry.path: DeadCodeEntry#path.
  DeadCodeEntry.class_name: DeadCodeEntry#class_name.
  ComplexityEntry.path: ComplexityEntry#path.
  ComplexityEntry.complexity: ComplexityEntry#complexity.
  RepoStats.file_count: RepoStats#file_count.
  RepoStats.function_count: RepoStats#function_count.
  RepoStats.class_count: RepoStats#class_count.
  RepoStats.total_files: RepoStats#total_files.
  RepoStats.total_functions: RepoStats#total_functions.
  RepoStats.total_classes: RepoStats#total_classes.
  JobStatus.message: JobStatus#message.
  DiscoveredContext.path: DiscoveredContext#path.
  MpcToolContent: MpcToolContent#
  CgcMcpToolResponse.content: CgcMcpToolResponse#content.
  IndexedRepository.file_count: IndexedRepository#file_count.
  CallerEntry.caller_name: CallerEntry#caller_name.
  CallerEntry.caller_file_path: CallerEntry#caller_file_path.
  CallerEntry.caller_line_number: CallerEntry#caller_line_number.
  CallerEntry.call_line_number: CallerEntry#call_line_number.
  ComplexityEntry.line_number: ComplexityEntry#line_number.
  RepoStats.module_count: RepoStats#module_count.
  JobStatus.progress: JobStatus#progress.
  JobStatus.error: JobStatus#error.
  DiscoveredContext.name: DiscoveredContext#name.
  MpcToolContent.type: MpcToolContent#type.
  MpcToolContent.text: MpcToolContent#text.
  CgcTool.name: CgcTool#name.
  CgcTool.description: CgcTool#description.
  CgcTool.inputSchema: CgcTool#inputSchema.
  CalleeEntry.called_name: CalleeEntry#called_name.
  CalleeEntry.called_file_path: CalleeEntry#called_file_path.
  CalleeEntry.called_line_number: CalleeEntry#called_line_number.
  RepoStats.repo_path: RepoStats#repo_path.
  RepoStats.total_modules: RepoStats#total_modules.
  JobStatus.job_id: JobStatus#job_id.
---
# Module: [`extensions/vscode/src/types/cgc.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts)

## Classes
### `CalleeEntry`
- def: [`extensions/vscode/src/types/cgc.ts:36`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L36)
- signature: `interface CalleeEntry`
- members:
  - `called_file_path` — [`L38`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L38)
  - `called_line_number` — [`L39`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L39)
  - `called_name` — [`L37`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L37)
- used by: [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`findCallees`](../mcp/service.ts.md#CgcService.findCallees)

### `CallerEntry`
- def: [`extensions/vscode/src/types/cgc.ts:29`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L29) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- signature: `interface CallerEntry`
- members:
  - `call_line_number` — [`L33`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L33)
  - `caller_file_path` — [`L31`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L31)
  - `caller_line_number` — [`L32`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L32)
  - `caller_name` — [`L30`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L30)
- used by: [`activate`](../extension.ts.md#activate), [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`findCallers`](../mcp/service.ts.md#CgcService.findCallers)

### `CgcEvent`
- def: [`extensions/vscode/src/types/cgc.ts:87`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L87)
- signature: `interface CgcEvent`
- members:
  - `payload` — [`L89`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L89)
  - `type` — [`L88`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L88) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
- uses (calls/refs, reference-scoped): [`CgcEventType`](cgc.ts.md#CgcEventType)
- used by: [`emit`](../mcp/eventBus.ts.md#CgcEventBus.emit), [`_subscribeEvents`](../views/statusBarItem.ts.md#CgcStatusBarItem._subscribeEvents), [`<constructor>`](../views/controlPanel.ts.md#SidebarControlPanel.-constructor), [`eventBus.ts`](../mcp/eventBus.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-eventBus.ts), [`Listener`](../mcp/eventBus.ts.md#Listener)

### `CgcEventType`
- def: [`extensions/vscode/src/types/cgc.ts:76`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L76) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
- signature: `type CgcEventType`
- used by: [`emit`](../mcp/eventBus.ts.md#CgcEventBus.emit), [`on`](../mcp/eventBus.ts.md#CgcEventBus.on), [`eventBus.ts`](../mcp/eventBus.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-eventBus.ts), [`listeners`](../mcp/eventBus.ts.md#CgcEventBus.listeners), [`off`](../mcp/eventBus.ts.md#CgcEventBus.off), [`type`](cgc.ts.md#CgcEvent.type)

### `CgcMcpToolResponse`
- def: [`extensions/vscode/src/types/cgc.ts:6`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L6) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- signature: `interface CgcMcpToolResponse`
- members:
  - `content` — [`L7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L7) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- uses (calls/refs, reference-scoped): [`MpcToolContent`](cgc.ts.md#MpcToolContent)
- used by: [`callTool`](../mcp/client.ts.md#CgcMcpClient.callTool), [`client.ts`](../mcp/client.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-client.ts)

### `CgcTool`
- def: [`extensions/vscode/src/types/cgc.ts:10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L10)
- signature: `interface CgcTool`
- members:
  - `description` — [`L12`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L12)
  - `inputSchema` — [`L13`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L13)
  - `name` — [`L11`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L11)
- used by: [`client.ts`](../mcp/client.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-client.ts), [`listTools`](../mcp/client.ts.md#CgcMcpClient.listTools)

### `ComplexityEntry`
- def: [`extensions/vscode/src/types/cgc.ts:42`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L42) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- signature: `interface ComplexityEntry`
- members:
  - `complexity` — [`L46`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L46) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `cyclomatic_complexity` — [`L45`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L45) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `function_name` — [`L43`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L43) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `line_number` — [`L47`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L47) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `path` — [`L44`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L44) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- used by: [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`renderDashboardHtml`](../webview/dashboardTemplate.ts.md#renderDashboardHtml), [`getComplexityHotspots`](../mcp/service.ts.md#CgcService.getComplexityHotspots), [`dashboardTemplate.ts`](../webview/dashboardTemplate.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-webview-dashboardTemplate.ts), [`hotspots`](../webview/dashboardTemplate.ts.md#DashboardPayload.typeLiteral0.hotspots)  (1 test-only)

### `DeadCodeEntry`
- def: [`extensions/vscode/src/types/cgc.ts:22`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L22) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
- signature: `interface DeadCodeEntry`
- members:
  - `class_name` — [`L26`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L26)
  - `function_name` — [`L23`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L23)
  - `line_number` — [`L25`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L25)
  - `path` — [`L24`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L24)
- used by: [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`refreshForDocument`](../providers/editorProviders.ts.md#CgcDeadCodeDiagnostics.refreshForDocument), [`editorProviders.ts`](../providers/editorProviders.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-providers-editorProviders.ts), [`findDeadCode`](../mcp/service.ts.md#CgcService.findDeadCode), [`index`](../providers/editorProviders.ts.md#CgcDeadCodeDiagnostics.index)

### `DiscoveredContext`
- def: [`extensions/vscode/src/types/cgc.ts:71`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L71)
- signature: `interface DiscoveredContext`
- members:
  - `name` — [`L73`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L73)
  - `path` — [`L72`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L72)
- used by: [`activate`](../extension.ts.md#activate), [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`discoverContexts`](../mcp/service.ts.md#CgcService.discoverContexts)

### `IndexedRepository`
- def: [`extensions/vscode/src/types/cgc.ts:16`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L16) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
- signature: `interface IndexedRepository`
- members:
  - `file_count` — [`L19`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L19)
  - `path` — [`L18`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L18)
  - `repo_name` — [`L17`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L17)
- used by: [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`renderDashboardHtml`](../webview/dashboardTemplate.ts.md#renderDashboardHtml), [`listRepositories`](../mcp/service.ts.md#CgcService.listRepositories), [`dashboardTemplate.ts`](../webview/dashboardTemplate.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-webview-dashboardTemplate.ts), [`repos`](../webview/dashboardTemplate.ts.md#DashboardPayload.typeLiteral0.repos)  (1 test-only)

### `JobStatus`
- def: [`extensions/vscode/src/types/cgc.ts:63`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L63)
- signature: `interface JobStatus`
- members:
  - `error` — [`L68`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L68)
  - `job_id` — [`L64`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L64)
  - `message` — [`L67`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L67)
  - `progress` — [`L66`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L66)
  - `status` — [`L65`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L65)
- used by: [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`startPolling`](../mcp/jobPoller.ts.md#JobPoller.startPolling), [`checkJobStatus`](../mcp/service.ts.md#CgcService.checkJobStatus)

### `MpcToolContent`
- def: [`extensions/vscode/src/types/cgc.ts:1`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L1) — documented in [extensions-vscode-src-mcp-client.ts](../../../../../concepts/extensions-vscode-src-mcp-client.ts.md)
- signature: `interface MpcToolContent`
- members:
  - `text` — [`L3`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L3)
  - `type` — [`L2`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L2)
- used by: [`CgcMcpToolResponse`](cgc.ts.md#CgcMcpToolResponse)

### `RepoStats`
- def: [`extensions/vscode/src/types/cgc.ts:50`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L50) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- signature: `interface RepoStats`
- members:
  - `class_count` — [`L54`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L54) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `file_count` — [`L52`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L52) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `function_count` — [`L53`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L53) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `module_count` — [`L55`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L55) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `repo_path` — [`L51`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L51)
  - `total_classes` — [`L59`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L59) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `total_files` — [`L57`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L57) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `total_functions` — [`L58`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L58) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `total_modules` — [`L60`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/types/cgc.ts#L60)
- used by: [`path`](../views/controlPanel.ts.md#SidebarControlPanel.buildHtml.data-typeLiteral60.discoveredContexts.Array.typeLiteral170.path), [`render`](../views/controlPanel.ts.md#SidebarControlPanel.render), [`service.ts`](../mcp/service.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-mcp-service.ts), [`getRepoStats`](../mcp/service.ts.md#CgcService.getRepoStats), [`controlPanel.ts`](../views/controlPanel.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-views-controlPanel.ts), [`stats`](../views/controlPanel.ts.md#SidebarControlPanel.buildHtml.data-typeLiteral60.stats)

