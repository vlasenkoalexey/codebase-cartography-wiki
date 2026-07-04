---
title: 'Module: tests/unit/mcp/test_fts5_bm25_ranking.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_fts5_bm25_ranking.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_fts5_bm25_ranking`/
symbols:
  _insert_symbol: _insert_symbol().
  TestNormalizeBm25._call: TestNormalizeBm25#_call().
  _make_fts_conn: _make_fts_conn().
  TestFtsSearchRanked._call: TestFtsSearchRanked#_call().
  TestASTCacheFtsSearchRanked.test_falls_back_for_short_query: TestASTCacheFtsSearchRanked#test_falls_back_for_short_query().
  TestFtsSearchRanked.test_returns_relevance_score: TestFtsSearchRanked#test_returns_relevance_score().
  TestFtsSearchRanked.test_sorted_best_first: TestFtsSearchRanked#test_sorted_best_first().
  TestFtsSearchRanked.test_score_range: TestFtsSearchRanked#test_score_range().
  TestFtsSearchRanked.test_short_query_returns_empty: TestFtsSearchRanked#test_short_query_returns_empty().
  TestFtsSearchRanked.test_language_filter: TestFtsSearchRanked#test_language_filter().
  TestFtsSearchRanked.test_kind_priority_class_over_import: TestFtsSearchRanked#test_kind_priority_class_over_import().
  TestFtsSearchRanked.test_limit_respected: TestFtsSearchRanked#test_limit_respected().
  TestFtsSearchRanked.test_result_keys: TestFtsSearchRanked#test_result_keys().
  TestASTCacheFtsSearchRanked.test_delegates_to_query_module: TestASTCacheFtsSearchRanked#test_delegates_to_query_module().
  _c: _c.
  TestFtsSymbolToMatch.test_shape: TestFtsSymbolToMatch#test_shape().
  TestExecuteSymbolSearchFtsPath.test_uses_fts_when_available: TestExecuteSymbolSearchFtsPath#test_uses_fts_when_available().
  _skip_no_fts5: _skip_no_fts5.
  TestNormalizeBm25.test_worst_is_best_match: TestNormalizeBm25#test_worst_is_best_match().
  TestNormalizeBm25.test_identical_scores_give_one: TestNormalizeBm25#test_identical_scores_give_one().
  TestNormalizeBm25.test_worst_match_gives_zero_illegal_input: TestNormalizeBm25#test_worst_match_gives_zero_illegal_input().
  TestNormalizeBm25.test_positive_raw_returns_zero: TestNormalizeBm25#test_positive_raw_returns_zero().
  TestNormalizeBm25.test_clamped_at_one: TestNormalizeBm25#test_clamped_at_one().
  TestNormalizeBm25.test_minmax_best_gets_one_worst_gets_zero: TestNormalizeBm25#test_minmax_best_gets_one_worst_gets_zero().
  TestNormalizeBm25.test_minmax_weak_match_scores_low: TestNormalizeBm25#test_minmax_weak_match_scores_low().
  TestFtsSearchRanked: TestFtsSearchRanked#
  TestFtsSearchRanked.test_no_fts5_table_returns_empty: TestFtsSearchRanked#test_no_fts5_table_returns_empty().
  TestExecuteSymbolSearchFtsPath.test_falls_back_when_fts_empty: TestExecuteSymbolSearchFtsPath#test_falls_back_when_fts_empty().
  TestExecuteSymbolSearchFtsPath.test_skips_fts_for_short_query: TestExecuteSymbolSearchFtsPath#test_skips_fts_for_short_query().
  _FTS5_AVAILABLE: _FTS5_AVAILABLE.
  _RANKED_ROW: _RANKED_ROW.
  _SCHEMA_FTS: _SCHEMA_FTS.
  TestNormalizeBm25: TestNormalizeBm25#
  TestASTCacheFtsSearchRanked: TestASTCacheFtsSearchRanked#
  TestFtsSymbolToMatch: TestFtsSymbolToMatch#
  TestExecuteSymbolSearchFtsPath: TestExecuteSymbolSearchFtsPath#
---
# Module: [`tests/unit/mcp/test_fts5_bm25_ranking.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py)

