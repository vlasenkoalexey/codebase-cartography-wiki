---
title: 'Module: tests/unit/test_fts_search_test_demotion.py'
type: catalog
provenance: extracted
module: tests/unit/test_fts_search_test_demotion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_fts_search_test_demotion`/
symbols:
  _insert: _insert().
  TestFtsSearchRankedTestDemotion.test_production_symbol_beats_test_mock_by_default: TestFtsSearchRankedTestDemotion#test_production_symbol_beats_test_mock_by_default().
  TestFtsSearchRankedTestDemotion.test_query_wants_tests_allows_test_symbol_up: TestFtsSearchRankedTestDemotion#test_query_wants_tests_allows_test_symbol_up().
  TestFtsSearchRankedTestDemotion.test_multiple_test_symbols_demoted_below_single_production: TestFtsSearchRankedTestDemotion#test_multiple_test_symbols_demoted_below_single_production().
  TestFtsSearchRankedTestDemotion.test_production_promoted_even_when_buried_past_limit: TestFtsSearchRankedTestDemotion#test_production_promoted_even_when_buried_past_limit().
  TestFtsSearchRankedTestDemotion.test_secondary_sort_is_relevance_within_same_tier: TestFtsSearchRankedTestDemotion#test_secondary_sort_is_relevance_within_same_tier().
  TestFtsSearchRankedTestDemotion.test_language_filter_preserved_with_demotion: TestFtsSearchRankedTestDemotion#test_language_filter_preserved_with_demotion().
  TestFtsSearchRankedTestDemotion.test_empty_query_returns_empty: TestFtsSearchRankedTestDemotion#test_empty_query_returns_empty().
  _make_fts_conn: _make_fts_conn().
  TestFtsSearchRankedTestDemotion: TestFtsSearchRankedTestDemotion#
---
# Module: [`tests/unit/test_fts_search_test_demotion.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py)

## Classes
### `TestFtsSearchRankedTestDemotion`
- def: [`tests/unit/test_fts_search_test_demotion.py:71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L71)
- doc: Production symbol must rank above test-file mock with the same name.
- signature: `class TestFtsSearchRankedTestDemotion:`
- members:
  - `test_empty_query_returns_empty(self)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L253) — Short queries still short-circuit (unchanged behavior).
  - `test_language_filter_preserved_with_demotion(self)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L221) — language= filter still works after demotion is added.
  - `test_multiple_test_symbols_demoted_below_single_production(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L138) — Several test-file symbols all rank below the one production symbol.
  - `test_production_promoted_even_when_buried_past_limit(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L167) — Codex P2 on #316: over-fetch so a production hit BM25-ranked outside
  - `test_production_symbol_beats_test_mock_by_default(self)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L74) — Core regression: fts_search_ranked returns production file first.
  - `test_query_wants_tests_allows_test_symbol_up(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L116) — When query contains 'test', test symbols are NOT demoted.
  - `test_secondary_sort_is_relevance_within_same_tier(self)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L205) — Within the production tier, relevance_score is set for all results.
- uses (calls/refs, reference-scoped): [`fts_search_ranked`](../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked)  (2 test-only)

## Functions
- `_insert(conn: sqlite3.Connection, name: str, *, kind: str = "function", file_path: str = "src/foo.py", language: str = "python", line: int = 1)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L43)
- `_make_fts_conn()` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_search_test_demotion.py#L21) — Return an in-memory connection with the FTS5 schema used by fts_search_ranked.

