---
title: 'Module: tests/unit/test_ast_cache_cascade_search.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_cascade_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_cascade_search`/
symbols:
  test_cascade_private_fallback_helpers_cover_error_paths: test_cascade_private_fallback_helpers_cover_error_paths().
  test_cascade_conceptual_query_promotes_production_above_tests: test_cascade_conceptual_query_promotes_production_above_tests().
  _insert: _insert().
  test_cascade_test_intent_query_keeps_test_symbols_on_top: test_cascade_test_intent_query_keeps_test_symbols_on_top().
  test_cascade_search_exact_tier_scores_first: test_cascade_search_exact_tier_scores_first().
  test_cascade_search_like_fallback: test_cascade_search_like_fallback().
  test_cascade_search_fuzzy_fallback_handles_typo: test_cascade_search_fuzzy_fallback_handles_typo().
  test_cascade_search_respects_language_filter: test_cascade_search_respects_language_filter().
  test_cascade_search_short_or_empty_queries_stop_early: test_cascade_search_short_or_empty_queries_stop_early().
  _make_conn: _make_conn().
  _seed_q3_style_rows: _seed_q3_style_rows().
  _make_fts_conn: _make_fts_conn().
  _insert_fts: _insert_fts().
  _Q3_STYLE_QUERY: _Q3_STYLE_QUERY.
  _Q3_STYLE_TEST_NAMES: _Q3_STYLE_TEST_NAMES.
---
# Module: [`tests/unit/test_ast_cache_cascade_search.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py)

## Functions
- `_insert(conn: sqlite3.Connection, name: str, kind: str = "function", file_path: str = "app.py", language: str = "python", line: int = 1)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L25)
- `_insert_fts(conn: sqlite3.Connection, name: str, kind: str = "function", file_path: str = "app.py", language: str = "python", line: int = 1)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L164)
- `_make_conn()` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L8)
- `_make_fts_conn()` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L153) — In-memory conn with the production FTS5 schema (porter, #604/#606).
- `_seed_q3_style_rows(conn: sqlite3.Connection)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L194) — 1 production symbol + 6 test symbols sharing MORE query tokens.
- `test_cascade_conceptual_query_promotes_production_above_tests()` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L210) — #607 RED: top-`limit` window must not be saturated by test symbols.
- `test_cascade_private_fallback_helpers_cover_error_paths()` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L104)
- `test_cascade_search_exact_tier_scores_first()` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L41)
- `test_cascade_search_fuzzy_fallback_handles_typo()` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L67)
- `test_cascade_search_like_fallback()` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L54)
- `test_cascade_search_respects_language_filter()` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L80)
- `test_cascade_search_short_or_empty_queries_stop_early()` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L92)
- `test_cascade_test_intent_query_keeps_test_symbols_on_top()` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L231) — Counter-direction pin: a query that asks about tests is NOT demoted.

## Module values
- `_Q3_STYLE_QUERY` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L150)
- `_Q3_STYLE_TEST_NAMES` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_cascade_search.py#L184)

