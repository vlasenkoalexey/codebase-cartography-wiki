---
title: 'Module: tests/test_reflect.py'
type: catalog
provenance: extracted
module: tests/test_reflect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_reflect`/
symbols:
  _doc: _doc().
  _NOW: _NOW.
  _write_raw_doc: _write_raw_doc().
  _run: _run().
  _make_graph: _make_graph().
  test_lessons_artifact_cannot_be_globbed_back_into_memory: test_lessons_artifact_cannot_be_globbed_back_into_memory().
  _days_before: _days_before().
  test_evenly_split_verdict_when_signals_cancel: test_evenly_split_verdict_when_signals_cancel().
  test_render_byte_stable_across_independent_aggregations: test_render_byte_stable_across_independent_aggregations().
  test_sidecar_write_classifies_and_keys_by_canonical_id: test_sidecar_write_classifies_and_keys_by_canonical_id().
  test_sidecar_is_byte_identical_across_runs: test_sidecar_is_byte_identical_across_runs().
  test_loader_marks_entry_stale_when_source_file_changes: test_loader_marks_entry_stale_when_source_file_changes().
  test_relative_source_file_not_spuriously_stale_in_graphify_out_layout: test_relative_source_file_not_spuriously_stale_in_graphify_out_layout().
  test_relative_source_file_resolved_via_graphify_root_marker: test_relative_source_file_resolved_via_graphify_root_marker().
  test_provenance_capped_to_five_most_recent: test_provenance_capped_to_five_most_recent().
  test_ambiguous_or_unresolved_citation_is_skipped: test_ambiguous_or_unresolved_citation_is_skipped().
  test_recency_decides_contested_verdict: test_recency_decides_contested_verdict().
  test_half_life_actually_feeds_decay: test_half_life_actually_feeds_decay().
  test_nonpositive_half_life_disables_decay: test_nonpositive_half_life_disables_decay().
  test_contested_node_renders_once_under_contested: test_contested_node_renders_once_under_contested().
  test_header_is_cautious: test_header_is_cautious().
  test_flat_layout_does_not_match_same_named_file_one_dir_up: test_flat_layout_does_not_match_same_named_file_one_dir_up().
  test_sources_split_into_preferred_tentative_contested: test_sources_split_into_preferred_tentative_contested().
  test_corroboration_threshold_promotes_only_repeated_nodes: test_corroboration_threshold_promotes_only_repeated_nodes().
  test_node_existence_gate_drops_stale_nodes: test_node_existence_gate_drops_stale_nodes().
  test_corroboration_counts_distinct_docs_not_citations: test_corroboration_counts_distinct_docs_not_citations().
  test_min_corroboration_is_honored_not_hardcoded: test_min_corroboration_is_honored_not_hardcoded().
  test_negative_only_node_absent_from_sources: test_negative_only_node_absent_from_sources().
  test_dead_ends_and_corrections_follow_doc_order: test_dead_ends_and_corrections_follow_doc_order().
  test_render_is_deterministic: test_render_is_deterministic().
  test_render_has_summary_and_sections: test_render_has_summary_and_sections().
  test_render_includes_by_topic_when_graph_present: test_render_includes_by_topic_when_graph_present().
  test_topic_sections_alpha_with_uncategorized_last: test_topic_sections_alpha_with_uncategorized_last().
  test_render_empty_memory_is_graceful: test_render_empty_memory_is_graceful().
  test_dead_ends_and_corrections_dedupe_by_question: test_dead_ends_and_corrections_dedupe_by_question().
  _overlay_graph: _overlay_graph().
  test_parse_round_trips_a_saved_doc: test_parse_round_trips_a_saved_doc().
  test_round_trip_survives_backslash_newline_and_quoted_node: test_round_trip_survives_backslash_newline_and_quoted_node().
  test_load_memory_docs_skips_foreign_and_sorts: test_load_memory_docs_skips_foreign_and_sorts().
  test_load_memory_docs_orders_by_date_then_filename: test_load_memory_docs_orders_by_date_then_filename().
  test_aggregate_counts_each_outcome: test_aggregate_counts_each_outcome().
  test_dead_ends_and_corrections_collected: test_dead_ends_and_corrections_collected().
  test_no_community_grouping_without_graph: test_no_community_grouping_without_graph().
  test_doc_community_tie_breaks_to_smallest_label: test_doc_community_tie_breaks_to_smallest_label().
  test_community_grouping_uses_plurality_community: test_community_grouping_uses_plurality_community().
  test_reflect_writes_lessons_file: test_reflect_writes_lessons_file().
  test_second_session_benefits_from_the_first: test_second_session_benefits_from_the_first().
  test_cli_reflect_groups_by_community_when_graph_present: test_cli_reflect_groups_by_community_when_graph_present().
  test_cli_node_existence_gate_drops_stale_node_end_to_end: test_cli_node_existence_gate_drops_stale_node_end_to_end().
  test_cli_reflect_if_stale_skips_when_fresh: test_cli_reflect_if_stale_skips_when_fresh().
  test_cli_reflect_if_stale_reruns_when_labels_newer: test_cli_reflect_if_stale_reruns_when_labels_newer().
  _overlay_corpus: _overlay_corpus().
  test_parse_returns_none_for_foreign_doc: test_parse_returns_none_for_foreign_doc().
  test_parse_handles_crlf: test_parse_handles_crlf().
  test_load_memory_docs_missing_dir_is_empty: test_load_memory_docs_missing_dir_is_empty().
  test_cli_reflect_end_to_end: test_cli_reflect_end_to_end().
  test_cli_save_result_rejects_bad_outcome: test_cli_save_result_rejects_bad_outcome().
  test_cli_save_result_reads_answer_from_file: test_cli_save_result_reads_answer_from_file().
  test_cli_save_result_requires_answer_or_answer_file: test_cli_save_result_requires_answer_or_answer_file().
  test_cli_reflect_cold_start_writes_empty_lessons: test_cli_reflect_cold_start_writes_empty_lessons().
  test_cli_reflect_respects_out_flag: test_cli_reflect_respects_out_flag().
  test_lessons_fresh_missing_output_is_not_fresh: test_lessons_fresh_missing_output_is_not_fresh().
  test_lessons_fresh_true_when_output_newer_than_inputs: test_lessons_fresh_true_when_output_newer_than_inputs().
  test_lessons_fresh_false_when_memory_newer: test_lessons_fresh_false_when_memory_newer().
  test_lessons_fresh_false_when_graph_newer: test_lessons_fresh_false_when_graph_newer().
  test_lessons_fresh_false_when_graph_sidecar_newer: test_lessons_fresh_false_when_graph_sidecar_newer().
  PYTHON: PYTHON.
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_reflect.py`](../../../../../raw/code/graphify/tests/test_reflect.py)

