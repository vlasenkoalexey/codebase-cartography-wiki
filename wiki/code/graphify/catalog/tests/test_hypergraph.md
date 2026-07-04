---
title: 'Module: tests/test_hypergraph.py'
type: catalog
provenance: extracted
module: tests/test_hypergraph.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_hypergraph`/
symbols:
  SAMPLE_EXTRACTION: SAMPLE_EXTRACTION.
  test_hyperedges_roundtrip_via_json_file: test_hyperedges_roundtrip_via_json_file().
  _make_report: _make_report().
  test_build_from_json_stores_hyperedges: test_build_from_json_stores_hyperedges().
  test_build_from_json_no_hyperedges: test_build_from_json_no_hyperedges().
  test_build_from_json_missing_hyperedges_key: test_build_from_json_missing_hyperedges_key().
  test_to_json_includes_hyperedges: test_to_json_includes_hyperedges().
  test_to_json_hyperedges_empty_when_none: test_to_json_hyperedges_empty_when_none().
  test_report_includes_hyperedges_section: test_report_includes_hyperedges_section().
  test_report_includes_hyperedge_node_list: test_report_includes_hyperedge_node_list().
  test_report_skips_hyperedges_section_when_empty: test_report_skips_hyperedges_section_when_empty().
  test_report_skips_hyperedges_section_when_key_missing: test_report_skips_hyperedges_section_when_key_missing().
  test_build_normalizes_member_aliases_to_nodes: test_build_normalizes_member_aliases_to_nodes().
  test_build_from_json_relativizes_hyperedge_source_file: test_build_from_json_relativizes_hyperedge_source_file().
  test_attach_hyperedges_adds_new: test_attach_hyperedges_adds_new().
  test_attach_hyperedges_deduplicates: test_attach_hyperedges_deduplicates().
  test_attach_hyperedges_multiple_different_ids: test_attach_hyperedges_multiple_different_ids().
  test_attach_hyperedges_skips_entry_without_id: test_attach_hyperedges_skips_entry_without_id().
  test_build_dedups_alias_members_preserving_order: test_build_dedups_alias_members_preserving_order().
  test_build_canonical_nodes_wins_over_alias: test_build_canonical_nodes_wins_over_alias().
  test_build_rekeys_alias_keyed_hyperedge_members: test_build_rekeys_alias_keyed_hyperedge_members().
  test_build_warns_once_per_aliased_hyperedge: test_build_warns_once_per_aliased_hyperedge().
  _alias_extraction: _alias_extraction().
  SAMPLE_DETECTION: SAMPLE_DETECTION.
---
# Module: [`tests/test_hypergraph.py`](../../../../../raw/code/graphify/tests/test_hypergraph.py)

## Functions
- `_alias_extraction()` — [`L242`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L242) — Three hyperedges, one per member-key spelling: nodes / members / node_ids.
- `_make_report(G)` — [`L195`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L195)
- `test_attach_hyperedges_adds_new()` — [`L111`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L111)
- `test_attach_hyperedges_deduplicates()` — [`L117`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L117)
- `test_attach_hyperedges_multiple_different_ids()` — [`L125`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L125)
- `test_attach_hyperedges_skips_entry_without_id()` — [`L134`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L134)
- `test_build_canonical_nodes_wins_over_alias()` — [`L283`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L283)
- `test_build_dedups_alias_members_preserving_order()` — [`L269`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L269)
- `test_build_from_json_missing_hyperedges_key()` — [`L101`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L101)
- `test_build_from_json_no_hyperedges()` — [`L95`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L95)
- `test_build_from_json_relativizes_hyperedge_source_file(tmp_path)` — [`L65`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L65) — build_from_json(root=...) must relativize hyperedge source_file like it
- `test_build_from_json_stores_hyperedges()` — [`L58`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L58)
- `test_build_normalizes_member_aliases_to_nodes()` — [`L259`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L259)
- `test_build_rekeys_alias_keyed_hyperedge_members()` — [`L301`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L301) — Alias normalization must run BEFORE the semantic id-remap loop so a
- `test_build_warns_once_per_aliased_hyperedge(capsys)` — [`L321`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L321)
- `test_hyperedges_roundtrip_via_json_file()` — [`L172`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L172) — Write graph.json then reload it - hyperedges must survive. — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_report_includes_hyperedge_node_list()` — [`L212`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L212)
- `test_report_includes_hyperedges_section()` — [`L204`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L204)
- `test_report_skips_hyperedges_section_when_empty()` — [`L224`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L224)
- `test_report_skips_hyperedges_section_when_key_missing()` — [`L231`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L231)
- `test_to_json_hyperedges_empty_when_none()` — [`L156`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L156)
- `test_to_json_includes_hyperedges()` — [`L144`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L144)

## Module values
- `SAMPLE_DETECTION` — [`L45`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L45)
- `SAMPLE_EXTRACTION` — [`L19`](../../../../../raw/code/graphify/tests/test_hypergraph.py#L19)

