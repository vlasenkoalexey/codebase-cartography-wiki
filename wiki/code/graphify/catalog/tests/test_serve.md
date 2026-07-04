---
title: 'Module: tests/test_serve.py'
type: catalog
provenance: extracted
module: tests/test_serve.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_serve`/
symbols:
  _make_graph: _make_graph().
  _make_big_graph: _make_big_graph().
  test_score_nodes_prefilter_is_identical_to_full_scan: test_score_nodes_prefilter_is_identical_to_full_scan().
  test_find_node_prefilter_is_identical_to_full_scan: test_find_node_prefilter_is_identical_to_full_scan().
  test_trigram_index_cached_and_rebuilt_per_graph: test_trigram_index_cached_and_rebuilt_per_graph().
  test_filter_graph_by_context_limits_traversal: test_filter_graph_by_context_limits_traversal().
  test_subgraph_to_text_annotates_node_with_learning_status: test_subgraph_to_text_annotates_node_with_learning_status().
  test_subgraph_to_text_marks_stale_status: test_subgraph_to_text_marks_stale_status().
  test_subgraph_to_text_learning_suffix_counts_against_budget: test_subgraph_to_text_learning_suffix_counts_against_budget().
  test_idf_cached_on_graph: test_idf_cached_on_graph().
  test_idf_new_graph_starts_fresh: test_idf_new_graph_starts_fresh().
  test_communities_from_graph_basic: test_communities_from_graph_basic().
  test_communities_from_graph_isolated: test_communities_from_graph_isolated().
  test_score_nodes_exact_label_match: test_score_nodes_exact_label_match().
  test_score_nodes_no_match: test_score_nodes_no_match().
  test_score_nodes_source_file_partial: test_score_nodes_source_file_partial().
  test_score_nodes_ignores_trailing_punctuation: test_score_nodes_ignores_trailing_punctuation().
  test_score_nodes_multiword_exact_label_outranks_superset: test_score_nodes_multiword_exact_label_outranks_superset().
  test_find_node_ignores_trailing_punctuation: test_find_node_ignores_trailing_punctuation().
  test_node_search_text_includes_all_matched_fields: test_node_search_text_includes_all_matched_fields().
  test_trigram_candidates_fast_path_fires_for_rare_term: test_trigram_candidates_fast_path_fires_for_rare_term().
  test_trigram_candidates_falls_back_on_common_term: test_trigram_candidates_falls_back_on_common_term().
  test_trigram_candidates_falls_back_on_short_token: test_trigram_candidates_falls_back_on_short_token().
  test_find_node_label_tokens_branch_covered_by_index: test_find_node_label_tokens_branch_covered_by_index().
  test_find_node_source_file_path_prefers_file_level_node: test_find_node_source_file_path_prefers_file_level_node().
  test_query_terms_filters_only_short_english_terms: test_query_terms_filters_only_short_english_terms().
  test_bfs_depth_1: test_bfs_depth_1().
  test_bfs_depth_2: test_bfs_depth_2().
  test_bfs_disconnected: test_bfs_disconnected().
  test_bfs_returns_edges: test_bfs_returns_edges().
  test_dfs_depth_1: test_dfs_depth_1().
  test_dfs_full_chain: test_dfs_full_chain().
  test_subgraph_to_text_contains_labels: test_subgraph_to_text_contains_labels().
  test_subgraph_to_text_truncates: test_subgraph_to_text_truncates().
  test_subgraph_to_text_edge_included: test_subgraph_to_text_edge_included().
  test_subgraph_to_text_includes_edge_context: test_subgraph_to_text_includes_edge_context().
  test_subgraph_to_text_no_overlay_is_unchanged: test_subgraph_to_text_no_overlay_is_unchanged().
  test_query_graph_text_explicit_context_filter_changes_traversal: test_query_graph_text_explicit_context_filter_changes_traversal().
  test_query_graph_text_heuristic_context_filter_changes_traversal: test_query_graph_text_heuristic_context_filter_changes_traversal().
  test_load_graph_roundtrip: test_load_graph_roundtrip().
  test_load_graph_rejects_oversized_file: test_load_graph_rejects_oversized_file().
  test_load_graph_accepts_under_cap: test_load_graph_accepts_under_cap().
  test_maybe_reload_detects_graph_change: test_maybe_reload_detects_graph_change().
  test_idf_downweights_common_terms: test_idf_downweights_common_terms().
  test_idf_rare_term_gets_high_weight: test_idf_rare_term_gets_high_weight().
  test_pick_seeds_diversity_recovers_starved_term: test_pick_seeds_diversity_recovers_starved_term().
  test_subgraph_to_text_truncation_hint_is_actionable: test_subgraph_to_text_truncation_hint_is_actionable().
  test_query_seeds_from_identifier_not_noise: test_query_seeds_from_identifier_not_noise().
  test_query_terms_chinese_segments_with_cached_jieba: test_query_terms_chinese_segments_with_cached_jieba().
  test_query_terms_non_chinese_scripts_are_not_segmented: test_query_terms_non_chinese_scripts_are_not_segmented().
  _write_graph: _write_graph().
  test_score_nodes_multiword_exact_label_outranks_superset._add: test_score_nodes_multiword_exact_label_outranks_superset()._add().
  test_communities_from_graph_no_community_attr: test_communities_from_graph_no_community_attr().
  test_find_node_matches_full_punctuated_unicode_label: test_find_node_matches_full_punctuated_unicode_label().
  test_trigrams_basic: test_trigrams_basic().
  test_query_terms_strips_search_punctuation: test_query_terms_strips_search_punctuation().
  test_query_terms_drops_question_stopwords: test_query_terms_drops_question_stopwords().
  test_query_terms_all_stopwords_falls_back_to_unfiltered: test_query_terms_all_stopwords_falls_back_to_unfiltered().
  test_query_graph_text_keeps_short_non_english_terms: test_query_graph_text_keeps_short_non_english_terms().
  test_infer_context_filters_for_calls_question: test_infer_context_filters_for_calls_question().
  test_resolve_context_filters_explicit_overrides_heuristic: test_resolve_context_filters_explicit_overrides_heuristic().
  test_load_graph_missing_file: test_load_graph_missing_file().
  test_load_graph_cache_key_changes_with_content: test_load_graph_cache_key_changes_with_content().
  test_idf_common_term_gets_low_weight: test_idf_common_term_gets_low_weight().
  test_pick_seeds_dominant_identifier_gives_one_seed: test_pick_seeds_dominant_identifier_gives_one_seed().
  test_pick_seeds_close_scores_keeps_multiple: test_pick_seeds_close_scores_keeps_multiple().
  test_pick_seeds_empty: test_pick_seeds_empty().
  test_pick_seeds_single: test_pick_seeds_single().
  test_pick_seeds_respects_max_k: test_pick_seeds_respects_max_k().
  test_pick_seeds_without_diversity_args_is_unchanged: test_pick_seeds_without_diversity_args_is_unchanged().
  test_query_graph_text_parameter_type_context_filter_changes_traversal: test_query_graph_text_parameter_type_context_filter_changes_traversal().
  test_query_graph_text_context_filter_aliases_resolve: test_query_graph_text_context_filter_aliases_resolve().
  test_query_terms_chinese_mixed: test_query_terms_chinese_mixed().
  test_query_terms_chinese_no_jieba_fallback: test_query_terms_chinese_no_jieba_fallback().
  test_score_nodes_chinese_substring_match: test_score_nodes_chinese_substring_match().
  test_query_text_chinese_finds_routing_nodes: test_query_text_chinese_finds_routing_nodes().
  test_community_header_shows_real_name: test_community_header_shows_real_name().
  test_community_header_skips_placeholder_name: test_community_header_skips_placeholder_name().
  test_community_header_falls_back_when_no_name: test_community_header_falls_back_when_no_name().
  test_community_header_sanitizes_name: test_community_header_sanitizes_name().
  _force_full_scan: _force_full_scan().
  _make_noisy_graph: _make_noisy_graph().
  test_query_terms_filters_only_short_english_terms.FakeJieba: test_query_terms_filters_only_short_english_terms().FakeJieba#
  test_query_terms_chinese_segments_with_cached_jieba.FakeJieba: test_query_terms_chinese_segments_with_cached_jieba().FakeJieba#
  test_query_terms_filters_only_short_english_terms.FakeJieba.cut: test_query_terms_filters_only_short_english_terms().FakeJieba#cut().
  test_query_terms_chinese_segments_with_cached_jieba.FakeJieba.cut: test_query_terms_chinese_segments_with_cached_jieba().FakeJieba#cut().
---
# Module: [`tests/test_serve.py`](../../../../../raw/code/graphify/tests/test_serve.py)

## Classes
### `FakeJieba`
- def: [`tests/test_serve.py:748`](../../../../../raw/code/graphify/tests/test_serve.py#L748)
- signature: `class FakeJieba:`
- members:
  - `cut(self, text)` — [`L285`](../../../../../raw/code/graphify/tests/test_serve.py#L285)
  - `cut(self, text)` — [`L749`](../../../../../raw/code/graphify/tests/test_serve.py#L749)
- used by: (1 test-only callers)

## Functions
- `_add(nid, label, src)` — [`L110`](../../../../../raw/code/graphify/tests/test_serve.py#L110)
- `_force_full_scan(monkeypatch)` — [`L141`](../../../../../raw/code/graphify/tests/test_serve.py#L141) — Disable the prefilter so a call exercises the original full-node scan.
- `_make_big_graph(n: int = 150)` — [`L146`](../../../../../raw/code/graphify/tests/test_serve.py#L146) — A graph large enough that the selectivity guard lets the fast-path fire for
- `_make_graph()` — [`L30`](../../../../../raw/code/graphify/tests/test_serve.py#L30)
- `_make_noisy_graph()` — [`L559`](../../../../../raw/code/graphify/tests/test_serve.py#L559) — 20 error-handler nodes + 1 rare identifier: FooBarService.
- `_write_graph(path, nodes: list[str])` — [`L505`](../../../../../raw/code/graphify/tests/test_serve.py#L505) — Write a minimal graph.json with the given node IDs.
- `test_bfs_depth_1()` — [`L320`](../../../../../raw/code/graphify/tests/test_serve.py#L320)
- `test_bfs_depth_2()` — [`L327`](../../../../../raw/code/graphify/tests/test_serve.py#L327)
- `test_bfs_disconnected()` — [`L332`](../../../../../raw/code/graphify/tests/test_serve.py#L332)
- `test_bfs_returns_edges()` — [`L337`](../../../../../raw/code/graphify/tests/test_serve.py#L337)
- `test_communities_from_graph_basic()` — [`L45`](../../../../../raw/code/graphify/tests/test_serve.py#L45)
- `test_communities_from_graph_isolated()` — [`L60`](../../../../../raw/code/graphify/tests/test_serve.py#L60)
- `test_communities_from_graph_no_community_attr()` — [`L54`](../../../../../raw/code/graphify/tests/test_serve.py#L54)
- `test_community_header_falls_back_when_no_name()` — [`L822`](../../../../../raw/code/graphify/tests/test_serve.py#L822)
- `test_community_header_sanitizes_name()` — [`L827`](../../../../../raw/code/graphify/tests/test_serve.py#L827)
- `test_community_header_shows_real_name()` — [`L812`](../../../../../raw/code/graphify/tests/test_serve.py#L812)
- `test_community_header_skips_placeholder_name()` — [`L816`](../../../../../raw/code/graphify/tests/test_serve.py#L816)
- `test_dfs_depth_1()` — [`L355`](../../../../../raw/code/graphify/tests/test_serve.py#L355)
- `test_dfs_full_chain()` — [`L362`](../../../../../raw/code/graphify/tests/test_serve.py#L362)
- `test_filter_graph_by_context_limits_traversal()` — [`L344`](../../../../../raw/code/graphify/tests/test_serve.py#L344)
- `test_find_node_ignores_trailing_punctuation()` — [`L126`](../../../../../raw/code/graphify/tests/test_serve.py#L126)
- `test_find_node_label_tokens_branch_covered_by_index()` — [`L223`](../../../../../raw/code/graphify/tests/test_serve.py#L223)
- `test_find_node_matches_full_punctuated_unicode_label()` — [`L131`](../../../../../raw/code/graphify/tests/test_serve.py#L131)
- `test_find_node_prefilter_is_identical_to_full_scan(monkeypatch)` — [`L211`](../../../../../raw/code/graphify/tests/test_serve.py#L211)
- `test_find_node_source_file_path_prefers_file_level_node()` — [`L231`](../../../../../raw/code/graphify/tests/test_serve.py#L231)
- `test_idf_cached_on_graph()` — [`L583`](../../../../../raw/code/graphify/tests/test_serve.py#L583) — IDF results are stored in G.graph so repeated queries don't recompute. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `test_idf_common_term_gets_low_weight()` — [`L608`](../../../../../raw/code/graphify/tests/test_serve.py#L608) — A term matching most nodes should get IDF < 1.
- `test_idf_downweights_common_terms()` — [`L572`](../../../../../raw/code/graphify/tests/test_serve.py#L572) — 'error' matches 20 nodes, 'foobarservice' matches 1 — IDF should make
- `test_idf_new_graph_starts_fresh()` — [`L591`](../../../../../raw/code/graphify/tests/test_serve.py#L591) — Two separate graph instances must not share an IDF cache. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `test_idf_rare_term_gets_high_weight()` — [`L599`](../../../../../raw/code/graphify/tests/test_serve.py#L599) — A term matching only 1 of N nodes should get IDF > 1.
- `test_infer_context_filters_for_calls_question()` — [`L308`](../../../../../raw/code/graphify/tests/test_serve.py#L308)
- `test_load_graph_accepts_under_cap(monkeypatch, tmp_path)` — [`L491`](../../../../../raw/code/graphify/tests/test_serve.py#L491)
- `test_load_graph_cache_key_changes_with_content(tmp_path)` — [`L536`](../../../../../raw/code/graphify/tests/test_serve.py#L536) — mtime_ns + size uniquely identifies a graph version (#874).
- `test_load_graph_missing_file(tmp_path)` — [`L470`](../../../../../raw/code/graphify/tests/test_serve.py#L470)
- `test_load_graph_rejects_oversized_file(monkeypatch, tmp_path, capsys)` — [`L477`](../../../../../raw/code/graphify/tests/test_serve.py#L477)
- `test_load_graph_roundtrip(tmp_path)` — [`L461`](../../../../../raw/code/graphify/tests/test_serve.py#L461)
- `test_maybe_reload_detects_graph_change(tmp_path)` — [`L514`](../../../../../raw/code/graphify/tests/test_serve.py#L514) — serve() picks up a new graph.json written after startup (#874).
- `test_node_search_text_includes_all_matched_fields()` — [`L165`](../../../../../raw/code/graphify/tests/test_serve.py#L165)
- `test_pick_seeds_close_scores_keeps_multiple()` — [`L628`](../../../../../raw/code/graphify/tests/test_serve.py#L628) — When all scores are within 20% of the top, keep up to 3 seeds.
- `test_pick_seeds_diversity_recovers_starved_term(monkeypatch)` — [`L657`](../../../../../raw/code/graphify/tests/test_serve.py#L657) — Reproduces #1445: a vague natural-language query where one term's
- `test_pick_seeds_dominant_identifier_gives_one_seed()` — [`L621`](../../../../../raw/code/graphify/tests/test_serve.py#L621) — FooBarService at 1000 vs error nodes at 1.0 → only 1 seed chosen.
- `test_pick_seeds_empty()` — [`L635`](../../../../../raw/code/graphify/tests/test_serve.py#L635)
- `test_pick_seeds_respects_max_k()` — [`L643`](../../../../../raw/code/graphify/tests/test_serve.py#L643) — Never return more than max_k seeds even when all scores are close.
- `test_pick_seeds_single()` — [`L639`](../../../../../raw/code/graphify/tests/test_serve.py#L639)
- `test_pick_seeds_without_diversity_args_is_unchanged()` — [`L650`](../../../../../raw/code/graphify/tests/test_serve.py#L650) — G/terms are optional and default to None: existing callers see identical
- `test_query_graph_text_context_filter_aliases_resolve()` — [`L725`](../../../../../raw/code/graphify/tests/test_serve.py#L725)
- `test_query_graph_text_explicit_context_filter_changes_traversal()` — [`L443`](../../../../../raw/code/graphify/tests/test_serve.py#L443)
- `test_query_graph_text_heuristic_context_filter_changes_traversal()` — [`L451`](../../../../../raw/code/graphify/tests/test_serve.py#L451)
- `test_query_graph_text_keeps_short_non_english_terms()` — [`L300`](../../../../../raw/code/graphify/tests/test_serve.py#L300)
- `test_query_graph_text_parameter_type_context_filter_changes_traversal()` — [`L707`](../../../../../raw/code/graphify/tests/test_serve.py#L707)
- `test_query_seeds_from_identifier_not_noise()` — [`L698`](../../../../../raw/code/graphify/tests/test_serve.py#L698) — 'FooBarService error handling' should expand from FooBarService,
- `test_query_terms_all_stopwords_falls_back_to_unfiltered()` — [`L276`](../../../../../raw/code/graphify/tests/test_serve.py#L276)
- `test_query_terms_chinese_mixed()` — [`L758`](../../../../../raw/code/graphify/tests/test_serve.py#L758) — Mixed Chinese and English text should be handled correctly.
- `test_query_terms_chinese_no_jieba_fallback(monkeypatch)` — [`L775`](../../../../../raw/code/graphify/tests/test_serve.py#L775) — When jieba is not installed, fallback to character bigrams.
- `test_query_terms_chinese_segments_with_cached_jieba(monkeypatch)` — [`L744`](../../../../../raw/code/graphify/tests/test_serve.py#L744) — Chinese text should use the cached jieba module and keep the original term.
- `test_query_terms_drops_question_stopwords()` — [`L269`](../../../../../raw/code/graphify/tests/test_serve.py#L269)
- `test_query_terms_filters_only_short_english_terms(monkeypatch)` — [`L281`](../../../../../raw/code/graphify/tests/test_serve.py#L281)
- `test_query_terms_non_chinese_scripts_are_not_segmented()` — [`L767`](../../../../../raw/code/graphify/tests/test_serve.py#L767) — Japanese kana and Hangul are kept as terms but not segmented as Chinese.
- `test_query_terms_strips_search_punctuation()` — [`L264`](../../../../../raw/code/graphify/tests/test_serve.py#L264)
- `test_query_text_chinese_finds_routing_nodes()` — [`L799`](../../../../../raw/code/graphify/tests/test_serve.py#L799) — Full pipeline: '页面路由' should find nodes with '路由' in label.
- `test_resolve_context_filters_explicit_overrides_heuristic()` — [`L312`](../../../../../raw/code/graphify/tests/test_serve.py#L312)
- `test_score_nodes_chinese_substring_match()` — [`L788`](../../../../../raw/code/graphify/tests/test_serve.py#L788) — Searching for '路由' should match a node with label containing '路由'.
- `test_score_nodes_exact_label_match()` — [`L69`](../../../../../raw/code/graphify/tests/test_serve.py#L69)
- `test_score_nodes_ignores_trailing_punctuation()` — [`L89`](../../../../../raw/code/graphify/tests/test_serve.py#L89)
- `test_score_nodes_multiword_exact_label_outranks_superset()` — [`L95`](../../../../../raw/code/graphify/tests/test_serve.py#L95) — A multi-word query equal to a whole label must resolve uniquely.
- `test_score_nodes_no_match()` — [`L76`](../../../../../raw/code/graphify/tests/test_serve.py#L76)
- `test_score_nodes_prefilter_is_identical_to_full_scan(monkeypatch)` — [`L198`](../../../../../raw/code/graphify/tests/test_serve.py#L198) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `test_score_nodes_source_file_partial()` — [`L81`](../../../../../raw/code/graphify/tests/test_serve.py#L81)
- `test_subgraph_to_text_annotates_node_with_learning_status()` — [`L397`](../../../../../raw/code/graphify/tests/test_serve.py#L397) — An annotated node gets a `learning=<status>` suffix inside its NODE
- `test_subgraph_to_text_contains_labels()` — [`L370`](../../../../../raw/code/graphify/tests/test_serve.py#L370)
- `test_subgraph_to_text_edge_included()` — [`L382`](../../../../../raw/code/graphify/tests/test_serve.py#L382)
- `test_subgraph_to_text_includes_edge_context()` — [`L389`](../../../../../raw/code/graphify/tests/test_serve.py#L389)
- `test_subgraph_to_text_learning_suffix_counts_against_budget()` — [`L417`](../../../../../raw/code/graphify/tests/test_serve.py#L417) — The learning= suffix is part of the NODE line BEFORE the budget cut, so it
- `test_subgraph_to_text_marks_stale_status()` — [`L410`](../../../../../raw/code/graphify/tests/test_serve.py#L410)
- `test_subgraph_to_text_no_overlay_is_unchanged()` — [`L436`](../../../../../raw/code/graphify/tests/test_serve.py#L436) — With no overlay on the graph, NODE lines carry no learning= suffix.
- `test_subgraph_to_text_truncates()` — [`L376`](../../../../../raw/code/graphify/tests/test_serve.py#L376)
- `test_subgraph_to_text_truncation_hint_is_actionable()` — [`L688`](../../../../../raw/code/graphify/tests/test_serve.py#L688) — Truncation message must tell Claude what to do, not just say truncated.
- `test_trigram_candidates_falls_back_on_common_term()` — [`L186`](../../../../../raw/code/graphify/tests/test_serve.py#L186)
- `test_trigram_candidates_falls_back_on_short_token()` — [`L193`](../../../../../raw/code/graphify/tests/test_serve.py#L193)
- `test_trigram_candidates_fast_path_fires_for_rare_term()` — [`L178`](../../../../../raw/code/graphify/tests/test_serve.py#L178)
- `test_trigram_index_cached_and_rebuilt_per_graph()` — [`L255`](../../../../../raw/code/graphify/tests/test_serve.py#L255)
- `test_trigrams_basic()` — [`L159`](../../../../../raw/code/graphify/tests/test_serve.py#L159)

