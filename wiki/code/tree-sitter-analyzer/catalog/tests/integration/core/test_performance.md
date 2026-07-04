---
title: 'Module: tests/integration/core/test_performance.py'
type: catalog
provenance: extracted
module: tests/integration/core/test_performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.core.test_performance`/TestPerformance
symbols:
  TestPerformanceMonitor.test_clear_metrics: Monitor#test_clear_metrics().
  TestPerformanceContext.test_context_manager_exit: Context#test_context_manager_exit().
  TestPerformanceIntegration.test_reset_between_sessions: Integration#test_reset_between_sessions().
  TestPerformanceContext.test_context_manager_with_exception: Context#test_context_manager_with_exception().
  TestPerformanceContext.test_context_manager_usage: Context#test_context_manager_usage().
  TestPerformanceIntegration.test_full_workflow: Integration#test_full_workflow().
  TestPerformanceIntegration.test_concurrent_operations: Integration#test_concurrent_operations().
  TestPerformanceMonitor.test_init: Monitor#test_init().
  TestPerformanceMonitor.test_measure_operation: Monitor#test_measure_operation().
  TestPerformanceMonitor.test_record_operation_when_monitoring_active: Monitor#test_record_operation_when_monitoring_active().
  TestPerformanceMonitor.test_record_operation_multiple_calls: Monitor#test_record_operation_multiple_calls().
  TestPerformanceMonitor.test_record_operation_different_operations: Monitor#test_record_operation_different_operations().
  TestPerformanceContext.test_init: Context#test_init().
  TestPerformanceContext.test_context_manager_exit_logs: Context#test_context_manager_exit_logs().
  TestPerformanceMonitor.test_stop_monitoring: Monitor#test_stop_monitoring().
  TestPerformanceMonitor.test_record_operation_when_monitoring_inactive: Monitor#test_record_operation_when_monitoring_inactive().
  TestPerformanceContext.test_context_manager_enter: Context#test_context_manager_enter().
  TestPerformanceMonitor.test_set_duration_internal: Monitor#test_set_duration_internal().
  TestPerformanceMonitor.test_start_monitoring: Monitor#test_start_monitoring().
  TestPerformanceMonitor.test_stop_monitoring_logs: Monitor#test_stop_monitoring_logs().
  TestPerformanceMonitor.test_get_last_duration: Monitor#test_get_last_duration().
  TestPerformanceMonitor.test_start_monitoring_logs: Monitor#test_start_monitoring_logs().
  TestPerformanceMonitor.test_get_operation_stats: Monitor#test_get_operation_stats().
  TestPerformanceMonitor.test_get_performance_summary: Monitor#test_get_performance_summary().
  TestPerformanceMonitor.test_clear_metrics_logs: Monitor#test_clear_metrics_logs().
  TestPerformanceMonitor: Monitor#
  TestPerformanceContext: Context#
  TestPerformanceIntegration: Integration#
---
# Module: [`tests/integration/core/test_performance.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py)

## Classes
### `TestPerformanceContext`
- def: [`tests/integration/core/test_performance.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L149)
- doc: PerformanceContext测试类
- signature: `class TestPerformanceContext:`
- members:
  - `test_context_manager_enter(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L160) — 测试上下文管理器__enter__
  - `test_context_manager_exit(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L168) — 测试上下文管理器__exit__
  - `test_context_manager_exit_logs(self, mock_log)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L183) — 测试上下文管理器__exit__日志输出
  - `test_context_manager_usage(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L209) — 测试实际使用场景
  - `test_context_manager_with_exception(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L197) — 测试上下文管理器处理异常
  - `test_init(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L152) — 测试PerformanceContext初始化
- uses (calls/refs, reference-scoped): [`PerformanceMonitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor), [`start_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.start_monitoring), [`_operation_stats`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._operation_stats), [`__exit__`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.__exit__), [`_total_operations`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._total_operations), [`measure_operation`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.measure_operation), [`PerformanceContext`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext), [`__enter__`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.__enter__), [`get_last_duration`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_last_duration), [`monitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.monitor), [`operation_name`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.operation_name), [`start_time`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.start_time)

### `TestPerformanceIntegration`
- def: [`tests/integration/core/test_performance.py:223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L223)
- doc: PerformanceMonitor集成测试
- signature: `class TestPerformanceIntegration:`
- members:
  - `test_concurrent_operations(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L258) — 测试并发操作
  - `test_full_workflow(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L226) — 测试完整工作流程
  - `test_reset_between_sessions(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L278) — 测试会话间重置
- uses (calls/refs, reference-scoped): [`PerformanceMonitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor), [`start_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.start_monitoring), [`_operation_stats`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._operation_stats), [`_total_operations`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._total_operations), [`clear_metrics`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.clear_metrics), [`get_performance_summary`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_performance_summary), [`measure_operation`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.measure_operation), [`__enter__`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.__enter__), [`stop_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.stop_monitoring)

### `TestPerformanceMonitor`
- def: [`tests/integration/core/test_performance.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L15)
- doc: PerformanceMonitor测试类
- signature: `class TestPerformanceMonitor:`
- members:
  - `test_clear_metrics(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L131) — 测试clear_metrics方法
  - `test_clear_metrics_logs(self, mock_log)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L142) — 测试clear_metrics日志输出
  - `test_get_last_duration(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L34) — 测试get_last_duration方法
  - `test_get_operation_stats(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L73) — 测试get_operation_stats方法
  - `test_get_performance_summary(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L80) — 测试get_performance_summary方法
  - `test_init(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L18) — 测试PerformanceMonitor初始化
  - `test_measure_operation(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L26) — 测试measure_operation方法
  - `test_record_operation_different_operations(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L121) — 测试记录不同操作
  - `test_record_operation_multiple_calls(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L106) — 测试多次记录同一操作
  - `test_record_operation_when_monitoring_active(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L96) — 测试monitoring active时记录操作
  - `test_record_operation_when_monitoring_inactive(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L89) — 测试monitoring inactive时不记录操作
  - `test_set_duration_internal(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L39) — 测试_set_duration内部方法
  - `test_start_monitoring(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L45) — 测试start_monitoring方法
  - `test_start_monitoring_logs(self, mock_log)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L59) — 测试start_monitoring日志输出
  - `test_stop_monitoring(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L51) — 测试stop_monitoring方法
  - `test_stop_monitoring_logs(self, mock_log)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_performance.py#L66) — 测试stop_monitoring日志输出
- uses (calls/refs, reference-scoped): [`PerformanceMonitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor), [`start_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.start_monitoring), [`_operation_stats`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._operation_stats), [`record_operation`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.record_operation), [`_total_operations`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._total_operations), [`clear_metrics`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.clear_metrics), [`get_performance_summary`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_performance_summary), [`measure_operation`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.measure_operation), [`PerformanceContext`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext), [`stop_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.stop_monitoring), [`get_last_duration`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_last_duration), [`_monitoring_active`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._monitoring_active), [`_last_duration`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._last_duration), [`_set_duration`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor._set_duration), [`get_operation_stats`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_operation_stats), [`monitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.monitor), [`operation_name`](../../../tree_sitter_analyzer/core/performance.md#PerformanceContext.operation_name)

