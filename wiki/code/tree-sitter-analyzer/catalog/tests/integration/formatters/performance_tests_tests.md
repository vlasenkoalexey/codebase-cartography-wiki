---
title: 'Module: tests/integration/formatters/performance_tests_tests.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/performance_tests_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.performance_tests_tests`/TestPerformance
symbols:
  TestPerformanceMetrics.test_metrics_creation: Metrics#test_metrics_creation().
  TestPerformanceMetrics.test_metrics_with_error: Metrics#test_metrics_with_error().
  TestPerformanceProfiler.test_start_profiling_resets_baseline: Profiler#test_start_profiling_resets_baseline().
  TestPerformanceProfiler.test_start_stop_profiling: Profiler#test_start_stop_profiling().
  TestPerformanceProfiler.test_stop_without_start_raises: Profiler#test_stop_without_start_raises().
  TestPerformanceTesterHelpers.test_estimate_element_count_with_list: TesterHelpers#test_estimate_element_count_with_list().
  TestPerformanceTesterHelpers.test_estimate_element_count_with_string: TesterHelpers#test_estimate_element_count_with_string().
  TestPerformanceTesterHelpers.test_estimate_element_count_with_scalar: TesterHelpers#test_estimate_element_count_with_scalar().
  TestPerformanceTesterHelpers.test_calculate_scalability_factor_single: TesterHelpers#test_calculate_scalability_factor_single().
  TestPerformanceTesterHelpers.test_calculate_scalability_factor_linear: TesterHelpers#test_calculate_scalability_factor_linear().
  TestPerformanceProfiler: Profiler#
  TestPerformanceMetrics: Metrics#
  TestPerformanceTesterHelpers: TesterHelpers#
---
# Module: [`tests/integration/formatters/performance_tests_tests.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py)

## Classes
### `TestPerformanceMetrics`
- def: [`tests/integration/formatters/performance_tests_tests.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L41)
- doc: Tests for PerformanceMetrics dataclass.
- signature: `class TestPerformanceMetrics:`
- members:
  - `test_metrics_creation(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L44)
  - `test_metrics_with_error(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L65)
- uses (calls/refs, reference-scoped): (13 test-only callers)

### `TestPerformanceProfiler`
- def: [`tests/integration/formatters/performance_tests_tests.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L17)
- doc: Tests for PerformanceProfiler.
- signature: `class TestPerformanceProfiler:`
- members:
  - `test_start_profiling_resets_baseline(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L34)
  - `test_start_stop_profiling(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L20)
  - `test_stop_without_start_raises(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L29)
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestPerformanceTesterHelpers`
- def: [`tests/integration/formatters/performance_tests_tests.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L86)
- doc: Tests for PerformanceTester helper methods.
- signature: `class TestPerformanceTesterHelpers:`
- members:
  - `test_calculate_scalability_factor_linear(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L107)
  - `test_calculate_scalability_factor_single(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L103)
  - `test_estimate_element_count_with_list(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L89)
  - `test_estimate_element_count_with_scalar(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L99)
  - `test_estimate_element_count_with_string(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_tests.py#L93)
- uses (calls/refs, reference-scoped): (3 test-only callers)

