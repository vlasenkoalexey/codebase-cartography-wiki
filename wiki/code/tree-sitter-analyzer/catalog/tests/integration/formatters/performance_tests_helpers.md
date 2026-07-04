---
title: 'Module: tests/integration/formatters/performance_tests_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/performance_tests_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.performance_tests_helpers`/
symbols:
  PerformanceTester.run_performance_test: PerformanceTester#run_performance_test().
  PerformanceTester.run_scalability_test: PerformanceTester#run_scalability_test().
  PerformanceTester.run_concurrent_performance_test: PerformanceTester#run_concurrent_performance_test().
  PerformanceTester.create_baseline: PerformanceTester#create_baseline().
  PerformanceTester.check_performance_regression: PerformanceTester#check_performance_regression().
  PerformanceTester.update_baseline: PerformanceTester#update_baseline().
  PerformanceTester.generate_performance_report: PerformanceTester#generate_performance_report().
  PerformanceMetrics: PerformanceMetrics#
  PerformanceMetrics.execution_time_ms: PerformanceMetrics#execution_time_ms.
  PerformanceMetrics.memory_usage_mb: PerformanceMetrics#memory_usage_mb.
  PerformanceMetrics.success: PerformanceMetrics#success.
  PerformanceProfiler.start_profiling: PerformanceProfiler#start_profiling().
  PerformanceProfiler.stop_profiling: PerformanceProfiler#stop_profiling().
  PerformanceTester.baselines: PerformanceTester#baselines.
  FormatPerformanceTester.benchmark_format_comparison: FormatPerformanceTester#benchmark_format_comparison().
  FormatPerformanceTester.test_format_performance: FormatPerformanceTester#test_format_performance().
  FormatPerformanceTester.test_format_scalability: FormatPerformanceTester#test_format_scalability().
  PerformanceTester.results_dir: PerformanceTester#results_dir.
  PerformanceMetrics.throughput_ops_per_sec: PerformanceMetrics#throughput_ops_per_sec.
  PerformanceMetrics.format_type: PerformanceMetrics#format_type.
  PerformanceTester.load_baselines: PerformanceTester#load_baselines().
  PerformanceTester._save_scalability_results: PerformanceTester#_save_scalability_results().
  PerformanceMetrics.test_name: PerformanceMetrics#test_name.
  PerformanceMetrics.timestamp: PerformanceMetrics#timestamp.
  PerformanceTester: PerformanceTester#
  PerformanceTester.save_baselines: PerformanceTester#save_baselines().
  PerformanceMetrics.peak_memory_mb: PerformanceMetrics#peak_memory_mb.
  PerformanceMetrics.cpu_usage_percent: PerformanceMetrics#cpu_usage_percent.
  PerformanceMetrics.file_size_bytes: PerformanceMetrics#file_size_bytes.
  PerformanceMetrics.element_count: PerformanceMetrics#element_count.
  PerformanceBaseline.baseline_memory_mb: PerformanceBaseline#baseline_memory_mb.
  PerformanceTester._save_performance_results: PerformanceTester#_save_performance_results().
  PerformanceTester._load_all_performance_results: PerformanceTester#_load_all_performance_results().
  PerformanceMetrics.error_message: PerformanceMetrics#error_message.
  PerformanceBaseline.baseline_time_ms: PerformanceBaseline#baseline_time_ms.
  PerformanceProfiler: PerformanceProfiler#
  PerformanceTester.profiler: PerformanceTester#profiler.
  ScalabilityTestResult: ScalabilityTestResult#
  PerformanceBaseline.acceptable_variance_percent: PerformanceBaseline#acceptable_variance_percent.
  PerformanceProfiler.start_time: PerformanceProfiler#start_time.
  PerformanceProfiler.tracemalloc_started: PerformanceProfiler#tracemalloc_started.
  PerformanceTester._estimate_element_count: PerformanceTester#_estimate_element_count().
  FormatPerformanceTester: FormatPerformanceTester#
  PerformanceBaseline: PerformanceBaseline#
  PerformanceProfiler.process: PerformanceProfiler#process.
  PerformanceProfiler.baseline_memory: PerformanceProfiler#baseline_memory.
  PerformanceTester._calculate_scalability_factor: PerformanceTester#_calculate_scalability_factor().
  FormatPerformanceTester.__init__: FormatPerformanceTester#__init__().
  ScalabilityTestResult.test_name: ScalabilityTestResult#test_name.
  PerformanceBaseline.last_updated: PerformanceBaseline#last_updated.
  FormatPerformanceTester.performance_tester: FormatPerformanceTester#performance_tester.
  FormatPerformanceTester.test_function: FormatPerformanceTester#test_function().
  ScalabilityTestResult.input_sizes: ScalabilityTestResult#input_sizes.
  ScalabilityTestResult.execution_times: ScalabilityTestResult#execution_times.
  ScalabilityTestResult.memory_usages: ScalabilityTestResult#memory_usages.
  ScalabilityTestResult.throughput_rates: ScalabilityTestResult#throughput_rates.
  ScalabilityTestResult.scalability_factor: ScalabilityTestResult#scalability_factor.
  ScalabilityTestResult.performance_threshold_exceeded: ScalabilityTestResult#performance_threshold_exceeded.
  ScalabilityTestResult.timestamp: ScalabilityTestResult#timestamp.
  PerformanceBaseline.test_name: PerformanceBaseline#test_name.
  PerformanceBaseline.created_timestamp: PerformanceBaseline#created_timestamp.
  PerformanceProfiler.__init__: PerformanceProfiler#__init__().
  PerformanceTester.__init__: PerformanceTester#__init__().
