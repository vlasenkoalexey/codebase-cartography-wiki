---
title: 'Module: tree_sitter_analyzer/mcp/utils/__init__.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/__init__.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils`/
symbols:
  get_performance_monitor: get_performance_monitor().
  get_cache_manager: get_cache_manager().
  MCP_UTILS_CAPABILITIES: MCP_UTILS_CAPABILITIES.
  BackwardCompatibleCacheManager.clear_all_caches: BackwardCompatibleCacheManager#clear_all_caches().
  BackwardCompatibleCacheManager.get_cache_stats: BackwardCompatibleCacheManager#get_cache_stats().
  BackwardCompatibleCacheManager._cache_service: BackwardCompatibleCacheManager#_cache_service.
  BackwardCompatibleCacheManager.__init__: BackwardCompatibleCacheManager#__init__().
  BackwardCompatibleCacheManager.__getattr__: BackwardCompatibleCacheManager#__getattr__().
  BackwardCompatibleCacheManager: BackwardCompatibleCacheManager#
  __author__: __author__.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/utils/__init__.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py)

## Classes
### `BackwardCompatibleCacheManager`
- def: [`tree_sitter_analyzer/mcp/utils/__init__.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L64)
- doc: Backward compatible cache manager wrapper
- signature: `class BackwardCompatibleCacheManager:`
- members:
  - `__getattr__(self, name: str)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L78) — Delegate other methods to the cache service
  - `clear_all_caches(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L70) — Backward compatibility: clear all caches
  - `get_cache_stats(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L74) — Backward compatibility: get cache statistics
- protocol/private: `__init__`[`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L67), `_cache_service`[`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L68)
- uses (calls/refs, reference-scoped): [`CacheService`](../../core/cache_service.md#CacheService), [`get_stats`](../../core/cache_service.md#CacheService.get_stats), [`clear`](../../core/cache_service.md#CacheService.clear)
- used by: [`get_cache_manager`](__init__.md#get_cache_manager)

## Functions
- `get_cache_manager()` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L82) — Backward compatibility: Get unified cache service
- `get_performance_monitor()` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L86) — Backward compatibility: Get unified performance monitor

## Module values
- `MCP_UTILS_CAPABILITIES` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L46)
- `__all__` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L103)
- `__author__` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/__init__.py#L43)

