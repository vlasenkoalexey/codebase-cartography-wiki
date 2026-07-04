---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`async-promises.ts`/
symbols:
  PromisePool.execute: PromisePool#execute().
  asyncExamples: asyncExamples.
  batchProcessUsers: batchProcessUsers().
  TaskQueue.enqueue: TaskQueue#enqueue().
  TaskQueue.processQueue: TaskQueue#processQueue().
  AsyncCache.cache: AsyncCache#cache.
  EventEmitter.emit: EventEmitter#emit().
  Semaphore.acquire: Semaphore#acquire().
  Semaphore.release: Semaphore#release().
  fetchUserProfile: fetchUserProfile().
  PromisePool.-constructor: PromisePool#`<constructor>`().
  EventEmitter.listeners: EventEmitter#listeners.
  EventEmitter.asyncListeners: EventEmitter#asyncListeners.
  EventEmitter.emitAsync: EventEmitter#emitAsync().
  AsyncCache.get: AsyncCache#get().
  Semaphore.execute: Semaphore#execute().
  EventEmitter.subscribe: EventEmitter#subscribe().
  PromisePool.add: PromisePool#add().
  EventEmitter: EventEmitter#
  PromisePool.tasks: PromisePool#tasks.
  PromisePool.running: PromisePool#running.
  Semaphore.permits: Semaphore#permits.
  TaskQueue.queue: TaskQueue#queue.
  TaskQueue.processing: TaskQueue#processing.
  fetchUserPosts: fetchUserPosts().
  AsyncCache.-constructor: AsyncCache#`<constructor>`().
  Semaphore.-constructor: Semaphore#`<constructor>`().
  TaskQueue.-constructor: TaskQueue#`<constructor>`().
  Semaphore.waiting: Semaphore#waiting.
  retryOperation: retryOperation().
  EventEmitter.subscribeAsync: EventEmitter#subscribeAsync().
  AsyncCache.clear: AsyncCache#clear().
  AsyncCache.has: AsyncCache#has().
  TaskQueue.-get-length: TaskQueue#`<get>length`().
  TaskQueue.-get-isProcessing: TaskQueue#`<get>isProcessing`().
  PromisePool: PromisePool#
  PromisePool.concurrency: PromisePool#concurrency.
  PromisePool.results: PromisePool#results.
  PromisePool.errors: PromisePool#errors.
  PromisePool.execute.Promise.typeLiteral139.results: PromisePool#execute().Promise:typeLiteral139:results.
  PromisePool.execute.Promise.typeLiteral139.errors: PromisePool#execute().Promise:typeLiteral139:errors.
  AsyncCache.ttl: AsyncCache#ttl.
  TaskQueue.processor: TaskQueue#processor.
  fetchUserData: fetchUserData().
  AsyncCache: AsyncCache#
  createPromise: createPromise().
  createRejectedPromise: createRejectedPromise().
  fetchUserData.Promise.typeLiteral9.id: fetchUserData().Promise:typeLiteral9:id.
  fetchUserData.Promise.typeLiteral9.name: fetchUserData().Promise:typeLiteral9:name.
  fetchUserData.Promise.typeLiteral9.email: fetchUserData().Promise:typeLiteral9:email.
  safeAsyncOperation: safeAsyncOperation().
  processInParallel: processInParallel().
  raceWithTimeout: raceWithTimeout().
  asyncGenerator: asyncGenerator().
  fetchDataStream: fetchDataStream().
  consumeAsyncGenerator: consumeAsyncGenerator().
  Semaphore: Semaphore#
  TaskQueue: TaskQueue#
  processStream: processStream().
  fetchUserProfile.Promise.typeLiteral216.user: fetchUserProfile().Promise:typeLiteral216:user.
  fetchUserProfile.Promise.typeLiteral216.user.typeLiteral217.id: fetchUserProfile().Promise:typeLiteral216:user.typeLiteral217:id.
  fetchUserProfile.Promise.typeLiteral216.user.typeLiteral217.name: fetchUserProfile().Promise:typeLiteral216:user.typeLiteral217:name.
  fetchUserProfile.Promise.typeLiteral216.user.typeLiteral217.email: fetchUserProfile().Promise:typeLiteral216:user.typeLiteral217:email.
  fetchUserProfile.Promise.typeLiteral216.posts: fetchUserProfile().Promise:typeLiteral216:posts.
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts)

