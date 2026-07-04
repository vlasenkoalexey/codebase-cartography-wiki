---
title: 'Module: src/extraction/parse-pool.ts'
type: catalog
provenance: extracted
module: src/extraction/parse-pool.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`parse-pool.ts`/
symbols:
  ParseWorkerPool.-constructor: ParseWorkerPool#`<constructor>`().
  ParseWorkerPool.spawnOne: ParseWorkerPool#spawnOne().
  ParseWorkerPool.onMessage: ParseWorkerPool#onMessage().
  ParseWorkerPool.drain: ParseWorkerPool#drain().
  ParseWorkerPool.dispatch: ParseWorkerPool#dispatch().
  ParseWorkerPool.onTimeout: ParseWorkerPool#onTimeout().
  ParseWorkerPool.requestParse: ParseWorkerPool#requestParse().
  ParseWorkerPool.onWorkerGone: ParseWorkerPool#onWorkerGone().
  ParseWorkerPool.destroy: ParseWorkerPool#destroy().
  ParseWorkerPool.recycle: ParseWorkerPool#recycle().
  ParseWorkerPool.settle: ParseWorkerPool#settle().
  ParseWorkerPool.removeWorker: ParseWorkerPool#removeWorker().
  ParsePoolWorker: ParsePoolWorker#
  ParseWorkerPool.workers: ParseWorkerPool#workers.
  ParseWorkerPool.inflight: ParseWorkerPool#inflight.
  ParseWorkerPool.idle: ParseWorkerPool#idle.
  ParseWorkerPool.-get-healthy: ParseWorkerPool#`<get>healthy`().
  ParseWorkerPool.queue: ParseWorkerPool#queue.
  ParseJob.task: ParseJob#task.
  ParseWorkerPool.pending: ParseWorkerPool#pending.
  ParseWorkerPool.parseCounts: ParseWorkerPool#parseCounts.
  ParseWorkerPool.destroyed: ParseWorkerPool#destroyed.
  resolveParsePoolSize: resolveParsePoolSize().
  ParseWorkerPool.recycleAll: ParseWorkerPool#recycleAll().
  ParseJob: ParseJob#
  ParseJob.settled: ParseJob#settled.
  ParseWorkerPool.createWorker: ParseWorkerPool#createWorker.
  ParseTask.language: ParseTask#language.
  ParseJob.resolve: ParseJob#resolve.
  ParseWorkerPoolOptions.languages: ParseWorkerPoolOptions#languages.
  ParseWorkerPoolOptions.createWorker: ParseWorkerPoolOptions#createWorker.
  ParseWorkerPool.languages: ParseWorkerPool#languages.
  ParsePoolWorker.terminate: ParsePoolWorker#terminate().
  ParseJob.timer: ParseJob#timer.
  ParseWorkerPool.maxSize: ParseWorkerPool#maxSize.
  ParseWorkerMessage.result: ParseWorkerMessage#result.
  ParseWorkerPool.-get-size: ParseWorkerPool#`<get>size`().
  ParsePoolWorker.on: ParsePoolWorker#on().
  ParseTask.filePath: ParseTask#filePath.
  ParseTask.content: ParseTask#content.
  ParseJob.id: ParseJob#id.
  ParseWorkerPoolOptions.workerScriptPath: ParseWorkerPoolOptions#workerScriptPath.
  ParseWorkerPool.totalCrashes: ParseWorkerPool#totalCrashes.
  ParseWorkerPool.log: ParseWorkerPool#log.
  ParseWorkerPool.-get-liveWorkers: ParseWorkerPool#`<get>liveWorkers`().
  ParsePoolWorker.postMessage: ParsePoolWorker#postMessage().
  ParseTask: ParseTask#
  ParseTask.frameworkNames: ParseTask#frameworkNames.
  MAX_PARSE_POOL_SIZE: MAX_PARSE_POOL_SIZE.
  ParseJob.reject: ParseJob#reject.
  ParseWorkerMessage: ParseWorkerMessage#
  ParseWorkerMessage.type: ParseWorkerMessage#type.
  ParseWorkerMessage.id: ParseWorkerMessage#id.
  ParseWorkerPoolOptions.size: ParseWorkerPoolOptions#size.
  ParseWorkerPoolOptions.recycleInterval: ParseWorkerPoolOptions#recycleInterval.
  ParseWorkerPoolOptions.parseTimeoutMs: ParseWorkerPoolOptions#parseTimeoutMs.
  ParseWorkerPoolOptions.log: ParseWorkerPoolOptions#log.
  ParseWorkerPool: ParseWorkerPool#
  ParseWorkerPool.recycleInterval: ParseWorkerPool#recycleInterval.
  ParseWorkerPool.parseTimeoutMs: ParseWorkerPool#parseTimeoutMs.
  DEFAULT_PARSE_POOL_CAP: DEFAULT_PARSE_POOL_CAP.
  DEFAULT_RECYCLE_INTERVAL: DEFAULT_RECYCLE_INTERVAL.
  DEFAULT_PARSE_TIMEOUT_MS: DEFAULT_PARSE_TIMEOUT_MS.
  MAX_CONCURRENT_SPAWN: MAX_CONCURRENT_SPAWN.
  CRASH_BUDGET: CRASH_BUDGET.
  ParseWorkerPoolOptions: ParseWorkerPoolOptions#
  ParseWorkerPool.nextId: ParseWorkerPool#nextId.
