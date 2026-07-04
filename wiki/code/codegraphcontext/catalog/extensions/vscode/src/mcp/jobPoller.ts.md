---
title: 'Module: extensions/vscode/src/mcp/jobPoller.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/mcp/jobPoller.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/mcp/`jobPoller.ts`/JobPoller#
symbols:
  JobPoller.startPolling: startPolling().
  JobPoller._stop: _stop().
  JobPoller.activeJobs: activeJobs.
  JobPoller.dispose: dispose().
  JobPoller.-constructor: '`<constructor>`().'
  JobPoller: ''
---
# Module: [`extensions/vscode/src/mcp/jobPoller.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts)

## Classes
### `JobPoller`
- def: [`extensions/vscode/src/mcp/jobPoller.ts:9`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L9)
- doc: Polls `check_job_status` for active indexing jobs and fires EventBus events.
- signature: `class JobPoller`
- members:
  - `<constructor>(service: CgcService)` — [`L12`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L12) — Polls `check_job_status` for active indexing jobs and fires EventBus events. — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `dispose(method)` — [`L54`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L54)
  - `startPolling(method)` — [`L18`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L18) — Start polling a job ID every 2 seconds.
  - `activeJobs` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L10)
- protocol/private: `_stop`[`L46`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/mcp/jobPoller.ts#L46)
- uses (calls/refs, reference-scoped): [`cgcEvents`](eventBus.ts.md#cgcEvents), [`emit`](eventBus.ts.md#CgcEventBus.emit), [`CgcService`](service.ts.md#CgcService), [`checkJobStatus`](service.ts.md#CgcService.checkJobStatus), [`status`](../types/cgc.ts.md#JobStatus.status), [`message`](../types/cgc.ts.md#JobStatus.message), [`error`](../types/cgc.ts.md#JobStatus.error), [`progress`](../types/cgc.ts.md#JobStatus.progress)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

