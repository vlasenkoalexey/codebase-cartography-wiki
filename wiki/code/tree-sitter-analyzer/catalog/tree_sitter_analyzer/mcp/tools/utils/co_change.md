---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/co_change.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/co_change.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.co_change`/
symbols:
  _CO_CHANGE_CACHE._CO_CHANGE_CACHE: _CO_CHANGE_CACHE._CO_CHANGE_CACHE.
  _compute_co_change: _compute_co_change().
  _co_change_cache_put: _co_change_cache_put().
  _co_change_cache_get: _co_change_cache_get().
  _CO_CHANGE_CACHE_MAXSIZE: _CO_CHANGE_CACHE_MAXSIZE.
  MIN_COMMITS_FOR_COUPLING_ANALYSIS: MIN_COMMITS_FOR_COUPLING_ANALYSIS.
  _build_co_change_summary: _build_co_change_summary().
  CoChangeCacheKey: CoChangeCacheKey.
  _empty_co_change_result: _empty_co_change_result().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/co_change.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py)

## Functions
- `_build_co_change_summary(target_file: str, coupled: list[dict[str, Any]], commits_analyzed: int, candidates_below_threshold: int)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L88) — Build the agent_summary dict for a co_change result.
- `_co_change_cache_get(key: CoChangeCacheKey)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L47) — LRU get: move hit to end (most-recently-used).
- `_co_change_cache_put(key: CoChangeCacheKey, value: dict[str, Any])` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L57) — LRU put: evict oldest entry if at capacity.
- `_compute_co_change(project_root: str, target_file: str, max_commits: int = 500, min_shared: int = 3, max_results: int = 20)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L152) — Compute git-history co-change coupling for *target_file*.
- `_empty_co_change_result(target_file: str, max_commits: int)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L69) — Return a graceful empty result (git unavailable or no history).

## Module values
- `CoChangeCacheKey` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L36)
- `MIN_COMMITS_FOR_COUPLING_ANALYSIS` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L44)
- `_CO_CHANGE_CACHE` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L37)
- `_CO_CHANGE_CACHE_MAXSIZE` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/co_change.py#L35)