---
# Module: [`tests/integration/formatters/performance_tests_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py)

## Classes
### `FormatPerformanceTester`
- def: [`tests/integration/formatters/performance_tests_helpers.py:621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L621)
- doc: Specialized performance tester for format operations
- signature: `class FormatPerformanceTester:`
- members:
  - `benchmark_format_comparison(self, analyzer_function: Callable, test_data: str, language: str)` — [`L677`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L677) — Benchmark and compare all format types
  - `test_format_performance(self, analyzer_function: Callable, test_data: str, language: str, format_types: list[str] = None)` — [`L627`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L627) — Test performance across different format types
  - `test_format_scalability(self, analyzer_function: Callable, data_generator: Callable[[int], str], language: str, format_type: str = "full", size_range: list[int] = None)` — [`L655`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L655) — Test format scalability with increasing data sizes
  - `test_function(data, format_type=format_type)` — [`L644`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L644)
  - `performance_tester` — [`L625`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L625)
- protocol/private: `__init__`[`L624`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L624)
- uses (calls/refs, reference-scoped): (9 test-only callers)
- used by: (2 test-only callers)

### `PerformanceBaseline`
- def: [`tests/integration/formatters/performance_tests_helpers.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L56)
- doc: Performance baseline for regression detection
- signature: `class PerformanceBaseline:`
- members:
  - `acceptable_variance_percent` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L62)
  - `baseline_memory_mb` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L61)
  - `baseline_time_ms` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L60)
  - `created_timestamp` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L63)
  - `last_updated` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L64)
  - `test_name` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L59)
- used by: (5 test-only callers)

### `PerformanceMetrics`
- def: [`tests/integration/formatters/performance_tests_helpers.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L24)
- doc: Performance measurement results
- signature: `class PerformanceMetrics:`
- members:
  - `cpu_usage_percent` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L31)
  - `element_count` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L34)
  - `error_message` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L38)
  - `execution_time_ms` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L28)
  - `file_size_bytes` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L33)
  - `format_type` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L35)
  - `memory_usage_mb` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L29)
  - `peak_memory_mb` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L30)
  - `success` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L37)
  - `test_name` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L27)
  - `throughput_ops_per_sec` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L32)
  - `timestamp` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L36)
- used by: (14 test-only callers)

### `PerformanceProfiler`
- def: [`tests/integration/formatters/performance_tests_helpers.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L67)
- doc: Profiles performance of format operations
- signature: `class PerformanceProfiler:`
- members:
  - `start_profiling(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L76) — Start performance profiling
  - `stop_profiling(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L88) — Stop profiling and return metrics
  - `baseline_memory` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L72)
  - `process` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L71)
  - `start_time` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L73)
  - `tracemalloc_started` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L74)
- protocol/private: `__init__`[`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L70)
- used by: (5 test-only callers)

### `PerformanceTester`
- def: [`tests/integration/formatters/performance_tests_helpers.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L119)
- doc: Main performance testing framework
- signature: `class PerformanceTester:`
- members:
  - `_calculate_scalability_factor(self, sizes: list[int], times: list[float])` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L538) — Calculate how performance scales with input size
  - `_estimate_element_count(self, test_data: Any)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L528) — Estimate number of elements in test data
  - `_load_all_performance_results(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L594) — Load all performance results from files
  - `_save_performance_results(self, test_name: str, aggregate_metrics: PerformanceMetrics, individual_results: list[PerformanceMetrics])` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L564) — Save performance test results
  - `_save_scalability_results(self, result: ScalabilityTestResult)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L584) — Save scalability test results
  - `check_performance_regression(self, test_name: str, current_metrics: PerformanceMetrics)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L341) — Check for performance regression against baseline
  - `create_baseline(self, test_name: str, metrics: PerformanceMetrics, acceptable_variance_percent: float = 20)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L393) — Create performance baseline
  - `generate_performance_report(self)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L446) — Generate comprehensive performance report
  - `load_baselines(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L424) — Load performance baselines from file
  - `run_concurrent_performance_test(self, test_name: str, test_function: Callable, test_data_list: list[Any], max_workers: int = 4, format_type: str = "full")` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L291) — Run concurrent performance tests
  - `run_performance_test(self, test_name: str, test_function: Callable, test_data: Any, format_type: str = "full", iterations: int = 5)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L130) — Run performance test with multiple iterations
  - `run_scalability_test(self, test_name: str, test_function: Callable, data_generator: Callable[[int], Any], size_range: list[int], format_type: str = "full")` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L231) — Run scalability test across different input sizes
  - `save_baselines(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L435) — Save performance baselines to file
  - `update_baseline(self, test_name: str, metrics: PerformanceMetrics)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L413) — Update existing baseline
  - `baselines` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L127)
  - `profiler` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L126)
  - `results_dir` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L123)
- protocol/private: `__init__`[`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L122)
- uses (calls/refs, reference-scoped): (32 test-only callers)
- used by: (8 test-only callers)

### `ScalabilityTestResult`
- def: [`tests/integration/formatters/performance_tests_helpers.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L42)
- doc: Scalability test results
- signature: `class ScalabilityTestResult:`
- members:
  - `execution_times` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L47)
  - `input_sizes` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L46)
  - `memory_usages` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L48)
  - `performance_threshold_exceeded` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L51)
  - `scalability_factor` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L50)
  - `test_name` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L45)
  - `throughput_rates` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L49)
  - `timestamp` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/performance_tests_helpers.py#L52)
- used by: (3 test-only callers)

