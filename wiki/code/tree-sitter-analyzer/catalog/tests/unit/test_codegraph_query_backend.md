---
title: 'Module: tests/unit/test_codegraph_query_backend.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_backend.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_backend`/
symbols:
  test_backend_resolves_definitions_without_symbol_resolver: test_backend_resolves_definitions_without_symbol_resolver().
  test_backend_falls_back_to_symbols_json: test_backend_falls_back_to_symbols_json().
  test_backend_semantic_symbols_rank_token_vector_matches: test_backend_semantic_symbols_rank_token_vector_matches().
  test_backend_semantic_symbols_maps_semantic_score_to_confidence: test_backend_semantic_symbols_maps_semantic_score_to_confidence().
  test_backend_resolves_enum_as_definition: test_backend_resolves_enum_as_definition().
  RowCache: RowCache#
  _connect: _connect().
  test_backend_prefers_fts_definition_rows: test_backend_prefers_fts_definition_rows().
  test_backend_normalizes_callers_and_callees_from_cache_rows: test_backend_normalizes_callers_and_callees_from_cache_rows().
  RowCache.get_conn: RowCache#get_conn().
  RowCache._get_conn: RowCache#_get_conn().
  RowCache.conn: RowCache#conn.
  RowCache._fts5_available: RowCache#_fts5_available.
  RowCache.fts5_available: RowCache#fts5_available.
  RowCache.__init__: RowCache#__init__().
---
# Module: [`tests/unit/test_codegraph_query_backend.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py)

## Classes
### `RowCache`
- def: [`tests/unit/test_codegraph_query_backend.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L14)
- signature: `class RowCache:`
- members:
  - `get_conn(self)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L21)
  - `conn` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L19)
  - `fts5_available` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L16)
- protocol/private: `__init__`[`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L18), `_fts5_available`[`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L15), `_get_conn`[`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L24)
- used by: (5 test-only callers)

## Functions
- `_connect()` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L28)
- `test_backend_falls_back_to_symbols_json()` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L100)
- `test_backend_normalizes_callers_and_callees_from_cache_rows()` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L209)
- `test_backend_prefers_fts_definition_rows()` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L69)
- `test_backend_resolves_definitions_without_symbol_resolver()` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L34)
- `test_backend_resolves_enum_as_definition()` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L251) — #961 split: ``enum`` rows are definition sites (added to kind filter).
- `test_backend_semantic_symbols_maps_semantic_score_to_confidence()` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L173) — semantic_symbols must populate 'confidence' from semantic_score.
- `test_backend_semantic_symbols_rank_token_vector_matches()` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_backend.py#L146)