## Functions
- `_days_before(n: int)` — [`L39`](../../../../../raw/code/graphify/tests/test_reflect.py#L39)
- `_doc(outcome=None, nodes=None, question="q", correction="", date="2026-01-01")` — [`L145`](../../../../../raw/code/graphify/tests/test_reflect.py#L145)
- `_make_graph(tmp_path: Path)` — [`L560`](../../../../../raw/code/graphify/tests/test_reflect.py#L560) — Build a minimal graph.json + analysis/labels in tmp_path/graphify-out/.
- `_overlay_corpus(mem: Path)` — [`L738`](../../../../../raw/code/graphify/tests/test_reflect.py#L738) — A corpus with: a PREFERRED node (2 useful), a TENTATIVE node (1 useful),
- `_overlay_graph(out: Path, nodes: list[dict])` — [`L730`](../../../../../raw/code/graphify/tests/test_reflect.py#L730) — Write a minimal graph.json under ``out`` with the given node dicts.
- `_run(args: list[str], cwd: Path)` — [`L43`](../../../../../raw/code/graphify/tests/test_reflect.py#L43)
- `_write_raw_doc(mem: Path, filename: str, date: str, *, outcome="dead_end", question="q", nodes=None)` — [`L114`](../../../../../raw/code/graphify/tests/test_reflect.py#L114) — Write a memory doc with a controlled date so ordering is deterministic to assert.
- `test_aggregate_counts_each_outcome()` — [`L152`](../../../../../raw/code/graphify/tests/test_reflect.py#L152)
- `test_ambiguous_or_unresolved_citation_is_skipped(tmp_path)` — [`L939`](../../../../../raw/code/graphify/tests/test_reflect.py#L939) — A label shared by >1 node id (ambiguous) or absent from the graph — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_cli_node_existence_gate_drops_stale_node_end_to_end(tmp_path)` — [`L541`](../../../../../raw/code/graphify/tests/test_reflect.py#L541) — Through reflect()/CLI with a real graph.json: a cited node that isn't in the
- `test_cli_reflect_cold_start_writes_empty_lessons(tmp_path)` — [`L502`](../../../../../raw/code/graphify/tests/test_reflect.py#L502) — First run with no graphify-out/memory/ still succeeds and writes a valid doc.
- `test_cli_reflect_end_to_end(tmp_path)` — [`L459`](../../../../../raw/code/graphify/tests/test_reflect.py#L459)
- `test_cli_reflect_groups_by_community_when_graph_present(tmp_path)` — [`L522`](../../../../../raw/code/graphify/tests/test_reflect.py#L522) — With a real graph.json present, reflect auto-detects it and groups lessons
- `test_cli_reflect_if_stale_reruns_when_labels_newer(tmp_path)` — [`L673`](../../../../../raw/code/graphify/tests/test_reflect.py#L673) — A label refresh changes LESSONS.md topic headings, so --if-stale must rebuild.
- `test_cli_reflect_if_stale_skips_when_fresh(tmp_path)` — [`L647`](../../../../../raw/code/graphify/tests/test_reflect.py#L647) — `reflect --if-stale` skips the rebuild when LESSONS.md is already current,
- `test_cli_reflect_respects_out_flag(tmp_path)` — [`L512`](../../../../../raw/code/graphify/tests/test_reflect.py#L512)
- `test_cli_save_result_reads_answer_from_file(tmp_path)` — [`L481`](../../../../../raw/code/graphify/tests/test_reflect.py#L481) — --answer-file lets callers pass a long/multiline answer via a file instead
- `test_cli_save_result_rejects_bad_outcome(tmp_path)` — [`L473`](../../../../../raw/code/graphify/tests/test_reflect.py#L473) — argparse `choices` rejects an unknown outcome before save_query_result runs.
- `test_cli_save_result_requires_answer_or_answer_file(tmp_path)` — [`L495`](../../../../../raw/code/graphify/tests/test_reflect.py#L495) — Neither --answer nor --answer-file -> clean argparse error, not a crash.
- `test_community_grouping_uses_plurality_community()` — [`L316`](../../../../../raw/code/graphify/tests/test_reflect.py#L316)
- `test_contested_node_renders_once_under_contested()` — [`L382`](../../../../../raw/code/graphify/tests/test_reflect.py#L382) — A mixed-signal node appears in a single Contested line, not silently in both
- `test_corroboration_counts_distinct_docs_not_citations()` — [`L220`](../../../../../raw/code/graphify/tests/test_reflect.py#L220) — A node cited twice *within one doc* counts as ONE corroborating result, so it — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_corroboration_threshold_promotes_only_repeated_nodes()` — [`L183`](../../../../../raw/code/graphify/tests/test_reflect.py#L183) — One save can't mint a 'preferred' lesson; a second distinct result promotes it.
- `test_dead_ends_and_corrections_collected()` — [`L280`](../../../../../raw/code/graphify/tests/test_reflect.py#L280)
- `test_dead_ends_and_corrections_dedupe_by_question()` — [`L700`](../../../../../raw/code/graphify/tests/test_reflect.py#L700) — Saving the same Q&A more than once must not duplicate lines in the dead-ends
- `test_dead_ends_and_corrections_follow_doc_order(tmp_path)` — [`L291`](../../../../../raw/code/graphify/tests/test_reflect.py#L291) — dead_ends/corrections are appended in doc order, so their determinism rides on
- `test_doc_community_tie_breaks_to_smallest_label()` — [`L306`](../../../../../raw/code/graphify/tests/test_reflect.py#L306) — A doc whose source nodes split evenly across communities lands in the
- `test_evenly_split_verdict_when_signals_cancel()` — [`L253`](../../../../../raw/code/graphify/tests/test_reflect.py#L253) — A same-date useful + dead_end on one node cancel to score 0 -> 'evenly split'.
- `test_flat_layout_does_not_match_same_named_file_one_dir_up(tmp_path)` — [`L886`](../../../../../raw/code/graphify/tests/test_reflect.py#L886) — In a flat layout (graph.json at the project root), the resolver must use the
- `test_half_life_actually_feeds_decay()` — [`L238`](../../../../../raw/code/graphify/tests/test_reflect.py#L238) — Two stale useful + one fresh dead_end: a long half-life (≈no decay) lets the 2 — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_header_is_cautious()` — [`L394`](../../../../../raw/code/graphify/tests/test_reflect.py#L394) — The header nudges verification, not blind reuse.
- `test_lessons_artifact_cannot_be_globbed_back_into_memory(tmp_path)` — [`L401`](../../../../../raw/code/graphify/tests/test_reflect.py#L401) — Regression guard: the LESSONS.md output must never be re-ingested as a memory
- `test_lessons_fresh_false_when_graph_newer(tmp_path)` — [`L619`](../../../../../raw/code/graphify/tests/test_reflect.py#L619)
- `test_lessons_fresh_false_when_graph_sidecar_newer(tmp_path, sidecar_name)` — [`L632`](../../../../../raw/code/graphify/tests/test_reflect.py#L632)
- `test_lessons_fresh_false_when_memory_newer(tmp_path)` — [`L609`](../../../../../raw/code/graphify/tests/test_reflect.py#L609)
- `test_lessons_fresh_missing_output_is_not_fresh(tmp_path)` — [`L593`](../../../../../raw/code/graphify/tests/test_reflect.py#L593)
- `test_lessons_fresh_true_when_output_newer_than_inputs(tmp_path)` — [`L599`](../../../../../raw/code/graphify/tests/test_reflect.py#L599)
- `test_load_memory_docs_missing_dir_is_empty(tmp_path)` — [`L110`](../../../../../raw/code/graphify/tests/test_reflect.py#L110)
- `test_load_memory_docs_orders_by_date_then_filename(tmp_path)` — [`L127`](../../../../../raw/code/graphify/tests/test_reflect.py#L127) — Determinism hinges on this sort: docs come back oldest-first, filename as tiebreak.
- `test_load_memory_docs_skips_foreign_and_sorts(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_reflect.py#L98)
- `test_loader_marks_entry_stale_when_source_file_changes(tmp_path)` — [`L817`](../../../../../raw/code/graphify/tests/test_reflect.py#L817) — load_learning_overlay recomputes the file fingerprint: unchanged source => — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_min_corroboration_is_honored_not_hardcoded()` — [`L229`](../../../../../raw/code/graphify/tests/test_reflect.py#L229) — Two distinct useful results -> preferred at k=2, but only tentative at k=3. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_negative_only_node_absent_from_sources()` — [`L271`](../../../../../raw/code/graphify/tests/test_reflect.py#L271) — A node seen only in dead_end docs never appears as a source bucket entry, but
- `test_no_community_grouping_without_graph()` — [`L301`](../../../../../raw/code/graphify/tests/test_reflect.py#L301)
- `test_node_existence_gate_drops_stale_nodes()` — [`L211`](../../../../../raw/code/graphify/tests/test_reflect.py#L211) — A cited node no longer in the graph is dropped from lessons entirely.
- `test_nonpositive_half_life_disables_decay()` — [`L262`](../../../../../raw/code/graphify/tests/test_reflect.py#L262) — half_life<=0 turns decay off (full weight), so a stale useful and a fresh — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_parse_handles_crlf()` — [`L90`](../../../../../raw/code/graphify/tests/test_reflect.py#L90)
- `test_parse_returns_none_for_foreign_doc()` — [`L69`](../../../../../raw/code/graphify/tests/test_reflect.py#L69) — A plain markdown file with no frontmatter is skipped, not crashed on.
- `test_parse_round_trips_a_saved_doc(tmp_path)` — [`L53`](../../../../../raw/code/graphify/tests/test_reflect.py#L53) — parse_memory_doc reads back exactly what save_query_result wrote, including
- `test_provenance_capped_to_five_most_recent(tmp_path)` — [`L916`](../../../../../raw/code/graphify/tests/test_reflect.py#L916) — A node cited by >5 useful results keeps exactly the 5 most-recent in
- `test_recency_decides_contested_verdict()` — [`L195`](../../../../../raw/code/graphify/tests/test_reflect.py#L195) — A fresh dead_end outweighs a stale useful (30d half-life), so the contested — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_reflect_writes_lessons_file(tmp_path)` — [`L424`](../../../../../raw/code/graphify/tests/test_reflect.py#L424)
- `test_relative_source_file_not_spuriously_stale_in_graphify_out_layout(tmp_path)` — [`L840`](../../../../../raw/code/graphify/tests/test_reflect.py#L840) — Regression: with a RELATIVE source_file and graph.json under graphify-out/, — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_relative_source_file_resolved_via_graphify_root_marker(tmp_path)` — [`L866`](../../../../../raw/code/graphify/tests/test_reflect.py#L866) — When a committed .graphify_root marker records the project root (e.g. a
- `test_render_byte_stable_across_independent_aggregations(tmp_path)` — [`L371`](../../../../../raw/code/graphify/tests/test_reflect.py#L371) — The headline guarantee: identical memory/ contents + same `now` -> byte-identical — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_render_empty_memory_is_graceful()` — [`L415`](../../../../../raw/code/graphify/tests/test_reflect.py#L415) — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_render_has_summary_and_sections()` — [`L339`](../../../../../raw/code/graphify/tests/test_reflect.py#L339)
- `test_render_includes_by_topic_when_graph_present()` — [`L355`](../../../../../raw/code/graphify/tests/test_reflect.py#L355)
- `test_render_is_deterministic()` — [`L333`](../../../../../raw/code/graphify/tests/test_reflect.py#L333)
- `test_round_trip_survives_backslash_newline_and_quoted_node(tmp_path)` — [`L75`](../../../../../raw/code/graphify/tests/test_reflect.py#L75) — save -> parse preserves tricky characters in the question, the correction,
- `test_second_session_benefits_from_the_first(tmp_path)` — [`L433`](../../../../../raw/code/graphify/tests/test_reflect.py#L433) — The issue's worked example: session 1 records a win and a dead end; session 2 — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_sidecar_is_byte_identical_across_runs(tmp_path)` — [`L795`](../../../../../raw/code/graphify/tests/test_reflect.py#L795) — Two reflect runs on identical input + fixed `now` produce a byte-identical — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `test_sidecar_write_classifies_and_keys_by_canonical_id(tmp_path)` — [`L755`](../../../../../raw/code/graphify/tests/test_reflect.py#L755) — reflect with a graph writes .graphify_learning.json next to graph.json with
- `test_sources_split_into_preferred_tentative_contested()` — [`L163`](../../../../../raw/code/graphify/tests/test_reflect.py#L163) — Corroboration (k>=2) + sign decide the bucket, not raw frequency:
- `test_topic_sections_alpha_with_uncategorized_last()` — [`L362`](../../../../../raw/code/graphify/tests/test_reflect.py#L362) — Topic headers render alphabetically, with Uncategorized always last.

## Module values
- `FIXTURES` — [`L33`](../../../../../raw/code/graphify/tests/test_reflect.py#L33)
- `PYTHON` — [`L32`](../../../../../raw/code/graphify/tests/test_reflect.py#L32)
- `_NOW` — [`L36`](../../../../../raw/code/graphify/tests/test_reflect.py#L36)

