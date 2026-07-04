---
title: 'Module: tests/test_pipeline.py'
type: catalog
provenance: extracted
module: tests/test_pipeline.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_pipeline`/
symbols:
  run_pipeline: run_pipeline().
  test_pipeline_runs_end_to_end: test_pipeline_runs_end_to_end().
  test_pipeline_graph_has_edges: test_pipeline_graph_has_edges().
  test_pipeline_all_nodes_have_community: test_pipeline_all_nodes_have_community().
  test_pipeline_report_mentions_top_god_node: test_pipeline_report_mentions_top_god_node().
  test_pipeline_detection_finds_code_and_docs: test_pipeline_detection_finds_code_and_docs().
  test_pipeline_incremental_update: test_pipeline_incremental_update().
  test_pipeline_extraction_confidence_labels: test_pipeline_extraction_confidence_labels().
  test_pipeline_no_self_loops: test_pipeline_no_self_loops().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_pipeline.py`](../../../../../raw/code/graphify/tests/test_pipeline.py)

## Functions
- `run_pipeline(tmp_path: Path)` — [`L23`](../../../../../raw/code/graphify/tests/test_pipeline.py#L23) — Run the full pipeline on the fixtures directory. Returns a dict of outputs.
- `test_pipeline_all_nodes_have_community(tmp_path)` — [`L117`](../../../../../raw/code/graphify/tests/test_pipeline.py#L117)
- `test_pipeline_detection_finds_code_and_docs(tmp_path)` — [`L132`](../../../../../raw/code/graphify/tests/test_pipeline.py#L132)
- `test_pipeline_extraction_confidence_labels(tmp_path)` — [`L146`](../../../../../raw/code/graphify/tests/test_pipeline.py#L146)
- `test_pipeline_graph_has_edges(tmp_path)` — [`L112`](../../../../../raw/code/graphify/tests/test_pipeline.py#L112)
- `test_pipeline_incremental_update(tmp_path)` — [`L138`](../../../../../raw/code/graphify/tests/test_pipeline.py#L138) — Second run on unchanged corpus should produce identical node/edge counts.
- `test_pipeline_no_self_loops(tmp_path)` — [`L154`](../../../../../raw/code/graphify/tests/test_pipeline.py#L154)
- `test_pipeline_report_mentions_top_god_node(tmp_path)` — [`L126`](../../../../../raw/code/graphify/tests/test_pipeline.py#L126)
- `test_pipeline_runs_end_to_end(tmp_path)` — [`L107`](../../../../../raw/code/graphify/tests/test_pipeline.py#L107)

## Module values
- `FIXTURES` — [`L20`](../../../../../raw/code/graphify/tests/test_pipeline.py#L20)

