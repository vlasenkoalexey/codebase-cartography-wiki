---
title: 'Module: tests/unit/test_semantic_symbol_search.py'
type: catalog
provenance: extracted
module: tests/unit/test_semantic_symbol_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_semantic_symbol_search`/
symbols:
  _make_cache: _make_cache().
  TestSemanticSymbolSearchBm25Path.test_candidate_pool_size_is_multiplied: TestSemanticSymbolSearchBm25Path#test_candidate_pool_size_is_multiplied().
  TestSemanticSymbolSearchFallback.test_returns_scored_results: TestSemanticSymbolSearchFallback#test_returns_scored_results().
  TestSemanticSymbolSearchFallback.test_short_query_uses_full_scan: TestSemanticSymbolSearchFallback#test_short_query_uses_full_scan().
  TestSemanticSymbolSearchFallback.test_empty_query_returns_empty: TestSemanticSymbolSearchFallback#test_empty_query_returns_empty().
  TestSemanticSymbolSearchFallback.test_no_fts5_uses_full_scan: TestSemanticSymbolSearchFallback#test_no_fts5_uses_full_scan().
  TestSemanticSymbolSearchBm25Path.test_bm25_prefilter_called_for_long_query: TestSemanticSymbolSearchBm25Path#test_bm25_prefilter_called_for_long_query().
  TestSemanticSymbolSearchBm25Path.test_falls_back_when_fts_returns_empty: TestSemanticSymbolSearchBm25Path#test_falls_back_when_fts_returns_empty().
  TestSemanticSymbolSearchBm25Path.test_semantic_score_in_results: TestSemanticSymbolSearchBm25Path#test_semantic_score_in_results().
  TestSemanticSymbolSearchBm25Path.test_fts_exception_falls_back_to_full_scan: TestSemanticSymbolSearchBm25Path#test_fts_exception_falls_back_to_full_scan().
  TestSemanticSymbolSearchFallbackSchema.test_symbols_from_json_returns_results: TestSemanticSymbolSearchFallbackSchema#test_symbols_from_json_returns_results().
  TestSemanticSymbolSearchTestDeprioritization.test_impl_ranks_above_test_for_concept_query: TestSemanticSymbolSearchTestDeprioritization#test_impl_ranks_above_test_for_concept_query().
  TestSemanticSymbolSearchTestDeprioritization.test_test_intent_query_keeps_tests_on_top: TestSemanticSymbolSearchTestDeprioritization#test_test_intent_query_keeps_tests_on_top().
  TestSemanticSymbolSearchFallbackSchema.test_symbols_from_json_empty_on_corrupt_row: TestSemanticSymbolSearchFallbackSchema#test_symbols_from_json_empty_on_corrupt_row().
  TestSemanticSymbolSearchFallbackSchema.test_symbols_from_json_fallback_on_symbol_rows_error: TestSemanticSymbolSearchFallbackSchema#test_symbols_from_json_fallback_on_symbol_rows_error().
  _SCHEMA: _SCHEMA.
  TestSemanticSymbolSearchFallbackSchema._make_legacy_cache: TestSemanticSymbolSearchFallbackSchema#_make_legacy_cache().
  TestSemanticSymbolSearchFallback: TestSemanticSymbolSearchFallback#
  TestSemanticSymbolSearchBm25Path: TestSemanticSymbolSearchBm25Path#
  TestSemanticSymbolSearchFallbackSchema: TestSemanticSymbolSearchFallbackSchema#
  TestSemanticSymbolSearchTestDeprioritization: TestSemanticSymbolSearchTestDeprioritization#
---
# Module: [`tests/unit/test_semantic_symbol_search.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py)

## Classes
### `TestSemanticSymbolSearchBm25Path`
- def: [`tests/unit/test_semantic_symbol_search.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L107)
- signature: `class TestSemanticSymbolSearchBm25Path:`
- members:
  - `test_bm25_prefilter_called_for_long_query(self)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L108)
  - `test_candidate_pool_size_is_multiplied(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L125) — Pool size = limit * _BM25_CANDIDATE_MULTIPLIER.
  - `test_falls_back_when_fts_returns_empty(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L116) — When BM25 finds nothing, fall back to full scan.
  - `test_fts_exception_falls_back_to_full_scan(self)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L150) — When fts_search_ranked raises, _candidate_symbols catches and falls back.
  - `test_semantic_score_in_results(self)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L136)
- uses (calls/refs, reference-scoped): [`search`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch.search), [`SemanticSymbolSearch`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch), [`_BM25_CANDIDATE_MULTIPLIER`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch._BM25_CANDIDATE_MULTIPLIER)  (1 test-only)

### `TestSemanticSymbolSearchFallback`
- def: [`tests/unit/test_semantic_symbol_search.py:66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L66)
- signature: `class TestSemanticSymbolSearchFallback:`
- members:
  - `test_empty_query_returns_empty(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L91)
  - `test_no_fts5_uses_full_scan(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L96)
  - `test_returns_scored_results(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L67)
  - `test_short_query_uses_full_scan(self)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L82) — Queries shorter than 2 chars bypass BM25 pre-filter.
- uses (calls/refs, reference-scoped): [`search`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch.search), [`SemanticSymbolSearch`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch)  (1 test-only)

### `TestSemanticSymbolSearchFallbackSchema`
- def: [`tests/unit/test_semantic_symbol_search.py:160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L160)
- doc: Tests for the _symbols_from_json path used on older DB schemas.
- signature: `class TestSemanticSymbolSearchFallbackSchema:`
- members:
  - `_make_legacy_cache(self, rows: list[tuple[str, str, str, str]])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L163) — Cache backed by ast_index (no ast_symbol_rows table).
  - `test_symbols_from_json_empty_on_corrupt_row(self)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L194)
  - `test_symbols_from_json_fallback_on_symbol_rows_error(self)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L211) — ast_symbol_rows raises sqlite3.Error → falls back to _symbols_from_json.
  - `test_symbols_from_json_returns_results(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L185)
- uses (calls/refs, reference-scoped): [`search`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch.search), [`SemanticSymbolSearch`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch)

### `TestSemanticSymbolSearchTestDeprioritization`
- def: [`tests/unit/test_semantic_symbol_search.py:238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L238)
- doc: Impl symbols must rank above test symbols (shared utils.test_detection).
- signature: `class TestSemanticSymbolSearchTestDeprioritization:`
- members:
  - `test_impl_ranks_above_test_for_concept_query(self)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L241)
  - `test_test_intent_query_keeps_tests_on_top(self)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L256)
- uses (calls/refs, reference-scoped): [`search`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch.search), [`SemanticSymbolSearch`](../../tree_sitter_analyzer/semantic_search.md#SemanticSymbolSearch)  (1 test-only)

## Functions
- `_make_cache(rows: list[tuple[str, str, str, str]])` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L30) — Return a mock cache with FTS5 + symbol_rows seeded from rows.

## Module values
- `_SCHEMA` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_symbol_search.py#L15)

