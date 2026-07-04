---
title: 'Module: tests/unit/core/test_split_components.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_split_components.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_split_components`/TestCoreComponents#
symbols:
  TestCoreComponents.test_analysis_request_creation: test_analysis_request_creation().
  TestCoreComponents.test_analysis_request_from_mcp: test_analysis_request_from_mcp().
  TestCoreComponents.test_performance_monitor_basic: test_performance_monitor_basic().
  TestCoreComponents.test_performance_monitor_clear: test_performance_monitor_clear().
  TestCoreComponents: ''
---
# Module: [`tests/unit/core/test_split_components.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py)

## Classes
### `TestCoreComponents`
- def: [`tests/unit/core/test_split_components.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py#L12)
- doc: Test suite for split core components
- signature: `class TestCoreComponents:`
- members:
  - `test_analysis_request_creation(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py#L15) — Test AnalysisRequest creation and defaults
  - `test_analysis_request_from_mcp(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py#L23) — Test AnalysisRequest conversion from MCP arguments
  - `test_performance_monitor_basic(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py#L35) — Test PerformanceMonitor basic functionality
  - `test_performance_monitor_clear(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_split_components.py#L52) — Test PerformanceMonitor metric clearing
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`format_type`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`PerformanceMonitor`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor), [`start_monitoring`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.start_monitoring), [`from_mcp_arguments`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.from_mcp_arguments), [`clear_metrics`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.clear_metrics), [`get_performance_summary`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_performance_summary), [`measure_operation`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.measure_operation), [`get_operation_stats`](../../../tree_sitter_analyzer/core/performance.md#PerformanceMonitor.get_operation_stats)

