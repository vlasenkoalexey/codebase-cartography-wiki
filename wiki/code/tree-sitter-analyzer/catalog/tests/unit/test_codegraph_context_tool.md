---
title: 'Module: tests/unit/test_codegraph_context_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_context_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_context_tool`/
symbols:
  test_small_helpers_cover_bounds_and_fallbacks: test_small_helpers_cover_bounds_and_fallbacks().
  test_context_ignores_edgestore_when_only_non_call_edges: test_context_ignores_edgestore_when_only_non_call_edges().
  test_call_graph_falls_back_when_edgestore_probe_fails: test_call_graph_falls_back_when_edgestore_probe_fails().
  test_context_uses_edgestore_without_lazy_callgraph_parse: test_context_uses_edgestore_without_lazy_callgraph_parse().
  test_expand_nodes_handles_graph_limits_and_trace_chain: test_expand_nodes_handles_graph_limits_and_trace_chain().
  test_expand_nodes_handles_edgestore_query_errors: test_expand_nodes_handles_edgestore_query_errors().
  test_build_edges_handles_fallback_targets_and_duplicates: test_build_edges_handles_fallback_targets_and_duplicates().
  test_build_edges_handles_edgestore_targets_and_duplicates: test_build_edges_handles_edgestore_targets_and_duplicates().
  test_next_step_honest_when_only_non_prod_matches: test_next_step_honest_when_only_non_prod_matches().
  test_tool_accessors_require_project_root: test_tool_accessors_require_project_root().
  test_resolve_entry_points_degrades_and_dedupes: test_resolve_entry_points_degrades_and_dedupes().
  test_resolve_entry_points_handles_cache_and_search_errors: test_resolve_entry_points_handles_cache_and_search_errors().
  test_resolve_entry_points_stops_at_limit: test_resolve_entry_points_stops_at_limit().
  test_resolve_entry_points_ranks_multiword_name_match_first: test_resolve_entry_points_ranks_multiword_name_match_first().
  test_entry_rank_v2_sinks_test_file_below_impl: test_entry_rank_v2_sinks_test_file_below_impl().
  test_resolve_entry_points_keeps_tests_when_task_wants_tests: test_resolve_entry_points_keeps_tests_when_task_wants_tests().
  test_resolve_entry_points_uses_compound_recall_for_multiword: test_resolve_entry_points_uses_compound_recall_for_multiword().
  test_resolve_entry_points_single_word_falls_back_to_substring_cascade: test_resolve_entry_points_single_word_falls_back_to_substring_cascade().
  test_resolve_entry_points_skips_cascade_when_fts_has_hits: test_resolve_entry_points_skips_cascade_when_fts_has_hits().
  test_resolve_entry_points_falls_back_when_fts_only_returns_imports: test_resolve_entry_points_falls_back_when_fts_only_returns_imports().
  test_examples_and_scripts_ranked_below_production: test_examples_and_scripts_ranked_below_production().
  indexed_project: indexed_project().
  test_edge_store_accessor_degrades_without_cache_connection: test_edge_store_accessor_degrades_without_cache_connection().
  test_build_code_blocks_truncates_long_bodies: test_build_code_blocks_truncates_long_bodies().
  test_context_caps_inline_edges: test_context_caps_inline_edges().
  test_schema_requires_task: test_schema_requires_task().
  test_build_code_blocks_hints_when_end_unknown: test_build_code_blocks_hints_when_end_unknown().
  test_build_code_blocks_keeps_short_bodies_untruncated: test_build_code_blocks_keeps_short_bodies_untruncated().
  test_context_returns_entry_points_graph_and_source: test_context_returns_entry_points_graph_and_source().
  test_context_not_found_is_a_successful_stop_signal: test_context_not_found_is_a_successful_stop_signal().
  test_context_lean_default_omits_nodes_edges: test_context_lean_default_omits_nodes_edges().
  test_context_include_graph_true_returns_full_nodes_edges: test_context_include_graph_true_returns_full_nodes_edges().
  test_context_include_graph_string_false_stays_lean: test_context_include_graph_string_false_stays_lean().
  test_context_lean_stats_advertise_graph_totals: test_context_lean_stats_advertise_graph_totals().
  test_context_related_symbols_grouped_by_file: test_context_related_symbols_grouped_by_file().
  test_build_related_symbols_groups_by_file: test_build_related_symbols_groups_by_file().
  test_entry_point_body_inlines_full_under_budget: test_entry_point_body_inlines_full_under_budget().
  test_entry_point_ranked_before_high_degree_noise: test_entry_point_ranked_before_high_degree_noise().
  test_next_step_references_top_symbol_when_production_match_found: test_next_step_references_top_symbol_when_production_match_found().
  test_codegraph_context_registered: test_codegraph_context_registered().
  test_extract_symbol_candidates_handles_identifiers: test_extract_symbol_candidates_handles_identifiers().
  test_call_graph_falls_back_when_edgestore_probe_fails.FakeCachedCallGraph.build: test_call_graph_falls_back_when_edgestore_probe_fails().FakeCachedCallGraph#build().
  test_name_match_score_counts_distinct_task_words: test_name_match_score_counts_distinct_task_words().
  test_is_test_file_detects_cross_language_test_paths: test_is_test_file_detects_cross_language_test_paths().
  test_task_wants_tests_detects_test_intent: test_task_wants_tests_detects_test_intent().
  test_compound_candidates_builds_camelcase_word_pairs: test_compound_candidates_builds_camelcase_word_pairs().
  test_build_code_blocks_skips_empty_snippets: test_build_code_blocks_skips_empty_snippets().
  test_generic_verbs_dropped_when_specific_candidate_present: test_generic_verbs_dropped_when_specific_candidate_present().
  test_english_connectives_filtered_from_candidates: test_english_connectives_filtered_from_candidates().
  test_generic_verb_kept_when_sole_signal: test_generic_verb_kept_when_sole_signal().
  test_quoted_generic_verb_is_kept_as_explicit_symbol: test_quoted_generic_verb_is_kept_as_explicit_symbol().
  test_qualified_generic_method_is_kept: test_qualified_generic_method_is_kept().
  test_non_dot_qualified_generic_methods_are_kept: test_non_dot_qualified_generic_methods_are_kept().
  test_lowercase_qualified_anchor_still_drops_bare_verb: test_lowercase_qualified_anchor_still_drops_bare_verb().
  test_file_path_does_not_anchor_filter: test_file_path_does_not_anchor_filter().
  test_snake_or_camel_path_components_do_not_anchor_filter: test_snake_or_camel_path_components_do_not_anchor_filter().
  test_windows_path_components_do_not_anchor_filter: test_windows_path_components_do_not_anchor_filter().
  test_generic_nouns_and_stop_words_not_candidates: test_generic_nouns_and_stop_words_not_candidates().
  test_quoted_stop_word_token_kept_as_candidate: test_quoted_stop_word_token_kept_as_candidate().
  test_capitalized_stop_word_kept_unquoted: test_capitalized_stop_word_kept_unquoted().
  test_plain_lowercase_stop_word_still_filtered: test_plain_lowercase_stop_word_still_filtered().
  test_wants_tests_skips_non_prod_demotion: test_wants_tests_skips_non_prod_demotion().
  test_is_non_prod_file_branches: test_is_non_prod_file_branches().
  test_next_step_lean_non_prod_only_warns: test_next_step_lean_non_prod_only_warns().
  test_next_step_lean_entry_points_without_code: test_next_step_lean_entry_points_without_code().
  test_next_step_lean_production_anchor: test_next_step_lean_production_anchor().
  test_call_graph_falls_back_when_edgestore_probe_fails.FakeCachedCallGraph: test_call_graph_falls_back_when_edgestore_probe_fails().FakeCachedCallGraph#
  FakeCachedCallGraph.built: FakeCachedCallGraph#built.
  test_call_graph_falls_back_when_edgestore_probe_fails.BrokenEdgeStore: test_call_graph_falls_back_when_edgestore_probe_fails().BrokenEdgeStore#
  test_call_graph_falls_back_when_edgestore_probe_fails.FakeCache: test_call_graph_falls_back_when_edgestore_probe_fails().FakeCache#
  FakeCachedCallGraph.cache: FakeCachedCallGraph#cache.
  FakeCachedCallGraph.fallback: FakeCachedCallGraph#fallback.
  test_resolve_entry_points_degrades_and_dedupes.FallbackCache: test_resolve_entry_points_degrades_and_dedupes().FallbackCache#
  test_resolve_entry_points_handles_cache_and_search_errors.BrokenCache: test_resolve_entry_points_handles_cache_and_search_errors().BrokenCache#
  test_resolve_entry_points_stops_at_limit.ManyHitsCache: test_resolve_entry_points_stops_at_limit().ManyHitsCache#
  test_resolve_entry_points_ranks_multiword_name_match_first.RankedCache: test_resolve_entry_points_ranks_multiword_name_match_first().RankedCache#
  test_entry_rank_v2_sinks_test_file_below_impl.TestVsImplCache: test_entry_rank_v2_sinks_test_file_below_impl().TestVsImplCache#
  test_resolve_entry_points_keeps_tests_when_task_wants_tests.TestIntentCache: test_resolve_entry_points_keeps_tests_when_task_wants_tests().TestIntentCache#
  test_resolve_entry_points_uses_compound_recall_for_multiword.CompoundCache: test_resolve_entry_points_uses_compound_recall_for_multiword().CompoundCache#
  test_resolve_entry_points_single_word_falls_back_to_substring_cascade.CamelCaseCache: test_resolve_entry_points_single_word_falls_back_to_substring_cascade().CamelCaseCache#
  test_resolve_entry_points_skips_cascade_when_fts_has_hits.ExactCache: test_resolve_entry_points_skips_cascade_when_fts_has_hits().ExactCache#
  test_resolve_entry_points_falls_back_when_fts_only_returns_imports.ImportOnlyCache: test_resolve_entry_points_falls_back_when_fts_only_returns_imports().ImportOnlyCache#
  test_expand_nodes_handles_graph_limits_and_trace_chain.FakeGraph: test_expand_nodes_handles_graph_limits_and_trace_chain().FakeGraph#
  test_expand_nodes_handles_edgestore_query_errors.BrokenEdgeGraph: test_expand_nodes_handles_edgestore_query_errors().BrokenEdgeGraph#
  test_build_edges_handles_fallback_targets_and_duplicates.EdgeGraph: test_build_edges_handles_fallback_targets_and_duplicates().EdgeGraph#
  test_build_edges_handles_edgestore_targets_and_duplicates.EdgeStoreGraph: test_build_edges_handles_edgestore_targets_and_duplicates().EdgeStoreGraph#
  test_small_helpers_cover_bounds_and_fallbacks.always_fails: test_small_helpers_cover_bounds_and_fallbacks().always_fails().
  test_small_helpers_cover_bounds_and_fallbacks.falls_back_to_one_arg: test_small_helpers_cover_bounds_and_fallbacks().falls_back_to_one_arg().
  test_small_helpers_cover_bounds_and_fallbacks.ChainFallback: test_small_helpers_cover_bounds_and_fallbacks().ChainFallback#
  test_small_helpers_cover_bounds_and_fallbacks.ChainBroken: test_small_helpers_cover_bounds_and_fallbacks().ChainBroken#
  test_context_uses_edgestore_without_lazy_callgraph_parse.fail_if_lazy_parse_builds: test_context_uses_edgestore_without_lazy_callgraph_parse().fail_if_lazy_parse_builds().
  test_examples_and_scripts_ranked_below_production.MixedCache: test_examples_and_scripts_ranked_below_production().MixedCache#
  test_call_graph_falls_back_when_edgestore_probe_fails.BrokenEdgeStore.has_edges: test_call_graph_falls_back_when_edgestore_probe_fails().BrokenEdgeStore#has_edges().
  test_call_graph_falls_back_when_edgestore_probe_fails.FakeCachedCallGraph.__init__: test_call_graph_falls_back_when_edgestore_probe_fails().FakeCachedCallGraph#__init__().
  FakeCachedCallGraph.project_root: FakeCachedCallGraph#project_root.
  test_resolve_entry_points_degrades_and_dedupes.FallbackCache.fts_search_ranked: test_resolve_entry_points_degrades_and_dedupes().FallbackCache#fts_search_ranked().
  test_resolve_entry_points_degrades_and_dedupes.FallbackCache.fts_search: test_resolve_entry_points_degrades_and_dedupes().FallbackCache#fts_search().
  test_resolve_entry_points_handles_cache_and_search_errors.BrokenCache.fts_search_ranked: test_resolve_entry_points_handles_cache_and_search_errors().BrokenCache#fts_search_ranked().
  test_resolve_entry_points_handles_cache_and_search_errors.BrokenCache.fts_search: test_resolve_entry_points_handles_cache_and_search_errors().BrokenCache#fts_search().
  test_resolve_entry_points_stops_at_limit.ManyHitsCache.fts_search_ranked: test_resolve_entry_points_stops_at_limit().ManyHitsCache#fts_search_ranked().
  test_resolve_entry_points_ranks_multiword_name_match_first.RankedCache.fts_search_ranked: test_resolve_entry_points_ranks_multiword_name_match_first().RankedCache#fts_search_ranked().
  test_entry_rank_v2_sinks_test_file_below_impl.TestVsImplCache.fts_search_ranked: test_entry_rank_v2_sinks_test_file_below_impl().TestVsImplCache#fts_search_ranked().
  test_resolve_entry_points_keeps_tests_when_task_wants_tests.TestIntentCache.fts_search_ranked: test_resolve_entry_points_keeps_tests_when_task_wants_tests().TestIntentCache#fts_search_ranked().
  test_resolve_entry_points_uses_compound_recall_for_multiword.CompoundCache.fts_search_ranked: test_resolve_entry_points_uses_compound_recall_for_multiword().CompoundCache#fts_search_ranked().
  test_resolve_entry_points_uses_compound_recall_for_multiword.CompoundCache.search_symbols_cascade: test_resolve_entry_points_uses_compound_recall_for_multiword().CompoundCache#search_symbols_cascade().
  test_resolve_entry_points_single_word_falls_back_to_substring_cascade.CamelCaseCache.fts_search_ranked: test_resolve_entry_points_single_word_falls_back_to_substring_cascade().CamelCaseCache#fts_search_ranked().
  test_resolve_entry_points_single_word_falls_back_to_substring_cascade.CamelCaseCache.search_symbols_cascade: test_resolve_entry_points_single_word_falls_back_to_substring_cascade().CamelCaseCache#search_symbols_cascade().
  test_resolve_entry_points_skips_cascade_when_fts_has_hits.ExactCache.fts_search_ranked: test_resolve_entry_points_skips_cascade_when_fts_has_hits().ExactCache#fts_search_ranked().
  test_resolve_entry_points_skips_cascade_when_fts_has_hits.ExactCache.search_symbols_cascade: test_resolve_entry_points_skips_cascade_when_fts_has_hits().ExactCache#search_symbols_cascade().
  test_resolve_entry_points_falls_back_when_fts_only_returns_imports.ImportOnlyCache.fts_search_ranked: test_resolve_entry_points_falls_back_when_fts_only_returns_imports().ImportOnlyCache#fts_search_ranked().
  test_resolve_entry_points_falls_back_when_fts_only_returns_imports.ImportOnlyCache.search_symbols_cascade: test_resolve_entry_points_falls_back_when_fts_only_returns_imports().ImportOnlyCache#search_symbols_cascade().
  test_expand_nodes_handles_graph_limits_and_trace_chain.FakeGraph.callees_of: test_expand_nodes_handles_graph_limits_and_trace_chain().FakeGraph#callees_of().
  test_expand_nodes_handles_graph_limits_and_trace_chain.FakeGraph.callers_of: test_expand_nodes_handles_graph_limits_and_trace_chain().FakeGraph#callers_of().
  test_expand_nodes_handles_graph_limits_and_trace_chain.FakeGraph.call_chain: test_expand_nodes_handles_graph_limits_and_trace_chain().FakeGraph#call_chain().
  test_expand_nodes_handles_edgestore_query_errors.BrokenEdgeGraph.query_callees: test_expand_nodes_handles_edgestore_query_errors().BrokenEdgeGraph#query_callees().
  test_expand_nodes_handles_edgestore_query_errors.BrokenEdgeGraph.query_callers: test_expand_nodes_handles_edgestore_query_errors().BrokenEdgeGraph#query_callers().
  test_build_edges_handles_fallback_targets_and_duplicates.EdgeGraph.callees_of: test_build_edges_handles_fallback_targets_and_duplicates().EdgeGraph#callees_of().
  test_build_edges_handles_edgestore_targets_and_duplicates.EdgeStoreGraph.query_callees: test_build_edges_handles_edgestore_targets_and_duplicates().EdgeStoreGraph#query_callees().
  test_small_helpers_cover_bounds_and_fallbacks.ChainFallback.call_chain: test_small_helpers_cover_bounds_and_fallbacks().ChainFallback#call_chain().
  test_small_helpers_cover_bounds_and_fallbacks.ChainBroken.call_chain: test_small_helpers_cover_bounds_and_fallbacks().ChainBroken#call_chain().
  test_examples_and_scripts_ranked_below_production.MixedCache.fts_search_ranked: test_examples_and_scripts_ranked_below_production().MixedCache#fts_search_ranked().
