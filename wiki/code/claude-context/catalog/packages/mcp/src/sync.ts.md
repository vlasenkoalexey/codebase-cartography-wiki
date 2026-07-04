---
title: 'Module: packages/mcp/src/sync.ts'
type: catalog
provenance: extracted
module: packages/mcp/src/sync.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-mcp 0.1.15 src/`sync.ts`/
symbols:
  SyncManager.handleSyncIndex: SyncManager#handleSyncIndex().
  SyncManager.startBackgroundSync: SyncManager#startBackgroundSync().
  SyncManager.setupTriggerWatcher: SyncManager#setupTriggerWatcher().
  SyncManager.-constructor: SyncManager#`<constructor>`().
  SyncManager.acquireGlobalSyncLock: SyncManager#acquireGlobalSyncLock().
  getBackgroundSyncIntervalMs: getBackgroundSyncIntervalMs().
  SyncManager.triggerDebounceTimer: SyncManager#triggerDebounceTimer.
  SyncManager.getSyncLockStaleMs: SyncManager#getSyncLockStaleMs().
  SyncManager.releaseGlobalSyncLock: SyncManager#releaseGlobalSyncLock().
  SyncManager.stopTriggerWatcher: SyncManager#stopTriggerWatcher().
  SyncManager.snapshotManager: SyncManager#snapshotManager.
  SyncManager.syncLockToken: SyncManager#syncLockToken.
  SyncManager.triggerWatcher: SyncManager#triggerWatcher.
  DEFAULT_SYNC_INTERVAL_MS: DEFAULT_SYNC_INTERVAL_MS.
  DEFAULT_SYNC_LOCK_STALE_MS: DEFAULT_SYNC_LOCK_STALE_MS.
  SyncManager.isSyncing: SyncManager#isSyncing.
  DEFAULT_INITIAL_SYNC_DELAY_MS: DEFAULT_INITIAL_SYNC_DELAY_MS.
  SYNC_LOCK_STALE_ENV: SYNC_LOCK_STALE_ENV.
  SyncManager: SyncManager#
  SyncManager.context: SyncManager#context.
  SyncManager.getSyncLockPath: SyncManager#getSyncLockPath().
  MIN_SYNC_INTERVAL_MS: MIN_SYNC_INTERVAL_MS.
  isBackgroundSyncEnabled: isBackgroundSyncEnabled().
  SyncManager.isTriggerWatcherEnabled: SyncManager#isTriggerWatcherEnabled().
---
# Module: [`packages/mcp/src/sync.ts`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts)

## Classes
### `SyncManager`
- def: [`packages/mcp/src/sync.ts:59`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L59)
- signature: `class SyncManager`
- members:
  - `<constructor>(context: Context, snapshotManager: SnapshotManager)` — [`L67`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L67)
  - `acquireGlobalSyncLock(method)` — [`L91`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L91) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `getSyncLockPath(method)` — [`L72`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L72) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `getSyncLockStaleMs(method)` — [`L76`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L76) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `handleSyncIndex(method)` — [`L159`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L159) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `isTriggerWatcherEnabled(method)` — [`L318`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L318) — Read CLAUDE_CONTEXT_TRIGGER_WATCHER. Default ON — the watcher is cheap and only — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `releaseGlobalSyncLock(method)` — [`L140`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L140) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `setupTriggerWatcher(method)` — [`L335`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L335) — Watch for trigger file changes to enable instant re-index. — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `startBackgroundSync(method)` — [`L273`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L273) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `stopTriggerWatcher(method)` — [`L399`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L399) — Stop the watcher (idempotent). Useful for tests or graceful shutdown. — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `context` — [`L60`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L60) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `isSyncing` — [`L62`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L62) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `snapshotManager` — [`L61`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L61) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `syncLockToken` — [`L63`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L63) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `triggerDebounceTimer` — [`L65`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L65) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
  - `triggerWatcher` — [`L64`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L64) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- uses (calls/refs, reference-scoped): [`getIndexedCodebases`](snapshot.ts.md#SnapshotManager.getIndexedCodebases), [`getCodebaseInfo`](snapshot.ts.md#SnapshotManager.getCodebaseInfo), [`requestSplitter`](config.ts.md#CodebaseIndexOptions.requestSplitter), [`RequestSplitterType`](config.ts.md#RequestSplitterType), [`SnapshotManager`](snapshot.ts.md#SnapshotManager), [`requestCustomExtensions`](config.ts.md#CodebaseIndexOptions.requestCustomExtensions), [`requestIgnorePatterns`](config.ts.md#CodebaseIndexOptions.requestIgnorePatterns), [`resolveRequestSplitterType`](splitter.ts.md#resolveRequestSplitterType), [`createRequestSplitter`](splitter.ts.md#createRequestSplitter), [`getBackgroundSyncIntervalMs`](sync.ts.md#getBackgroundSyncIntervalMs), [`DEFAULT_SYNC_LOCK_STALE_MS`](sync.ts.md#DEFAULT_SYNC_LOCK_STALE_MS), [`DEFAULT_INITIAL_SYNC_DELAY_MS`](sync.ts.md#DEFAULT_INITIAL_SYNC_DELAY_MS), [`SYNC_LOCK_STALE_ENV`](sync.ts.md#SYNC_LOCK_STALE_ENV), [`isBackgroundSyncEnabled`](sync.ts.md#isBackgroundSyncEnabled)
- used by: [`<constructor>`](index.ts.md#ContextMcpServer.-constructor), [`originalConsoleWarn`](index.ts.md#originalConsoleWarn), [`start`](index.ts.md#ContextMcpServer.start), [`syncManager`](index.ts.md#ContextMcpServer.syncManager)

## Functions
- `getBackgroundSyncIntervalMs()` — [`L41`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L41) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- `isBackgroundSyncEnabled()` — [`L15`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L15) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)

## Module values
- `DEFAULT_INITIAL_SYNC_DELAY_MS` — [`L9`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L9) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- `DEFAULT_SYNC_INTERVAL_MS` — [`L10`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L10) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- `DEFAULT_SYNC_LOCK_STALE_MS` — [`L12`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L12) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- `MIN_SYNC_INTERVAL_MS` — [`L11`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L11) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)
- `SYNC_LOCK_STALE_ENV` — [`L13`](../../../../../../../raw/code/claude-context/packages/mcp/src/sync.ts#L13) — documented in [packages-mcp-src-sync.ts](../../../../concepts/packages-mcp-src-sync.ts.md)

