---
title: 'Module: tests/benchmarks/test_large_file_performance.py'
type: catalog
provenance: extracted
module: tests/benchmarks/test_large_file_performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.benchmarks.test_large_file_performance`/
symbols:
  TestLargeFilePerformance._create_large_python_file: TestLargeFilePerformance#_create_large_python_file().
  TestLargeFilePerformance.temp_dir: TestLargeFilePerformance#temp_dir.
  TestLargeFilePerformance.test_analyze_large_file_scale: TestLargeFilePerformance#test_analyze_large_file_scale().
  TestLargeFilePerformance.test_analyze_large_file_structure: TestLargeFilePerformance#test_analyze_large_file_structure().
  TestLargeFilePerformance.test_query_large_file: TestLargeFilePerformance#test_query_large_file().
  TestLargeFilePerformance.test_analyze_very_large_file: TestLargeFilePerformance#test_analyze_very_large_file().
  TestLargeFilePerformance.test_cache_performance_large_file: TestLargeFilePerformance#test_cache_performance_large_file().
  TestLargeFilePerformance.test_memory_usage_large_file: TestLargeFilePerformance#test_memory_usage_large_file().
  TestLargeFilePerformance.test_concurrent_large_file_analysis: TestLargeFilePerformance#test_concurrent_large_file_analysis().
  TestLargeFilePerformance.test_large_file_with_complexity: TestLargeFilePerformance#test_large_file_with_complexity().
  TestLargeFilePerformance.test_large_file_with_details: TestLargeFilePerformance#test_large_file_with_details().
  TestLargeFilePerformance.server: TestLargeFilePerformance#server.
  TestLargeFilePerformance.teardown_method: TestLargeFilePerformance#teardown_method().
  pytestmark: pytestmark.
  TestLargeFilePerformance: TestLargeFilePerformance#
  TestLargeFilePerformance.setup_method: TestLargeFilePerformance#setup_method().
---
# Module: [`tests/benchmarks/test_large_file_performance.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py)

## Classes
### `TestLargeFilePerformance`
- def: [`tests/benchmarks/test_large_file_performance.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L25)
- doc: Tests for large file processing performance.
- signature: `class TestLargeFilePerformance:`
- members:
  - `_create_large_python_file(self, num_functions: int = 100)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L39) — Create a large Python file for testing.
  - `setup_method(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L28) — Set up test fixtures.
  - `teardown_method(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L33) — Clean up test fixtures.
  - `test_analyze_large_file_scale(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L52) — Test performance of analyzing large file with code scale.
  - `test_analyze_large_file_structure(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L77) — Test performance of analyzing large file structure.
  - `test_analyze_very_large_file(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L123) — Test performance with very large file (500 functions).
  - `test_cache_performance_large_file(self)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L149) — Test cache performance with large file.
  - `test_concurrent_large_file_analysis(self)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L214) — Test concurrent analysis of multiple large files.
  - `test_large_file_with_complexity(self)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L245) — Test performance with complexity analysis enabled.
  - `test_large_file_with_details(self)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L269) — Test performance with detailed analysis.
  - `test_memory_usage_large_file(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L185) — Test memory usage with large file.
  - `test_query_large_file(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L100) — Test performance of querying large file.
  - `server` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L30)
  - `temp_dir` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L31)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`AnalyzeCodeStructureTool`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)

## Module values
- `pytestmark` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_large_file_performance.py#L22)

