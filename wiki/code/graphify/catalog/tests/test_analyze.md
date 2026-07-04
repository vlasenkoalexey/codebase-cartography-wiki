---
title: 'Module: tests/test_analyze.py'
type: catalog
provenance: extracted
module: tests/test_analyze.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_analyze`/
symbols:
  make_graph: make_graph().
  _make_cycle_graph_directed: _make_cycle_graph_directed().
  _make_file_node: _make_file_node().
  _make_simple_graph: _make_simple_graph().
  test_surprising_connections_cross_source_multi_file: test_surprising_connections_cross_source_multi_file().
  test_surprising_connections_excludes_concept_nodes: test_surprising_connections_excludes_concept_nodes().
  test_surprising_connections_have_why_field: test_surprising_connections_have_why_field().
  test_surprising_connections_have_required_keys: test_surprising_connections_have_required_keys().
  test_god_nodes_returns_list: test_god_nodes_returns_list().
  test_god_nodes_sorted_by_degree: test_god_nodes_sorted_by_degree().
  test_god_nodes_have_required_keys: test_god_nodes_have_required_keys().
  test_surprising_connections_single_file_uses_community_bridges: test_surprising_connections_single_file_uses_community_bridges().
  test_cross_language_inferred_calls_suppressed: test_cross_language_inferred_calls_suppressed().
  test_cross_language_inferred_uses_suppressed: test_cross_language_inferred_uses_suppressed().
  test_cross_language_semantically_similar_not_suppressed: test_cross_language_semantically_similar_not_suppressed().
  test_cross_language_extracted_calls_not_suppressed: test_cross_language_extracted_calls_not_suppressed().
  test_graph_diff_new_nodes: test_graph_diff_new_nodes().
  test_graph_diff_removed_nodes: test_graph_diff_removed_nodes().
  test_graph_diff_new_edges: test_graph_diff_new_edges().
  test_graph_diff_empty_diff: test_graph_diff_empty_diff().
  test_code_doc_inferred_calls_suppressed: test_code_doc_inferred_calls_suppressed().
  test_code_doc_inferred_uses_suppressed: test_code_doc_inferred_uses_suppressed().
  test_code_doc_extracted_calls_not_suppressed: test_code_doc_extracted_calls_not_suppressed().
  test_code_doc_inferred_semantically_similar_not_suppressed: test_code_doc_inferred_semantically_similar_not_suppressed().
  test_code_unknown_extension_inferred_calls_suppressed: test_code_unknown_extension_inferred_calls_suppressed().
  test_find_import_cycles_returns_structured_records: test_find_import_cycles_returns_structured_records().
  test_find_import_cycles_detects_2_and_3_cycles: test_find_import_cycles_detects_2_and_3_cycles().
  test_find_import_cycles_includes_self_loop_cycle: test_find_import_cycles_includes_self_loop_cycle().
  test_find_import_cycles_respects_max_cycle_length: test_find_import_cycles_respects_max_cycle_length().
  test_find_import_cycles_skips_nodes_without_source_file: test_find_import_cycles_skips_nodes_without_source_file().
  test_find_import_cycles_handles_undirected_graph_input: test_find_import_cycles_handles_undirected_graph_input().
  test_find_import_cycles_ignores_non_import_relations: test_find_import_cycles_ignores_non_import_relations().
  test_find_import_cycles_no_cycles: test_find_import_cycles_no_cycles().
  _make_cross_lang_graph: _make_cross_lang_graph().
  _make_code_doc_graph: _make_code_doc_graph().
  test_surprising_connections_ambiguous_scores_higher_than_extracted: test_surprising_connections_ambiguous_scores_higher_than_extracted().
  test_surprise_score_accepts_precomputed_degrees: test_surprise_score_accepts_precomputed_degrees().
  test_surprising_connections_cross_type_scores_higher: test_surprising_connections_cross_type_scores_higher().
  test_same_language_inferred_calls_not_suppressed: test_same_language_inferred_calls_not_suppressed().
  test_file_category: test_file_category().
  test_is_concept_node_empty_source: test_is_concept_node_empty_source().
  test_is_concept_node_real_file: test_is_concept_node_real_file().
  test_code_paper_inferred_calls_not_suppressed: test_code_paper_inferred_calls_not_suppressed().
  test_is_json_key_node_noise_label: test_is_json_key_node_noise_label().
  test_is_json_key_node_non_json_file: test_is_json_key_node_non_json_file().
  test_god_nodes_excludes_npm_dep_block_keys: test_god_nodes_excludes_npm_dep_block_keys().
  test_is_json_key_node_real_label: test_is_json_key_node_real_label().
  test_god_nodes_excludes_json_noise: test_god_nodes_excludes_json_noise().
  test_god_nodes_filter_is_case_insensitive: test_god_nodes_filter_is_case_insensitive().
  test_find_import_cycles_empty_graph: test_find_import_cycles_empty_graph().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_analyze.py`](../../../../../raw/code/graphify/tests/test_analyze.py)

