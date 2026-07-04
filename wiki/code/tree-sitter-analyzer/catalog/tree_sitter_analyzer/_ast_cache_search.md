---
title: 'Module: tree_sitter_analyzer/_ast_cache_search.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_search`/
symbols:
  search_symbols_cascade: search_symbols_cascade().
  _extend_fuzzy_results: _extend_fuzzy_results().
  _row_get: _row_get().
  _add_result: _add_result().
  _name_match_bonus: _name_match_bonus().
  _score_result: _score_result().
  _extend_results: _extend_results().
  _bounded_levenshtein: _bounded_levenshtein().
  _like_rows: _like_rows().
  _fuzzy_rows: _fuzzy_rows().
  _normalise_symbol: _normalise_symbol().
  _KIND_BONUS: _KIND_BONUS.
  _exact_rows: _exact_rows().
  _apply_file_colocation_bonus: _apply_file_colocation_bonus().
  _tier_rank: _tier_rank().
  _camel_initials: _camel_initials().
---
# Module: [`tree_sitter_analyzer/_ast_cache_search.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py)

## Functions
- `_add_result(results: list[dict[str, Any]], seen: set[tuple[str, str, int]], row: sqlite3.Row | dict[str, Any], query: str, tier: str, base_score: float)` — [`L205`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L205)
- `_apply_file_colocation_bonus(results: list[dict[str, Any]])` — [`L262`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L262)
- `_bounded_levenshtein(left: str, right: str, max_distance: int)` — [`L287`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L287)
- `_camel_initials(value: str)` — [`L283`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L283)
- `_exact_rows(conn: sqlite3.Connection, query: str, language: str | None)` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L100)
- `_extend_fuzzy_results(conn: sqlite3.Connection, query: str, language: str | None, limit: int, results: list[dict[str, Any]], seen: set[tuple[str, str, int]])` — [`L183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L183)
- `_extend_results(results: list[dict[str, Any]], seen: set[tuple[str, str, int]], rows: list[sqlite3.Row], query: str, tier: str, base_score: float)` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L171)
- `_fuzzy_rows(conn: sqlite3.Connection, language: str | None, limit: int)` — [`L149`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L149)
- `_like_rows(conn: sqlite3.Connection, query: str, language: str | None, limit: int)` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L122)
- `_name_match_bonus(name: str, query: str)` — [`L246`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L246)
- `_normalise_symbol(value: str)` — [`L279`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L279)
- `_row_get(row: sqlite3.Row | dict[str, Any], key: str, default: Any = None)` — [`L231`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L231)
- `_score_result(row: dict[str, Any], query: str, base_score: float)` — [`L240`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L240)
- `_tier_rank(tier: str)` — [`L275`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L275)
- `search_symbols_cascade(conn: sqlite3.Connection, query: str, language: str | None = None, limit: int = 100, fts5_available: bool = True)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L23) — Cascade symbol search: exact -> FTS5 -> LIKE -> fuzzy edit distance.

## Module values
- `_KIND_BONUS` — [`L12`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_search.py#L12)

