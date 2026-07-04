---
title: 'Module: tests/tools_recorders/test_gpu_recorder.py'
type: catalog
provenance: extracted
module: tests/tools_recorders/test_gpu_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.tools_recorders.test_gpu_recorder`/
symbols:
  recorder: recorder().
  mock_pipeline_state: mock_pipeline_state().
  test_destructive_ram_eviction: test_destructive_ram_eviction().
  test_string_interning_compression: test_string_interning_compression().
  test_dependency_edge_mapping: test_dependency_edge_mapping().
  test_ai_threat_score_quantization: test_ai_threat_score_quantization().
  test_function_csr_flattening: test_function_csr_flattening().
---
# Module: [`tests/tools_recorders/test_gpu_recorder.py`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py)

## Functions
- `mock_pipeline_state()` — [`L10`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L10) — Provides a standardized pipeline state for testing the columnar pivot.
- `recorder()` — [`L5`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L5) — Initializes the GPURecorder for WebGL payload generation testing.
- `test_ai_threat_score_quantization(recorder, mock_pipeline_state)` — [`L155`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L155) — Proves that XGBoost AI Threat Scores are safely stripped of their percentage
- `test_dependency_edge_mapping(recorder, mock_pipeline_state)` — [`L128`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L128) — Proves that inbound and outbound edges are perfectly mapped,
- `test_destructive_ram_eviction(recorder, mock_pipeline_state)` — [`L72`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L72) — Verifies Stage 3.3: Destructive RAM Eviction.
- `test_function_csr_flattening(recorder, mock_pipeline_state)` — [`L175`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L175) — Proves the nested functions dictionary is correctly flattened into the
- `test_string_interning_compression(recorder, mock_pipeline_state)` — [`L104`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_gpu_recorder.py#L104) — Proves that repetitive strings (like languages and authors) are correctly

