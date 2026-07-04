---
title: 'Module: tests/unit/test_incremental_sync.py'
type: catalog
provenance: extracted
module: tests/unit/test_incremental_sync.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_incremental_sync`/
symbols:
  TestRecursionErrorHandling.test_recursion_error_in_one_file_does_not_abort_sync: TestRecursionErrorHandling#test_recursion_error_in_one_file_does_not_abort_sync().
  TestAnyExceptionDoesNotAbortSync.test_value_error_in_one_file_does_not_abort_sync: TestAnyExceptionDoesNotAbortSync#test_value_error_in_one_file_does_not_abort_sync().
  TestAnyExceptionDoesNotAbortSync.test_os_error_in_one_file_does_not_abort_sync: TestAnyExceptionDoesNotAbortSync#test_os_error_in_one_file_does_not_abort_sync().
  TestSavepointRollbackOnPartialWrite.test_second_sync_reindexes_file_after_savepoint_rollback: TestSavepointRollbackOnPartialWrite#test_second_sync_reindexes_file_after_savepoint_rollback().
  TestRecursionErrorHandling.test_recursion_error_detail_has_file_attribution: TestRecursionErrorHandling#test_recursion_error_detail_has_file_attribution().
  TestSavepointRollbackOnPartialWrite.test_partial_write_rolled_back_so_next_sync_treats_file_as_new: TestSavepointRollbackOnPartialWrite#test_partial_write_rolled_back_so_next_sync_treats_file_as_new().
  cache: cache().
  sync: sync().
  TestRecursionErrorHandling._boom_on_pathological: TestRecursionErrorHandling#_boom_on_pathological().
  TestRecursionErrorHandling._boom: TestRecursionErrorHandling#_boom().
  TestAnyExceptionDoesNotAbortSync._boom_on_bad: TestAnyExceptionDoesNotAbortSync#_boom_on_bad().
  TestAnyExceptionDoesNotAbortSync._boom_os: TestAnyExceptionDoesNotAbortSync#_boom_os().
  TestSavepointRollbackOnPartialWrite._fail_after_ast_index: TestSavepointRollbackOnPartialWrite#_fail_after_ast_index().
  TestSavepointRollbackOnPartialWrite._fail_once: TestSavepointRollbackOnPartialWrite#_fail_once().
  project: project().
  TestSyncFromScratch: TestSyncFromScratch#
  TestSyncFromScratch.test_sync_indexes_all_new_files: TestSyncFromScratch#test_sync_indexes_all_new_files().
  TestSyncFromScratch.test_sync_populates_cache: TestSyncFromScratch#test_sync_populates_cache().
  TestSyncFromScratch.test_sync_details_list: TestSyncFromScratch#test_sync_details_list().
  TestSyncNoChanges: TestSyncNoChanges#
  TestSyncNoChanges.test_sync_unchanged_after_initial_index: TestSyncNoChanges#test_sync_unchanged_after_initial_index().
  TestSyncModifiedFile: TestSyncModifiedFile#
  TestSyncModifiedFile.test_detects_modified_file: TestSyncModifiedFile#test_detects_modified_file().
  TestSyncModifiedFile.test_reindexes_modified_content: TestSyncModifiedFile#test_reindexes_modified_content().
  TestSyncDeletedFile: TestSyncDeletedFile#
  TestSyncDeletedFile.test_detects_deleted_file: TestSyncDeletedFile#test_detects_deleted_file().
  TestSyncDeletedFile.test_removes_deleted_from_cache: TestSyncDeletedFile#test_removes_deleted_from_cache().
  TestSyncNewFile: TestSyncNewFile#
  TestSyncNewFile.test_detects_new_file: TestSyncNewFile#test_detects_new_file().
  TestSyncMixedChanges: TestSyncMixedChanges#
  TestSyncMixedChanges.test_handles_mixed_changes: TestSyncMixedChanges#test_handles_mixed_changes().
  TestSyncMaxFiles: TestSyncMaxFiles#
  TestSyncMaxFiles.test_respects_max_files: TestSyncMaxFiles#test_respects_max_files().
  TestSyncCallback: TestSyncCallback#
  TestSyncCallback.test_callback_receives_details: TestSyncCallback#test_callback_receives_details().
  TestGetChanges: TestGetChanges#
  TestGetChanges.test_get_changes_empty: TestGetChanges#test_get_changes_empty().
  TestGetChanges.test_get_changes_after_index: TestGetChanges#test_get_changes_after_index().
  TestGetChanges.test_get_changes_detects_modification: TestGetChanges#test_get_changes_detects_modification().
  TestGetChanges.test_get_changes_detects_deletion: TestGetChanges#test_get_changes_detects_deletion().
  TestGetChanges.test_get_changes_detects_new_file: TestGetChanges#test_get_changes_detects_new_file().
  TestSyncResultDict: TestSyncResultDict#
  TestSyncResultDict.test_to_dict_keys: TestSyncResultDict#test_to_dict_keys().
  TestContentHashComparison: TestContentHashComparison#
  TestContentHashComparison.test_mtime_only_change_not_reindexed: TestContentHashComparison#test_mtime_only_change_not_reindexed().
  TestRecursionErrorHandling: TestRecursionErrorHandling#
  TestAnyExceptionDoesNotAbortSync: TestAnyExceptionDoesNotAbortSync#
  TestSavepointRollbackOnPartialWrite: TestSavepointRollbackOnPartialWrite#
---
# Module: [`tests/unit/test_incremental_sync.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py)

