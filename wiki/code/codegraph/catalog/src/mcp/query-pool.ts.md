---
title: 'Module: src/mcp/query-pool.ts'
type: catalog
provenance: extracted
module: src/mcp/query-pool.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`query-pool.ts`/
symbols:
  QueryPool.onWorkerGone: QueryPool#onWorkerGone().
  QueryPool.drain: QueryPool#drain().
  QueryPool.run: QueryPool#run().
  QueryPool.-constructor: QueryPool#`<constructor>`().
  QueryPool.onMessage: QueryPool#onMessage().
  QueryPool.destroy: QueryPool#destroy().
  QueryPool.spawnOne: QueryPool#spawnOne().
  QueryPool.settle: QueryPool#settle().
  busyGuidance: busyGuidance().
  QueryPool.inflight: QueryPool#inflight.
  QueryPool.-get-healthy: QueryPool#`<get>healthy`().
  QueryPool.idle: QueryPool#idle.
  QueryPool.queue: QueryPool#queue.
  QueryPool.workers: QueryPool#workers.
  PoolWorker: PoolWorker#
  QueryPool.pendingWorkers: QueryPool#pendingWorkers.
  Job.settled: Job#settled.
  Job: Job#
  QueryPool: QueryPool#
  Job.resolve: Job#resolve.
  resolvePoolSize: resolvePoolSize().
  QueryPool.createWorker: QueryPool#createWorker.
  Job.softTimer: Job#softTimer.
  QueryPool.totalCrashes: QueryPool#totalCrashes.
  QueryPool.destroyed: QueryPool#destroyed.
  QueryPool.maxSize: QueryPool#maxSize.
  WorkerMessage.result: WorkerMessage#result.
  QueryPoolOptions.createWorker: QueryPoolOptions#createWorker.
  resolveBusyTimeoutMs: resolveBusyTimeoutMs().
  PoolWorker.on: PoolWorker#on().
  MAX_POOL_SIZE: MAX_POOL_SIZE.
  Job.retries: Job#retries.
  QueryPool.-get-size: QueryPool#`<get>size`().
  QueryPool.-get-liveWorkers: QueryPool#`<get>liveWorkers`().
  PoolWorker.terminate: PoolWorker#terminate().
  DEFAULT_BUSY_TIMEOUT_MS: DEFAULT_BUSY_TIMEOUT_MS.
  WorkerMessage: WorkerMessage#
  WorkerMessage.type: WorkerMessage#type.
  Job.id: Job#id.
  Job.toolName: Job#toolName.
  Job.args: Job#args.
  Job.enqueuedAt: Job#enqueuedAt.
  QueryPoolOptions.root: QueryPoolOptions#root.
  QueryPoolOptions.size: QueryPoolOptions#size.
  QueryPool.root: QueryPool#root.
  QueryPool.softTimeoutMs: QueryPool#softTimeoutMs.
  QueryPool.maxRetries: QueryPool#maxRetries.
  WORKER_FILE: WORKER_FILE.
  PoolWorker.postMessage: PoolWorker#postMessage().
  CRASH_BUDGET: CRASH_BUDGET.
  MAX_CONCURRENT_SPAWN: MAX_CONCURRENT_SPAWN.
  WorkerMessage.ok: WorkerMessage#ok.
  QueryPoolOptions: QueryPoolOptions#
  QueryPoolOptions.softTimeoutMs: QueryPoolOptions#softTimeoutMs.
  QueryPoolOptions.maxRetries: QueryPoolOptions#maxRetries.
  QueryPool.nextId: QueryPool#nextId.
  WorkerMessage.id: WorkerMessage#id.
---
# Module: [`src/mcp/query-pool.ts`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts)

