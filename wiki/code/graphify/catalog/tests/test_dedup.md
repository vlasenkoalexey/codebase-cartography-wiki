---
title: 'Module: tests/test_dedup.py'
type: catalog
provenance: extracted
module: tests/test_dedup.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_dedup`/
symbols:
  _make_nodes: _make_nodes().
  test_exact_duplicates_merged: test_exact_duplicates_merged().
  test_typo_merged: test_typo_merged().
  test_unrelated_not_merged: test_unrelated_not_merged().
  test_short_low_entropy_not_merged: test_short_low_entropy_not_merged().
  test_edges_rewired_after_merge: test_edges_rewired_after_merge().
  test_self_loops_dropped_after_merge: test_self_loops_dropped_after_merge().
  test_community_boost_aids_merge: test_community_boost_aids_merge().
  test_single_node_no_crash: test_single_node_no_crash().
  test_dedup_llm_flag_accepted: test_dedup_llm_flag_accepted().
  test_dedup_does_not_merge_numeric_variants: test_dedup_does_not_merge_numeric_variants().
  test_dedup_does_not_merge_short_insertion_variants: test_dedup_does_not_merge_short_insertion_variants().
  test_dedup_does_not_merge_model_with_suffix: test_dedup_does_not_merge_model_with_suffix().
  test_dedup_still_merges_real_typos: test_dedup_still_merges_real_typos().
  test_entropy_short_label_low: test_entropy_short_label_low().
  test_entropy_normal_label_high: test_entropy_normal_label_high().
  test_entropy_empty_string: test_entropy_empty_string().
  test_shingles_produces_trigrams: test_shingles_produces_trigrams().
  test_shingles_short_string: test_shingles_short_string().
  test_empty_inputs: test_empty_inputs().
  test_build_calls_dedup: test_build_calls_dedup().
  test_variant_pair_helper: test_variant_pair_helper().
  test_prefix_extension_symbols_not_merged: test_prefix_extension_symbols_not_merged().
  test_pass2_winner_union_does_not_pull_in_uncompared_same_label_nodes: test_pass2_winner_union_does_not_pull_in_uncompared_same_label_nodes().
  test_prefix_guard_does_not_block_same_length_typos: test_prefix_guard_does_not_block_same_length_typos().
  test_prefix_guard_fires_for_extension_pairs: test_prefix_guard_fires_for_extension_pairs().
  test_numeric_tokens_differ_helper: test_numeric_tokens_differ_helper().
  test_dedup_does_not_merge_numbered_siblings: test_dedup_does_not_merge_numbered_siblings().
  test_dedup_does_not_merge_crossfile_rationale_boilerplate: test_dedup_does_not_merge_crossfile_rationale_boilerplate().
  test_dedup_does_not_merge_crossfile_document_headings: test_dedup_does_not_merge_crossfile_document_headings().
  test_dedup_still_merges_samefile_rationale_duplicates: test_dedup_still_merges_samefile_rationale_duplicates().
  test_dedup_does_not_merge_crossfile_shared_prefix_divergence: test_dedup_does_not_merge_crossfile_shared_prefix_divergence().
  test_dedup_still_merges_crossfile_true_duplicates: test_dedup_still_merges_crossfile_true_duplicates().
  test_cross_chunk_id_collision_emits_warning: test_cross_chunk_id_collision_emits_warning().
  test_same_id_same_source_file_no_warning: test_same_id_same_source_file_no_warning().
  _make_edges: _make_edges().
---
# Module: [`tests/test_dedup.py`](../../../../../raw/code/graphify/tests/test_dedup.py)

## Functions
- `_make_edges(src, tgt, relation="relates_to")` — [`L37`](../../../../../raw/code/graphify/tests/test_dedup.py#L37)
- `_make_nodes(*labels)` — [`L34`](../../../../../raw/code/graphify/tests/test_dedup.py#L34)
- `test_build_calls_dedup()` — [`L125`](../../../../../raw/code/graphify/tests/test_dedup.py#L125) — build() should deduplicate near-identical nodes across extractions.
- `test_community_boost_aids_merge()` — [`L90`](../../../../../raw/code/graphify/tests/test_dedup.py#L90)
- `test_cross_chunk_id_collision_emits_warning(capsys)` — [`L371`](../../../../../raw/code/graphify/tests/test_dedup.py#L371) — When two nodes share the same ID but come from different source files
- `test_dedup_does_not_merge_crossfile_document_headings()` — [`L315`](../../../../../raw/code/graphify/tests/test_dedup.py#L315) — Document nodes are file-anchored too: near-identical headings in different
- `test_dedup_does_not_merge_crossfile_rationale_boilerplate()` — [`L300`](../../../../../raw/code/graphify/tests/test_dedup.py#L300) — Rationale nodes are file-anchored like code (#1205): parallel modules'
- `test_dedup_does_not_merge_crossfile_shared_prefix_divergence()` — [`L343`](../../../../../raw/code/graphify/tests/test_dedup.py#L343) — Cross-file labels sharing a long prefix but diverging in a distinguishing
- `test_dedup_does_not_merge_model_with_suffix(tmp_path)` — [`L156`](../../../../../raw/code/graphify/tests/test_dedup.py#L156) — M1 vs M1 Pro must not merge (#878).
- `test_dedup_does_not_merge_numbered_siblings()` — [`L287`](../../../../../raw/code/graphify/tests/test_dedup.py#L287) — Long labels differing only in embedded numbers (ADR/section/issue ids)
- `test_dedup_does_not_merge_numeric_variants(tmp_path)` — [`L142`](../../../../../raw/code/graphify/tests/test_dedup.py#L142) — Chip SKU variants (ASR1603 vs ASR1605) must not be merged (#878).
- `test_dedup_does_not_merge_short_insertion_variants(tmp_path)` — [`L149`](../../../../../raw/code/graphify/tests/test_dedup.py#L149) — Short labels differing by an insertion (cranel vs cranelr) must not merge (#878).
- `test_dedup_llm_flag_accepted()` — [`L115`](../../../../../raw/code/graphify/tests/test_dedup.py#L115) — deduplicate_entities accepts dedup_llm_backend without crashing when no ambiguous pairs exist.
- `test_dedup_still_merges_crossfile_true_duplicates()` — [`L358`](../../../../../raw/code/graphify/tests/test_dedup.py#L358) — The #1243 guard only drops the prefix bonus — a genuine cross-file
- `test_dedup_still_merges_real_typos()` — [`L163`](../../../../../raw/code/graphify/tests/test_dedup.py#L163) — Genuine same-length single-char typos should still merge (#878 non-regression).
- `test_dedup_still_merges_samefile_rationale_duplicates()` — [`L328`](../../../../../raw/code/graphify/tests/test_dedup.py#L328) — The file-anchored guard only blocks cross-file pairs — near-identical
- `test_edges_rewired_after_merge()` — [`L72`](../../../../../raw/code/graphify/tests/test_dedup.py#L72)
- `test_empty_inputs()` — [`L103`](../../../../../raw/code/graphify/tests/test_dedup.py#L103)
- `test_entropy_empty_string()` — [`L15`](../../../../../raw/code/graphify/tests/test_dedup.py#L15)
- `test_entropy_normal_label_high()` — [`L12`](../../../../../raw/code/graphify/tests/test_dedup.py#L12)
- `test_entropy_short_label_low()` — [`L9`](../../../../../raw/code/graphify/tests/test_dedup.py#L9)
- `test_exact_duplicates_merged()` — [`L41`](../../../../../raw/code/graphify/tests/test_dedup.py#L41)
- `test_numeric_tokens_differ_helper()` — [`L275`](../../../../../raw/code/graphify/tests/test_dedup.py#L275) — _numeric_tokens_differ compares digit runs as zero-padding-insensitive
- `test_pass2_winner_union_does_not_pull_in_uncompared_same_label_nodes()` — [`L211`](../../../../../raw/code/graphify/tests/test_dedup.py#L211) — Pass 2's winner selection must consider only the verified pair (#1247).
- `test_prefix_extension_symbols_not_merged()` — [`L182`](../../../../../raw/code/graphify/tests/test_dedup.py#L182) — Distinct symbols whose name is a strict prefix-extension of another must not
- `test_prefix_guard_does_not_block_same_length_typos()` — [`L241`](../../../../../raw/code/graphify/tests/test_dedup.py#L241) — The prefix-extension guard must not fire for same-length pairs — only strict
- `test_prefix_guard_fires_for_extension_pairs()` — [`L256`](../../../../../raw/code/graphify/tests/test_dedup.py#L256) — The prefix-extension guard must fire for pairs where one is a strict prefix
- `test_same_id_same_source_file_no_warning(capsys)` — [`L393`](../../../../../raw/code/graphify/tests/test_dedup.py#L393) — When two nodes share both ID and source_file (same-file dedup),
- `test_self_loops_dropped_after_merge()` — [`L82`](../../../../../raw/code/graphify/tests/test_dedup.py#L82)
- `test_shingles_produces_trigrams()` — [`L21`](../../../../../raw/code/graphify/tests/test_dedup.py#L21)
- `test_shingles_short_string()` — [`L27`](../../../../../raw/code/graphify/tests/test_dedup.py#L27)
- `test_short_low_entropy_not_merged()` — [`L64`](../../../../../raw/code/graphify/tests/test_dedup.py#L64)
- `test_single_node_no_crash()` — [`L109`](../../../../../raw/code/graphify/tests/test_dedup.py#L109)
- `test_typo_merged()` — [`L49`](../../../../../raw/code/graphify/tests/test_dedup.py#L49)
- `test_unrelated_not_merged()` — [`L57`](../../../../../raw/code/graphify/tests/test_dedup.py#L57)
- `test_variant_pair_helper()` — [`L173`](../../../../../raw/code/graphify/tests/test_dedup.py#L173) — _is_variant_pair correctly identifies chip-model variant pairs (#878).