---
# Module: [`src/extraction/parse-pool.ts`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts)

## Classes
### `ParseJob`
- def: [`src/extraction/parse-pool.ts:98`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L98) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- signature: `interface ParseJob`
- members:
  - `id` — [`L99`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L99) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `reject` — [`L102`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L102) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `resolve` — [`L101`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L101) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `settled` — [`L103`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L103) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `task` — [`L100`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L100) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `timer` — [`L104`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L104) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- uses (calls/refs, reference-scoped): [`ExtractionResult`](../types.ts.md#ExtractionResult), [`ParseTask`](parse-pool.ts.md#ParseTask)
- used by: [`onMessage`](parse-pool.ts.md#ParseWorkerPool.onMessage), [`drain`](parse-pool.ts.md#ParseWorkerPool.drain), [`dispatch`](parse-pool.ts.md#ParseWorkerPool.dispatch), [`onTimeout`](parse-pool.ts.md#ParseWorkerPool.onTimeout), [`requestParse`](parse-pool.ts.md#ParseWorkerPool.requestParse), [`settle`](parse-pool.ts.md#ParseWorkerPool.settle), [`inflight`](parse-pool.ts.md#ParseWorkerPool.inflight), [`queue`](parse-pool.ts.md#ParseWorkerPool.queue)

### `ParsePoolWorker`
- def: [`src/extraction/parse-pool.ts:39`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L39) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- doc: Minimal worker surface the pool drives — satisfied by a real `worker_threads`
- signature: `interface ParsePoolWorker`
- members:
  - `on(method)` — [`L42`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L42) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `postMessage(method)` — [`L40`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L40) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `terminate(method)` — [`L41`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L41) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- used by: [`spawnOne`](parse-pool.ts.md#ParseWorkerPool.spawnOne), [`onMessage`](parse-pool.ts.md#ParseWorkerPool.onMessage), [`dispatch`](parse-pool.ts.md#ParseWorkerPool.dispatch), [`onTimeout`](parse-pool.ts.md#ParseWorkerPool.onTimeout), [`onWorkerGone`](parse-pool.ts.md#ParseWorkerPool.onWorkerGone), [`destroy`](parse-pool.ts.md#ParseWorkerPool.destroy), [`recycle`](parse-pool.ts.md#ParseWorkerPool.recycle), [`removeWorker`](parse-pool.ts.md#ParseWorkerPool.removeWorker), [`workers`](parse-pool.ts.md#ParseWorkerPool.workers), [`inflight`](parse-pool.ts.md#ParseWorkerPool.inflight), [`idle`](parse-pool.ts.md#ParseWorkerPool.idle), [`parseCounts`](parse-pool.ts.md#ParseWorkerPool.parseCounts), [`pending`](parse-pool.ts.md#ParseWorkerPool.pending), [`createWorker`](parse-pool.ts.md#ParseWorkerPool.createWorker), [`createWorker`](parse-pool.ts.md#ParseWorkerPoolOptions.createWorker)

### `ParseTask`
- def: [`src/extraction/parse-pool.ts:49`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L49)
- doc: A single file to parse. `language` is resolved on the main thread (it holds
- signature: `interface ParseTask`
- members:
  - `content` — [`L51`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L51) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `filePath` — [`L50`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L50) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `frameworkNames` — [`L53`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L53) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `language` — [`L52`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L52) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language)
- used by: [`indexAll`](index.ts.md#ExtractionOrchestrator.indexAll), [`dispatch`](parse-pool.ts.md#ParseWorkerPool.dispatch), [`onTimeout`](parse-pool.ts.md#ParseWorkerPool.onTimeout), [`requestParse`](parse-pool.ts.md#ParseWorkerPool.requestParse), [`task`](parse-pool.ts.md#ParseJob.task)

### `ParseWorkerMessage`
- def: [`src/extraction/parse-pool.ts:108`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L108) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- doc: Shape of a message a worker posts back (grammar-load ack or a parse result).
- signature: `interface ParseWorkerMessage`
- members:
  - `id` — [`L110`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L110) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `result` — [`L111`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L111) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `type` — [`L109`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L109) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- uses (calls/refs, reference-scoped): [`ExtractionResult`](../types.ts.md#ExtractionResult)
- used by: [`spawnOne`](parse-pool.ts.md#ParseWorkerPool.spawnOne), [`onMessage`](parse-pool.ts.md#ParseWorkerPool.onMessage)

### `ParseWorkerPool`
- def: [`src/extraction/parse-pool.ts:131`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L131)
- signature: `class ParseWorkerPool`
- members:
  - `<constructor>(opts: ParseWorkerPoolOptions)` — [`L151`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L151) — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
  - `<get>healthy` — [`L175`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L175) — False once the crash budget is exhausted (or after destroy). — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `<get>liveWorkers` — [`L172`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L172) — Live worker count (for tests).
  - `<get>size` — [`L169`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L169) — Pool size cap (for logging).
  - `destroy(method)` — [`L345`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L345) — Terminate all workers and reject any outstanding parses.
  - `dispatch(method)` — [`L266`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L266) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `drain(method)` — [`L298`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L298) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `onMessage(method)` — [`L211`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L211) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `onTimeout(method)` — [`L284`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L284) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `onWorkerGone(method)` — [`L237`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L237) — A worker died (crash hook / OOM exit / spawn error). Reject its in-flight — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `recycle(method)` — [`L251`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L251) — Tear down a worker that has hit its recycle threshold and replace it. Not a — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `recycleAll(method)` — [`L340`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L340) — Recycle every idle worker now (fresh WASM heaps). The orchestrator calls
  - `removeWorker(method)` — [`L259`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L259)
  - `requestParse(method)` — [`L184`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L184) — Parse one file on the pool. Resolves with the extraction result, or REJECTS — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `settle(method)` — [`L328`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L328) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `spawnOne(method)` — [`L192`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L192) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `createWorker` — [`L148`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L148) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `destroyed` — [`L142`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L142) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `idle` — [`L132`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L132) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `inflight` — [`L134`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L134) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `languages` — [`L144`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L144) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `log` — [`L149`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L149)
  - `maxSize` — [`L145`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L145) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `nextId` — [`L140`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L140)
  - `parseCounts` — [`L139`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L139) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `parseTimeoutMs` — [`L147`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L147) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `pending` — [`L138`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L138) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `queue` — [`L133`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L133) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `recycleInterval` — [`L146`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L146) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `totalCrashes` — [`L141`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L141) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `workers` — [`L135`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L135) — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`ParsePoolWorker`](parse-pool.ts.md#ParsePoolWorker), [`task`](parse-pool.ts.md#ParseJob.task), [`ParseJob`](parse-pool.ts.md#ParseJob), [`settled`](parse-pool.ts.md#ParseJob.settled), [`createWorker`](parse-pool.ts.md#ParseWorkerPoolOptions.createWorker), [`language`](parse-pool.ts.md#ParseTask.language), [`languages`](parse-pool.ts.md#ParseWorkerPoolOptions.languages), [`resolve`](parse-pool.ts.md#ParseJob.resolve), [`terminate`](parse-pool.ts.md#ParsePoolWorker.terminate), [`timer`](parse-pool.ts.md#ParseJob.timer), [`result`](parse-pool.ts.md#ParseWorkerMessage.result), [`content`](parse-pool.ts.md#ParseTask.content), [`filePath`](parse-pool.ts.md#ParseTask.filePath), [`id`](parse-pool.ts.md#ParseJob.id), [`on`](parse-pool.ts.md#ParsePoolWorker.on), [`workerScriptPath`](parse-pool.ts.md#ParseWorkerPoolOptions.workerScriptPath), [`ParseTask`](parse-pool.ts.md#ParseTask), [`ParseWorkerMessage`](parse-pool.ts.md#ParseWorkerMessage), [`MAX_PARSE_POOL_SIZE`](parse-pool.ts.md#MAX_PARSE_POOL_SIZE), [`frameworkNames`](parse-pool.ts.md#ParseTask.frameworkNames), [`id`](parse-pool.ts.md#ParseWorkerMessage.id), [`log`](parse-pool.ts.md#ParseWorkerPoolOptions.log), [`parseTimeoutMs`](parse-pool.ts.md#ParseWorkerPoolOptions.parseTimeoutMs), [`postMessage`](parse-pool.ts.md#ParsePoolWorker.postMessage), [`recycleInterval`](parse-pool.ts.md#ParseWorkerPoolOptions.recycleInterval), [`reject`](parse-pool.ts.md#ParseJob.reject), [`size`](parse-pool.ts.md#ParseWorkerPoolOptions.size), [`type`](parse-pool.ts.md#ParseWorkerMessage.type), [`ParseWorkerPoolOptions`](parse-pool.ts.md#ParseWorkerPoolOptions), [`CRASH_BUDGET`](parse-pool.ts.md#CRASH_BUDGET), [`DEFAULT_PARSE_TIMEOUT_MS`](parse-pool.ts.md#DEFAULT_PARSE_TIMEOUT_MS), [`DEFAULT_RECYCLE_INTERVAL`](parse-pool.ts.md#DEFAULT_RECYCLE_INTERVAL), [`MAX_CONCURRENT_SPAWN`](parse-pool.ts.md#MAX_CONCURRENT_SPAWN)
- used by: [`indexAll`](index.ts.md#ExtractionOrchestrator.indexAll), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-index.ts)

### `ParseWorkerPoolOptions`
- def: [`src/extraction/parse-pool.ts:114`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L114)
- signature: `interface ParseWorkerPoolOptions`
- members:
  - `createWorker` — [`L126`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L126) — Worker factory (tests inject a fake). Defaults to a real `worker_threads` Worker. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `languages` — [`L116`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L116) — Languages to load grammars for in every worker at spawn. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `log` — [`L128`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L128) — Optional verbose logger (the orchestrator's `[worker] …` logger). — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `parseTimeoutMs` — [`L124`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L124) — Base per-parse timeout (ms); scaled by file size per parse. Default 10s. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `recycleInterval` — [`L122`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L122) — Parses per worker before recycle. Default 250. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `size` — [`L118`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L118) — Number of worker threads (≥1). Clamp the resolved value before passing. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
  - `workerScriptPath` — [`L120`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L120) — Compiled `parse-worker.js` path. Required unless `createWorker` is given. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language), [`ParsePoolWorker`](parse-pool.ts.md#ParsePoolWorker)
- used by: [`indexAll`](index.ts.md#ExtractionOrchestrator.indexAll), [`<constructor>`](parse-pool.ts.md#ParseWorkerPool.-constructor)

## Functions
- `resolveParsePoolSize(envVal: string | undefined, cpuCount: number)` — [`L87`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L87) — Resolve the pool size from the `CODEGRAPH_PARSE_WORKERS` override and the

## Module values
- `CRASH_BUDGET` — [`L77`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L77) — Total worker deaths before the pool stops respawning and fails outstanding
- `DEFAULT_PARSE_POOL_CAP` — [`L57`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L57) — Default upper bound on the pool size derived from the core count.
- `DEFAULT_PARSE_TIMEOUT_MS` — [`L63`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L63) — Base per-parse timeout; scaled up for large files by the caller's formula.
- `DEFAULT_RECYCLE_INTERVAL` — [`L61`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L61) — Parses a worker performs before it's recycled to reclaim WASM heap. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- `MAX_CONCURRENT_SPAWN` — [`L70`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L70) — Max workers cold-starting at once. A worker's cold start is heavy (module load — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)
- `MAX_PARSE_POOL_SIZE` — [`L59`](../../../../../../raw/code/codegraph/src/extraction/parse-pool.ts#L59) — Hard ceiling on pool size regardless of an explicit env override. — documented in [extraction-parse-pool.ts](../../../concepts/extraction-parse-pool.ts.md)