---
# Module: [`tests/unit/test_codegraph_context_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py)

## Classes
### `BrokenCache`
- def: [`tests/unit/test_codegraph_context_tool.py:181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L181)
- signature: `class BrokenCache:`
- members:
  - `fts_search(self, candidate: str, limit: int)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L185)
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L182)
- used by: (1 test-only callers)

### `BrokenEdgeGraph`
- def: [`tests/unit/test_codegraph_context_tool.py:660`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L660)
- signature: `class BrokenEdgeGraph:`
- members:
  - `query_callees(self, name: str, file_path: str | None = None, max_depth=1)` — [`L661`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L661)
  - `query_callers(self, name: str, file_path: str | None = None)` — [`L664`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L664)
- used by: (1 test-only callers)

### `BrokenEdgeStore`
- def: [`tests/unit/test_codegraph_context_tool.py:118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L118)
- signature: `class BrokenEdgeStore:`
- members:
  - `has_edges(self, edge_kind)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L119)
- used by: (1 test-only callers)

### `CamelCaseCache`
- def: [`tests/unit/test_codegraph_context_tool.py:469`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L469)
- signature: `class CamelCaseCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L470`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L470)
  - `search_symbols_cascade(self, query: str, limit: int)` — [`L474`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L474)
- used by: (1 test-only callers)

