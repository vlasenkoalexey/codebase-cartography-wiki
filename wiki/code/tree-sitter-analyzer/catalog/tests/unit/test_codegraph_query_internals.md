---
title: 'Module: tests/unit/test_codegraph_query_internals.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_internals.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_internals`/TestCodeGraphQueryInternals#
symbols:
  TestCodeGraphQueryInternals.test_apply_concept_fallback_degrades_on_missing_seed_or_matches: test_apply_concept_fallback_degrades_on_missing_seed_or_matches().
  TestCodeGraphQueryInternals.test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors: test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors().
  TestCodeGraphQueryInternals.test_query_concept_token_normalization_prefers_signature_names: test_query_concept_token_normalization_prefers_signature_names().
  TestCodeGraphQueryInternals.test_query_state_add_symbols_dedupes_repeated_entries: test_query_state_add_symbols_dedupes_repeated_entries().
  TestCodeGraphQueryInternals.test_uml_facet_uses_current_symbols_when_no_relationships: test_uml_facet_uses_current_symbols_when_no_relationships().
  TestCodeGraphQueryInternals.test_resolve_query_normalizes_code_like_signature_tokens: test_resolve_query_normalizes_code_like_signature_tokens().
  TestCodeGraphQueryInternals.test_resolve_query_filters_non_declaration_for_type_query: test_resolve_query_filters_non_declaration_for_type_query().
  TestCodeGraphQueryInternals.test_resolve_query_keeps_matching_declaration_for_type_query: test_resolve_query_keeps_matching_declaration_for_type_query().
  TestCodeGraphQueryInternals.test_resolve_query_drops_test_shadow_when_source_definition_exists: test_resolve_query_drops_test_shadow_when_source_definition_exists().
  TestCodeGraphQueryInternals.test_resolve_query_keeps_test_shadow_with_file_hint: test_resolve_query_keeps_test_shadow_with_file_hint().
  TestCodeGraphQueryInternals.test_resolve_queries_stops_at_limit_and_dedupes: test_resolve_queries_stops_at_limit_and_dedupes().
  TestCodeGraphQueryInternals.test_filter_symbols_supports_predicates_and_inverse_selection: test_filter_symbols_supports_predicates_and_inverse_selection().
  TestCodeGraphQueryInternals.test_filter_symbols_reports_bad_regex: test_filter_symbols_reports_bad_regex().
  TestCodeGraphQueryInternals.test_filter_symbols_covers_empty_case_and_negative_predicates: test_filter_symbols_covers_empty_case_and_negative_predicates().
  TestCodeGraphQueryInternals.test_declared_type_entries_keep_broad_matches_without_exact_declaration: test_declared_type_entries_keep_broad_matches_without_exact_declaration().
  TestCodeGraphQueryInternals.test_query_concept_helpers_cover_empty_dedupe_and_limit_paths: test_query_concept_helpers_cover_empty_dedupe_and_limit_paths().
  TestCodeGraphQueryInternals.test_declaration_query_filter_keeps_unrelated_symbols: test_declaration_query_filter_keeps_unrelated_symbols().
  TestCodeGraphQueryInternals.test_declared_type_entries_prefer_exact_type_declaration: test_declared_type_entries_prefer_exact_type_declaration().
  TestCodeGraphQueryInternals.test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors.FailingBackend: test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors().FailingBackend#
  TestCodeGraphQueryInternals: ''
  TestCodeGraphQueryInternals.test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors.FailingBackend.__init__: test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors().FailingBackend#__init__().
  ? TestCodeGraphQueryInternals.test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors.FailingBackend.resolve_definitions
  : test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors().FailingBackend#resolve_definitions().
---
# Module: [`tests/unit/test_codegraph_query_internals.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py)

## Classes
### `FailingBackend`
- def: [`tests/unit/test_codegraph_query_internals.py:116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L116)
- signature: `class FailingBackend:`
- members:
  - `resolve_definitions(self, token)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L120)
- protocol/private: `__init__`[`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L117)
- used by: (1 test-only callers)

### `TestCodeGraphQueryInternals`
- def: [`tests/unit/test_codegraph_query_internals.py:23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L23)
- signature: `class TestCodeGraphQueryInternals:`
- members:
  - `test_apply_concept_fallback_degrades_on_missing_seed_or_matches(self)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L311)
  - `test_declaration_query_filter_keeps_unrelated_symbols(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L179)
  - `test_declared_type_entries_keep_broad_matches_without_exact_declaration(self)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L282)
  - `test_declared_type_entries_prefer_exact_type_declaration(self)` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L266)
  - `test_filter_symbols_covers_empty_case_and_negative_predicates(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L68)
  - `test_filter_symbols_reports_bad_regex(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L61)
  - `test_filter_symbols_supports_predicates_and_inverse_selection(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L24)
  - `test_query_concept_helpers_cover_empty_dedupe_and_limit_paths(self)` — [`L339`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L339)
  - `test_query_concept_token_normalization_prefers_signature_names(self)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L212)
  - `test_query_state_add_symbols_dedupes_repeated_entries(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L94)
  - `test_resolve_queries_stops_at_limit_and_dedupes(self)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L296)
  - `test_resolve_query_drops_test_shadow_when_source_definition_exists(self)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L186)
  - `test_resolve_query_filters_non_declaration_for_type_query(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L146)
  - `test_resolve_query_keeps_matching_declaration_for_type_query(self)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L158)
  - `test_resolve_query_keeps_test_shadow_with_file_hint(self)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L199)
  - `test_resolve_query_normalizes_code_like_signature_tokens(self)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L129)
  - `test_resolve_query_uses_raw_query_fallback_and_handles_resolver_errors(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L112)
  - `test_uml_facet_uses_current_symbols_when_no_relationships(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals.py#L102)
- uses (calls/refs, reference-scoped): [`_ChainStep`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep), [`current`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.current), [`_apply_concept_fallback`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_apply_concept_fallback), [`_QueryState`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState), [`concept_query_terms`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#concept_query_terms), [`normalized_query_terms`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#normalized_query_terms), [`symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.symbols), [`symbol_candidate_tokens`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#symbol_candidate_tokens), [`uml_facet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_facets.md#uml_facet), [`files`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.files), [`filter_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.md#filter_symbols), [`add_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.add_symbols), [`_resolve_query`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_resolve_query), [`concept_entries_for_queries`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#concept_entries_for_queries), [`_filter_declaration_query_symbols`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_filter_declaration_query_symbols), [`_resolve_queries`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_resolve_queries), [`seed_queries`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.seed_queries), [`narrow_declared_type_entries`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#narrow_declared_type_entries), [`_primary_signature_terms`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#_primary_signature_terms), [`declared_type_name`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#declared_type_name), [`symbols_from_concept_entries`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_concepts.md#symbols_from_concept_entries)  (3 test-only)