## Classes
### `Job`
- def: [`src/mcp/query-pool.ts:80`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L80) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- signature: `interface Job`
- members:
  - `args` — [`L83`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L83) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `enqueuedAt` — [`L87`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L87) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `id` — [`L81`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L81) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `resolve` — [`L84`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L84) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `retries` — [`L85`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L85) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `settled` — [`L86`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L86) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `softTimer` — [`L88`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L88) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `toolName` — [`L82`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L82) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- uses (calls/refs, reference-scoped): [`ToolResult`](tools.ts.md#ToolResult)
- used by: [`onWorkerGone`](query-pool.ts.md#QueryPool.onWorkerGone), [`drain`](query-pool.ts.md#QueryPool.drain), [`run`](query-pool.ts.md#QueryPool.run), [`settle`](query-pool.ts.md#QueryPool.settle), [`inflight`](query-pool.ts.md#QueryPool.inflight), [`queue`](query-pool.ts.md#QueryPool.queue)

### `PoolWorker`
- def: [`src/mcp/query-pool.ts:40`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L40) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- doc: Minimal worker surface the pool drives — satisfied by a real `worker_threads`
- signature: `interface PoolWorker`
- members:
  - `on(method)` — [`L43`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L43) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `postMessage(method)` — [`L41`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L41) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `terminate(method)` — [`L42`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L42) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- used by: [`onWorkerGone`](query-pool.ts.md#QueryPool.onWorkerGone), [`drain`](query-pool.ts.md#QueryPool.drain), [`destroy`](query-pool.ts.md#QueryPool.destroy), [`onMessage`](query-pool.ts.md#QueryPool.onMessage), [`spawnOne`](query-pool.ts.md#QueryPool.spawnOne), [`inflight`](query-pool.ts.md#QueryPool.inflight), [`idle`](query-pool.ts.md#QueryPool.idle), [`workers`](query-pool.ts.md#QueryPool.workers), [`pendingWorkers`](query-pool.ts.md#QueryPool.pendingWorkers), [`createWorker`](query-pool.ts.md#QueryPool.createWorker), [`createWorker`](query-pool.ts.md#QueryPoolOptions.createWorker)

### `QueryPool`
- def: [`src/mcp/query-pool.ts:142`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L142)
- signature: `class QueryPool`
- members:
  - `<constructor>(opts: QueryPoolOptions)` — [`L162`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L162) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `<get>healthy` — [`L182`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L182) — False once the crash budget is exhausted (or after destroy). The ToolHandler — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `<get>liveWorkers` — [`L175`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L175) — Live worker count (for tests/status).
  - `<get>size` — [`L172`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L172) — Pool size cap (for logging/status).
  - `destroy(method)` — [`L294`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L294) — Terminate all workers and answer any outstanding calls gracefully. — documented in [mcp-daemon.ts](../../../concepts/mcp-daemon.ts.md)
  - `drain(method)` — [`L244`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L244) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `onMessage(method)` — [`L202`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L202) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `onWorkerGone(method)` — [`L223`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L223) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `run(method)` — [`L275`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L275) — Run a read tool on the pool. Always resolves (never rejects). — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `settle(method)` — [`L267`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L267) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `spawnOne(method)` — [`L186`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L186) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `createWorker` — [`L160`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L160) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `destroyed` — [`L155`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L155) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `idle` — [`L143`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L143) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `inflight` — [`L145`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L145) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `maxRetries` — [`L159`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L159) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `maxSize` — [`L157`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L157) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `nextId` — [`L153`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L153)
  - `pendingWorkers` — [`L152`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L152) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `queue` — [`L144`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L144) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `root` — [`L156`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L156)
  - `softTimeoutMs` — [`L158`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L158) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `totalCrashes` — [`L154`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L154) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `workers` — [`L146`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L146) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- uses (calls/refs, reference-scoped): [`ToolResult`](tools.ts.md#ToolResult), [`content`](tools.ts.md#ToolResult.content), [`text`](tools.ts.md#ToolResult.content.Array.typeLiteral23.text), [`busyGuidance`](query-pool.ts.md#busyGuidance), [`type`](tools.ts.md#ToolResult.content.Array.typeLiteral23.type), [`isError`](tools.ts.md#ToolResult.isError), [`PoolWorker`](query-pool.ts.md#PoolWorker), [`settled`](query-pool.ts.md#Job.settled), [`Job`](query-pool.ts.md#Job), [`resolve`](query-pool.ts.md#Job.resolve), [`softTimer`](query-pool.ts.md#Job.softTimer), [`createWorker`](query-pool.ts.md#QueryPoolOptions.createWorker), [`resolveBusyTimeoutMs`](query-pool.ts.md#resolveBusyTimeoutMs), [`result`](query-pool.ts.md#WorkerMessage.result), [`MAX_POOL_SIZE`](query-pool.ts.md#MAX_POOL_SIZE), [`on`](query-pool.ts.md#PoolWorker.on), [`retries`](query-pool.ts.md#Job.retries), [`WorkerMessage`](query-pool.ts.md#WorkerMessage), [`args`](query-pool.ts.md#Job.args), [`enqueuedAt`](query-pool.ts.md#Job.enqueuedAt), [`id`](query-pool.ts.md#Job.id), [`root`](query-pool.ts.md#QueryPoolOptions.root), [`size`](query-pool.ts.md#QueryPoolOptions.size), [`terminate`](query-pool.ts.md#PoolWorker.terminate), [`toolName`](query-pool.ts.md#Job.toolName), [`type`](query-pool.ts.md#WorkerMessage.type), [`QueryPoolOptions`](query-pool.ts.md#QueryPoolOptions), [`CRASH_BUDGET`](query-pool.ts.md#CRASH_BUDGET), [`MAX_CONCURRENT_SPAWN`](query-pool.ts.md#MAX_CONCURRENT_SPAWN), [`WORKER_FILE`](query-pool.ts.md#WORKER_FILE), [`maxRetries`](query-pool.ts.md#QueryPoolOptions.maxRetries), [`ok`](query-pool.ts.md#WorkerMessage.ok), [`postMessage`](query-pool.ts.md#PoolWorker.postMessage), [`softTimeoutMs`](query-pool.ts.md#QueryPoolOptions.softTimeoutMs)
- used by: [`tools.ts`](tools.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-tools.ts), [`execute`](tools.ts.md#ToolHandler.execute), [`engine.ts`](engine.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-engine.ts), [`maybeStartPool`](engine.ts.md#MCPEngine.maybeStartPool), [`stop`](engine.ts.md#MCPEngine.stop), [`queryPool`](engine.ts.md#MCPEngine.queryPool), [`setQueryPool`](tools.ts.md#ToolHandler.setQueryPool), [`queryPool`](tools.ts.md#ToolHandler.queryPool)

### `QueryPoolOptions`
- def: [`src/mcp/query-pool.ts:91`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L91) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- signature: `interface QueryPoolOptions`
- members:
  - `createWorker` — [`L101`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L101) — Worker factory (tests inject a fake). Defaults to a real `worker_threads` Worker. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `maxRetries` — [`L99`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L99) — Retries for an in-flight call whose worker crashed. Default 1. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `root` — [`L93`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L93) — Default project root each worker opens at spawn. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `size` — [`L95`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L95) — Max worker threads. Defaults to `clamp(cores-1, 1, 16)`. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `softTimeoutMs` — [`L97`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L97) — Linger before a queued call gets busy-guidance. Default 45s. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- uses (calls/refs, reference-scoped): [`PoolWorker`](query-pool.ts.md#PoolWorker)
- used by: [`<constructor>`](query-pool.ts.md#QueryPool.-constructor), [`maybeStartPool`](engine.ts.md#MCPEngine.maybeStartPool)

### `WorkerMessage`
- def: [`src/mcp/query-pool.ts:73`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L73) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- doc: Shape of a message a worker posts back (ready handshake or a tool result).
- signature: `interface WorkerMessage`
- members:
  - `id` — [`L76`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L76)
  - `ok` — [`L75`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L75) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `result` — [`L77`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L77) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
  - `type` — [`L74`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L74) — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- uses (calls/refs, reference-scoped): [`ToolResult`](tools.ts.md#ToolResult)
- used by: [`onMessage`](query-pool.ts.md#QueryPool.onMessage), [`spawnOne`](query-pool.ts.md#QueryPool.spawnOne)

## Functions
- `busyGuidance(waitedMs: number)` — [`L129`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L129) — Success-shaped overload guidance (NEVER isError — see the abandonment rule). — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- `resolveBusyTimeoutMs()` — [`L120`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L120)
- `resolvePoolSize(envVal: string | undefined, cpuCount: number)` — [`L111`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L111) — Resolve the pool size from the `CODEGRAPH_QUERY_POOL_SIZE` override and the

## Module values
- `CRASH_BUDGET` — [`L60`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L60) — Total worker deaths before the pool declares itself unhealthy and the caller — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- `DEFAULT_BUSY_TIMEOUT_MS` — [`L49`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L49) — Default linger before a queued call is answered with busy-guidance.
- `MAX_CONCURRENT_SPAWN` — [`L70`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L70) — Max workers cold-starting at once. A worker's cold start is heavy — full — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- `MAX_POOL_SIZE` — [`L52`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L52) — Hard ceiling on pool size regardless of core count / env. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)
- `WORKER_FILE` — [`L32`](../../../../../../raw/code/codegraph/src/mcp/query-pool.ts#L32) — Compiled sibling — `query-worker.js` lives next to this file in `dist/mcp/`. — documented in [mcp-query-pool.ts](../../../concepts/mcp-query-pool.ts.md)

