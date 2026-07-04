---
title: 'Module: tree_sitter_analyzer/file_watcher.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/file_watcher.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.file_watcher`/
symbols:
  FileWatcherDaemon.get_stats: FileWatcherDaemon#get_stats().
  FileWatcherDaemon._do_sync: FileWatcherDaemon#_do_sync().
  FileWatcherDaemon._enqueue: FileWatcherDaemon#_enqueue().
  FileWatcherDaemon._run_watchdog: FileWatcherDaemon#_run_watchdog().
  FileWatcherDaemon.start: FileWatcherDaemon#start().
  FileWatcherDaemon._run_polling: FileWatcherDaemon#_run_polling().
  FileWatcherDaemon._flush_pending: FileWatcherDaemon#_flush_pending().
  FileWatcherDaemon.stop: FileWatcherDaemon#stop().
  WatcherStats.to_dict: WatcherStats#to_dict().
  FileWatcherDaemon._take_snapshot: FileWatcherDaemon#_take_snapshot().
  FileWatcherDaemon._detect_changes: FileWatcherDaemon#_detect_changes().
  FileWatcherDaemon._stats: FileWatcherDaemon#_stats.
  FileWatcherDaemon._thread: FileWatcherDaemon#_thread.
  FileWatcherDaemon._run_loop: FileWatcherDaemon#_run_loop().
  FileWatcherDaemon: FileWatcherDaemon#
  FileWatcherDaemon._debounce_timer: FileWatcherDaemon#_debounce_timer.
  WatcherEvent.to_dict: WatcherEvent#to_dict().
  FileWatcherDaemon.is_running: FileWatcherDaemon#is_running().
  FileWatcherDaemon._stop_event: FileWatcherDaemon#_stop_event.
  logger: logger.
  FileWatcherDaemon.__init__: FileWatcherDaemon#__init__().
  _WatchdogHandler.dispatch: _WatchdogHandler#dispatch().
  FileWatcherDaemon.poll_interval: FileWatcherDaemon#poll_interval().
  FileWatcherDaemon.backend: FileWatcherDaemon#backend().
  WatcherStats.events_processed: WatcherStats#events_processed.
  WatcherStats.syncs_triggered: WatcherStats#syncs_triggered.
  WatcherStats.last_sync_at: WatcherStats#last_sync_at.
  WatcherStats.errors: WatcherStats#errors.
  FileWatcherDaemon._stats_lock: FileWatcherDaemon#_stats_lock.
  FileWatcherDaemon._snapshot: FileWatcherDaemon#_snapshot.
  FileWatcherDaemon._sync: FileWatcherDaemon#_sync.
  FileWatcherDaemon._cache: FileWatcherDaemon#_cache.
  FileWatcherDaemon._backend: FileWatcherDaemon#_backend.
  FileWatcherDaemon._started_at: FileWatcherDaemon#_started_at.
  FileWatcherDaemon._pending: FileWatcherDaemon#_pending.
  _WatchdogHandler: _WatchdogHandler#
  FileWatcherDaemon.trigger_sync: FileWatcherDaemon#trigger_sync().
  _WatchdogHandler.__init__: _WatchdogHandler#__init__().
  WatcherStats: WatcherStats#
  WatcherStats.uptime_seconds: WatcherStats#uptime_seconds.
  FileWatcherDaemon._poll_interval: FileWatcherDaemon#_poll_interval.
  FileWatcherDaemon._on_sync: FileWatcherDaemon#_on_sync.
  FileWatcherDaemon._pending_lock: FileWatcherDaemon#_pending_lock.
  FileWatcherDaemon._snapshot_lock: FileWatcherDaemon#_snapshot_lock.
  _DEFAULT_DEBOUNCE_SEC: _DEFAULT_DEBOUNCE_SEC.
  _DEFAULT_POLL_INTERVAL_SEC: _DEFAULT_POLL_INTERVAL_SEC.
  WatcherEvent.timestamp: WatcherEvent#timestamp.
  WatcherEvent.file_path: WatcherEvent#file_path.
  WatcherEvent.event_type: WatcherEvent#event_type.
  FileWatcherDaemon._debounce: FileWatcherDaemon#_debounce.
  WatcherEvent: WatcherEvent#
  _WatchdogHandler.__slots__: _WatchdogHandler#__slots__.
---
# Module: [`tree_sitter_analyzer/file_watcher.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py)

