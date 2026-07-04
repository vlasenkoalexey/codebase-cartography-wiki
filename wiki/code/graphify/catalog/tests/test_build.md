---
title: 'Module: tests/test_build.py'
type: catalog
provenance: extracted
module: tests/test_build.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_build`/
symbols:
  test_build_merge_preserves_call_edge_direction: test_build_merge_preserves_call_edge_direction().
  load_extraction: load_extraction().
  test_build_from_json_preserves_first_direction_on_bidirectional_pair: test_build_from_json_preserves_first_direction_on_bidirectional_pair().
  test_build_from_json_node_count: test_build_from_json_node_count().
  test_build_from_json_edge_count: test_build_from_json_edge_count().
  test_nodes_have_label: test_nodes_have_label().
  test_edges_have_confidence: test_edges_have_confidence().
  test_ambiguous_edge_preserved: test_ambiguous_edge_preserved().
  test_edge_missing_source_file_backfilled_from_node: test_edge_missing_source_file_backfilled_from_node().
  test_edge_data_multidigraph: test_edge_data_multidigraph().
  test_edge_data_node_link_multigraph_roundtrip: test_edge_data_node_link_multigraph_roundtrip().
  test_build_merge_prune_absolute_paths_match_relative_nodes: test_build_merge_prune_absolute_paths_match_relative_nodes().
  test_build_merge_prune_windows_backslash_paths: test_build_merge_prune_windows_backslash_paths().
  test_build_merge_replaces_changed_file_stale_edges: test_build_merge_replaces_changed_file_stale_edges().
  test_build_merge_root_collapses_convention_drift: test_build_merge_root_collapses_convention_drift().
  test_dedupe_edges_collapses_exact_parallels: test_dedupe_edges_collapses_exact_parallels().
  test_dedupe_edges_is_idempotent: test_dedupe_edges_is_idempotent().
  test_dedupe_nodes_collapses_by_id_last_wins: test_dedupe_nodes_collapses_by_id_last_wins().
  test_legacy_node_source_canonicalized: test_legacy_node_source_canonicalized().
  test_legacy_edge_from_to_canonicalized: test_legacy_edge_from_to_canonicalized().
  test_source_file_backslash_normalized: test_source_file_backslash_normalized().
  test_build_merges_multiple_extractions: test_build_merges_multiple_extractions().
  test_none_file_type_defaults_to_concept: test_none_file_type_defaults_to_concept().
  test_missing_file_type_defaults_to_concept: test_missing_file_type_defaults_to_concept().
  test_real_invalid_file_type_coerced_to_concept: test_real_invalid_file_type_coerced_to_concept().
  test_file_type_synonym_mapping: test_file_type_synonym_mapping().
  test_ghost_merge_unique_located_node_still_merges: test_ghost_merge_unique_located_node_still_merges().
  test_ghost_merge_skipped_on_basename_collision: test_ghost_merge_skipped_on_basename_collision().
  test_edge_data_simple_graph: test_edge_data_simple_graph().
  test_edge_datas_simple_graph_returns_singleton_list: test_edge_datas_simple_graph_returns_singleton_list().
  test_edge_data_multigraph_with_parallel_edges: test_edge_data_multigraph_with_parallel_edges().
  test_edge_datas_multigraph_returns_all_parallel_edges: test_edge_datas_multigraph_returns_all_parallel_edges().
  test_build_from_json_relativizes_absolute_source_file: test_build_from_json_relativizes_absolute_source_file().
  test_build_relativizes_absolute_source_file: test_build_relativizes_absolute_source_file().
  test_build_from_json_relative_source_file_unchanged: test_build_from_json_relative_source_file_unchanged().
  test_build_merge_rejects_oversized_existing_graph: test_build_merge_rejects_oversized_existing_graph().
  test_build_from_json_skips_non_hashable_node_id: test_build_from_json_skips_non_hashable_node_id().
  test_build_from_json_skips_edge_with_non_hashable_endpoint: test_build_from_json_skips_edge_with_non_hashable_endpoint().
  test_graph_has_legacy_ids_detects_old_scheme: test_graph_has_legacy_ids_detects_old_scheme().
  test_semantic_rekey_relative_vs_absolute_source_file: test_semantic_rekey_relative_vs_absolute_source_file().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_build.py`](../../../../../raw/code/graphify/tests/test_build.py)

