---
title: 'Module: src/utils.ts'
type: catalog
provenance: extracted
module: src/utils.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/`utils.ts`/
symbols:
  normalizePath: normalizePath().
  validatePathWithinRoot: validatePathWithinRoot().
  FileLock.acquire: FileLock#acquire().
  MemoryMonitor.start: MemoryMonitor#start().
  FileLock.release: FileLock#release().
  isConfigLeafNode: isConfigLeafNode().
  FileLock.lockPath: FileLock#lockPath.
  safeJsonParse: safeJsonParse().
  clamp: clamp().
  Mutex.withLock: Mutex#withLock().
  Mutex.acquire: Mutex#acquire().
  FileLock.withLock: FileLock#withLock().
  FileLock.withLockAsync: FileLock#withLockAsync().
  MemoryMonitor.-constructor: MemoryMonitor#`<constructor>`().
  validateProjectPath: validateProjectPath().
  FileLock: FileLock#
  Mutex.locked: Mutex#locked.
  MemoryMonitor.checkInterval: MemoryMonitor#checkInterval.
  MemoryMonitor.peakUsage: MemoryMonitor#peakUsage.
  FileLock.-constructor: FileLock#`<constructor>`().
  Mutex.isLocked: Mutex#isLocked().
  MemoryMonitor.stop: MemoryMonitor#stop().
  CONFIG_LEAF_LANGUAGES: CONFIG_LEAF_LANGUAGES.
  FileLock.held: FileLock#held.
  Mutex: Mutex#
  MemoryMonitor.onThresholdExceeded: MemoryMonitor#onThresholdExceeded.
  MemoryMonitor.getPeakUsage: MemoryMonitor#getPeakUsage().
  SENSITIVE_PATHS: SENSITIVE_PATHS.
  isConfigLeafNode.node-typeLiteral2.language: isConfigLeafNode().(node)typeLiteral2:language.
  isWithinDir: isWithinDir().
  Mutex.waitQueue: Mutex#waitQueue.
  MemoryMonitor.threshold: MemoryMonitor#threshold.
  isConfigLeafNode.node-typeLiteral2.kind: isConfigLeafNode().(node)typeLiteral2:kind.
  validatePathWithinRoot.options-typeLiteral9.allowSymlinkEscape: validatePathWithinRoot().(options)typeLiteral9:allowSymlinkEscape.
  FileLock.STALE_TIMEOUT_MS: FileLock#STALE_TIMEOUT_MS.
  FileLock.isProcessAlive: FileLock#isProcessAlive().
  processInBatches: processInBatches().
  debounce: debounce().
  throttle: throttle().
  MemoryMonitor: MemoryMonitor#
  readFileInChunks: readFileInChunks().
  estimateSize: estimateSize().
  MemoryMonitor.getCurrentUsage: MemoryMonitor#getCurrentUsage().
---
# Module: [`src/utils.ts`](../../../../../raw/code/codegraph/src/utils.ts)

