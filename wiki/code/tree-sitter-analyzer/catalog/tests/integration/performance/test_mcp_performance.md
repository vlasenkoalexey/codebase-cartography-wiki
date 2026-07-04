---
title: 'Module: tests/integration/performance/test_mcp_performance.py'
type: catalog
provenance: extracted
module: tests/integration/performance/test_mcp_performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.performance.test_mcp_performance`/
symbols:
  TestCompositeWorkflowPerformance.test_full_analysis_workflow_performance: TestCompositeWorkflowPerformance#test_full_analysis_workflow_performance().
  TestCompositeWorkflowPerformance.test_search_and_extract_workflow_performance: TestCompositeWorkflowPerformance#test_search_and_extract_workflow_performance().
  PerformanceMonitor.start_measurement: PerformanceMonitor#start_measurement().
  PerformanceMonitor.end_measurement: PerformanceMonitor#end_measurement().
  TestSingleToolPerformance.test_check_code_scale_performance: TestSingleToolPerformance#test_check_code_scale_performance().
  TestSingleToolPerformance.test_analyze_code_structure_performance: TestSingleToolPerformance#test_analyze_code_structure_performance().
  TestSingleToolPerformance.test_extract_code_section_performance: TestSingleToolPerformance#test_extract_code_section_performance().
  TestSingleToolPerformance.test_query_code_performance: TestSingleToolPerformance#test_query_code_performance().
  TestSingleToolPerformance.test_list_files_performance: TestSingleToolPerformance#test_list_files_performance().
  TestSingleToolPerformance.test_search_content_performance: TestSingleToolPerformance#test_search_content_performance().
  TestLargeScalePerformance.test_large_project_file_listing: TestLargeScalePerformance#test_large_project_file_listing().
  TestLargeScalePerformance.test_large_project_content_search: TestLargeScalePerformance#test_large_project_content_search().
  TestMemoryOptimization.test_memory_usage_optimization: TestMemoryOptimization#test_memory_usage_optimization().
  PerformanceMonitor.process: PerformanceMonitor#process.
  performance_monitor: performance_monitor().
  PerformanceMonitor.start_time: PerformanceMonitor#start_time.
  PerformanceMonitor.start_memory: PerformanceMonitor#start_memory.
  PerformanceMonitor: PerformanceMonitor#
  PerformanceMonitor.__init__: PerformanceMonitor#__init__().
  sample_code_file: sample_code_file().
  large_code_file: large_code_file().
  large_project_structure: large_project_structure().
  TestSingleToolPerformance: TestSingleToolPerformance#
  TestCompositeWorkflowPerformance: TestCompositeWorkflowPerformance#
  TestLargeScalePerformance: TestLargeScalePerformance#
  TestMemoryOptimization: TestMemoryOptimization#
---
# Module: [`tests/integration/performance/test_mcp_performance.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py)

## Classes
### `PerformanceMonitor`
- def: [`tests/integration/performance/test_mcp_performance.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L31)
- doc: パフォーマンス測定ユーティリティ
- signature: `class PerformanceMonitor:`
- members:
  - `end_measurement(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L44) — 測定終了と結果取得
  - `start_measurement(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L39) — 測定開始
  - `process` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L35)
  - `start_memory` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L37)
  - `start_time` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L36)
- protocol/private: `__init__`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L34)
- used by: (1 test-only callers)

### `TestCompositeWorkflowPerformance`
- def: [`tests/integration/performance/test_mcp_performance.py:334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L334)
- doc: 複合ワークフローのパフォーマンステスト（目標: 10秒以内）
- signature: `class TestCompositeWorkflowPerformance:`
- members:
  - `test_full_analysis_workflow_performance(self, large_code_file, performance_monitor)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L338) — 完全解析ワークフローのパフォーマンステスト
  - `test_search_and_extract_workflow_performance(self, large_project_structure, performance_monitor)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L397) — 検索・抽出ワークフローのパフォーマンステスト
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)

### `TestLargeScalePerformance`
- def: [`tests/integration/performance/test_mcp_performance.py:448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L448)
- doc: 大規模プロジェクト対応のパフォーマンステスト（10,000ファイル対応）
- signature: `class TestLargeScalePerformance:`
- members:
  - `test_large_project_content_search(self, large_project_structure, performance_monitor)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L487) — 大規模プロジェクトでのコンテンツ検索
  - `test_large_project_file_listing(self, large_project_structure, performance_monitor)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L453) — 大規模プロジェクトでのファイル一覧取得
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute)

### `TestMemoryOptimization`
- def: [`tests/integration/performance/test_mcp_performance.py:521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L521)
- doc: メモリ使用量最適化の検証
- signature: `class TestMemoryOptimization:`
- members:
  - `test_memory_usage_optimization(self, large_code_file, performance_monitor)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L525) — メモリ使用量最適化の確認
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)

### `TestSingleToolPerformance`
- def: [`tests/integration/performance/test_mcp_performance.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L156)
- doc: 単一ツールのパフォーマンステスト（目標: 3秒以内）
- signature: `class TestSingleToolPerformance:`
- members:
  - `test_analyze_code_structure_performance(self, sample_code_file, performance_monitor)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L189) — analyze_code_structure ツールのパフォーマンステスト
  - `test_check_code_scale_performance(self, sample_code_file, performance_monitor)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L160) — check_code_scale ツールのパフォーマンステスト
  - `test_extract_code_section_performance(self, large_code_file, performance_monitor)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L213) — extract_code_section ツールのパフォーマンステスト
  - `test_list_files_performance(self, large_project_structure, performance_monitor)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L269) — list_files ツールのパフォーマンステスト
  - `test_query_code_performance(self, sample_code_file, performance_monitor)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L242) — query_code ツールのパフォーマンステスト
  - `test_search_content_performance(self, large_project_structure, performance_monitor)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L295) — search_content ツールのパフォーマンステスト
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)

## Functions
- `large_code_file(tmp_path)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L99) — 大規模コードファイル作成（1000行以上）
- `large_project_structure(tmp_path)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L128) — 大規模プロジェクト構造作成（1000ファイル）
- `performance_monitor()` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L57) — パフォーマンスモニター
- `sample_code_file(tmp_path)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/performance/test_mcp_performance.py#L63) — サンプルコードファイル作成

