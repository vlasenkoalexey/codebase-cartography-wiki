---
title: 'Module: tests/test_scip_ingest.py'
type: catalog
provenance: extracted
module: tests/test_scip_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_scip_ingest`/
symbols:
  _make_symbol_doc: _make_symbol_doc().
  test_relationship_edges_survive_validate_extraction_and_build: test_relationship_edges_survive_validate_extraction_and_build().
  test_ingest_is_reference_emits_scip_ref_edge: test_ingest_is_reference_emits_scip_ref_edge().
  test_ingest_is_definition_emits_scip_def_edge: test_ingest_is_definition_emits_scip_def_edge().
  test_ingest_is_implementation_emits_scip_impl_edge: test_ingest_is_implementation_emits_scip_impl_edge().
  test_ingest_is_type_definition_emits_scip_typed_edge: test_ingest_is_type_definition_emits_scip_typed_edge().
  test_ingest_relationship_priority_order: test_ingest_relationship_priority_order().
  test_ingest_relationship_no_boolean_flags_defaults_to_ref: test_ingest_relationship_no_boolean_flags_defaults_to_ref().
  test_ingest_multiple_relationships_on_one_symbol: test_ingest_multiple_relationships_on_one_symbol().
  test_ingest_relationship_without_target_symbol_is_skipped: test_ingest_relationship_without_target_symbol_is_skipped().
  test_ingest_duplicate_edges_are_deduplicated: test_ingest_duplicate_edges_are_deduplicated().
  test_ingest_edge_structure_complete: test_ingest_edge_structure_complete().
  test_ingest_node_id_contains_source_file_and_symbol_suffix: test_ingest_node_id_contains_source_file_and_symbol_suffix().
  test_ingest_node_id_is_deterministic: test_ingest_node_id_is_deterministic().
  test_ingest_relationship_item_not_a_dict_is_skipped: test_ingest_relationship_item_not_a_dict_is_skipped().
  test_ingest_empty_doc_returns_empty_lists: test_ingest_empty_doc_returns_empty_lists().
  test_ingest_dict_without_documents_key: test_ingest_dict_without_documents_key().
  test_ingest_documents_not_a_list_is_skipped: test_ingest_documents_not_a_list_is_skipped().
  test_ingest_documents_empty_list: test_ingest_documents_empty_list().
  test_ingest_single_symbol_no_relationships: test_ingest_single_symbol_no_relationships().
  test_ingest_symbol_without_display_name_uses_suffix: test_ingest_symbol_without_display_name_uses_suffix().
  test_ingest_symbol_trailing_hash_no_display_name_has_non_empty_label: test_ingest_symbol_trailing_hash_no_display_name_has_non_empty_label().
  test_ingest_symbol_without_hash_uses_full_symbol_as_label: test_ingest_symbol_without_hash_uses_full_symbol_as_label().
  test_ingest_symbol_without_occurrences_has_empty_source_location: test_ingest_symbol_without_occurrences_has_empty_source_location().
  test_ingest_symbol_without_occurrences_key: test_ingest_symbol_without_occurrences_key().
  test_ingest_multiple_symbols_in_one_document: test_ingest_multiple_symbols_in_one_document().
  test_ingest_multiple_documents: test_ingest_multiple_documents().
  test_ingest_edge_source_location_from_first_occurrence: test_ingest_edge_source_location_from_first_occurrence().
  test_ingest_node_id_differs_by_source_file: test_ingest_node_id_differs_by_source_file().
  test_ingest_duplicate_symbols_in_same_file_are_deduplicated: test_ingest_duplicate_symbols_in_same_file_are_deduplicated().
  test_ingest_non_dict_input_returns_empty: test_ingest_non_dict_input_returns_empty().
  test_ingest_document_item_not_a_dict_is_skipped: test_ingest_document_item_not_a_dict_is_skipped().
  test_ingest_symbol_item_not_a_dict_is_skipped: test_ingest_symbol_item_not_a_dict_is_skipped().
  test_ingest_symbol_without_symbol_id_is_skipped: test_ingest_symbol_without_symbol_id_is_skipped().
  test_ingest_document_without_symbols_key: test_ingest_document_without_symbols_key().
  test_ingest_document_with_symbols_not_a_list: test_ingest_document_with_symbols_not_a_list().
  test_ingest_symbol_without_kind_defaults_to_unknown: test_ingest_symbol_without_kind_defaults_to_unknown().
  test_ingest_default_source_file_is_empty_string: test_ingest_default_source_file_is_empty_string().
  test_ingest_source_file_falls_back_to_function_param: test_ingest_source_file_falls_back_to_function_param().
  test_ingest_document_relative_path_overrides_source_file_param: test_ingest_document_relative_path_overrides_source_file_param().
  test_ingest_document_without_language_defaults_to_function_param: test_ingest_document_without_language_defaults_to_function_param().
  test_ingest_symbol_with_short_range_uses_first_element_as_line: test_ingest_symbol_with_short_range_uses_first_element_as_line().
  test_ingest_symbol_with_non_dict_occurrence_is_skipped: test_ingest_symbol_with_non_dict_occurrence_is_skipped().
  test_ingest_symbol_with_non_list_range_falls_back_to_zero: test_ingest_symbol_with_non_list_range_falls_back_to_zero().
  test_ingest_symbol_with_documentation_becomes_description: test_ingest_symbol_with_documentation_becomes_description().
  test_ingest_symbol_with_empty_documentation_skips_description: test_ingest_symbol_with_empty_documentation_skips_description().
  test_ingest_symbol_without_documentation_omits_description: test_ingest_symbol_without_documentation_omits_description().
  test_ingest_symbol_without_relationships_key_still_creates_node: test_ingest_symbol_without_relationships_key_still_creates_node().
  test_make_scip_node_id_with_hash_separator: test_make_scip_node_id_with_hash_separator().
  test_make_scip_node_id_without_hash: test_make_scip_node_id_without_hash().
  test_make_scip_node_id_special_characters_are_sanitised: test_make_scip_node_id_special_characters_are_sanitised().
  test_make_scip_node_id_deterministic: test_make_scip_node_id_deterministic().
  test_make_scip_node_id_source_file_affects_hash: test_make_scip_node_id_source_file_affects_hash().
  test_make_scip_node_id_symbol_affects_hash: test_make_scip_node_id_symbol_affects_hash().
  test_make_scip_node_id_empty_after_sanitisation_falls_back: test_make_scip_node_id_empty_after_sanitisation_falls_back().
  test_scip_kind_to_file_type_always_code: test_scip_kind_to_file_type_always_code().
  test_build_scip_metadata_with_description: test_build_scip_metadata_with_description().
  test_build_scip_metadata_without_description: test_build_scip_metadata_without_description().
  test_ingest_many_symbols: test_ingest_many_symbols().
  test_ingest_edge_with_zero_sourceline_has_empty_location: test_ingest_edge_with_zero_sourceline_has_empty_location().
  test_relationship_target_in_same_document_resolves_via_index: test_relationship_target_in_same_document_resolves_via_index().
  test_relationship_target_across_documents_resolves_via_index: test_relationship_target_across_documents_resolves_via_index().
  test_relationship_target_unknown_emits_stub_node: test_relationship_target_unknown_emits_stub_node().
  test_non_string_relative_path_falls_back_to_default: test_non_string_relative_path_falls_back_to_default().
  test_non_string_language_falls_back: test_non_string_language_falls_back().
  test_non_string_symbol_id_is_skipped: test_non_string_symbol_id_is_skipped().
  test_relationships_none_is_treated_as_empty: test_relationships_none_is_treated_as_empty().
  test_relationship_symbol_non_string_is_skipped: test_relationship_symbol_non_string_is_skipped().
  test_non_string_kind_falls_back_to_unknown: test_non_string_kind_falls_back_to_unknown().
  test_non_string_display_name_falls_back: test_non_string_display_name_falls_back().
  test_documentation_with_non_string_entries_is_ignored: test_documentation_with_non_string_entries_is_ignored().
  test_unrecognized_top_level_structure_returns_empty: test_unrecognized_top_level_structure_returns_empty().
  test_documents_field_non_list_returns_empty: test_documents_field_non_list_returns_empty().
  test_document_entry_non_dict_is_skipped: test_document_entry_non_dict_is_skipped().
  test_occurrence_negative_line_falls_back_to_zero: test_occurrence_negative_line_falls_back_to_zero().
  test_duplicate_local_symbol_resolves_to_same_document: test_duplicate_local_symbol_resolves_to_same_document().
  test_unique_cross_document_symbol_still_resolves: test_unique_cross_document_symbol_still_resolves().
  test_ambiguous_duplicate_target_across_docs_creates_stub: test_ambiguous_duplicate_target_across_docs_creates_stub().
  test_relationship_truthy_string_flag_is_ignored: test_relationship_truthy_string_flag_is_ignored().
  test_relationship_int_flag_is_ignored: test_relationship_int_flag_is_ignored().
  test_relationship_boolean_true_routes_correctly: test_relationship_boolean_true_routes_correctly().
  test_occurrence_bool_line_falls_back_to_zero: test_occurrence_bool_line_falls_back_to_zero().
  test_duplicate_same_document_definition_does_not_create_false_ambiguity: test_duplicate_same_document_definition_does_not_create_false_ambiguity().
  test_ingest_node_metadata_html_escaped: test_ingest_node_metadata_html_escaped().
  test_ingest_node_metadata_control_chars_stripped: test_ingest_node_metadata_control_chars_stripped().
  test_ingest_relationship_metadata_sanitized: test_ingest_relationship_metadata_sanitized().
---
# Module: [`tests/test_scip_ingest.py`](../../../../../raw/code/graphify/tests/test_scip_ingest.py)

## Functions
- `_make_symbol_doc(symbol_id: str, kind: str, rels: list[object])` — [`L261`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L261) — Helper to build a minimal SCIP document with one symbol.
- `test_ambiguous_duplicate_target_across_docs_creates_stub()` — [`L1389`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1389) — When a target symbol is defined in 2+ documents AND the source is in a — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_build_scip_metadata_with_description()` — [`L950`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L950) — All three fields present when description is non-empty.
- `test_build_scip_metadata_without_description()` — [`L960`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L960) — scip_description is omitted when description is empty string.
- `test_document_entry_non_dict_is_skipped()` — [`L1287`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1287) — A non-dict entry in `documents` is silently skipped.
- `test_documentation_with_non_string_entries_is_ignored()` — [`L1260`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1260) — `documentation` first entry that isn't a string yields empty description (not crash). — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_documents_field_non_list_returns_empty()` — [`L1282`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1282) — `documents` as a non-list returns the empty result.
- `test_duplicate_local_symbol_resolves_to_same_document()` — [`L1324`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1324) — When two docs both have `F#`, a relationship from b.py's F# to F# must — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_duplicate_same_document_definition_does_not_create_false_ambiguity()` — [`L1543`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1543) — Duplicate symbol records within the SAME document collapse to one node id
- `test_ingest_default_source_file_is_empty_string()` — [`L657`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L657) — When no relative_path is given on document, source_file defaults to ''.
- `test_ingest_dict_without_documents_key()` — [`L26`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L26) — documents key not present → no processing → empty result. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_document_item_not_a_dict_is_skipped()` — [`L541`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L541) — Non-dict entries in the documents list are silently skipped.
- `test_ingest_document_relative_path_overrides_source_file_param()` — [`L687`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L687) — Document relative_path takes precedence over the source_file parameter. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_document_with_symbols_not_a_list()` — [`L631`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L631) — When symbols is not a list, that document is skipped.
- `test_ingest_document_without_language_defaults_to_function_param()` — [`L703`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L703) — When doc has no language field, uses the language function parameter.
- `test_ingest_document_without_symbols_key()` — [`L624`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L624) — Document dict without 'symbols' key is treated as empty list.
- `test_ingest_documents_empty_list()` — [`L38`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L38) — Empty documents list produces empty nodes and edges. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_documents_not_a_list_is_skipped()` — [`L32`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L32) — When documents is not a list, ingestion stops and returns empty. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_duplicate_edges_are_deduplicated()` — [`L386`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L386) — The same source→target→relation→location edge is only emitted once. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_duplicate_symbols_in_same_file_are_deduplicated()` — [`L501`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L501) — The same symbol appearing twice in a document yields only one node.
- `test_ingest_edge_source_location_from_first_occurrence()` — [`L423`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L423) — source_location on edges uses the line from the first occurrence range[0].
- `test_ingest_edge_structure_complete()` — [`L405`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L405) — Verify every field in the emitted edge dict. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_edge_with_zero_sourceline_has_empty_location()` — [`L992`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L992) — When sourceline is 0, source_location on edge is empty string. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_empty_doc_returns_empty_lists()` — [`L20`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L20) — Empty dict input produces empty nodes and edges.
- `test_ingest_is_definition_emits_scip_def_edge()` — [`L293`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L293) — is_definition → relation 'scip_def'. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_is_implementation_emits_scip_impl_edge()` — [`L304`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L304) — is_implementation → relation 'scip_impl' (takes priority over is_definition). — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_is_reference_emits_scip_ref_edge()` — [`L281`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L281) — is_reference → relation 'scip_ref'.
- `test_ingest_is_type_definition_emits_scip_typed_edge()` — [`L315`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L315) — is_type_definition → relation 'scip_typed'. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_many_symbols()` — [`L975`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L975) — Ingestion handles a large number of symbols gracefully.
- `test_ingest_multiple_documents()` — [`L231`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L231) — Symbols from multiple documents all become nodes.
- `test_ingest_multiple_relationships_on_one_symbol()` — [`L356`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L356) — A symbol with multiple relationships emits one edge per relationship.
- `test_ingest_multiple_symbols_in_one_document()` — [`L193`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L193) — Multiple symbols in a single document all become nodes.
- `test_ingest_node_id_contains_source_file_and_symbol_suffix()` — [`L448`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L448) — Node id is derived from source_file and symbol suffix.
- `test_ingest_node_id_differs_by_source_file()` — [`L474`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L474) — Same symbol in different files produces different node ids. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_node_id_is_deterministic()` — [`L462`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L462) — Same input produces the same node id. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_node_metadata_control_chars_stripped()` — [`L1612`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1612) — Control characters in SCIP description must not survive into the graph. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_node_metadata_html_escaped()` — [`L1585`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1585) — SCIP-supplied description must be HTML-escaped before reaching node — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_non_dict_input_returns_empty(bad_input: object)` — [`L535`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L535) — Non-dict inputs are guarded and return empty nodes/edges. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_relationship_item_not_a_dict_is_skipped()` — [`L603`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L603) — Non-dict entries in the relationships list are silently skipped.
- `test_ingest_relationship_metadata_sanitized()` — [`L1638`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1638) — SCIP relationship payloads embedded in edge metadata must be sanitized.
- `test_ingest_relationship_no_boolean_flags_defaults_to_ref()` — [`L345`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L345) — When none of is_* flags are set, relation defaults to 'scip_ref'. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_relationship_priority_order()` — [`L326`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L326) — Implementation > TypeDefinition > Definition > Reference. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_relationship_without_target_symbol_is_skipped()` — [`L372`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L372) — Relationship with empty or missing symbol field is ignored. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_single_symbol_no_relationships()` — [`L44`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L44) — A single symbol with no relationships yields one node and zero edges. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_source_file_falls_back_to_function_param()` — [`L672`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L672) — The source_file param provides a fallback when doc has no relative_path.
- `test_ingest_symbol_item_not_a_dict_is_skipped()` — [`L560`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L560) — Non-dict entries in the symbols list are silently skipped. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_symbol_trailing_hash_no_display_name_has_non_empty_label()` — [`L101`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L101) — Symbol ending with '#' and no display_name must produce a non-empty label. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_ingest_symbol_with_documentation_becomes_description()` — [`L790`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L790) — The first element of documentation[] becomes scip_description metadata.
- `test_ingest_symbol_with_empty_documentation_skips_description()` — [`L812`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L812) — When documentation[0] is empty string, scip_description is omitted.
- `test_ingest_symbol_with_non_dict_occurrence_is_skipped()` — [`L742`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L742) — Only the first occurrence is used; if it is not a dict, sourceline stays 0.
- `test_ingest_symbol_with_non_list_range_falls_back_to_zero()` — [`L769`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L769) — When range is not a list, sourceline stays 0 (empty source_location).
- `test_ingest_symbol_with_short_range_uses_first_element_as_line()` — [`L721`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L721) — A range list with exactly 2 elements (minimum required) sets sourceline from range[0].
- `test_ingest_symbol_without_display_name_uses_suffix()` — [`L80`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L80) — When display_name is missing, label falls back to the portion after #.
- `test_ingest_symbol_without_documentation_omits_description()` — [`L834`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L834) — When documentation key is missing, scip_description is not in metadata.
- `test_ingest_symbol_without_hash_uses_full_symbol_as_label()` — [`L131`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L131) — When symbol has no #, the label is the full symbol id.
- `test_ingest_symbol_without_kind_defaults_to_unknown()` — [`L638`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L638) — When kind is missing, metadata uses 'unknown'.
- `test_ingest_symbol_without_occurrences_has_empty_source_location()` — [`L152`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L152) — When occurrences list is empty, source_location is empty string.
- `test_ingest_symbol_without_occurrences_key()` — [`L173`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L173) — When occurrences key is missing entirely, falls back to empty source_location.
- `test_ingest_symbol_without_relationships_key_still_creates_node()` — [`L855`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L855) — Missing relationships key — symbol still becomes a node.
- `test_ingest_symbol_without_symbol_id_is_skipped()` — [`L586`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L586) — A symbol dict with empty or missing 'symbol' field produces no node.
- `test_make_scip_node_id_deterministic()` — [`L899`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L899) — Same inputs always produce the same id.
- `test_make_scip_node_id_empty_after_sanitisation_falls_back()` — [`L920`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L920) — If sanitised suffix is empty, uses just the hash.
- `test_make_scip_node_id_source_file_affects_hash()` — [`L906`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L906) — Different source_file produces different hash.
- `test_make_scip_node_id_special_characters_are_sanitised()` — [`L892`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L892) — Non-alphanumeric characters are replaced with underscores.
- `test_make_scip_node_id_symbol_affects_hash()` — [`L913`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L913) — Different symbol produces different hash.
- `test_make_scip_node_id_with_hash_separator()` — [`L875`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L875) — Symbol with # uses suffix after last #.
- `test_make_scip_node_id_without_hash()` — [`L885`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L885) — Symbol without # uses the full symbol (sanitised) as suffix.
- `test_non_string_display_name_falls_back()` — [`L1245`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1245) — `display_name` as a non-string falls back to the symbol suffix.
- `test_non_string_kind_falls_back_to_unknown()` — [`L1231`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1231) — A symbol with `kind` as a non-string falls back to 'unknown'.
- `test_non_string_language_falls_back()` — [`L1157`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1157) — `language` as a non-string falls back to the function default.
- `test_non_string_relative_path_falls_back_to_default()` — [`L1143`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1143) — `relative_path` as a non-string falls back to the function's source_file default.
- `test_non_string_symbol_id_is_skipped()` — [`L1173`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1173) — A symbol entry with `symbol: <int>` is silently skipped.
- `test_occurrence_bool_line_falls_back_to_zero()` — [`L1522`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1522) — range[0] = True (which is technically an int subclass) must not produce 'LTrue'.
- `test_occurrence_negative_line_falls_back_to_zero()` — [`L1299`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1299) — An occurrence with a negative line number resolves source_location to empty.
- `test_relationship_boolean_true_routes_correctly()` — [`L1488`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1488) — Actual boolean True still routes to the corresponding scip_ relation.
- `test_relationship_edges_survive_validate_extraction_and_build()` — [`L1105`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1105) — Result passes Graphify's validate_extraction and build_from_json keeps the edges. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `test_relationship_int_flag_is_ignored()` — [`L1462`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1462) — `"is_implementation": 1` is truthy but not True — must not route to scip_impl.
- `test_relationship_symbol_non_string_is_skipped()` — [`L1206`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1206) — A relationship entry whose `symbol` is a non-string is silently skipped.
- `test_relationship_target_across_documents_resolves_via_index()` — [`L1044`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1044) — Cross-document relationship resolves to the target document's node id.
- `test_relationship_target_in_same_document_resolves_via_index()` — [`L1018`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1018) — Cross-symbol relationship within ONE document resolves via the symbol index.
- `test_relationship_target_unknown_emits_stub_node()` — [`L1076`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1076) — A relationship targeting a symbol NOT in any document creates a stub external node.
- `test_relationship_truthy_string_flag_is_ignored()` — [`L1435`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1435) — `"is_implementation": "false"` is a truthy STRING — must not route to
- `test_relationships_none_is_treated_as_empty()` — [`L1191`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1191) — A symbol with `relationships: None` ingests without error and emits no edges.
- `test_scip_kind_to_file_type_always_code()` — [`L936`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L936) — Any kind string maps to 'code'.
- `test_unique_cross_document_symbol_still_resolves()` — [`L1359`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1359) — When a target symbol is defined in exactly ONE other document, the edge
- `test_unrecognized_top_level_structure_returns_empty()` — [`L1275`](../../../../../raw/code/graphify/tests/test_scip_ingest.py#L1275) — Top-level non-dict shapes still return the empty result.

