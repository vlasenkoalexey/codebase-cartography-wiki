---
title: 'Module: tests/tools_recorders/test_llm_recorder.py'
type: catalog
provenance: extracted
module: tests/tools_recorders/test_llm_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.tools_recorders.test_llm_recorder`/
symbols:
  recorder: recorder().
  mock_pipeline_state: mock_pipeline_state().
  test_parse_threat_score: test_parse_threat_score().
  test_build_markdown_generates_context: test_build_markdown_generates_context().
  test_generate_sqlite_graph: test_generate_sqlite_graph().
  test_llm_recorder_empty_state: test_llm_recorder_empty_state().
  test_generate_artifacts_integration: test_generate_artifacts_integration().
---
# Module: [`tests/tools_recorders/test_llm_recorder.py`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py)

## Functions
- `mock_pipeline_state()` — [`L24`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L24) — Provides a comprehensive, standardized pipeline state for the recorder to consume.
- `recorder()` — [`L9`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L9) — Initializes the LLMRecorder with a controlled schema for deterministic testing.
- `test_build_markdown_generates_context(recorder, mock_pipeline_state)` — [`L162`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L162) — Proves the Markdown builder successfully weaves data into LLM context chunks.
- `test_generate_artifacts_integration(recorder, mock_pipeline_state, tmp_path)` — [`L269`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L269) — Proves the main entry point orchestrates both artifact generation sequences.
- `test_generate_sqlite_graph(recorder, mock_pipeline_state, tmp_path)` — [`L192`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L192) — Proves the SQLite builder correctly provisions tables and inserts schema-aligned data.
- `test_llm_recorder_empty_state(recorder, tmp_path)` — [`L241`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L241) — Proves the generator survives an empty repository without math/division errors.
- `test_parse_threat_score(recorder)` — [`L148`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_llm_recorder.py#L148) — Proves the string-to-float conversion for ML Threat Scores is fault-tolerant.

