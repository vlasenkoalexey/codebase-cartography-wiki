---
title: 'Module: tests/unit/mcp/test_ast_cache_watch_modes.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_ast_cache_watch_modes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_ast_cache_watch_modes`/
symbols:
  tool: tool().
  cache: cache().
  project: project().
  TestWatchStart: TestWatchStart#
  TestWatchStart.test_watch_start_starts_watcher: TestWatchStart#test_watch_start_starts_watcher().
  TestWatchStart.test_watch_start_idempotent: TestWatchStart#test_watch_start_idempotent().
  TestWatchStart.test_watch_start_custom_interval: TestWatchStart#test_watch_start_custom_interval().
  TestWatchStart.test_watch_start_can_sync_after_start: TestWatchStart#test_watch_start_can_sync_after_start().
  TestWatchStop: TestWatchStop#
  TestWatchStop.test_watch_stop_when_not_running: TestWatchStop#test_watch_stop_when_not_running().
  TestWatchStop.test_watch_stop_stops_running_watcher: TestWatchStop#test_watch_stop_stops_running_watcher().
  TestWatchStop.test_watch_stop_includes_stats: TestWatchStop#test_watch_stop_includes_stats().
  TestWatchStatus: TestWatchStatus#
  TestWatchStatus.test_watch_status_no_watcher: TestWatchStatus#test_watch_status_no_watcher().
  TestWatchStatus.test_watch_status_running: TestWatchStatus#test_watch_status_running().
  TestWatchStatus.test_watch_status_after_stop: TestWatchStatus#test_watch_status_after_stop().
  TestWatchModeValidation: TestWatchModeValidation#
  TestWatchModeValidation.test_watch_modes_in_valid_modes: TestWatchModeValidation#test_watch_modes_in_valid_modes().
  TestWatchModeValidation.test_invalid_mode_rejected: TestWatchModeValidation#test_invalid_mode_rejected().
  TestWatchToolDefinition: TestWatchToolDefinition#
  TestWatchToolDefinition.test_watch_modes_in_schema: TestWatchToolDefinition#test_watch_modes_in_schema().
  TestWatchToolDefinition.test_watch_params_in_schema: TestWatchToolDefinition#test_watch_params_in_schema().
  TestWatchToolDefinition.test_description_mentions_watch: TestWatchToolDefinition#test_description_mentions_watch().
---
# Module: [`tests/unit/mcp/test_ast_cache_watch_modes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py)

## Classes
### `TestWatchModeValidation`
- def: [`tests/unit/mcp/test_ast_cache_watch_modes.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L118)
- signature: `class TestWatchModeValidation:`
- members:
  - `test_invalid_mode_rejected(self, tool, project)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L124)
  - `test_watch_modes_in_valid_modes(self, tool, project)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L119)

### `TestWatchStart`
- def: [`tests/unit/mcp/test_ast_cache_watch_modes.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L36)
- signature: `class TestWatchStart:`
- members:
  - `test_watch_start_can_sync_after_start(self, tool, cache, project)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L59)
  - `test_watch_start_custom_interval(self, tool, project)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L50)
  - `test_watch_start_idempotent(self, tool, project)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L44)
  - `test_watch_start_starts_watcher(self, tool, project)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L37)

### `TestWatchStatus`
- def: [`tests/unit/mcp/test_ast_cache_watch_modes.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L93)
- signature: `class TestWatchStatus:`
- members:
  - `test_watch_status_after_stop(self, tool, project)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L109)
  - `test_watch_status_no_watcher(self, tool, project)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L94)
  - `test_watch_status_running(self, tool, project)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L100)

### `TestWatchStop`
- def: [`tests/unit/mcp/test_ast_cache_watch_modes.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L68)
- signature: `class TestWatchStop:`
- members:
  - `test_watch_stop_includes_stats(self, tool, project)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L81)
  - `test_watch_stop_stops_running_watcher(self, tool, project)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L74)
  - `test_watch_stop_when_not_running(self, tool, project)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L69)

### `TestWatchToolDefinition`
- def: [`tests/unit/mcp/test_ast_cache_watch_modes.py:129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L129)
- signature: `class TestWatchToolDefinition:`
- members:
  - `test_description_mentions_watch(self, tool)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L142)
  - `test_watch_modes_in_schema(self, tool)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L130)
  - `test_watch_params_in_schema(self, tool)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L137)

## Functions
- `cache(project)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L19)
- `project(tmp_path)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L10)
- `tool(project)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_ast_cache_watch_modes.py#L26)