## Classes
### `FileWatcherDaemon`
- def: [`tree_sitter_analyzer/file_watcher.py:67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L67)
- doc: Background file watcher that triggers incremental AST cache syncs.
- signature: `class FileWatcherDaemon:`
- members:
  - `backend(self)` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L123) — Public accessor for _backend.
  - `get_stats(self)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L152)
  - `is_running(self)` — [`L149`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L149)
  - `poll_interval(self)` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L118) — Public accessor for _poll_interval.
  - `start(self)` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L127)
  - `stop(self, timeout: float = 5)` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L140)
  - `trigger_sync(self)` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L164)
- protocol/private: `__init__`[`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L87), `_backend`[`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L100), `_cache`[`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L96), `_debounce`[`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L99), `_debounce_timer`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L109), `_detect_changes`[`L230`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L230), `_do_sync`[`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L288), `_enqueue`[`L261`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L261), `_flush_pending`[`L273`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L273), `_on_sync`[`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L101), `_pending`[`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L107), `_pending_lock`[`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L108), `_poll_interval`[`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L98), `_run_loop`[`L167`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L167), `_run_polling`[`L173`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L173), `_run_watchdog`[`L184`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L184), `_snapshot`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L114), `_snapshot_lock`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L115), `_started_at`[`L105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L105), `_stats`[`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L111), `_stats_lock`[`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L112), `_stop_event`[`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L104), `_sync`[`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L97), `_take_snapshot`[`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L210), `_thread`[`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L103)
- uses (calls/refs, reference-scoped): [`EXT_TO_LANG`](_lang_extension_map.md#EXT_TO_LANG.EXT_TO_LANG), [`sync`](incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](incremental_sync.md#IncrementalSync), [`to_dict`](incremental_sync.md#SyncResult.to_dict), [`to_dict`](file_watcher.md#WatcherStats.to_dict), [`logger`](file_watcher.md#logger), [`errors`](file_watcher.md#WatcherStats.errors), [`events_processed`](file_watcher.md#WatcherStats.events_processed), [`last_sync_at`](file_watcher.md#WatcherStats.last_sync_at), [`syncs_triggered`](file_watcher.md#WatcherStats.syncs_triggered), [`_WatchdogHandler`](file_watcher.md#_WatchdogHandler), [`WatcherStats`](file_watcher.md#WatcherStats), [`uptime_seconds`](file_watcher.md#WatcherStats.uptime_seconds), [`_DEFAULT_DEBOUNCE_SEC`](file_watcher.md#_DEFAULT_DEBOUNCE_SEC), [`_DEFAULT_POLL_INTERVAL_SEC`](file_watcher.md#_DEFAULT_POLL_INTERVAL_SEC)
- used by: [`run_watch_health`](health_homeostasis.md#run_watch_health), [`_watcher`](mcp/tools/ast_cache_tool.md#ASTCacheTool._watcher), [`_handle_watch_start`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_watch_start), [`_on_project_root_changed`](mcp/tools/ast_cache_tool.md#ASTCacheTool._on_project_root_changed), [`_handle_watch_stop`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_watch_stop), [`_handle_watch_status`](mcp/tools/ast_cache_tool.md#ASTCacheTool._handle_watch_status)  (3 test-only)

### `WatcherEvent`
- def: [`tree_sitter_analyzer/file_watcher.py:36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L36)
- signature: `class WatcherEvent:`
- members:
  - `to_dict(self)` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L41)
  - `event_type` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L39)
  - `file_path` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L38)
  - `timestamp` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L37)

### `WatcherStats`
- def: [`tree_sitter_analyzer/file_watcher.py:50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L50)
- signature: `class WatcherStats:`
- members:
  - `to_dict(self)` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L57)
  - `errors` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L54)
  - `events_processed` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L51)
  - `last_sync_at` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L53)
  - `syncs_triggered` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L52)
  - `uptime_seconds` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L55)
- used by: [`get_stats`](file_watcher.md#FileWatcherDaemon.get_stats), [`_do_sync`](file_watcher.md#FileWatcherDaemon._do_sync), [`_enqueue`](file_watcher.md#FileWatcherDaemon._enqueue), [`_stats`](file_watcher.md#FileWatcherDaemon._stats)

### `_WatchdogHandler`
- def: [`tree_sitter_analyzer/file_watcher.py:302`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L302)
- members:
  - `dispatch(self, event: Any)` — [`L308`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L308)
- protocol/private: `__init__`[`L305`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L305), `__slots__`[`L303`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L303)
- uses (calls/refs, reference-scoped): [`EXT_TO_LANG`](_lang_extension_map.md#EXT_TO_LANG.EXT_TO_LANG)
- used by: [`_run_watchdog`](file_watcher.md#FileWatcherDaemon._run_watchdog)

## Module values
- `_DEFAULT_DEBOUNCE_SEC` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L31)
- `_DEFAULT_POLL_INTERVAL_SEC` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L32)
- `logger` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_watcher.py#L29)