## Classes
### `AsyncCache`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts:229`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L229)
- signature: `class AsyncCache`
- members:
  - `<constructor>(ttlMs?: number)` — [`L233`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L233)
  - `clear(method)` — [`L259`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L259)
  - `get(method)` — [`L237`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L237)
  - `has(method)` — [`L263`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L263)
  - `cache` — [`L230`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L230)
  - `ttl` — [`L231`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L231)
- used by: (2 test-only callers)

### `EventEmitter`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts:145`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L145)
- signature: `class EventEmitter`
- members:
  - `emit(method)` — [`L169`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L169)
  - `emitAsync(method)` — [`L175`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L175)
  - `subscribe(method)` — [`L149`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L149)
  - `subscribeAsync(method)` — [`L159`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L159)
  - `asyncListeners` — [`L147`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L147)
  - `listeners` — [`L146`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L146)
- used by: (7 test-only callers)

### `PromisePool`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts:182`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L182)
- signature: `class PromisePool`
- members:
  - `<constructor>(concurrency?: number)` — [`L189`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L189)
  - `add(method)` — [`L193`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L193)
  - `execute(method)` — [`L197`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L197)
  - `concurrency` — [`L183`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L183)
  - `errors` — [`L187`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L187)
  - `errors` — [`L197`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L197)
  - `results` — [`L186`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L186)
  - `results` — [`L197`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L197)
  - `running` — [`L185`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L185)
  - `tasks` — [`L184`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L184)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (6 test-only callers)

### `Semaphore`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts:269`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L269)
- signature: `class Semaphore`
- members:
  - `<constructor>(permits: number)` — [`L273`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L273)
  - `acquire(method)` — [`L277`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L277)
  - `execute(method)` — [`L297`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L297)
  - `release(method)` — [`L288`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L288)
  - `permits` — [`L270`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L270)
  - `waiting` — [`L271`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L271)
- used by: (1 test-only callers)

### `TaskQueue`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts:308`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L308)
- signature: `class TaskQueue`
- members:
  - `<constructor>(processor: (item: T) => Promise<void>)` — [`L313`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L313)
  - `<get>isProcessing` — [`L343`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L343)
  - `<get>length` — [`L339`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L339)
  - `enqueue(method)` — [`L317`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L317)
  - `processQueue(method)` — [`L324`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L324)
  - `processing` — [`L310`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L310)
  - `processor` — [`L311`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L311)
  - `queue` — [`L309`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L309)
- used by: (2 test-only callers)

## Functions
- `asyncGenerator(count: number)` — [`L121`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L121)
- `batchProcessUsers(userIds: number[])` — [`L404`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L404)
- `consumeAsyncGenerator(generator: AsyncGenerator<T>)` — [`L136`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L136)
- `createPromise(value: T, delay?: number)` — [`L8`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L8) — Async and Promises
- `createRejectedPromise(error: string, delay?: number)` — [`L14`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L14)
- `fetchDataStream(urls: string[])` — [`L128`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L128)
- `fetchUserData(id: number)` — [`L21`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L21)
- `fetchUserPosts(userId: number)` — [`L36`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L36)
- `fetchUserProfile(userId: number)` — [`L387`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L387)
- `processInParallel(items: T[], processor: (item: T) => Promise<any>, concurrency?: number)` — [`L87`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L87)
- `processStream(items: T[], transformer: (item: T) => Promise<R>, batchSize?: number)` — [`L349`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L349)
- `raceWithTimeout(promise: Promise<T>, timeoutMs: number)` — [`L109`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L109)
- `retryOperation(operation: () => Promise<T>, maxRetries?: number, delay?: number)` — [`L61`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L61)
- `safeAsyncOperation(operation: () => Promise<T>)` — [`L47`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L47)

## Module values
- `asyncExamples` — [`L366`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L366)
- `email` — [`L21`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L21)
- `email` — [`L388`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L388)
- `id` — [`L21`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L21)
- `id` — [`L388`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L388)
- `name` — [`L21`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L21)
- `name` — [`L388`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L388)
- `posts` — [`L389`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L389)
- `user` — [`L388`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/async-promises.ts#L388)

