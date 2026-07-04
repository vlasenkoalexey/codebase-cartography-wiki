---
title: 'Module: tree_sitter_analyzer/mcp/utils/path_resolver.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/path_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.path_resolver`/
symbols:
  PathResolver: PathResolver#
  PathResolver.resolve: PathResolver#resolve().
  PathResolver.project_root: PathResolver#project_root.
  PathResolver._cache: PathResolver#_cache.
  PathResolver.validate_path: PathResolver#validate_path().
  _normalize_path_cross_platform: _normalize_path_cross_platform().
  PathResolver.get_relative_path: PathResolver#get_relative_path().
  PathResolver.set_project_root: PathResolver#set_project_root().
  logger: logger.
  PathResolver._add_to_cache: PathResolver#_add_to_cache().
  resolve_path: resolve_path().
  PathResolver._cache_size_limit: PathResolver#_cache_size_limit.
  PathResolver.get_cache_stats: PathResolver#get_cache_stats().
  PathResolver.is_relative: PathResolver#is_relative().
  _is_windows_absolute_path: _is_windows_absolute_path().
  PathResolver.clear_cache: PathResolver#clear_cache().
  PathResolver.get_project_root: PathResolver#get_project_root().
  PathResolver.__init__: PathResolver#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/utils/path_resolver.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py)

## Classes
### `PathResolver`
- def: [`tree_sitter_analyzer/mcp/utils/path_resolver.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L99) — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
- doc: Utility class for resolving file paths in MCP tools.
- signature: `class PathResolver:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L107) — Initialize the path resolver.
  - `_add_to_cache(self, file_path: str, resolved_path: str)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L231) — Add a resolved path to the cache.
  - `clear_cache(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L249) — Clear the path resolution cache.
  - `get_cache_stats(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L255) — Get cache statistics.
  - `get_project_root(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L371) — Get the current project root.
  - `get_relative_path(self, absolute_path: str)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L276) — Get the relative path from project root to the given absolute path.
  - `is_relative(self, file_path: str)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L264) — Check if a file path is relative.
  - `resolve(self, file_path: str)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L132) — Resolve a file path to an absolute path. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `set_project_root(self, project_root: str)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L380) — Set or update the project root.
  - `validate_path(self, file_path: str)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L326) — Validate if a file path is valid and safe.
  - `project_root` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L114)
- protocol/private: `_cache`[`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L115), `_cache_size_limit`[`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L116)
- uses (calls/refs, reference-scoped): [`_normalize_path_cross_platform`](path_resolver.md#_normalize_path_cross_platform), [`logger`](path_resolver.md#logger), [`_is_windows_absolute_path`](path_resolver.md#_is_windows_absolute_path)
- used by: [`resolve_and_validate_file_path`](../tools/base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`path_resolver`](../tools/base_tool.md#BaseMCPTool.path_resolver), [`resolve_and_validate_directory_path`](../tools/base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`resolve_path`](path_resolver.md#resolve_path), [`_check_file_in_roots`](../tools/search_content_tool.md#SearchContentTool._check_file_in_roots)  (83 test-only)

## Functions
- `_is_windows_absolute_path(path_str: str)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L82) — Check if a path is a Windows-style absolute path.
- `_normalize_path_cross_platform(path_str: str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L17) — Normalize path for cross-platform compatibility.
- `resolve_path(file_path: str, project_root: str | None = None)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L404) — Convenience function to resolve a file path.

## Module values
- `logger` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/path_resolver.py#L14)

