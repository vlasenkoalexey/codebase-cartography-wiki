---
title: 'Module: tests/unit/test_file_watcher.py'
type: catalog
provenance: extracted
module: tests/unit/test_file_watcher.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_file_watcher`/
symbols:
  TestOnSyncCallback.test_callback_receives_result: TestOnSyncCallback#test_callback_receives_result().
  cache: cache().
  watcher: watcher().
  TestPollingDetection.test_detects_new_file: TestPollingDetection#test_detects_new_file().
  TestPollingDetection.test_detects_modified_file: TestPollingDetection#test_detects_modified_file().
  _wait_until: _wait_until().
  TestOnSyncCallback.on_sync: TestOnSyncCallback#on_sync().
  project: project().
  TestWatcherLifecycle: TestWatcherLifecycle#
  TestWatcherLifecycle.test_start_stop: TestWatcherLifecycle#test_start_stop().
  TestWatcherLifecycle.test_double_start_is_noop: TestWatcherLifecycle#test_double_start_is_noop().
  TestWatcherLifecycle.test_stop_when_not_started: TestWatcherLifecycle#test_stop_when_not_started().
  TestManualTriggerSync: TestManualTriggerSync#
  TestManualTriggerSync.test_trigger_sync_indexes_new_files: TestManualTriggerSync#test_trigger_sync_indexes_new_files().
  TestManualTriggerSync.test_trigger_sync_populates_cache: TestManualTriggerSync#test_trigger_sync_populates_cache().
  TestManualTriggerSync.test_trigger_sync_idempotent: TestManualTriggerSync#test_trigger_sync_idempotent().
  TestWatcherStats: TestWatcherStats#
  TestWatcherStats.test_initial_stats: TestWatcherStats#test_initial_stats().
  TestWatcherStats.test_stats_after_sync: TestWatcherStats#test_stats_after_sync().
  TestWatcherStats.test_uptime_after_start: TestWatcherStats#test_uptime_after_start().
  TestPollingDetection: TestPollingDetection#
  TestOnSyncCallback: TestOnSyncCallback#
  TestDebounce: TestDebounce#
  TestDebounce.test_rapid_events_batched: TestDebounce#test_rapid_events_batched().
  TestNonSourceFiles: TestNonSourceFiles#
  TestNonSourceFiles.test_ignores_non_source_files: TestNonSourceFiles#test_ignores_non_source_files().
---
# Module: [`tests/unit/test_file_watcher.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py)

## Classes
### `TestDebounce`
- def: [`tests/unit/test_file_watcher.py:155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L155)
- signature: `class TestDebounce:`
- members:
  - `test_rapid_events_batched(self, cache, watcher)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L156)

### `TestManualTriggerSync`
- def: [`tests/unit/test_file_watcher.py:68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L68)
- signature: `class TestManualTriggerSync:`
- members:
  - `test_trigger_sync_idempotent(self, watcher)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L79)
  - `test_trigger_sync_indexes_new_files(self, watcher, project)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L69)
  - `test_trigger_sync_populates_cache(self, watcher, cache)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L74)

### `TestNonSourceFiles`
- def: [`tests/unit/test_file_watcher.py:164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L164)
- signature: `class TestNonSourceFiles:`
- members:
  - `test_ignores_non_source_files(self, watcher, project)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L165)

### `TestOnSyncCallback`
- def: [`tests/unit/test_file_watcher.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L139)
- signature: `class TestOnSyncCallback:`
- members:
  - `on_sync(r)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L143)
  - `test_callback_receives_result(self, cache, project)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L140)
- uses (calls/refs, reference-scoped): [`_enqueue`](../../tree_sitter_analyzer/file_watcher.md#FileWatcherDaemon._enqueue), [`_flush_pending`](../../tree_sitter_analyzer/file_watcher.md#FileWatcherDaemon._flush_pending), [`stop`](../../tree_sitter_analyzer/file_watcher.md#FileWatcherDaemon.stop), [`FileWatcherDaemon`](../../tree_sitter_analyzer/file_watcher.md#FileWatcherDaemon)

### `TestPollingDetection`
- def: [`tests/unit/test_file_watcher.py:106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L106)
- signature: `class TestPollingDetection:`
- members:
  - `test_detects_modified_file(self, watcher, project, cache)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L123)
  - `test_detects_new_file(self, watcher, project, cache)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L107)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestWatcherLifecycle`
- def: [`tests/unit/test_file_watcher.py:50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L50)
- signature: `class TestWatcherLifecycle:`
- members:
  - `test_double_start_is_noop(self, watcher)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L58)
  - `test_start_stop(self, watcher)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L51)
  - `test_stop_when_not_started(self, watcher)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L64)

### `TestWatcherStats`
- def: [`tests/unit/test_file_watcher.py:86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L86)
- signature: `class TestWatcherStats:`
- members:
  - `test_initial_stats(self, watcher)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L87)
  - `test_stats_after_sync(self, watcher)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L93)
  - `test_uptime_after_start(self, watcher)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L98)

## Functions
- `_wait_until(predicate, timeout: float = 3, interval: float = 0.05)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L12) — Poll predicate until true or timeout. Returns the final predicate value.
- `cache(project)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L37)
- `project(tmp_path)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L28)
- `watcher(cache)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_watcher.py#L44)