## Classes
### `FileLock`
- def: [`src/utils.ts:223`](../../../../../raw/code/codegraph/src/utils.ts#L223) — documented in [utils.ts](../../concepts/utils.ts.md)
- doc: Cross-process file lock using a lock file with PID tracking.
- signature: `class FileLock`
- members:
  - `<constructor>(lockPath: string)` — [`L230`](../../../../../raw/code/codegraph/src/utils.ts#L230) — Cross-process file lock using a lock file with PID tracking.
  - `acquire(method)` — [`L237`](../../../../../raw/code/codegraph/src/utils.ts#L237) — Acquire the lock. Throws if the lock is held by another live process. — documented in [utils.ts](../../concepts/utils.ts.md)
  - `isProcessAlive(method)` — [`L325`](../../../../../raw/code/codegraph/src/utils.ts#L325) — Check if a process is still running — documented in [utils.ts](../../concepts/utils.ts.md)
  - `release(method)` — [`L284`](../../../../../raw/code/codegraph/src/utils.ts#L284) — Release the lock
  - `withLock(method)` — [`L301`](../../../../../raw/code/codegraph/src/utils.ts#L301) — Execute a function while holding the lock — documented in [utils.ts](../../concepts/utils.ts.md)
  - `withLockAsync(method)` — [`L313`](../../../../../raw/code/codegraph/src/utils.ts#L313) — Execute an async function while holding the lock — documented in [utils.ts](../../concepts/utils.ts.md)
  - `STALE_TIMEOUT_MS` — [`L228`](../../../../../raw/code/codegraph/src/utils.ts#L228) — Locks older than this are considered stale regardless of PID status — documented in [utils.ts](../../concepts/utils.ts.md)
  - `held` — [`L225`](../../../../../raw/code/codegraph/src/utils.ts#L225) — documented in [utils.ts](../../concepts/utils.ts.md)
  - `lockPath` — [`L224`](../../../../../raw/code/codegraph/src/utils.ts#L224) — documented in [utils.ts](../../concepts/utils.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](index.ts.md#CodeGraph.indexAll), [`sync`](index.ts.md#CodeGraph.sync), [`watcher`](index.ts.md#CodeGraph.watcher), [`healSegmentVocabIfEmpty`](index.ts.md#CodeGraph.healSegmentVocabIfEmpty), [`indexFiles`](index.ts.md#CodeGraph.indexFiles), [`close`](index.ts.md#CodeGraph.close), [`fileLock`](index.ts.md#CodeGraph.fileLock)

### `MemoryMonitor`
- def: [`src/utils.ts:551`](../../../../../raw/code/codegraph/src/utils.ts#L551)
- doc: Memory monitor for tracking usage during operations
- signature: `class MemoryMonitor`
- members:
  - `<constructor>(thresholdMB?: number, onThresholdExceeded?: ((usage: number) => void) | undefined)` — [`L557`](../../../../../raw/code/codegraph/src/utils.ts#L557) — Memory monitor for tracking usage during operations
  - `getCurrentUsage(method)` — [`L603`](../../../../../raw/code/codegraph/src/utils.ts#L603) — Get current memory usage in bytes
  - `getPeakUsage(method)` — [`L596`](../../../../../raw/code/codegraph/src/utils.ts#L596) — Get peak memory usage in bytes
  - `start(method)` — [`L568`](../../../../../raw/code/codegraph/src/utils.ts#L568) — Start monitoring memory usage — documented in [utils.ts](../../concepts/utils.ts.md)
  - `stop(method)` — [`L586`](../../../../../raw/code/codegraph/src/utils.ts#L586) — Stop monitoring — documented in [utils.ts](../../concepts/utils.ts.md)
  - `checkInterval` — [`L552`](../../../../../raw/code/codegraph/src/utils.ts#L552) — documented in [utils.ts](../../concepts/utils.ts.md)
  - `onThresholdExceeded` — [`L555`](../../../../../raw/code/codegraph/src/utils.ts#L555) — documented in [utils.ts](../../concepts/utils.ts.md)
  - `peakUsage` — [`L553`](../../../../../raw/code/codegraph/src/utils.ts#L553) — documented in [utils.ts](../../concepts/utils.ts.md)
  - `threshold` — [`L554`](../../../../../raw/code/codegraph/src/utils.ts#L554) — documented in [utils.ts](../../concepts/utils.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts)

### `Mutex`
- def: [`src/utils.ts:375`](../../../../../raw/code/codegraph/src/utils.ts#L375)
- doc: Simple mutex lock for preventing concurrent operations
- signature: `class Mutex`
- members:
  - `acquire(method)` — [`L384`](../../../../../raw/code/codegraph/src/utils.ts#L384) — Acquire the lock
  - `isLocked(method)` — [`L417`](../../../../../raw/code/codegraph/src/utils.ts#L417) — Check if the lock is currently held
  - `withLock(method)` — [`L405`](../../../../../raw/code/codegraph/src/utils.ts#L405) — Execute a function while holding the lock
  - `locked` — [`L376`](../../../../../raw/code/codegraph/src/utils.ts#L376)
  - `waitQueue` — [`L377`](../../../../../raw/code/codegraph/src/utils.ts#L377)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](index.ts.md#CodeGraph.indexAll), [`sync`](index.ts.md#CodeGraph.sync), [`healSegmentVocabIfEmpty`](index.ts.md#CodeGraph.healSegmentVocabIfEmpty), [`indexFiles`](index.ts.md#CodeGraph.indexFiles), [`indexMutex`](index.ts.md#CodeGraph.indexMutex), [`isIndexing`](index.ts.md#CodeGraph.isIndexing)

## Functions
- `clamp(value: number, min: number, max: number)` — [`L205`](../../../../../raw/code/codegraph/src/utils.ts#L205) — Clamp a numeric value to a range.
- `debounce(...args: unknown[])` — [`L453`](../../../../../raw/code/codegraph/src/utils.ts#L453) — Debounce a function
- `estimateSize(obj: unknown)` — [`L511`](../../../../../raw/code/codegraph/src/utils.ts#L511) — Estimate memory usage of an object (rough approximation)
- `isConfigLeafNode(node: { kind: string; language?: string | undefined; })` — [`L64`](../../../../../raw/code/codegraph/src/utils.ts#L64) — A config-leaf node is a single key lifted out of a pure config/data file —
- `isWithinDir(child: string, parent: string)` — [`L73`](../../../../../raw/code/codegraph/src/utils.ts#L73) — Whether `child` is `parent` itself or sits underneath it. Case-insensitive on — documented in [utils.ts](../../concepts/utils.ts.md)
- `normalizePath(filePath: string)` — [`L213`](../../../../../raw/code/codegraph/src/utils.ts#L213) — Normalize a file path to use forward slashes. — documented in [sync-watcher.ts](../../concepts/sync-watcher.ts.md)
- `processInBatches(items: T[], batchSize: number, processor: (item: T, index: number) => Promise<R>, onBatchComplete?: ((completed: number, total: number) => void) | undefined)` — [`L344`](../../../../../raw/code/codegraph/src/utils.ts#L344) — Process items in batches to manage memory
- `readFileInChunks(filePath: string, chunkSize?: number)` — [`L427`](../../../../../raw/code/codegraph/src/utils.ts#L427) — Chunked file reader for large files
- `safeJsonParse(value: string, fallback: T)` — [`L193`](../../../../../raw/code/codegraph/src/utils.ts#L193) — Safely parse JSON with a fallback value.
- `throttle(...args: unknown[])` — [`L477`](../../../../../raw/code/codegraph/src/utils.ts#L477) — Throttle a function
- `validatePathWithinRoot(projectRoot: string, filePath: string, options?: { allowSymlinkEscape?: boolean | undefined; } | undefined)` — [`L110`](../../../../../raw/code/codegraph/src/utils.ts#L110) — Validate that a file path stays within the project root, resolving symlinks. — documented in [utils.ts](../../concepts/utils.ts.md)
- `validateProjectPath(dirPath: string)` — [`L158`](../../../../../raw/code/codegraph/src/utils.ts#L158) — Validate that a path is a safe project root directory.

## Module values
- `CONFIG_LEAF_LANGUAGES` — [`L53`](../../../../../raw/code/codegraph/src/utils.ts#L53) — Config "languages" whose nodes are pure key/value DATA lifted from a config
- `SENSITIVE_PATHS` — [`L43`](../../../../../raw/code/codegraph/src/utils.ts#L43) — Sensitive system directories that should never be used as project roots.
- `allowSymlinkEscape` — [`L113`](../../../../../raw/code/codegraph/src/utils.ts#L113) — documented in [utils.ts](../../concepts/utils.ts.md)
- `kind` — [`L64`](../../../../../raw/code/codegraph/src/utils.ts#L64)
- `language` — [`L64`](../../../../../raw/code/codegraph/src/utils.ts#L64)