### `ChainBroken`
- def: [`tests/unit/test_codegraph_context_tool.py:831`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L831)
- signature: `class ChainBroken:`
- members:
  - `call_chain(self, *args, **kwargs)` — [`L832`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L832)
- used by: (1 test-only callers)

### `ChainFallback`
- def: [`tests/unit/test_codegraph_context_tool.py:825`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L825)
- signature: `class ChainFallback:`
- members:
  - `call_chain(self, name: str, file_path: str | None = None, depth: int = 4)` — [`L826`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L826)
- used by: (1 test-only callers)

### `CompoundCache`
- def: [`tests/unit/test_codegraph_context_tool.py:419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L419)
- signature: `class CompoundCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L420)
  - `search_symbols_cascade(self, query: str, limit: int)` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L433)
- used by: (1 test-only callers)

### `EdgeGraph`
- def: [`tests/unit/test_codegraph_context_tool.py:688`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L688)
- signature: `class EdgeGraph:`
- members:
  - `callees_of(self, name: str, file_path: str | None = None)` — [`L689`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L689)
- used by: (1 test-only callers)

### `EdgeStoreGraph`
- def: [`tests/unit/test_codegraph_context_tool.py:737`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L737)
- signature: `class EdgeStoreGraph:`
- members:
  - `query_callees(self, name: str, file_path: str | None = None, max_depth: int = 1)` — [`L738`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L738)
