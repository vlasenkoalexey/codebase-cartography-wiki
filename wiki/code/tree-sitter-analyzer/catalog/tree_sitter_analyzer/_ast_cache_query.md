---
title: 'Module: tree_sitter_analyzer/_ast_cache_query.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_query`/
symbols:
  fts_search_ranked: fts_search_ranked().
  backfill_cross_file_edges: backfill_cross_file_edges().
  get_stats: get_stats().
  get_cross_file_stats: get_cross_file_stats().
  _normalize_bm25: _normalize_bm25().
  invalidate: invalidate().
  lookup: lookup().
  fts_search: fts_search().
  search_symbols_linear: search_symbols_linear().
  query_callers_enhanced: query_callers_enhanced().
  query_callees_enhanced: query_callees_enhanced().
  logger: logger.
  _SQL_COUNT_RESOLVED_EDGES: _SQL_COUNT_RESOLVED_EDGES.
  _SQL_COUNT_CROSS_FILE_EDGES: _SQL_COUNT_CROSS_FILE_EDGES.
  _SQL_UPDATE_CALLEE_RESOLVED: _SQL_UPDATE_CALLEE_RESOLVED.
  _KIND_WEIGHT_DEFAULT: _KIND_WEIGHT_DEFAULT.
  _DEMOTION_OVERFETCH_FACTOR: _DEMOTION_OVERFETCH_FACTOR.
  _DEMOTION_OVERFETCH_FLOOR: _DEMOTION_OVERFETCH_FLOOR.
  _KIND_WEIGHT._KIND_WEIGHT: _KIND_WEIGHT._KIND_WEIGHT.
---
# Module: [`tree_sitter_analyzer/_ast_cache_query.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py)

## Functions
- `_normalize_bm25(raw: float, worst: float, best: float | None = None)` — [`L135`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L135) — Normalize a raw FTS5 BM25 score to [0.0, 1.0].
- `backfill_cross_file_edges(cache: Any, conn: sqlite3.Connection)` — [`L407`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L407) — Resolve cross-file call edges and persist callee_resolved_file.
- `fts_search(conn: sqlite3.Connection, query: str, language: str | None = None, limit: int = 100)` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L97) — FTS5-backed symbol search. Returns list of symbol dicts.
- `fts_search_ranked(conn: sqlite3.Connection, query: str, language: str | None = None, limit: int = 100)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L178) — BM25-ranked FTS5 symbol search with kind-priority and test-file demotion.
- `get_cross_file_stats(conn: sqlite3.Connection)` — [`L388`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L388) — Return cross-file edge resolution statistics.
- `get_stats(conn: sqlite3.Connection, fts5_available: bool | None, db_path: str)` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L297) — Return aggregate index statistics.
- `invalidate(conn: sqlite3.Connection, file_path: str, project_root: str, fts5_available: bool | None)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L42) — Remove all cached rows for file_path. Returns True if a row was deleted.
- `lookup(conn: sqlite3.Connection, file_path: str, project_root: str)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L70) — Look up one file's cached AST metadata. Returns None if not indexed.
- `query_callees_enhanced(cache: Any, caller_name: str, caller_file: str | None = None, max_depth: int = 1)` — [`L472`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L472) — Enhanced callees lookup with cross-file import resolution.
- `query_callers_enhanced(cache: Any, callee_name: str, callee_file: str | None = None, max_depth: int = 1)` — [`L448`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L448) — Enhanced callers lookup with cross-file import resolution.
- `search_symbols_linear(conn: sqlite3.Connection, query: str, language: str | None = None)` — [`L270`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L270) — Linear (non-FTS5) symbol search. Returns list of symbol dicts.

## Module values
- `_DEMOTION_OVERFETCH_FACTOR` — [`L174`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L174)
- `_DEMOTION_OVERFETCH_FLOOR` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L175)
- `_KIND_WEIGHT` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L158)
- `_KIND_WEIGHT_DEFAULT` — [`L167`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L167)
- `_SQL_COUNT_CROSS_FILE_EDGES` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L30)
- `_SQL_COUNT_RESOLVED_EDGES` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L26)
- `_SQL_UPDATE_CALLEE_RESOLVED` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L35)
- `logger` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_query.py#L21)

