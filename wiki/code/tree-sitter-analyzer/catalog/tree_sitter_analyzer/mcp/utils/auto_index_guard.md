---
title: 'Module: tree_sitter_analyzer/mcp/utils/auto_index_guard.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/auto_index_guard.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.auto_index_guard`/
symbols:
  ensure_indexed: ensure_indexed().
  reset: reset().
  _resolve_pending_unresolved_refs: _resolve_pending_unresolved_refs().
  is_indexed: is_indexed().
  _mark_resolution_converged: _mark_resolution_converged().
  _indexed_roots._indexed_roots: _indexed_roots._indexed_roots.
  mark_dirty: mark_dirty().
  _open_cache: _open_cache().
  _resolution_converged: _resolution_converged().
  logger: logger.
  _lock: _lock.
---
# Module: [`tree_sitter_analyzer/mcp/utils/auto_index_guard.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py)

## Functions
- `_mark_resolution_converged(cache: Any)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L149)
- `_open_cache(project_root: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L118)
- `_resolution_converged(cache: Any)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L140)
- `_resolve_pending_unresolved_refs(cache: Any)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L127) — Attempt the resolve-only pass. Returns True on success, False if it failed.
- `ensure_indexed(project_root: str | None, max_files: int = 20000, *, auto_build: bool = True)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L41) — Return a ready-to-query ASTCache, optionally auto-indexing if empty.
- `is_indexed(project_root: str)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L169)
- `mark_dirty(project_root: str)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L158) — Mark a project root as needing re-index on next ``ensure_indexed``.
- `reset()` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L163) — Clear all cached state (for testing).

## Module values
- `_indexed_roots` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L38)
- `_lock` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L37)
- `logger` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/auto_index_guard.py#L35)

