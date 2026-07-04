---
title: 'Module: tests/unit/mcp/test_mcp_utils_init.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_utils_init.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_utils_init`/
symbols:
  TestImportErrorFallback.test_fallback_get_cache_manager_returns_none: TestImportErrorFallback#test_fallback_get_cache_manager_returns_none().
  TestImportErrorFallback.test_fallback_get_performance_monitor_returns_none: TestImportErrorFallback#test_fallback_get_performance_monitor_returns_none().
  TestMcpUtilsCapabilities.test_capabilities_is_dict: TestMcpUtilsCapabilities#test_capabilities_is_dict().
  TestMcpUtilsCapabilities.test_capabilities_has_version: TestMcpUtilsCapabilities#test_capabilities_has_version().
  TestBackwardCompatibleCacheManager.test_get_cache_manager_returns_object: TestBackwardCompatibleCacheManager#test_get_cache_manager_returns_object().
  TestBackwardCompatibleCacheManager.test_get_cache_stats_returns_dict: TestBackwardCompatibleCacheManager#test_get_cache_stats_returns_dict().
  TestBackwardCompatibleCacheManager.test_delegation_via_getattr: TestBackwardCompatibleCacheManager#test_delegation_via_getattr().
  TestBackwardCompatibleCacheManager.test_clear_all_caches: TestBackwardCompatibleCacheManager#test_clear_all_caches().
  TestGetPerformanceMonitor.test_get_performance_monitor_returns_object: TestGetPerformanceMonitor#test_get_performance_monitor_returns_object().
  _snapshot_modules: _snapshot_modules().
  _restore_modules: _restore_modules().
  TestImportErrorFallback.test_fallback_get_cache_manager_returns_none.BlockFinder: TestImportErrorFallback#test_fallback_get_cache_manager_returns_none().BlockFinder#
  TestImportErrorFallback.test_fallback_get_performance_monitor_returns_none.BlockFinder: TestImportErrorFallback#test_fallback_get_performance_monitor_returns_none().BlockFinder#
  TestMcpUtilsCapabilities: TestMcpUtilsCapabilities#
  TestBackwardCompatibleCacheManager: TestBackwardCompatibleCacheManager#
  TestGetPerformanceMonitor: TestGetPerformanceMonitor#
  TestImportErrorFallback: TestImportErrorFallback#
  TestImportErrorFallback.test_fallback_get_cache_manager_returns_none.BlockFinder.find_spec: TestImportErrorFallback#test_fallback_get_cache_manager_returns_none().BlockFinder#find_spec().
  TestImportErrorFallback.test_fallback_get_performance_monitor_returns_none.BlockFinder.find_spec: TestImportErrorFallback#test_fallback_get_performance_monitor_returns_none().BlockFinder#find_spec().
---
# Module: [`tests/unit/mcp/test_mcp_utils_init.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py)

## Classes
### `BlockFinder`
- def: [`tests/unit/mcp/test_mcp_utils_init.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L105)
- signature: `class BlockFinder:`
- members:
  - `find_spec(self, fullname, path, target=None)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L74)
  - `find_spec(self, fullname, path, target=None)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L106)
- used by: (1 test-only callers)

### `TestBackwardCompatibleCacheManager`
- def: [`tests/unit/mcp/test_mcp_utils_init.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L38)
- signature: `class TestBackwardCompatibleCacheManager:`
- members:
  - `test_clear_all_caches(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L52)
  - `test_delegation_via_getattr(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L48)
  - `test_get_cache_manager_returns_object(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L39)
  - `test_get_cache_stats_returns_dict(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L43)
- uses (calls/refs, reference-scoped): [`get_cache_manager`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#get_cache_manager)

### `TestGetPerformanceMonitor`
- def: [`tests/unit/mcp/test_mcp_utils_init.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L57)
- signature: `class TestGetPerformanceMonitor:`
- members:
  - `test_get_performance_monitor_returns_object(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L58)
- uses (calls/refs, reference-scoped): [`get_performance_monitor`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#get_performance_monitor)

### `TestImportErrorFallback`
- def: [`tests/unit/mcp/test_mcp_utils_init.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L63)
- signature: `class TestImportErrorFallback:`
- members:
  - `test_fallback_get_cache_manager_returns_none(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L64) — Test that fallback returns None when core services unavailable.
  - `test_fallback_get_performance_monitor_returns_none(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L96) — Test that fallback performance monitor returns None.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestMcpUtilsCapabilities`
- def: [`tests/unit/mcp/test_mcp_utils_init.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L29)
- signature: `class TestMcpUtilsCapabilities:`
- members:
  - `test_capabilities_has_version(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L33)
  - `test_capabilities_is_dict(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L30)
- uses (calls/refs, reference-scoped): [`MCP_UTILS_CAPABILITIES`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#MCP_UTILS_CAPABILITIES)

## Functions
- `_restore_modules(prefix: str, snapshot: dict[str, object])` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L17)
- `_snapshot_modules(prefix: str)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_utils_init.py#L13)

