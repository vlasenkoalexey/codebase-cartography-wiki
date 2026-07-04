---
title: 'Module: tests/test_semantic_cleanup.py'
type: catalog
provenance: extracted
module: tests/test_semantic_cleanup.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_semantic_cleanup`/
symbols:
  _valid_fragment: _valid_fragment().
  test_validate_semantic_fragment_accepts_valid: test_validate_semantic_fragment_accepts_valid().
  test_validate_semantic_fragment_rejects_oversize_payload: test_validate_semantic_fragment_rejects_oversize_payload().
  test_validate_semantic_fragment_rejects_too_many_nodes: test_validate_semantic_fragment_rejects_too_many_nodes().
  test_validate_semantic_fragment_rejects_too_many_edges: test_validate_semantic_fragment_rejects_too_many_edges().
  test_validate_semantic_fragment_rejects_path_separator_in_id: test_validate_semantic_fragment_rejects_path_separator_in_id().
  test_validate_semantic_fragment_rejects_invalid_file_type: test_validate_semantic_fragment_rejects_invalid_file_type().
  test_validate_semantic_fragment_accepts_rationale_file_type: test_validate_semantic_fragment_accepts_rationale_file_type().
  test_validate_semantic_fragment_accepts_concept_file_type: test_validate_semantic_fragment_accepts_concept_file_type().
  test_load_validated_semantic_fragment_accepts_valid: test_load_validated_semantic_fragment_accepts_valid().
  test_validate_hyperedge_rejects_bad_id: test_validate_hyperedge_rejects_bad_id().
  test_validate_hyperedge_rejects_bad_node_ref: test_validate_hyperedge_rejects_bad_node_ref().
  test_validate_hyperedge_requires_list: test_validate_hyperedge_requires_list().
  test_validate_hyperedge_caps_count: test_validate_hyperedge_caps_count().
  test_validate_accepts_node_ids_keyed_hyperedge: test_validate_accepts_node_ids_keyed_hyperedge().
  test_validate_semantic_fragment_rejects_non_object: test_validate_semantic_fragment_rejects_non_object().
  test_load_validated_semantic_fragment_rejects_oversize_before_parse: test_load_validated_semantic_fragment_rejects_oversize_before_parse().
  test_load_validated_semantic_fragment_rejects_invalid_json: test_load_validated_semantic_fragment_rejects_invalid_json().
  test_sanitize_drops_rationale_filetype_node: test_sanitize_drops_rationale_filetype_node().
  test_sanitize_converts_sentence_rationale_node_to_attribute: test_sanitize_converts_sentence_rationale_node_to_attribute().
  test_sanitize_converts_allowed_filetype_sentence_via_rationale_for_edge: test_sanitize_converts_allowed_filetype_sentence_via_rationale_for_edge().
  test_sanitize_keeps_short_concept_named_node_with_punctuation: test_sanitize_keeps_short_concept_named_node_with_punctuation().
  test_sanitize_filters_hyperedges_after_node_removal: test_sanitize_filters_hyperedges_after_node_removal().
  test_sanitize_drops_hyperedge_with_only_unknown_refs: test_sanitize_drops_hyperedge_with_only_unknown_refs().
  test_sanitize_boundary_sentence_threshold: test_sanitize_boundary_sentence_threshold().
  test_sanitize_rationale_only_propagates_through_rationale_for_edges: test_sanitize_rationale_only_propagates_through_rationale_for_edges().
  test_sanitize_keeps_members_keyed_hyperedge: test_sanitize_keeps_members_keyed_hyperedge().
---
# Module: [`tests/test_semantic_cleanup.py`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py)

## Functions
- `_valid_fragment()` — [`L8`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L8)
- `test_load_validated_semantic_fragment_accepts_valid(tmp_path)` — [`L82`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L82)
- `test_load_validated_semantic_fragment_rejects_invalid_json(tmp_path)` — [`L101`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L101) — Invalid JSON returns an error instead of raising.
- `test_load_validated_semantic_fragment_rejects_oversize_before_parse(tmp_path, monkeypatch)` — [`L90`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L90) — Oversize files are rejected by stat() — payload is never parsed.
- `test_sanitize_boundary_sentence_threshold()` — [`L279`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L279) — Boundary: a label with exactly 8 words + colon is sentence-like;
- `test_sanitize_converts_allowed_filetype_sentence_via_rationale_for_edge()` — [`L192`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L192) — F3: a node with file_type='document' (allowed) that is BOTH sentence-like
- `test_sanitize_converts_sentence_rationale_node_to_attribute()` — [`L171`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L171) — Sentence-like rationale node connected via `rationale_for` → attribute on target.
- `test_sanitize_drops_hyperedge_with_only_unknown_refs()` — [`L268`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L268) — A hyperedge referencing only nodes not present in the fragment is dropped.
- `test_sanitize_drops_rationale_filetype_node()` — [`L155`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L155) — A node with file_type='rationale' is removed wholesale.
- `test_sanitize_filters_hyperedges_after_node_removal()` — [`L233`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L233) — F4: hyperedges referencing removed nodes are repaired or dropped.
- `test_sanitize_keeps_members_keyed_hyperedge(capsys)` — [`L347`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L347) — #1561: a `members`-keyed hyperedge with >=2 surviving members must be
- `test_sanitize_keeps_short_concept_named_node_with_punctuation()` — [`L217`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L217) — A short named node with a period (e.g. abbreviation) is NOT sentence-like.
- `test_sanitize_rationale_only_propagates_through_rationale_for_edges()` — [`L314`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L314) — A rationale node connected to ONE target via `rationale_for` and to ANOTHER
- `test_validate_accepts_node_ids_keyed_hyperedge()` — [`L368`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L368) — #1561: an alias-keyed hyperedge must not be rejected for a missing
- `test_validate_hyperedge_caps_count(monkeypatch)` — [`L140`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L140)
- `test_validate_hyperedge_rejects_bad_id()` — [`L115`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L115)
- `test_validate_hyperedge_rejects_bad_node_ref()` — [`L124`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L124)
- `test_validate_hyperedge_requires_list()` — [`L133`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L133)
- `test_validate_semantic_fragment_accepts_concept_file_type()` — [`L72`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L72) — LLM output with file_type='concept' must pass validation for the same reason.
- `test_validate_semantic_fragment_accepts_rationale_file_type()` — [`L61`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L61) — LLM output with file_type='rationale' must pass validation so the cleanup
- `test_validate_semantic_fragment_accepts_valid()` — [`L16`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L16)
- `test_validate_semantic_fragment_rejects_invalid_file_type()` — [`L54`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L54)
- `test_validate_semantic_fragment_rejects_non_object()` — [`L20`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L20)
- `test_validate_semantic_fragment_rejects_oversize_payload(monkeypatch)` — [`L25`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L25)
- `test_validate_semantic_fragment_rejects_path_separator_in_id()` — [`L47`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L47)
- `test_validate_semantic_fragment_rejects_too_many_edges(monkeypatch)` — [`L41`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L41)
- `test_validate_semantic_fragment_rejects_too_many_nodes(monkeypatch)` — [`L33`](../../../../../raw/code/graphify/tests/test_semantic_cleanup.py#L33)

