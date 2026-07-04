---
title: 'Module: tests/test_confidence.py'
type: catalog
provenance: extracted
module: tests/test_confidence.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_confidence`/
symbols:
  test_report_shows_avg_confidence_for_inferred: test_report_shows_avg_confidence_for_inferred().
  test_report_inferred_tag_with_score: test_report_inferred_tag_with_score().
  test_confidence_score_round_trip: test_confidence_score_round_trip().
  test_to_json_defaults_missing_confidence_score: test_to_json_defaults_missing_confidence_score().
  _make_extraction: _make_extraction().
  test_extracted_edges_have_score_1: test_extracted_edges_have_score_1().
  test_inferred_edges_score_in_range: test_inferred_edges_score_in_range().
  test_ambiguous_edges_score_at_most_04: test_ambiguous_edges_score_at_most_04().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_confidence.py`](../../../../../raw/code/graphify/tests/test_confidence.py)

## Functions
- `_make_extraction(**edge_overrides)` — [`L17`](../../../../../raw/code/graphify/tests/test_confidence.py#L17) — Return a minimal extraction dict with one edge of each confidence type.
- `test_ambiguous_edges_score_at_most_04()` — [`L65`](../../../../../raw/code/graphify/tests/test_confidence.py#L65) — AMBIGUOUS edges must have confidence_score <= 0.4.
- `test_confidence_score_round_trip()` — [`L80`](../../../../../raw/code/graphify/tests/test_confidence.py#L80) — confidence_score survives build_from_json → to_json → JSON parse round-trip. — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_extracted_edges_have_score_1()` — [`L40`](../../../../../raw/code/graphify/tests/test_confidence.py#L40) — EXTRACTED edges must have confidence_score == 1.0.
- `test_inferred_edges_score_in_range()` — [`L50`](../../../../../raw/code/graphify/tests/test_confidence.py#L50) — INFERRED edges must have confidence_score between 0.0 and 1.0.
- `test_report_inferred_tag_with_score()` — [`L154`](../../../../../raw/code/graphify/tests/test_confidence.py#L154) — Surprising connections section shows confidence score next to INFERRED edges.
- `test_report_shows_avg_confidence_for_inferred()` — [`L136`](../../../../../raw/code/graphify/tests/test_confidence.py#L136) — Report summary line should include avg confidence for INFERRED edges.
- `test_to_json_defaults_missing_confidence_score()` — [`L101`](../../../../../raw/code/graphify/tests/test_confidence.py#L101) — Edges lacking confidence_score get sensible defaults in to_json.

## Module values
- `FIXTURES` — [`L14`](../../../../../raw/code/graphify/tests/test_confidence.py#L14)