## Functions
- `_make_code_doc_graph()` — [`L352`](../../../../../raw/code/graphify/tests/test_analyze.py#L352)
- `_make_cross_lang_graph()` — [`L149`](../../../../../raw/code/graphify/tests/test_analyze.py#L149) — Helper: Python node in backend/, TypeScript node in frontend/, different communities.
- `_make_cycle_graph_directed()` — [`L615`](../../../../../raw/code/graphify/tests/test_analyze.py#L615)
- `_make_file_node(path: str)` — [`L609`](../../../../../raw/code/graphify/tests/test_analyze.py#L609) — Create a graph node resembling real graphify schema.
- `_make_simple_graph(nodes, edges)` — [`L290`](../../../../../raw/code/graphify/tests/test_analyze.py#L290) — Helper: build a small nx.Graph from node/edge specs.
- `make_graph()` — [`L14`](../../../../../raw/code/graphify/tests/test_analyze.py#L14)
- `test_code_doc_extracted_calls_not_suppressed()` — [`L395`](../../../../../raw/code/graphify/tests/test_analyze.py#L395) — EXTRACTED code↔doc edges are real facts — must not be penalised.
- `test_code_doc_inferred_calls_suppressed()` — [`L361`](../../../../../raw/code/graphify/tests/test_analyze.py#L361) — Code→doc INFERRED calls edge should score lower than same-language EXTRACTED. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_code_doc_inferred_semantically_similar_not_suppressed()` — [`L407`](../../../../../raw/code/graphify/tests/test_analyze.py#L407) — `semantically_similar_to` across code↔doc is explicit LLM insight — must not be suppressed.
- `test_code_doc_inferred_uses_suppressed()` — [`L378`](../../../../../raw/code/graphify/tests/test_analyze.py#L378) — Code→doc INFERRED uses edge should score lower than same-language EXTRACTED.
- `test_code_paper_inferred_calls_not_suppressed()` — [`L447`](../../../../../raw/code/graphify/tests/test_analyze.py#L447) — Code↔paper INFERRED calls should still surface — it is a meaningful link. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_code_unknown_extension_inferred_calls_suppressed()` — [`L424`](../../../../../raw/code/graphify/tests/test_analyze.py#L424) — _file_category falls back to 'doc' for unknown extensions, so INFERRED — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_cross_language_extracted_calls_not_suppressed()` — [`L229`](../../../../../raw/code/graphify/tests/test_analyze.py#L229) — EXTRACTED cross-language edges are real structural facts — must not be penalised. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_cross_language_inferred_calls_suppressed()` — [`L159`](../../../../../raw/code/graphify/tests/test_analyze.py#L159) — Cross-language INFERRED calls edge should score lower than same-language EXTRACTED.
- `test_cross_language_inferred_uses_suppressed()` — [`L176`](../../../../../raw/code/graphify/tests/test_analyze.py#L176) — Cross-language INFERRED uses edge (the exact rsl-siege-manager false positive) should be suppressed. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_cross_language_semantically_similar_not_suppressed()` — [`L193`](../../../../../raw/code/graphify/tests/test_analyze.py#L193) — `semantically_similar_to` across languages is a genuine insight — must not be suppressed. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_file_category()` — [`L250`](../../../../../raw/code/graphify/tests/test_analyze.py#L250)
- `test_find_import_cycles_detects_2_and_3_cycles()` — [`L664`](../../../../../raw/code/graphify/tests/test_analyze.py#L664)
- `test_find_import_cycles_empty_graph()` — [`L712`](../../../../../raw/code/graphify/tests/test_analyze.py#L712)
- `test_find_import_cycles_handles_undirected_graph_input()` — [`L691`](../../../../../raw/code/graphify/tests/test_analyze.py#L691)
- `test_find_import_cycles_ignores_non_import_relations()` — [`L700`](../../../../../raw/code/graphify/tests/test_analyze.py#L700)
- `test_find_import_cycles_includes_self_loop_cycle()` — [`L672`](../../../../../raw/code/graphify/tests/test_analyze.py#L672)
- `test_find_import_cycles_no_cycles()` — [`L716`](../../../../../raw/code/graphify/tests/test_analyze.py#L716)
- `test_find_import_cycles_respects_max_cycle_length()` — [`L678`](../../../../../raw/code/graphify/tests/test_analyze.py#L678)
- `test_find_import_cycles_returns_structured_records()` — [`L653`](../../../../../raw/code/graphify/tests/test_analyze.py#L653)
- `test_find_import_cycles_skips_nodes_without_source_file()` — [`L684`](../../../../../raw/code/graphify/tests/test_analyze.py#L684)
- `test_god_nodes_excludes_json_noise()` — [`L568`](../../../../../raw/code/graphify/tests/test_analyze.py#L568) — god_nodes must not return generic JSON key nodes like 'name' or 'id'. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_god_nodes_excludes_npm_dep_block_keys(dep_key: str)` — [`L492`](../../../../../raw/code/graphify/tests/test_analyze.py#L492) — npm package.json dep-block keys must be filtered from god_nodes output.
- `test_god_nodes_filter_is_case_insensitive()` — [`L586`](../../../../../raw/code/graphify/tests/test_analyze.py#L586) — JSON-key filter must match regardless of label casing.
- `test_god_nodes_have_required_keys()` — [`L32`](../../../../../raw/code/graphify/tests/test_analyze.py#L32)
- `test_god_nodes_returns_list()` — [`L18`](../../../../../raw/code/graphify/tests/test_analyze.py#L18)
- `test_god_nodes_sorted_by_degree()` — [`L25`](../../../../../raw/code/graphify/tests/test_analyze.py#L25) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_graph_diff_empty_diff()` — [`L337`](../../../../../raw/code/graphify/tests/test_analyze.py#L337)
- `test_graph_diff_new_edges()` — [`L321`](../../../../../raw/code/graphify/tests/test_analyze.py#L321)
- `test_graph_diff_new_nodes()` — [`L300`](../../../../../raw/code/graphify/tests/test_analyze.py#L300)
- `test_graph_diff_removed_nodes()` — [`L311`](../../../../../raw/code/graphify/tests/test_analyze.py#L311)
- `test_is_concept_node_empty_source()` — [`L266`](../../../../../raw/code/graphify/tests/test_analyze.py#L266)
- `test_is_concept_node_real_file()` — [`L272`](../../../../../raw/code/graphify/tests/test_analyze.py#L272)
- `test_is_json_key_node_noise_label()` — [`L471`](../../../../../raw/code/graphify/tests/test_analyze.py#L471)
- `test_is_json_key_node_non_json_file()` — [`L477`](../../../../../raw/code/graphify/tests/test_analyze.py#L477)
- `test_is_json_key_node_real_label()` — [`L562`](../../../../../raw/code/graphify/tests/test_analyze.py#L562)
- `test_same_language_inferred_calls_not_suppressed()` — [`L210`](../../../../../raw/code/graphify/tests/test_analyze.py#L210) — INFERRED calls within the same language family must not be affected.
- `test_surprise_score_accepts_precomputed_degrees()` — [`L109`](../../../../../raw/code/graphify/tests/test_analyze.py#L109)
- `test_surprising_connections_ambiguous_scores_higher_than_extracted()` — [`L90`](../../../../../raw/code/graphify/tests/test_analyze.py#L90) — AMBIGUOUS edge should score higher than an otherwise identical EXTRACTED edge. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `test_surprising_connections_cross_source_multi_file()` — [`L40`](../../../../../raw/code/graphify/tests/test_analyze.py#L40) — Multi-file graph: should find cross-file edges between real entities.
- `test_surprising_connections_cross_type_scores_higher()` — [`L130`](../../../../../raw/code/graphify/tests/test_analyze.py#L130) — Code↔paper edge should score higher than code↔code edge.
- `test_surprising_connections_excludes_concept_nodes()` — [`L50`](../../../../../raw/code/graphify/tests/test_analyze.py#L50) — Concept nodes (empty source_file) must not appear in surprises.
- `test_surprising_connections_have_required_keys()` — [`L278`](../../../../../raw/code/graphify/tests/test_analyze.py#L278)
- `test_surprising_connections_have_why_field()` — [`L241`](../../../../../raw/code/graphify/tests/test_analyze.py#L241)
- `test_surprising_connections_single_file_uses_community_bridges()` — [`L63`](../../../../../raw/code/graphify/tests/test_analyze.py#L63) — Single-file graph: should return cross-community edges, not empty list. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)

## Module values
- `FIXTURES` — [`L11`](../../../../../raw/code/graphify/tests/test_analyze.py#L11)

