---
title: 'Module: tests/integration/test_phase7_performance_integration.py'
type: catalog
provenance: extracted
module: tests/integration/test_phase7_performance_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_phase7_performance_integration`/
symbols:
  TestPhase7PerformanceIntegration.test_scalability_limits: TestPhase7PerformanceIntegration#test_scalability_limits().
  TestPhase7PerformanceIntegration.test_sustained_load_performance: TestPhase7PerformanceIntegration#test_sustained_load_performance().
  TestPhase7PerformanceIntegration.test_large_scale_file_analysis_performance: TestPhase7PerformanceIntegration#test_large_scale_file_analysis_performance().
  TestPhase7PerformanceIntegration.test_memory_efficiency_under_load: TestPhase7PerformanceIntegration#test_memory_efficiency_under_load().
  TestPhase7PerformanceIntegration.test_error_recovery_performance: TestPhase7PerformanceIntegration#test_error_recovery_performance().
  _create_task_for_tool: _create_task_for_tool().
  TestPhase7PerformanceIntegration.test_concurrent_search_performance: TestPhase7PerformanceIntegration#test_concurrent_search_performance().
  TestPhase7PerformanceIntegration.test_resource_cleanup_efficiency: TestPhase7PerformanceIntegration#test_resource_cleanup_efficiency().
  _collect_scalability_tasks: _collect_scalability_tasks().
  TestPhase7PerformanceIntegration.large_scale_project: TestPhase7PerformanceIntegration#large_scale_project().
  _SEARCH_QUERIES: _SEARCH_QUERIES.
  DEFAULT_SUSTAINED_LOAD_ITERATIONS: DEFAULT_SUSTAINED_LOAD_ITERATIONS.
  DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS: DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS.
  DEFAULT_SCALABILITY_RECOVERY_SECONDS: DEFAULT_SCALABILITY_RECOVERY_SECONDS.
  DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS: DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS.
  DEFAULT_MEMORY_EFFICIENCY_FILES: DEFAULT_MEMORY_EFFICIENCY_FILES.
  _partition_task_results: _partition_task_results().
  _collect_handled_errors: _collect_handled_errors().
  TestPhase7PerformanceIntegration: TestPhase7PerformanceIntegration#
---
# Module: [`tests/integration/test_phase7_performance_integration.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py)

## Classes
### `TestPhase7PerformanceIntegration`
- def: [`tests/integration/test_phase7_performance_integration.py:103`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L103)
- doc: Phase 7 パフォーマンス統合テスト
- signature: `class TestPhase7PerformanceIntegration:`
- members:
  - `large_scale_project(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L107) — 大規模プロジェクト作成（パフォーマンステスト用）
  - `test_concurrent_search_performance(self, large_scale_project)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L193) — 同時検索のパフォーマンステスト
  - `test_error_recovery_performance(self, large_scale_project)` — [`L586`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L586) — エラー回復パフォーマンステスト
  - `test_large_scale_file_analysis_performance(self, large_scale_project)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L120) — 大規模ファイル分析のパフォーマンステスト
  - `test_memory_efficiency_under_load(self, large_scale_project)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L259) — 負荷下でのメモリ効率性テスト
  - `test_resource_cleanup_efficiency(self, large_scale_project)` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L506) — リソースクリーンアップ効率性テスト
  - `test_scalability_limits(self, large_scale_project)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L336) — スケーラビリティ限界テスト
  - `test_sustained_load_performance(self, large_scale_project)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L420) — 持続負荷パフォーマンステスト
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`SearchContentTool`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`AnalyzeScaleTool`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`set_project_path`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path)  (14 test-only)

## Functions
- `_collect_handled_errors(results)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L93) — Return results that represent handled errors (raised exception or error dict).
- `_collect_scalability_tasks(tools, load_level, project_root)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L71) — Build task list for one scalability load level, skipping tools with no files.
- `_create_task_for_tool(tool, i: int, project_root: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L43) — Return an execute coroutine for the given tool/index, or None if no files.
- `_partition_task_results(tasks, results)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L81) — Split gathered results into valid and error buckets based on task metadata.

## Module values
- `DEFAULT_MEMORY_EFFICIENCY_FILES` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L38)
- `DEFAULT_RESOURCE_CLEANUP_SETTLE_SECONDS` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L37)
- `DEFAULT_SCALABILITY_RECOVERY_SECONDS` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L36)
- `DEFAULT_SUSTAINED_LOAD_INTERVAL_SECONDS` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L35)
- `DEFAULT_SUSTAINED_LOAD_ITERATIONS` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L34)
- `_SEARCH_QUERIES` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_performance_integration.py#L40)

