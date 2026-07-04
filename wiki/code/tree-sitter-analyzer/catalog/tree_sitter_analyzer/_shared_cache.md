---
title: 'Module: tree_sitter_analyzer/_shared_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_shared_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._shared_cache`/
symbols:
  SharedCache: SharedCache#
  get_shared_cache: get_shared_cache().
  SharedCache.get_language: SharedCache#get_language().
  SharedCache.set_language: SharedCache#set_language().
  SharedCache._make_key: SharedCache#_make_key().
  SharedCache.get_security_validation: SharedCache#get_security_validation().
  SharedCache.get_language_meta: SharedCache#get_language_meta().
  SharedCache.set_security_validation: SharedCache#set_security_validation().
  SharedCache.get_metrics: SharedCache#get_metrics().
  SharedCache.clear: SharedCache#clear().
  SharedCache.set_metrics: SharedCache#set_metrics().
  SharedCache.set_language_meta: SharedCache#set_language_meta().
  SharedCache.get_resolved_path: SharedCache#get_resolved_path().
  SharedCache.set_resolved_path: SharedCache#set_resolved_path().
  SharedCache.__new__: SharedCache#__new__().
  SharedCache._instance: SharedCache#_instance.
  SharedCache.initialize: SharedCache#initialize.
  SharedCache._initialize: SharedCache#_initialize().
  SharedCache._language_cache: SharedCache#_language_cache.
  SharedCache._language_meta_cache: SharedCache#_language_meta_cache.
  SharedCache._security_cache: SharedCache#_security_cache.
  SharedCache._metrics_cache: SharedCache#_metrics_cache.
  SharedCache._resolved_paths: SharedCache#_resolved_paths.
---
# Module: [`tree_sitter_analyzer/_shared_cache.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py)

## Classes
### `SharedCache`
- def: [`tree_sitter_analyzer/_shared_cache.py:6`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L6) — documented in [tree_sitter_analyzer-mcp-server](../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: Process-wide singleton cache shared across all layers (core, MCP, CLI).
- signature: `class SharedCache:`
- members:
  - `clear(self)` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L101)
  - `get_language(self, file_path: str, project_root: str | None = None)` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L31)
  - `get_language_meta(self, abs_path: str, project_root: str | None = None)` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L45)
  - `get_metrics(self, file_path: str, project_root: str | None = None)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L73)
  - `get_resolved_path(self, original_path: str, project_root: str | None = None)` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L87)
  - `get_security_validation(self, file_path: str, project_root: str | None = None)` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L59)
  - `set_language(self, file_path: str, language: str, project_root: str | None = None)` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L38)
  - `set_language_meta(self, abs_path: str, meta: dict[str, Any], project_root: str | None = None)` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L52)
  - `set_metrics(self, file_path: str, metrics: dict[str, Any], project_root: str | None = None)` — [`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L80)
  - `set_resolved_path(self, original_path: str, resolved_path: str, project_root: str | None = None)` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L94)
  - `set_security_validation(self, file_path: str, result: tuple[bool, str], project_root: str | None = None)` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L66)
  - `initialize` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L105)
- protocol/private: `__new__`[`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L14), `_initialize`[`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L20), `_instance`[`L12`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L12), `_language_cache`[`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L21), `_language_meta_cache`[`L22`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L22), `_make_key`[`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L27), `_metrics_cache`[`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L24), `_resolved_paths`[`L25`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L25), `_security_cache`[`L23`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L23)
- used by: [`compute_file_metrics`](mcp/utils/file_metrics.md#compute_file_metrics), [`resolve_and_validate_file_path`](mcp/tools/base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`set_project_path`](mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`path_resolver`](mcp/tools/base_tool.md#BaseMCPTool.path_resolver), [`get_shared_cache`](_shared_cache.md#get_shared_cache), [`_validate_file_path_security`](mcp/server.md#TreeSitterAnalyzerMCPServer._validate_file_path_security), [`get_cached_language`](_language_detector_helpers.md#get_cached_language), [`store_cached_language`](_language_detector_helpers.md#store_cached_language), [`_validate_security`](mcp/server_utils/code_scale_handler.md#_validate_security)  (55 test-only)

## Functions
- `get_shared_cache()` — [`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_shared_cache.py#L108) — documented in [tree_sitter_analyzer-mcp-server](../../concepts/tree_sitter_analyzer-mcp-server.md)