## Functions
- `load_extraction()` — [`L50`](../../../../../raw/code/graphify/tests/test_build.py#L50)
- `test_ambiguous_edge_preserved()` — [`L70`](../../../../../raw/code/graphify/tests/test_build.py#L70)
- `test_build_from_json_edge_count()` — [`L57`](../../../../../raw/code/graphify/tests/test_build.py#L57)
- `test_build_from_json_node_count()` — [`L53`](../../../../../raw/code/graphify/tests/test_build.py#L53)
- `test_build_from_json_preserves_first_direction_on_bidirectional_pair(tmp_path)` — [`L327`](../../../../../raw/code/graphify/tests/test_build.py#L327) — Regression for #1061. — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_build_from_json_relative_source_file_unchanged(tmp_path)` — [`L508`](../../../../../raw/code/graphify/tests/test_build.py#L508) — Already-relative source_file paths must not be modified.
- `test_build_from_json_relativizes_absolute_source_file(tmp_path)` — [`L470`](../../../../../raw/code/graphify/tests/test_build.py#L470) — Semantic subagents emit absolute source_file paths; build_from_json must
- `test_build_from_json_skips_edge_with_non_hashable_endpoint()` — [`L702`](../../../../../raw/code/graphify/tests/test_build.py#L702)
- `test_build_from_json_skips_non_hashable_node_id()` — [`L686`](../../../../../raw/code/graphify/tests/test_build.py#L686)
- `test_build_merge_preserves_call_edge_direction(tmp_path)` — [`L260`](../../../../../raw/code/graphify/tests/test_build.py#L260) — Regression for #760.
- `test_build_merge_prune_absolute_paths_match_relative_nodes(tmp_path)` — [`L519`](../../../../../raw/code/graphify/tests/test_build.py#L519) — #1007: manifest stores absolute paths, graph nodes store relative paths.
- `test_build_merge_prune_windows_backslash_paths(tmp_path)` — [`L550`](../../../../../raw/code/graphify/tests/test_build.py#L550) — #1007: prune_sources with Windows-style backslash absolute paths must still match.
- `test_build_merge_rejects_oversized_existing_graph(monkeypatch, tmp_path)` — [`L674`](../../../../../raw/code/graphify/tests/test_build.py#L674) — #F4: build_merge must refuse to read an existing graph.json that
- `test_build_merge_replaces_changed_file_stale_edges(tmp_path)` — [`L572`](../../../../../raw/code/graphify/tests/test_build.py#L572) — Re-extracting a CHANGED file must REPLACE its prior nodes/edges, not
- `test_build_merge_root_collapses_convention_drift(tmp_path)` — [`L624`](../../../../../raw/code/graphify/tests/test_build.py#L624) — Skill contract: the extraction subagent must emit source_file as the
- `test_build_merges_multiple_extractions()` — [`L128`](../../../../../raw/code/graphify/tests/test_build.py#L128)
- `test_build_relativizes_absolute_source_file(tmp_path)` — [`L493`](../../../../../raw/code/graphify/tests/test_build.py#L493) — build() passes root through to build_from_json (#932).
- `test_dedupe_edges_collapses_exact_parallels()` — [`L10`](../../../../../raw/code/graphify/tests/test_build.py#L10)
- `test_dedupe_edges_is_idempotent()` — [`L25`](../../../../../raw/code/graphify/tests/test_build.py#L25)
- `test_dedupe_nodes_collapses_by_id_last_wins()` — [`L36`](../../../../../raw/code/graphify/tests/test_build.py#L36)
- `test_edge_data_multidigraph()` — [`L430`](../../../../../raw/code/graphify/tests/test_build.py#L430)
- `test_edge_data_multigraph_with_parallel_edges()` — [`L409`](../../../../../raw/code/graphify/tests/test_build.py#L409)
- `test_edge_data_node_link_multigraph_roundtrip()` — [`L441`](../../../../../raw/code/graphify/tests/test_build.py#L441) — A node_link JSON with multigraph: true must load as MultiGraph and the
- `test_edge_data_simple_graph()` — [`L391`](../../../../../raw/code/graphify/tests/test_build.py#L391)
- `test_edge_datas_multigraph_returns_all_parallel_edges()` — [`L419`](../../../../../raw/code/graphify/tests/test_build.py#L419)
- `test_edge_datas_simple_graph_returns_singleton_list()` — [`L400`](../../../../../raw/code/graphify/tests/test_build.py#L400)
- `test_edge_missing_source_file_backfilled_from_node()` — [`L111`](../../../../../raw/code/graphify/tests/test_build.py#L111) — #1279: a semantic/LLM edge lacking source_file must inherit it from its
- `test_edges_have_confidence()` — [`L65`](../../../../../raw/code/graphify/tests/test_build.py#L65)
- `test_file_type_synonym_mapping()` — [`L192`](../../../../../raw/code/graphify/tests/test_build.py#L192) — Known invalid file_type values map to their canonical equivalents.
- `test_ghost_merge_skipped_on_basename_collision()` — [`L231`](../../../../../raw/code/graphify/tests/test_build.py#L231) — #1257: when two files with the same basename both define a symbol with the
- `test_ghost_merge_unique_located_node_still_merges()` — [`L210`](../../../../../raw/code/graphify/tests/test_build.py#L210) — #1145 ghost-merge: a semantic ghost collapses into the single AST node
- `test_graph_has_legacy_ids_detects_old_scheme()` — [`L725`](../../../../../raw/code/graphify/tests/test_build.py#L725) — The read-only-consumer nudge (query/serve) flags a pre-#1504 graph and
- `test_legacy_edge_from_to_canonicalized()` — [`L85`](../../../../../raw/code/graphify/tests/test_build.py#L85) — Legacy 'from'/'to' keys on edges are accepted alongside 'source'/'target'.
- `test_legacy_node_source_canonicalized()` — [`L75`](../../../../../raw/code/graphify/tests/test_build.py#L75) — Legacy 'source' key on nodes is renamed to 'source_file' before graph build.
- `test_missing_file_type_defaults_to_concept(capsys)` — [`L160`](../../../../../raw/code/graphify/tests/test_build.py#L160) — Nodes missing file_type entirely should also be canonicalized to 'concept'.
- `test_nodes_have_label()` — [`L61`](../../../../../raw/code/graphify/tests/test_build.py#L61)
- `test_none_file_type_defaults_to_concept(capsys)` — [`L140`](../../../../../raw/code/graphify/tests/test_build.py#L140) — Legacy nodes with file_type=None (e.g. preserved from older graph.json
- `test_real_invalid_file_type_coerced_to_concept()` — [`L177`](../../../../../raw/code/graphify/tests/test_build.py#L177) — Unknown file_type values are coerced through the synonym mapper, falling
- `test_semantic_rekey_relative_vs_absolute_source_file()` — [`L743`](../../../../../raw/code/graphify/tests/test_build.py#L743) — Re-key contract: a relative source_file is migrated; an absolute one is left
- `test_source_file_backslash_normalized()` — [`L96`](../../../../../raw/code/graphify/tests/test_build.py#L96) — Windows backslash paths and POSIX paths for the same file must produce one node.

## Module values
- `FIXTURES` — [`L7`](../../../../../raw/code/graphify/tests/test_build.py#L7)

