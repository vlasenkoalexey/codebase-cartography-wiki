---
title: 'Module: tests/test_semantic_similarity.py'
type: catalog
provenance: extracted
module: tests/test_semantic_similarity.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_semantic_similarity`/
symbols:
  _make_graph_with_semantic_edge: _make_graph_with_semantic_edge().
  _make_report_with_semantic_surprise: _make_report_with_semantic_surprise().
  test_semantic_edge_scores_higher_than_references: test_semantic_edge_scores_higher_than_references().
  test_semantic_edge_reason_mentions_similarity: test_semantic_edge_reason_mentions_similarity().
  test_semantic_edge_survives_build_from_json: test_semantic_edge_survives_build_from_json().
  test_semantic_edge_nodes_present: test_semantic_edge_nodes_present().
  test_semantic_edge_confidence_score_preserved: test_semantic_edge_confidence_score_preserved().
  test_report_renders_semantically_similar_tag: test_report_renders_semantically_similar_tag().
  test_report_semantic_tag_on_correct_line: test_report_semantic_tag_on_correct_line().
  test_report_no_semantic_tag_for_other_relations: test_report_no_semantic_tag_for_other_relations().
  _make_two_edge_graph: _make_two_edge_graph().
  _make_extraction_with_semantic_edge: _make_extraction_with_semantic_edge().
---
# Module: [`tests/test_semantic_similarity.py`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py)

## Functions
- `_make_extraction_with_semantic_edge()` — [`L13`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L13) — Two nodes in separate files connected by a semantically_similar_to edge.
- `_make_graph_with_semantic_edge()` — [`L39`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L39)
- `_make_report_with_semantic_surprise()` — [`L129`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L129)
- `_make_two_edge_graph()` — [`L43`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L43) — Graph with one semantically_similar_to edge and one references edge, both cross-file.
- `test_report_no_semantic_tag_for_other_relations()` — [`L166`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L166) — Non-semantic edges must not get the [semantically similar] tag.
- `test_report_renders_semantically_similar_tag()` — [`L151`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L151)
- `test_report_semantic_tag_on_correct_line()` — [`L156`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L156)
- `test_semantic_edge_confidence_score_preserved()` — [`L85`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L85)
- `test_semantic_edge_nodes_present()` — [`L75`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L75)
- `test_semantic_edge_reason_mentions_similarity()` — [`L113`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L113)
- `test_semantic_edge_scores_higher_than_references()` — [`L97`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L97)
- `test_semantic_edge_survives_build_from_json()` — [`L68`](../../../../../raw/code/graphify/tests/test_semantic_similarity.py#L68)