- used by: (1 test-only callers)

### `ExactCache`
- def: [`tests/unit/test_codegraph_context_tool.py:514`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L514)
- signature: `class ExactCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L515`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L515)
  - `search_symbols_cascade(self, query: str, limit: int)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L525)
- used by: (1 test-only callers)

### `FakeCache`
- def: [`tests/unit/test_codegraph_context_tool.py:122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L122)
- signature: `class FakeCache:`
- used by: (1 test-only callers)

### `FakeCachedCallGraph`
- def: [`tests/unit/test_codegraph_context_tool.py:125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L125)
- signature: `class FakeCachedCallGraph:`
- members:
  - `build(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L132)
  - `built` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L130)
  - `cache` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L128)
  - `fallback` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L129)
  - `project_root` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L127)
- protocol/private: `__init__`[`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L126)
- used by: (1 test-only callers)

### `FakeGraph`
- def: [`tests/unit/test_codegraph_context_tool.py:589`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L589)
- signature: `class FakeGraph:`
- members:
  - `call_chain(self, name: str, file_path: str | None = None, depth: int = 4)` — [`L600`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L600)
  - `callees_of(self, name: str, file_path: str | None = None)` — [`L590`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L590)
  - `callers_of(self, name: str, file_path: str | None = None)` — [`L597`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L597)
- used by: (1 test-only callers)

### `FallbackCache`
- def: [`tests/unit/test_codegraph_context_tool.py:154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L154)
- signature: `class FallbackCache:`
- members:
  - `fts_search(self, candidate: str, limit: int)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L158)
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L155)
- used by: (1 test-only callers)

### `ImportOnlyCache`
- def: [`tests/unit/test_codegraph_context_tool.py:554`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L554)
- signature: `class ImportOnlyCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L555`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L555)
  - `search_symbols_cascade(self, query: str, limit: int)` — [`L562`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L562)
- used by: (1 test-only callers)

### `ManyHitsCache`
- def: [`tests/unit/test_codegraph_context_tool.py:201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L201)
- signature: `class ManyHitsCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L202)
- used by: (1 test-only callers)

### `MixedCache`
- def: [`tests/unit/test_codegraph_context_tool.py:1677`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1677)
- signature: `class MixedCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L1678`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1678)
- used by: (1 test-only callers)

### `RankedCache`
- def: [`tests/unit/test_codegraph_context_tool.py:230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L230)
- signature: `class RankedCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L231)
- used by: (1 test-only callers)

### `TestIntentCache`
- def: [`tests/unit/test_codegraph_context_tool.py:359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L359)
- signature: `class TestIntentCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L360)
- used by: (1 test-only callers)

### `TestVsImplCache`
- def: [`tests/unit/test_codegraph_context_tool.py:304`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L304)
- signature: `class TestVsImplCache:`
- members:
  - `fts_search_ranked(self, candidate: str, limit: int)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L305)
