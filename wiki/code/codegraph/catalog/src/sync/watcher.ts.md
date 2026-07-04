---
title: 'Module: src/sync/watcher.ts'
type: catalog
provenance: extracted
module: src/sync/watcher.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/sync/`watcher.ts`/
symbols:
  FileWatcher.start: FileWatcher#start().
  FileWatcher.watchTree: FileWatcher#watchTree().
  FileWatcher.flush: FileWatcher#flush().
  FileWatcher.stop: FileWatcher#stop().
  FileWatcher.-constructor: FileWatcher#`<constructor>`().
  FileWatcher.handleChange: FileWatcher#handleChange().
  FileWatcher.startRecursive: FileWatcher#startRecursive().
  FileWatcher.getPendingFiles: FileWatcher#getPendingFiles().
  FileWatcher.degrade: FileWatcher#degrade().
  FileWatcher.handleDirEvent: FileWatcher#handleDirEvent().
  FileWatcher.shouldIgnoreDir: FileWatcher#shouldIgnoreDir().
  FileWatcher.projectRoot: FileWatcher#projectRoot.
  PendingFile: PendingFile#
  FileWatcher.warnInotifyLimit: FileWatcher#warnInotifyLimit().
  FileWatcher.isActive: FileWatcher#isActive().
  FileWatcher.dirWatchers: FileWatcher#dirWatchers.
  FileWatcher.debounceTimer: FileWatcher#debounceTimer.
  FileWatcher.pendingFiles: FileWatcher#pendingFiles.
  FileWatcher.scheduleSync: FileWatcher#scheduleSync().
  FileWatcher.lockRetryCount: FileWatcher#lockRetryCount.
  FileWatcher.syncFailureRetryCount: FileWatcher#syncFailureRetryCount.
  FileWatcher.ignoreMatcher: FileWatcher#ignoreMatcher.
  WatchOptions: WatchOptions#
  FileWatcher.stopped: FileWatcher#stopped.
  FileWatcher.recursiveWatcher: FileWatcher#recursiveWatcher.
  FileWatcher.degradedReason: FileWatcher#degradedReason.
  FileWatcher.onSyncComplete: FileWatcher#onSyncComplete.
  FileWatcher.onSyncError: FileWatcher#onSyncError.
  FileWatcher.onDegraded: FileWatcher#onDegraded.
  FileWatcher.startPerDirectory: FileWatcher#startPerDirectory().
  FileWatcher.ingestEventForTests: FileWatcher#ingestEventForTests().
  FileWatcher.waitUntilReady: FileWatcher#waitUntilReady().
  FileWatcher.scheduleRetrySync: FileWatcher#scheduleRetrySync().
  watchImpl: watchImpl.
  liveWatchersForTests: liveWatchersForTests.
  __setFsWatchForTests: __setFsWatchForTests().
  PendingFile.path: PendingFile#path.
  FileWatcher: FileWatcher#
  FileWatcher.readyWaiters: FileWatcher#readyWaiters.
  __emitWatchEventForTests: __emitWatchEventForTests().
  maxDirWatches: maxDirWatches().
  FileWatcher.isAlwaysIgnored: FileWatcher#isAlwaysIgnored().
  EXHAUSTION_REASON: EXHAUSTION_REASON.
  isWatchResourceExhaustion: isWatchResourceExhaustion().
  LockUnavailableError: LockUnavailableError#
  PendingFile.lastSeenMs: PendingFile#lastSeenMs.
  FileWatcher.inotifyLimitWarned: FileWatcher#inotifyLimitWarned.
  FileWatcher.inert: FileWatcher#inert.
  FileWatcher.syncing: FileWatcher#syncing.
  FileWatcher.ready: FileWatcher#ready.
  FileWatcher.debounceMs: FileWatcher#debounceMs.
  FileWatcher.unwatchDir: FileWatcher#unwatchDir().
  FileWatcher.isDegraded: FileWatcher#isDegraded().
  FileWatcher.getDegradedReason: FileWatcher#getDegradedReason().
  PendingFile.indexing: PendingFile#indexing.
  FileWatcher.dirCapWarned: FileWatcher#dirCapWarned.
  FileWatcher.syncStartedMs: FileWatcher#syncStartedMs.
  FileWatcher.inertForTests: FileWatcher#inertForTests.
  isInotifyWatchExhaustion: isInotifyWatchExhaustion().
  supportsRecursiveWatch: supportsRecursiveWatch().
  WatchFn: WatchFn#
  IS_TEST_RUNTIME: IS_TEST_RUNTIME.
  WatchOptions.onSyncComplete: WatchOptions#onSyncComplete.
  WatchOptions.onSyncError: WatchOptions#onSyncError.
  WatchOptions.onDegraded: WatchOptions#onDegraded.
  FileWatcher.syncFn: FileWatcher#syncFn.
  MAX_LOCK_RETRIES: MAX_LOCK_RETRIES.
  MAX_SYNC_FAILURE_RETRIES: MAX_SYNC_FAILURE_RETRIES.
  MAX_RETRY_BACKOFF_MS: MAX_RETRY_BACKOFF_MS.
  INOTIFY_LIMIT_REASON: INOTIFY_LIMIT_REASON.
  DEFAULT_MAX_DIR_WATCHES: DEFAULT_MAX_DIR_WATCHES.
  WatchOptions.debounceMs: WatchOptions#debounceMs.
  WatchOptions.inertForTests: WatchOptions#inertForTests.
  LockUnavailableError.-constructor: LockUnavailableError#`<constructor>`().
  PendingFile.firstSeenMs: PendingFile#firstSeenMs.
