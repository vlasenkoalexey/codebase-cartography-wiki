---
title: 'Module: tree_sitter_analyzer/core/performance.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.performance`/Performance
symbols:
  PerformanceMonitor: Monitor#
  PerformanceMonitor.start_monitoring: Monitor#start_monitoring().
  PerformanceMonitor._operation_stats: Monitor#_operation_stats.
  PerformanceContext.__exit__: Context#__exit__().
  PerformanceMonitor.record_operation: Monitor#record_operation().
  PerformanceMonitor._total_operations: Monitor#_total_operations.
  PerformanceMonitor.get_performance_summary: Monitor#get_performance_summary().
  PerformanceMonitor.clear_metrics: Monitor#clear_metrics().
  PerformanceMonitor.measure_operation: Monitor#measure_operation().
  PerformanceContext: Context#
  PerformanceContext.__enter__: Context#__enter__().
  PerformanceMonitor.stop_monitoring: Monitor#stop_monitoring().
  PerformanceMonitor.get_last_duration: Monitor#get_last_duration().
  PerformanceMonitor._monitoring_active: Monitor#_monitoring_active.
  PerformanceMonitor._last_duration: Monitor#_last_duration.
  PerformanceMonitor._set_duration: Monitor#_set_duration().
  PerformanceMonitor.get_operation_stats: Monitor#get_operation_stats().
  PerformanceContext.operation_name: Context#operation_name.
  PerformanceContext.monitor: Context#monitor.
  PerformanceContext.start_time: Context#start_time.
  PerformanceMonitor.set_duration: Monitor#set_duration.
  PerformanceContext.__init__: Context#__init__().
  PerformanceMonitor.__init__: Monitor#__init__().
---
# Module: [`tree_sitter_analyzer/core/performance.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py)

## Classes
### `PerformanceContext`
- def: [`tree_sitter_analyzer/core/performance.py:87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L87)
- members:
  - `monitor` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L92)
  - `operation_name` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L91)
  - `start_time` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L93)
- protocol/private: `__enter__`[`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L95), `__exit__`[`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L99), `__init__`[`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L90)
- uses (calls/refs, reference-scoped): [`PerformanceMonitor`](performance.md#PerformanceMonitor), [`log_performance`](../utils/logging.md#log_performance), [`record_operation`](performance.md#PerformanceMonitor.record_operation), [`set_duration`](performance.md#PerformanceMonitor.set_duration)
- used by: [`measure_operation`](performance.md#PerformanceMonitor.measure_operation), [`measure_operation`](_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin.measure_operation)  (7 test-only)

### `PerformanceMonitor`
- def: [`tree_sitter_analyzer/core/performance.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L12)
- doc: Performance monitoring (simplified version)
- signature: `class PerformanceMonitor:`
- members:
  - `_set_duration(self, duration: float)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L29) — Set operation time (internal use)
  - `clear_metrics(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L79) — Clear collected metrics
  - `get_last_duration(self)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L25) — Get last operation time
  - `get_operation_stats(self)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L45) — Get operation statistics
  - `get_performance_summary(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L49) — Get performance summary
  - `measure_operation(self, operation_name: str)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L21) — Return measurement context for operation
  - `record_operation(self, operation_name: str, duration: float)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L58) — Record operation
  - `start_monitoring(self)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L35) — Start performance monitoring
  - `stop_monitoring(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L40) — Stop performance monitoring
  - `set_duration` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L33)
- protocol/private: `__init__`[`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L15), `_last_duration`[`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L16), `_monitoring_active`[`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L17), `_operation_stats`[`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L18), `_total_operations`[`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/performance.py#L19)
- uses (calls/refs, reference-scoped): [`log_info`](../utils/logging.md#log_info), [`PerformanceContext`](performance.md#PerformanceContext)
- used by: [`_ensure_initialized`](analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`__exit__`](performance.md#PerformanceContext.__exit__), [`get_performance_monitor`](../mcp/utils/__init__.md#get_performance_monitor), [`__init__`](performance.md#PerformanceContext.__init__)  (27 test-only)

