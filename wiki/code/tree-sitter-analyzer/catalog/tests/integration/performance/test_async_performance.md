---
title: 'Module: tests/integration/performance/test_async_performance.py'
type: catalog
provenance: extracted
module: tests/integration/performance/test_async_performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.performance.test_async_performance`/test_
symbols:
  test_parser_cache_impact_on_queries: parser_cache_impact_on_queries().
  test_event_loop_responsiveness: event_loop_responsiveness().
  test_concurrent_analysis_performance: concurrent_analysis_performance().
  test_parser_cache_effectiveness: parser_cache_effectiveness().
  test_cache_invalidation_on_file_change: cache_invalidation_on_file_change().
  test_event_loop_responsiveness.heartbeat: event_loop_responsiveness().heartbeat().
---
# Module: [`tests/integration/performance/test_async_performance.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py)

## Functions
- `heartbeat()` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L87)
- `test_cache_invalidation_on_file_change(tmp_path)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L115) — Verify that changing the file invalidates the result cache.
- `test_concurrent_analysis_performance(tmp_path)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L13) — Measure performance of concurrent analysis.
- `test_event_loop_responsiveness(tmp_path)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L73) — Verify that the event loop remains responsive during analysis.
- `test_parser_cache_effectiveness(tmp_path)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L44) — Verify that repeated requests for the same file are faster due to caching.
- `test_parser_cache_impact_on_queries(tmp_path)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_async_performance.py#L144) — Verify that query execution doesn't cause redundant parsing hits if already parsed.