## Classes
### `TestAnyExceptionDoesNotAbortSync`
- def: [`tests/unit/test_incremental_sync.py:267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L267)
- doc: Issue #806: non-RecursionError per-file exceptions must not abort the whole sync.
- signature: `class TestAnyExceptionDoesNotAbortSync:`
- members:
  - `test_os_error_in_one_file_does_not_abort_sync(self, project, cache)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L294) — An OSError in index_file must be caught; remaining files still indexed.
  - `test_value_error_in_one_file_does_not_abort_sync(self, project, cache)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L270) — A ValueError in index_file must be caught; sibling files must still be indexed.
- protocol/private: `_boom_on_bad`[`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L278), `_boom_os`[`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L301)
- uses (calls/refs, reference-scoped): [`sync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync), [`errors`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.errors), [`details`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.details)

### `TestContentHashComparison`
- def: [`tests/unit/test_incremental_sync.py:196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L196)
- signature: `class TestContentHashComparison:`
- members:
  - `test_mtime_only_change_not_reindexed(self, sync, cache, project)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L200)

### `TestGetChanges`
- def: [`tests/unit/test_incremental_sync.py:147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L147)
- signature: `class TestGetChanges:`
- members:
  - `test_get_changes_after_index(self, sync, cache, project)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L154)
  - `test_get_changes_detects_deletion(self, sync, cache, project)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L170)
  - `test_get_changes_detects_modification(self, sync, cache, project)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L161)
  - `test_get_changes_detects_new_file(self, sync, cache, project)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L176)
  - `test_get_changes_empty(self, sync, project)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L148)

### `TestRecursionErrorHandling`
- def: [`tests/unit/test_incremental_sync.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L209)
- doc: Issue #805: RecursionError from deeply-nested AST must not abort sync.
- signature: `class TestRecursionErrorHandling:`
- members:
  - `test_recursion_error_detail_has_file_attribution(self, project, cache)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L244) — Error envelope must contain file path (Issue #806 partial fix).
  - `test_recursion_error_in_one_file_does_not_abort_sync(self, project, cache)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L212) — A RecursionError in index_file must be caught per-file; sibling files
- protocol/private: `_boom`[`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L251), `_boom_on_pathological`[`L222`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L222)
- uses (calls/refs, reference-scoped): [`sync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync), [`errors`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.errors), [`details`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.details)

### `TestSavepointRollbackOnPartialWrite`
- def: [`tests/unit/test_incremental_sync.py:317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L317)
- doc: Issue #886: savepoint must roll back partial ast_index writes on mid-write failure.
- signature: `class TestSavepointRollbackOnPartialWrite:`
- members:
  - `test_partial_write_rolled_back_so_next_sync_treats_file_as_new(self, project, cache)` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L325)
  - `test_second_sync_reindexes_file_after_savepoint_rollback(self, project, cache)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L357)
- protocol/private: `_fail_after_ast_index`[`L333`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L333), `_fail_once`[`L364`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L364)
- uses (calls/refs, reference-scoped): [`sync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../tree_sitter_analyzer/incremental_sync.md#IncrementalSync), [`errors`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.errors), [`details`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.details)

### `TestSyncCallback`
- def: [`tests/unit/test_incremental_sync.py:140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L140)
- signature: `class TestSyncCallback:`
- members:
  - `test_callback_receives_details(self, sync, cache, project)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L141)

### `TestSyncDeletedFile`
- def: [`tests/unit/test_incremental_sync.py:92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L92)
- signature: `class TestSyncDeletedFile:`
- members:
  - `test_detects_deleted_file(self, sync, cache, project)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L93)
  - `test_removes_deleted_from_cache(self, sync, cache, project)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L100)

### `TestSyncFromScratch`
- def: [`tests/unit/test_incremental_sync.py:36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L36)
- signature: `class TestSyncFromScratch:`
- members:
  - `test_sync_details_list(self, sync, project)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L49)
  - `test_sync_indexes_all_new_files(self, sync, project)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L37)
  - `test_sync_populates_cache(self, sync, cache, project)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L44)

### `TestSyncMaxFiles`
- def: [`tests/unit/test_incremental_sync.py:132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L132)
- signature: `class TestSyncMaxFiles:`
- members:
  - `test_respects_max_files(self, sync, cache, project)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L133)

### `TestSyncMixedChanges`
- def: [`tests/unit/test_incremental_sync.py:117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L117)
- signature: `class TestSyncMixedChanges:`
- members:
  - `test_handles_mixed_changes(self, sync, cache, project)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L118)

### `TestSyncModifiedFile`
- def: [`tests/unit/test_incremental_sync.py:67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L67)
- signature: `class TestSyncModifiedFile:`
- members:
  - `test_detects_modified_file(self, sync, cache, project)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L68)
  - `test_reindexes_modified_content(self, sync, cache, project)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L78)

### `TestSyncNewFile`
- def: [`tests/unit/test_incremental_sync.py:108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L108)
- signature: `class TestSyncNewFile:`
- members:
  - `test_detects_new_file(self, sync, cache, project)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L109)

### `TestSyncNoChanges`
- def: [`tests/unit/test_incremental_sync.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L57)
- signature: `class TestSyncNoChanges:`
- members:
  - `test_sync_unchanged_after_initial_index(self, sync, cache)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L58)

### `TestSyncResultDict`
- def: [`tests/unit/test_incremental_sync.py:183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L183)
- signature: `class TestSyncResultDict:`
- members:
  - `test_to_dict_keys(self, sync, project)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L184)

## Functions
- `cache(project)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L25)
- `project(tmp_path)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L15)
- `sync(cache)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_incremental_sync.py#L32)

