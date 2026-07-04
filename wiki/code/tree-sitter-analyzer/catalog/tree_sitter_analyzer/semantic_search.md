---
title: 'Module: tree_sitter_analyzer/semantic_search.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/semantic_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.semantic_search`/
symbols:
  SemanticSymbolSearch.search: SemanticSymbolSearch#search().
  SemanticSymbolSearch: SemanticSymbolSearch#
  _vectorize: _vectorize().
  SemanticSymbolSearch._candidate_symbols: SemanticSymbolSearch#_candidate_symbols().
  SemanticSymbolSearch._symbols: SemanticSymbolSearch#_symbols().
  SemanticSymbolSearch.cache: SemanticSymbolSearch#cache.
  SemanticSymbolSearch._BM25_CANDIDATE_MULTIPLIER: SemanticSymbolSearch#_BM25_CANDIDATE_MULTIPLIER.
  _TOKEN_RE: _TOKEN_RE.
  SemanticSymbolSearch._symbols_from_json: SemanticSymbolSearch#_symbols_from_json().
  _symbol_text: _symbol_text().
  _split_identifier_text: _split_identifier_text().
  _normalize_token: _normalize_token().
  _cosine: _cosine().
  SemanticSymbolSearch.__init__: SemanticSymbolSearch#__init__().
---
# Module: [`tree_sitter_analyzer/semantic_search.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py)

## Classes
### `SemanticSymbolSearch`
- def: [`tree_sitter_analyzer/semantic_search.py:17`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L17)
- doc: Deterministic token-vector search for offline symbol discovery.
- signature: `class SemanticSymbolSearch:`
- members:
  - `_candidate_symbols(self, query: str, limit: int)` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L62) — Return a BM25-narrowed candidate pool, or the full symbol set.
  - `search(self, query: str, *, limit: int = 20)` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L26)
  - `cache` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L21)
- protocol/private: `_BM25_CANDIDATE_MULTIPLIER`[`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L24), `__init__`[`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L20), `_symbols`[`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L76), `_symbols_from_json`[`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L98)
- uses (calls/refs, reference-scoped): [`_vectorize`](semantic_search.md#_vectorize), [`_cosine`](semantic_search.md#_cosine), [`_symbol_text`](semantic_search.md#_symbol_text)  (2 test-only)
- used by: [`semantic_symbols`](codegraph_query_backend.md#CodeGraphQueryBackend.semantic_symbols)  (14 test-only)

## Functions
- `_cosine(left: Counter[str], right: Counter[str])` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L155)
- `_normalize_token(token: str)` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L147)
- `_split_identifier_text(text: str)` — [`L142`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L142)
- `_symbol_text(symbol: dict[str, Any])` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L126)
- `_vectorize(text: str)` — [`L132`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L132)

## Module values
- `_TOKEN_RE` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_search.py#L14)

