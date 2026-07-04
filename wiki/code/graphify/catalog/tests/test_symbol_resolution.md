---
title: 'Module: tests/test_symbol_resolution.py'
type: catalog
provenance: extracted
module: tests/test_symbol_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_symbol_resolution`/test_
symbols:
  test_resolve_python_import_guided_calls_metadata_sanitizes_hostile_alias: resolve_python_import_guided_calls_metadata_sanitizes_hostile_alias().
  test_parse_python_import_aliases_supports_from_import_alias: parse_python_import_aliases_supports_from_import_alias().
  test_find_unique_python_symbol_returns_none_when_ambiguous: find_unique_python_symbol_returns_none_when_ambiguous().
  test_bash_make_id_identical_to_make_id: bash_make_id_identical_to_make_id().
  test_bash_make_id_unicode_matches_make_id: bash_make_id_unicode_matches_make_id().
  test_parse_python_import_aliases_accepts_top_level_import: parse_python_import_aliases_accepts_top_level_import().
  test_resolve_python_import_guided_calls_metadata_sanitizes_hostile_alias._fake_aliases: resolve_python_import_guided_calls_metadata_sanitizes_hostile_alias()._fake_aliases().
  test_normalise_callable_label_strips_function_punctuation: normalise_callable_label_strips_function_punctuation().
  test_node_is_resolvable_symbol_skips_rationale_and_doc_tags: node_is_resolvable_symbol_skips_rationale_and_doc_tags().
  test_build_label_index_collects_unique_symbols: build_label_index_collects_unique_symbols().
  test_resolve_cross_file_raw_calls_emits_unique_unqualified_call: resolve_cross_file_raw_calls_emits_unique_unqualified_call().
  test_resolve_cross_file_raw_calls_skips_member_calls: resolve_cross_file_raw_calls_skips_member_calls().
  test_resolve_cross_file_raw_calls_skips_ambiguous_duplicate_labels: resolve_cross_file_raw_calls_skips_ambiguous_duplicate_labels().
  test_resolve_cross_file_raw_calls_real_edge_survives_test_mock: resolve_cross_file_raw_calls_real_edge_survives_test_mock().
  test_resolve_cross_file_raw_calls_n_mock_scale: resolve_cross_file_raw_calls_n_mock_scale().
  test_resolve_cross_file_raw_calls_call_site_is_test_prefers_test_local: resolve_cross_file_raw_calls_call_site_is_test_prefers_test_local().
  test_resolve_cross_file_raw_calls_skips_existing_pair: resolve_cross_file_raw_calls_skips_existing_pair().
  test_build_python_symbol_index_uses_module_stem_and_label: build_python_symbol_index_uses_module_stem_and_label().
  test_resolve_python_import_guided_calls_emits_extracted_edge: resolve_python_import_guided_calls_emits_extracted_edge().
  test_bash_call_resolver_emits_source_edges: bash_call_resolver_emits_source_edges().
  test_bash_call_resolver_emits_call_edges_from_sourced_files: bash_call_resolver_emits_call_edges_from_sourced_files().
  test_bash_call_resolver_skips_existing_pair: bash_call_resolver_skips_existing_pair().
  test_bash_call_resolver_skips_ambiguous_multiple_candidates: bash_call_resolver_skips_ambiguous_multiple_candidates().
  test_bash_call_resolver_skips_non_bash_raw_calls: bash_call_resolver_skips_non_bash_raw_calls().
  test_parse_python_import_aliases_skips_function_local_imports: parse_python_import_aliases_skips_function_local_imports().
  test_node_is_resolvable_symbol_requires_code_file_type: node_is_resolvable_symbol_requires_code_file_type().
  test_build_label_index_excludes_non_code_nodes: build_label_index_excludes_non_code_nodes().
  test_resolve_bash_source_edges_skips_malformed_source: resolve_bash_source_edges_skips_malformed_source().
  test_resolve_bash_source_edges_skips_bash_function_node_missing_id: resolve_bash_source_edges_skips_bash_function_node_missing_id().
  test_resolve_bash_source_edges_skips_raw_call_missing_caller_nid: resolve_bash_source_edges_skips_raw_call_missing_caller_nid().
  test_resolve_bash_source_edges_accepts_none_per_file_entries: resolve_bash_source_edges_accepts_none_per_file_entries().
  test_resolve_bash_source_edges_skips_non_dict_lists: resolve_bash_source_edges_skips_non_dict_lists().
  test_resolve_bash_source_edges_relative_path_resolves_against_source_dir: resolve_bash_source_edges_relative_path_resolves_against_source_dir().
  test_iter_raw_calls_skips_non_dict_per_file_entries: iter_raw_calls_skips_non_dict_per_file_entries().
  test_iter_raw_calls_skips_non_list_raw_calls: iter_raw_calls_skips_non_list_raw_calls().
  test_iter_raw_calls_drops_non_dict_items_in_list: iter_raw_calls_drops_non_dict_items_in_list().
  test_resolve_cross_file_raw_calls_survives_malformed_raw_calls: resolve_cross_file_raw_calls_survives_malformed_raw_calls().
  test_resolve_python_import_guided_calls_survives_malformed_raw_calls: resolve_python_import_guided_calls_survives_malformed_raw_calls().
  test_resolve_bash_source_edges_skips_unhashable_callee: resolve_bash_source_edges_skips_unhashable_callee().
  test_resolve_python_import_guided_calls_non_dict_per_file_slot: resolve_python_import_guided_calls_non_dict_per_file_slot().
  test_resolve_python_import_guided_calls_per_file_shorter_than_paths: resolve_python_import_guided_calls_per_file_shorter_than_paths().
  test_resolve_python_import_guided_calls_per_file_none_slot: resolve_python_import_guided_calls_per_file_none_slot().
  test_resolve_python_import_guided_calls_metadata_is_sanitized: resolve_python_import_guided_calls_metadata_is_sanitized().
---
# Module: [`tests/test_symbol_resolution.py`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py)

## Functions
- `_fake_aliases(path: Path)` — [`L1052`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L1052)
- `test_bash_call_resolver_emits_call_edges_from_sourced_files(tmp_path: Path)` — [`L383`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L383)
- `test_bash_call_resolver_emits_source_edges(tmp_path: Path)` — [`L336`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L336)
- `test_bash_call_resolver_skips_ambiguous_multiple_candidates(tmp_path: Path)` — [`L499`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L499) — When a callee function is defined in multiple sourced files, skip it.
- `test_bash_call_resolver_skips_existing_pair(tmp_path: Path)` — [`L442`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L442)
- `test_bash_call_resolver_skips_non_bash_raw_calls(tmp_path: Path)` — [`L575`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L575) — Non-bash raw_calls inside sourced-file per_file entries are ignored.
- `test_bash_make_id_identical_to_make_id()` — [`L604`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L604)
- `test_bash_make_id_unicode_matches_make_id()` — [`L613`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L613) — _bash_make_id must produce identical output to _make_id for Unicode inputs.
- `test_build_label_index_collects_unique_symbols()` — [`L35`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L35)
- `test_build_label_index_excludes_non_code_nodes()` — [`L690`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L690) — label index must not include document/paper/image nodes even when
- `test_build_python_symbol_index_uses_module_stem_and_label()` — [`L246`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L246)
- `test_find_unique_python_symbol_returns_none_when_ambiguous(tmp_path: Path)` — [`L266`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L266)
- `test_iter_raw_calls_drops_non_dict_items_in_list()` — [`L852`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L852) — Items inside `raw_calls` list that aren't dicts must be dropped.
- `test_iter_raw_calls_skips_non_dict_per_file_entries()` — [`L836`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L836) — A non-dict per_file entry (e.g. junk fragment) must be silently skipped.
- `test_iter_raw_calls_skips_non_list_raw_calls()` — [`L843`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L843) — `raw_calls` that isn't a list must yield empty.
- `test_node_is_resolvable_symbol_requires_code_file_type()` — [`L672`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L672) — Document/paper/image/concept nodes MUST NOT be indexed as call targets,
- `test_node_is_resolvable_symbol_skips_rationale_and_doc_tags()` — [`L27`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L27)
- `test_normalise_callable_label_strips_function_punctuation()` — [`L21`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L21)
- `test_parse_python_import_aliases_accepts_top_level_import(tmp_path)` — [`L660`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L660) — A module-level `from helper import transform` IS file-wide evidence.
- `test_parse_python_import_aliases_skips_function_local_imports(tmp_path)` — [`L638`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L638) — A `from helper import transform` inside a function MUST NOT become
- `test_parse_python_import_aliases_supports_from_import_alias(tmp_path: Path)` — [`L232`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L232)
- `test_resolve_bash_source_edges_accepts_none_per_file_entries(tmp_path)` — [`L775`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L775) — A None entry in per_file (e.g. failed extraction) must be silently skipped.
- `test_resolve_bash_source_edges_relative_path_resolves_against_source_dir(tmp_path)` — [`L803`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L803) — `source ./helper.sh` from a/main.sh should resolve to a/helper.sh,
- `test_resolve_bash_source_edges_skips_bash_function_node_missing_id(tmp_path)` — [`L726`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L726) — A node tagged as bash_function but missing `id` must not raise KeyError.
- `test_resolve_bash_source_edges_skips_malformed_source(tmp_path)` — [`L705`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L705) — A `bash_sources` entry missing `target_path` must not raise KeyError.
- `test_resolve_bash_source_edges_skips_non_dict_lists(tmp_path)` — [`L785`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L785) — Non-dict entries in bash_sources/raw_calls/nodes must be silently skipped.
- `test_resolve_bash_source_edges_skips_raw_call_missing_caller_nid(tmp_path)` — [`L746`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L746) — A raw_call entry missing `caller_nid` must not raise KeyError.
- `test_resolve_bash_source_edges_skips_unhashable_callee(tmp_path)` — [`L892`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L892) — A bash raw_call with `callee: [list]` (unhashable for dict membership)
- `test_resolve_cross_file_raw_calls_call_site_is_test_prefers_test_local()` — [`L181`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L181) — A test file calling save() with both a src def and a test-local def present
- `test_resolve_cross_file_raw_calls_emits_unique_unqualified_call()` — [`L44`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L44)
- `test_resolve_cross_file_raw_calls_n_mock_scale()` — [`L154`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L154) — One src def plus many same-named test stubs: exactly one edge to src.
- `test_resolve_cross_file_raw_calls_real_edge_survives_test_mock()` — [`L127`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L127) — A real cross-file call must resolve to the SRC definition even when a
- `test_resolve_cross_file_raw_calls_skips_ambiguous_duplicate_labels()` — [`L102`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L102) — Two genuine NON-test defs of the same name: the god-node guard must still
- `test_resolve_cross_file_raw_calls_skips_existing_pair()` — [`L210`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L210)
- `test_resolve_cross_file_raw_calls_skips_member_calls()` — [`L81`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L81)
- `test_resolve_cross_file_raw_calls_survives_malformed_raw_calls()` — [`L860`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L860) — The python cross-file resolver returns [] (not crash) on bad raw_calls.
- `test_resolve_python_import_guided_calls_emits_extracted_edge(tmp_path: Path)` — [`L274`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L274)
- `test_resolve_python_import_guided_calls_metadata_is_sanitized(tmp_path: Path)` — [`L961`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L961) — Edge metadata produced by the import-guided resolver must pass through
- `test_resolve_python_import_guided_calls_metadata_sanitizes_hostile_alias(monkeypatch, tmp_path: Path)` — [`L1017`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L1017) — Strong regression for #cycle-2.7-Codex-v2: monkeypatch the alias parser
- `test_resolve_python_import_guided_calls_non_dict_per_file_slot(tmp_path)` — [`L927`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L927) — A non-dict per_file slot (e.g. a string) must not raise AttributeError.
- `test_resolve_python_import_guided_calls_per_file_none_slot(tmp_path)` — [`L951`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L951) — A None per_file slot is treated as empty fragment (no crash, no edges).
- `test_resolve_python_import_guided_calls_per_file_shorter_than_paths(tmp_path)` — [`L938`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L938) — per_file shorter than paths must not raise IndexError.
- `test_resolve_python_import_guided_calls_survives_malformed_raw_calls(tmp_path)` — [`L870`](../../../../../raw/code/graphify/tests/test_symbol_resolution.py#L870) — Python import-guided resolver also tolerates malformed raw_calls.

