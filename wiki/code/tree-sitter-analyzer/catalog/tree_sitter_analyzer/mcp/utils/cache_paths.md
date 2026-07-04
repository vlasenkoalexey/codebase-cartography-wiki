---
title: 'Module: tree_sitter_analyzer/mcp/utils/cache_paths.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/cache_paths.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.cache_paths`/
symbols:
  assert_cache_path: assert_cache_path().
  is_allowed_cache_path: is_allowed_cache_path().
  CACHE_DIR_NAME: CACHE_DIR_NAME.
  logger: logger.
  CachePathError: CachePathError#
  _ALLOWED_FILES._ALLOWED_FILES: _ALLOWED_FILES._ALLOWED_FILES.
  _ALLOWED_EXTENSIONS._ALLOWED_EXTENSIONS: _ALLOWED_EXTENSIONS._ALLOWED_EXTENSIONS.
  _ALLOWED_SUBDIRS._ALLOWED_SUBDIRS: _ALLOWED_SUBDIRS._ALLOWED_SUBDIRS.
---
# Module: [`tree_sitter_analyzer/mcp/utils/cache_paths.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py)

## Classes
### `CachePathError`  ·  implements/extends ValueError
- def: [`tree_sitter_analyzer/mcp/utils/cache_paths.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L75)
- doc: Raised when a write target falls outside the cache allowlist.
- signature: `class CachePathError(ValueError):`
- used by: [`assert_cache_path`](cache_paths.md#assert_cache_path)

## Functions
- `assert_cache_path(path: Path | str, project_root: Path | str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L125) — Resolve ``path`` under ``project_root`` and assert it is allowed.
- `is_allowed_cache_path(path: Path | str, project_root: Path | str)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L84) — Return True if ``path`` is allowed inside the cache directory.

## Module values
- `CACHE_DIR_NAME` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L42)
- `_ALLOWED_EXTENSIONS` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L58)
- `_ALLOWED_FILES` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L46)
- `_ALLOWED_SUBDIRS` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L67)
- `logger` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/cache_paths.py#L40)