- used by: (1 test-only callers)

## Functions
- `always_fails(*args)` — [`L811`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L811)
- `fail_if_lazy_parse_builds(self)` — [`L1083`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1083)
- `falls_back_to_one_arg(*args)` — [`L814`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L814)
- `indexed_project(tmp_path: Path)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L13)
- `test_build_code_blocks_hints_when_end_unknown(tmp_path: Path)` — [`L951`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L951) — A call-graph node with no end_line still gets an 'end unknown' hint.
- `test_build_code_blocks_keeps_short_bodies_untruncated(tmp_path: Path)` — [`L990`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L990)
- `test_build_code_blocks_skips_empty_snippets(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L884`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L884)
- `test_build_code_blocks_truncates_long_bodies(tmp_path: Path)` — [`L910`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L910) — A long function body is capped to _MAX_BLOCK_LINES with a marker.
- `test_build_edges_handles_edgestore_targets_and_duplicates()` — [`L731`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L731)
- `test_build_edges_handles_fallback_targets_and_duplicates()` — [`L682`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L682)
- `test_build_related_symbols_groups_by_file()` — [`L1346`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1346) — Unit test for _build_related_symbols pure function.
- `test_call_graph_falls_back_when_edgestore_probe_fails(monkeypatch: pytest.MonkeyPatch)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L110)
- `test_capitalized_stop_word_kept_unquoted()` — [`L1815`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1815) — Capitalised Server is symbol-shaped even unquoted.
- `test_codegraph_context_registered()` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L43)
- `test_compound_candidates_builds_camelcase_word_pairs()` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L390)
- `test_context_caps_inline_edges(indexed_project: Path)` — [`L1020`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1020) — execute() with include_graph=true caps echoed edges and records totals.
- `test_context_ignores_edgestore_when_only_non_call_edges(tmp_path: Path)` — [`L1100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1100)
- `test_context_include_graph_string_false_stays_lean(indexed_project: Path)` — [`L1243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1243) — Codex P2 #320: include_graph='false' / '0' (JS-style string) must stay
- `test_context_include_graph_true_returns_full_nodes_edges(indexed_project: Path)` — [`L1214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1214) — include_graph=true must return the full nodes + edges (back-compat).
- `test_context_lean_default_omits_nodes_edges(indexed_project: Path)` — [`L1151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1151) — Default call (no include_graph) must omit nodes/edges, include related_symbols.
- `test_context_lean_stats_advertise_graph_totals(indexed_project: Path)` — [`L1278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1278) — Lean response stats must expose nodes_total and edges_total.
- `test_context_not_found_is_a_successful_stop_signal(indexed_project: Path)` — [`L1127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1127)
- `test_context_related_symbols_grouped_by_file(indexed_project: Path)` — [`L1313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1313) — related_symbols must be a list of {file, symbols:[name:line]} dicts.
- `test_context_returns_entry_points_graph_and_source(indexed_project: Path)` — [`L1045`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1045) — include_graph=true returns entry points, nodes, edges, and source blocks.
- `test_context_uses_edgestore_without_lazy_callgraph_parse(indexed_project: Path, monkeypatch: pytest.MonkeyPatch)` — [`L1074`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1074)
- `test_edge_store_accessor_degrades_without_cache_connection()` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L99)
- `test_english_connectives_filtered_from_candidates()` — [`L1478`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1478) — RFC-0009 C (dogfood-discovered): natural-language connectives like 'like',
- `test_entry_point_body_inlines_full_under_budget(tmp_path: Path)` — [`L1391`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1391) — RFC-0009 A: an entry-point symbol whose body fits the entry budget inlines
- `test_entry_point_ranked_before_high_degree_noise(tmp_path: Path)` — [`L1422`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1422) — RFC-0009 B: a task's named entry point gets a code block BEFORE a
- `test_entry_rank_v2_sinks_test_file_below_impl()` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L293) — A test-file hit must rank BELOW an implementation hit of equal relevance.
- `test_examples_and_scripts_ranked_below_production()` — [`L1666`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1666) — Issue #441 sub-2: entry points from examples/, scripts/, corpus/ must
- `test_expand_nodes_handles_edgestore_query_errors()` — [`L654`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L654)
- `test_expand_nodes_handles_graph_limits_and_trace_chain()` — [`L583`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L583)
- `test_extract_symbol_candidates_handles_identifiers()` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L59)
- `test_file_path_does_not_anchor_filter()` — [`L1581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1581) — RFC-0009 C / Codex P2 #333 (6th round): an ordinary file path mentioned in
- `test_generic_nouns_and_stop_words_not_candidates()` — [`L1638`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1638) — Issue #441 sub-1: common stop-words and generic code-nouns ('server',
- `test_generic_verb_kept_when_sole_signal()` — [`L1500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1500) — RFC-0009 C is conservative: when a generic verb is the ONLY signal (no
- `test_generic_verbs_dropped_when_specific_candidate_present()` — [`L1460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1460) — RFC-0009 C: a bare generic verb ('dispatch') is dropped from candidates
- `test_is_non_prod_file_branches()` — [`L1871`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1871)
- `test_is_test_file_detects_cross_language_test_paths()` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L269)
- `test_lowercase_qualified_anchor_still_drops_bare_verb()` — [`L1565`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1565) — RFC-0009 C / Codex P2 #333 (5th round): when the only anchor is an
- `test_name_match_score_counts_distinct_task_words()` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L257)
- `test_next_step_honest_when_only_non_prod_matches(tmp_path: Path)` — [`L1720`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1720) — Issue #441 sub-3: next_step must not tell the agent to 'Answer from
- `test_next_step_lean_entry_points_without_code()` — [`L1894`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1894)
- `test_next_step_lean_non_prod_only_warns()` — [`L1883`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1883)
- `test_next_step_lean_production_anchor()` — [`L1903`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1903)
- `test_next_step_references_top_symbol_when_production_match_found(indexed_project: Path)` — [`L1765`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1765) — Issue #441 sub-3: when production matches are found, next_step should
- `test_non_dot_qualified_generic_methods_are_kept()` — [`L1540`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1540) — RFC-0009 C / Codex P2 #333 (3rd round): C++/Rust/PHP-style qualifiers
- `test_plain_lowercase_stop_word_still_filtered()` — [`L1826`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1826)
- `test_qualified_generic_method_is_kept()` — [`L1525`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1525) — RFC-0009 C / Codex P2 #333 (re-review): a generic verb that is the METHOD
- `test_quoted_generic_verb_is_kept_as_explicit_symbol()` — [`L1512`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1512) — RFC-0009 C / Codex P2 #333: a generic verb the user QUOTED (`` `dispatch` ``)
- `test_quoted_stop_word_token_kept_as_candidate()` — [`L1805`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1805) — `Request`/`Response` in backticks are explicit symbol refs.
- `test_resolve_entry_points_degrades_and_dedupes()` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L149)
- `test_resolve_entry_points_falls_back_when_fts_only_returns_imports()` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L541) — Cascade must run when FTS rows are non-empty but all UNUSABLE.
- `test_resolve_entry_points_handles_cache_and_search_errors()` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L176)
- `test_resolve_entry_points_keeps_tests_when_task_wants_tests()` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L347) — When the task asks about tests, test symbols must NOT be demoted.
- `test_resolve_entry_points_ranks_multiword_name_match_first()` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L216) — A symbol whose name matches MORE task words must rank first.
- `test_resolve_entry_points_single_word_falls_back_to_substring_cascade()` — [`L455`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L455) — A plain concept word with NO FTS hits must fall back to the cascade.
- `test_resolve_entry_points_skips_cascade_when_fts_has_hits()` — [`L501`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L501) — The substring cascade is a FALLBACK — it must not run when FTS hits.
- `test_resolve_entry_points_stops_at_limit()` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L196)
- `test_resolve_entry_points_uses_compound_recall_for_multiword()` — [`L407`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L407) — Compound recall surfaces multi-word methods FTS misses on plain words.
- `test_schema_requires_task()` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L74)
- `test_small_helpers_cover_bounds_and_fallbacks(tmp_path: Path)` — [`L780`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L780)
- `test_snake_or_camel_path_components_do_not_anchor_filter()` — [`L1596`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1596) — RFC-0009 C / Codex P2 #333 (7th round): a file path whose components are
- `test_task_wants_tests_detects_test_intent()` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L332)
- `test_tool_accessors_require_project_root()` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L84)
- `test_wants_tests_skips_non_prod_demotion()` — [`L1836`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1836) — Codex P2: test-intent queries must not demote tests/ via non_prod_tier.
- `test_windows_path_components_do_not_anchor_filter()` — [`L1617`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_context_tool.py#L1617) — RFC-0009 C / Codex P2 #333 (8th round): Windows-style paths (backslash

