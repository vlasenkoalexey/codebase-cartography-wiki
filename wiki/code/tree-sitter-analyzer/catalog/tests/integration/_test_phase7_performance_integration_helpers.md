---
title: 'Module: tests/integration/_test_phase7_performance_integration_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_performance_integration_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_performance_integration_helpers`/
symbols:
  PerformanceProfiler.start_profiling: PerformanceProfiler#start_profiling().
  PerformanceProfiler.end_profiling: PerformanceProfiler#end_profiling().
  create_large_scale_structure: create_large_scale_structure().
  PerformanceProfiler: PerformanceProfiler#
  PerformanceProfiler.process: PerformanceProfiler#process.
  nonnegative_float_from_env: nonnegative_float_from_env().
  _create_java_classes: _create_java_classes().
  _create_python_modules: _create_python_modules().
  _create_javascript_components: _create_javascript_components().
  positive_int_from_env: positive_int_from_env().
  PerformanceProfiler.start_time: PerformanceProfiler#start_time.
  PerformanceProfiler.start_memory: PerformanceProfiler#start_memory.
  PerformanceProfiler.start_cpu: PerformanceProfiler#start_cpu.
  _java_class_content: _java_class_content().
  _python_module_content: _python_module_content().
  _javascript_component_content: _javascript_component_content().
  DEFAULT_MEMORY_EFFICIENCY_FILES: DEFAULT_MEMORY_EFFICIENCY_FILES.
  DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS: DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS.
  DEFAULT_SCALABILITY_RECOVERY_SECONDS: DEFAULT_SCALABILITY_RECOVERY_SECONDS.
  DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS: DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS.
  DEFAULT_SUSTAINED_LOAD_ITERATIONS: DEFAULT_SUSTAINED_LOAD_ITERATIONS.
  PerformanceProfiler.__init__: PerformanceProfiler#__init__().
---
# Module: [`tests/integration/_test_phase7_performance_integration_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py)

## Classes
### `PerformanceProfiler`
- def: [`tests/integration/_test_phase7_performance_integration_helpers.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L37)
- doc: Performance measurement utility for integration tests.
- signature: `class PerformanceProfiler:`
- members:
  - `end_profiling(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L53) — Stop profiling and return elapsed resource metrics.
  - `start_profiling(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L46) — Start profiling after forcing collection.
  - `process` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L41)
  - `start_cpu` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L44)
  - `start_memory` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L43)
  - `start_time` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L42)
- protocol/private: `__init__`[`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L40)
- used by: (6 test-only callers)

## Functions
- `_create_java_classes(project_root: Path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L77)
- `_create_javascript_components(project_root: Path)` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L298)
- `_create_python_modules(project_root: Path)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L149)
- `_java_class_content(index: int)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L89)
- `_javascript_component_content(index: int)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L308)
- `_python_module_content(index: int)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L157)
- `create_large_scale_structure(project_root: Path)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L70) — Create a mixed-language project fixture for performance tests.
- `nonnegative_float_from_env(name: str, default: float)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L28) — Read a non-negative float env override without making test collection brittle.
- `positive_int_from_env(name: str, default: int)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L19) — Read a positive integer env override without making test collection brittle.

## Module values
- `DEFAULT_MEMORY_EFFICIENCY_FILES` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L12)
- `DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L13)
- `DEFAULT_SCALABILITY_RECOVERY_SECONDS` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L14)
- `DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L15)
- `DEFAULT_SUSTAINED_LOAD_ITERATIONS` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_performance_integration_helpers.py#L16)

