---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_concepts`/
symbols:
  concept_query_terms: concept_query_terms().
  normalized_query_terms: normalized_query_terms().
  symbol_candidate_tokens: symbol_candidate_tokens().
  concept_entries_for_queries: concept_entries_for_queries().
  _split_seed_queries: _split_seed_queries().
  _dedupe_tokens: _dedupe_tokens().
  narrow_declared_type_entries: narrow_declared_type_entries().
  _clean_identifier: _clean_identifier().
  declared_type_name: declared_type_name().
  _primary_signature_terms: _primary_signature_terms().
  _const_declaration_hint_terms: _const_declaration_hint_terms().
  _declared_type_name: _declared_type_name().
  _IDENTIFIER_RE: _IDENTIFIER_RE.
  symbols_from_concept_entries: symbols_from_concept_entries().
  _declared_const_name: _declared_const_name().
  _declaration_hint_terms: _declaration_hint_terms().
  _QUERY_STOPWORDS: _QUERY_STOPWORDS.
  _receiver_variable_terms: _receiver_variable_terms().
  _is_lower_camel: _is_lower_camel().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py)

## Functions
- `_clean_identifier(raw: str)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L218)
- `_const_declaration_hint_terms(query: str, terms: list[str])` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L266)
- `_declaration_hint_terms(query: str)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L282)
- `_declared_const_name(query: str)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L256)
- `_declared_type_name(query: str)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L251)
- `_dedupe_tokens(tokens: list[str])` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L293)
- `_is_lower_camel(token: str)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L278)
- `_primary_signature_terms(query: str, terms: list[str])` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L233)
- `_receiver_variable_terms(query: str)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L223)
- `_split_seed_queries(queries: list[str])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L198)
- `concept_entries_for_queries(cache: Any, queries: list[str], *, project_root: str, max_files: int)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L50) — Return file-level concept matches for unresolved chain seeds.
- `concept_query_terms(query: str)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L137) — Return terms for source concept search, including declaration hints.
- `declared_type_name(query: str)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L86) — Return the declared type name for ``type X ...`` query strings.
- `narrow_declared_type_entries(queries: list[str], entries: list[dict[str, Any]])` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L91) — Prefer exact ``type X`` declaration matches over broader mentions.
- `normalized_query_terms(query: str)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L115) — Extract identifier-like query terms while dropping syntax noise.
- `symbol_candidate_tokens(query: str)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L71) — Return high-signal resolver tokens for code-like query strings.
- `symbols_from_concept_entries(entries: list[dict[str, Any]], *, limit: int)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L163) — Lift nearby concept-search symbols into the query chain state.

## Module values
- `_IDENTIFIER_RE` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L10)
- `_QUERY_STOPWORDS` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L11)
- `__all__` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.py#L305)