---
# Module: [`src/sync/watcher.ts`](../../../../../../raw/code/codegraph/src/sync/watcher.ts)

## Classes
### `FileWatcher`
- def: [`src/sync/watcher.ts:247`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L247)
- doc: FileWatcher monitors a project directory for changes and triggers
- signature: `class FileWatcher`
- members:
  - `<constructor>(projectRoot: string, syncFn: () => Promise<{ filesChanged: number; durationMs: number; }>, options?: WatchOptions)` — [`L323`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L323) — FileWatcher monitors a project directory for changes and triggers
  - `degrade(method)` — [`L613`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L613) — Permanently disable live watching after a terminal runtime failure — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `flush(method)` — [`L772`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L772) — Flush pending changes by running sync. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `getDegradedReason(method)` — [`L646`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L646) — The reason live watching degraded, or null if it is healthy.
  - `getPendingFiles(method)` — [`L885`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L885) — Snapshot of files seen by the watcher since the last successful sync.
  - `handleChange(method)` — [`L550`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L550) — Shared change handler for both watch strategies. `rel` is a — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `handleDirEvent(method)` — [`L520`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L520) — Linux per-directory event handler. `filename` is relative to `dir`. A new — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `ingestEventForTests(method)` — [`L699`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L699) — documented in [utils.ts](../../../concepts/utils.ts.md)
  - `isActive(method)` — [`L706`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L706) — Whether the watcher is currently active.
  - `isAlwaysIgnored(method)` — [`L582`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L582) — Our own dirs are always ignored, regardless of .gitignore.
  - `isDegraded(method)` — [`L641`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L641) — Whether live watching has degraded permanently (until the next start()).
  - `scheduleRetrySync(method)` — [`L750`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L750) — Schedule a retry after a recoverable sync failure (lock contention). Kept — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `scheduleSync(method)` — [`L735`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L735) — Schedule a normal debounced sync after a source edit. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `shouldIgnoreDir(method)` — [`L598`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L598) — True for any directory that should NOT be watched (used while building the — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `start(method)` — [`L341`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L341) — Start watching for file changes. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `startPerDirectory(method)` — [`L436`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L436) — Linux: walk the (non-ignored) tree and watch each directory. One inotify — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `startRecursive(method)` — [`L413`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L413) — macOS/Windows: one recursive watcher for the whole tree. O(1) descriptors. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `stop(method)` — [`L653`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L653) — Stop watching for file changes. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `unwatchDir(method)` — [`L569`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L569) — Close and forget the watch for a directory that errored/was removed.
  - `waitUntilReady(method)` — [`L719`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L719) — Resolves once the watch set has been installed (or immediately if it
  - `warnInotifyLimit(method)` — [`L629`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L629) — Warn ONCE that the Linux inotify watch budget is exhausted (ENOSPC), and — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `watchTree(method)` — [`L449`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L449) — Add an inotify watch for `dir` and recurse into its non-ignored — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `debounceMs` — [`L316`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L316)
  - `debounceTimer` — [`L275`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L275) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `degradedReason` — [`L268`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L268) — One-way latch: the reason live watching was permanently disabled at runtime — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `dirCapWarned` — [`L253`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L253) — Set once the per-directory watch cap is hit, so we log only once.
  - `dirWatchers` — [`L251`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L251) — Linux: one watcher per watched directory (keyed by absolute path). — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `ignoreMatcher` — [`L313`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L313) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `inert` — [`L274`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L274) — Test-only inert mode: started, but with no OS watcher installed.
  - `inertForTests` — [`L321`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L321)
  - `inotifyLimitWarned` — [`L261`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L261) — Set once the Linux inotify watch limit (ENOSPC) is hit. Double duty: we
  - `lockRetryCount` — [`L270`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L270) — Consecutive lock-contention retries for watcher-triggered syncs. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `onDegraded` — [`L320`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L320) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `onSyncComplete` — [`L318`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L318) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `onSyncError` — [`L319`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L319) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `pendingFiles` — [`L283`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L283) — Files seen by the watcher since the last successful sync — populated on — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `projectRoot` — [`L315`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L315)
  - `ready` — [`L301`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L301) — True once the initial watch set is established. Unlike the previous
  - `readyWaiters` — [`L307`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L307) — Callbacks that resolve when the watch set is established. Used by tests
  - `recursiveWatcher` — [`L249`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L249) — macOS/Windows: the single recursive watcher. Null on Linux.
  - `stopped` — [`L292`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L292)
  - `syncFailureRetryCount` — [`L272`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L272) — Consecutive generic (non-lock) sync failures; reset only by a clean sync. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `syncFn` — [`L317`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L317)
  - `syncStartedMs` — [`L290`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L290) — Wall-clock ms at which the in-flight sync began. Combined with
  - `syncing` — [`L291`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L291)
- uses (calls/refs, reference-scoped): [`logDebug`](../errors.ts.md#logDebug), [`logWarn`](../errors.ts.md#logWarn), [`isSourceFile`](../extraction/grammars.ts.md#isSourceFile), [`normalizePath`](../utils.ts.md#normalizePath), [`watchDisabledReason`](watch-policy.ts.md#watchDisabledReason), [`loadExtensionOverrides`](../project-config.ts.md#loadExtensionOverrides), [`buildScopeIgnore`](../extraction/index.ts.md#buildScopeIgnore), [`ignores`](../extraction/index.ts.md#ScopeIgnore.ignores), [`PendingFile`](watcher.ts.md#PendingFile), [`isCodeGraphDataDir`](../directory.ts.md#isCodeGraphDataDir), [`WatchOptions`](watcher.ts.md#WatchOptions), [`liveWatchersForTests`](watcher.ts.md#liveWatchersForTests), [`watchImpl`](watcher.ts.md#watchImpl), [`path`](watcher.ts.md#PendingFile.path), [`maxDirWatches`](watcher.ts.md#maxDirWatches), [`LockUnavailableError`](watcher.ts.md#LockUnavailableError), [`EXHAUSTION_REASON`](watcher.ts.md#EXHAUSTION_REASON), [`isWatchResourceExhaustion`](watcher.ts.md#isWatchResourceExhaustion), [`lastSeenMs`](watcher.ts.md#PendingFile.lastSeenMs), [`ScopeIgnore`](../extraction/index.ts.md#ScopeIgnore), [`indexing`](watcher.ts.md#PendingFile.indexing), [`IS_TEST_RUNTIME`](watcher.ts.md#IS_TEST_RUNTIME), [`isInotifyWatchExhaustion`](watcher.ts.md#isInotifyWatchExhaustion), [`onDegraded`](watcher.ts.md#WatchOptions.onDegraded), [`onSyncComplete`](watcher.ts.md#WatchOptions.onSyncComplete), [`onSyncError`](watcher.ts.md#WatchOptions.onSyncError), [`supportsRecursiveWatch`](watcher.ts.md#supportsRecursiveWatch), [`INOTIFY_LIMIT_REASON`](watcher.ts.md#INOTIFY_LIMIT_REASON), [`MAX_LOCK_RETRIES`](watcher.ts.md#MAX_LOCK_RETRIES), [`MAX_RETRY_BACKOFF_MS`](watcher.ts.md#MAX_RETRY_BACKOFF_MS), [`MAX_SYNC_FAILURE_RETRIES`](watcher.ts.md#MAX_SYNC_FAILURE_RETRIES), [`debounceMs`](watcher.ts.md#WatchOptions.debounceMs), [`firstSeenMs`](watcher.ts.md#PendingFile.firstSeenMs), [`inertForTests`](watcher.ts.md#WatchOptions.inertForTests)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`watcher`](../index.ts.md#CodeGraph.watcher), [`watch`](../index.ts.md#CodeGraph.watch), [`getPendingFiles`](../index.ts.md#CodeGraph.getPendingFiles), [`getWatcherDegradedReason`](../index.ts.md#CodeGraph.getWatcherDegradedReason), [`isWatcherDegraded`](../index.ts.md#CodeGraph.isWatcherDegraded), [`unwatch`](../index.ts.md#CodeGraph.unwatch), [`liveWatchersForTests`](watcher.ts.md#liveWatchersForTests), [`__emitWatchEventForTests`](watcher.ts.md#__emitWatchEventForTests), [`isWatching`](../index.ts.md#CodeGraph.isWatching), [`waitUntilWatcherReady`](../index.ts.md#CodeGraph.waitUntilWatcherReady)

### `LockUnavailableError`  ·  implements/extends Error
- def: [`src/sync/watcher.ts:206`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L206)
- doc: Thrown by a `syncFn` to signal that the underlying sync couldn't acquire
- signature: `class LockUnavailableError`
- members:
  - `<constructor>(message?: string)` — [`L207`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L207) — Thrown by a `syncFn` to signal that the underlying sync couldn't acquire
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`flush`](watcher.ts.md#FileWatcher.flush), [`watch`](../index.ts.md#CodeGraph.watch)

### `PendingFile`
- def: [`src/sync/watcher.ts:218`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L218)
- doc: Per-file pending entry — tracks a source file the watcher saw an event for
- signature: `interface PendingFile`
- members:
  - `firstSeenMs` — [`L222`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L222) — Wall-clock ms at the first event we saw for this path since the last sync.
  - `indexing` — [`L230`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L230) — True when a sync is currently in flight that began AFTER this file's most
  - `lastSeenMs` — [`L224`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L224) — Wall-clock ms at the most recent event we saw for this path.
  - `path` — [`L220`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L220) — Project-relative POSIX path (e.g. "src/foo.ts").
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`tools.ts`](../mcp/tools.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-tools.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`handleStatus`](../mcp/tools.ts.md#ToolHandler.handleStatus), [`withStalenessNotice`](../mcp/tools.ts.md#ToolHandler.withStalenessNotice), [`getPendingFiles`](watcher.ts.md#FileWatcher.getPendingFiles), [`formatStaleBanner`](../mcp/tools.ts.md#formatStaleBanner), [`getPendingFiles`](../index.ts.md#CodeGraph.getPendingFiles), [`formatStaleFooter`](../mcp/tools.ts.md#formatStaleFooter)

### `WatchFn`
- def: [`src/sync/watcher.ts:120`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L120)
- doc: Indirection over `fs.watch` so tests can inject a fake that throws or emits
- signature: `type WatchFn`
- used by: [`watchImpl`](watcher.ts.md#watchImpl), [`__setFsWatchForTests`](watcher.ts.md#__setFsWatchForTests)

### `WatchOptions`
- def: [`src/sync/watcher.ts:160`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L160)
- doc: Options for the file watcher
- signature: `interface WatchOptions`
- members:
  - `debounceMs` — [`L166`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L166) — Debounce delay in milliseconds.
  - `inertForTests` — [`L196`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L196) — Test-only. When true, `start()` installs NO OS-level fs.watch — the
  - `onDegraded` — [`L186`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L186) — Callback fired ONCE when live watching degrades permanently and auto-sync
  - `onSyncComplete` — [`L171`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L171) — Callback when a sync completes (for logging/diagnostics).
  - `onSyncError` — [`L176`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L176) — Callback when a sync errors (for logging/diagnostics).
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-index.ts), [`<constructor>`](watcher.ts.md#FileWatcher.-constructor), [`watch`](../index.ts.md#CodeGraph.watch), [`onDegraded`](watcher.ts.md#FileWatcher.onDegraded), [`onSyncComplete`](watcher.ts.md#FileWatcher.onSyncComplete), [`onSyncError`](watcher.ts.md#FileWatcher.onSyncError)

## Functions
- `__emitWatchEventForTests(projectRoot: string, relPath: string)` — [`L907`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L907) — Test-only: synthesize a source-file change for the live watcher running at
- `__setFsWatchForTests(fn: any)` — [`L124`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L124)
- `isInotifyWatchExhaustion(err: unknown)` — [`L101`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L101) — True when an error is Linux inotify *watch-count* exhaustion. `fs.watch`
- `isWatchResourceExhaustion(err: unknown)` — [`L85`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L85) — True when an error is OS watch/file-descriptor exhaustion (EMFILE/ENFILE).
- `maxDirWatches()` — [`L138`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L138) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `supportsRecursiveWatch()` — [`L110`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L110) — Native recursive `fs.watch` is only reliable on macOS and Windows; on Linux

## Module values
- `DEFAULT_MAX_DIR_WATCHES` — [`L136`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L136) — Upper bound on simultaneously-watched directories on the Linux per-directory
- `EXHAUSTION_REASON` — [`L63`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L63) — Actionable degrade message; both exhaustion paths share it verbatim. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `INOTIFY_LIMIT_REASON` — [`L73`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L73) — Actionable, NON-fatal warning for Linux inotify watch-count exhaustion.
- `IS_TEST_RUNTIME` — [`L155`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L155)
- `MAX_LOCK_RETRIES` — [`L48`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L48) — Number of consecutive lock-contention retries the watcher tolerates before
- `MAX_RETRY_BACKOFF_MS` — [`L60`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L60) — Cap on the exponential retry backoff (either mode) so it never sleeps absurdly long.
- `MAX_SYNC_FAILURE_RETRIES` — [`L58`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L58) — Number of consecutive GENERIC (non-lock) sync failures the watcher tolerates
- `liveWatchersForTests` — [`L154`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L154) — Test seam (see {@link __emitWatchEventForTests}). Maps a watcher's project
- `watchImpl` — [`L121`](../../../../../../raw/code/codegraph/src/sync/watcher.ts#L121)