## Classes
### `TestASTCacheFtsSearchRanked`
- def: [`tests/unit/mcp/test_fts5_bm25_ranking.py:294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L294)
- signature: `class TestASTCacheFtsSearchRanked:`
- members:
  - `test_delegates_to_query_module(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L295) — When FTS5 available, ASTCache delegates to _ast_cache_query.fts_search_ranked.
  - `test_falls_back_for_short_query(self, tmp_path)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L320) — When query is 1 char, ASTCache falls back without calling FTS5.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`fts_search_ranked`](../../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked), [`fts_search_ranked`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.fts_search_ranked), [`project_root`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.project_root), [`_fts5_available`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache._fts5_available)

### `TestExecuteSymbolSearchFtsPath`
- def: [`tests/unit/mcp/test_fts5_bm25_ranking.py:371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L371)
- signature: `class TestExecuteSymbolSearchFtsPath:`
- members:
  - `test_falls_back_when_fts_empty(self, tmp_path)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L394) — When ASTCache.fts_search_ranked returns [], scatter search runs instead.
  - `test_skips_fts_for_short_query(self, tmp_path)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L421) — Single-character symbol skips the FTS path entirely.
  - `test_uses_fts_when_available(self, tmp_path)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L372) — When ASTCache.fts_search_ranked returns results, response has ranked metadata.
- uses (calls/refs, reference-scoped): [`execute_symbol_search`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#execute_symbol_search)  (1 test-only)

### `TestFtsSearchRanked`
- def: [`tests/unit/mcp/test_fts5_bm25_ranking.py:142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L142)
- signature: `class TestFtsSearchRanked:`
- members:
  - `test_kind_priority_class_over_import(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L216) — Class/function definitions must rank above import entries when BM25 score is equal.
  - `test_language_filter(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L207)
  - `test_limit_respected(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L260)
  - `test_no_fts5_table_returns_empty(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L197) — OperationalError on plain connection without FTS tables → empty list.
  - `test_result_keys(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L269)
  - `test_returns_relevance_score(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L154)
  - `test_score_range(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L179)
  - `test_short_query_returns_empty(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L189)
  - `test_sorted_best_first(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L166) — Exact name match should score higher than partial.
- protocol/private: `_call`[`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L143)
- uses (calls/refs, reference-scoped): [`fts_search_ranked`](../../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked)  (3 test-only)

### `TestFtsSymbolToMatch`
- def: [`tests/unit/mcp/test_fts5_bm25_ranking.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L353)
- signature: `class TestFtsSymbolToMatch:`
- members:
  - `test_shape(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L354)
- uses (calls/refs, reference-scoped): [`_fts_symbol_to_match`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#_fts_symbol_to_match)  (1 test-only)

### `TestNormalizeBm25`
- def: [`tests/unit/mcp/test_fts5_bm25_ranking.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L94)
- signature: `class TestNormalizeBm25:`
- members:
  - `test_clamped_at_one(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L116) — Score cannot exceed 1.0.
  - `test_identical_scores_give_one(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L104) — When all scores are identical raw==worst, result is 1.0.
  - `test_minmax_best_gets_one_worst_gets_zero(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L121) — Min-max normalization: best→1.0, worst→0.0, mid gets proportional score.
  - `test_minmax_weak_match_scores_low(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L128) — Weak match (-0.00002) vs strong match (-0.995) → weak scores near 0.0.
  - `test_positive_raw_returns_zero(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L112) — BM25 scores are always negative; positive value is anomalous → 0.0.
  - `test_worst_is_best_match(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L100) — raw=-1.5 with worst=-0.5 → raw is more negative, so it's the best match → 1.0.
  - `test_worst_match_gives_zero_illegal_input(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L108) — Non-negative raw is illegal BM25 → returns 0.0.
- protocol/private: `_call`[`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L95)
- uses (calls/refs, reference-scoped): [`_normalize_bm25`](../../../tree_sitter_analyzer/_ast_cache_query.md#_normalize_bm25)

## Functions
- `_insert_symbol(conn: sqlite3.Connection, name: str, kind: str = "function", file_path: str = "src/main.py", language: str = "python", line: int = 1, end_line: int = 10)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L47)
- `_make_fts_conn()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L35) — Return an in-memory SQLite connection with FTS5 tables initialised.

## Module values
- `_FTS5_AVAILABLE` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L74)
- `_RANKED_ROW` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L342)
- `_SCHEMA_FTS` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L19)
- `_c` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L76)
- `_skip_no_fts5` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fts5_bm25_ranking.py#L84)

