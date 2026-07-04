---
title: 'Module: tests/benchmarks/test_query_performance.py'
type: catalog
provenance: extracted
module: tests/benchmarks/test_query_performance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.benchmarks.test_query_performance`/
symbols:
  TestQueryPerformance.temp_dir: TestQueryPerformance#temp_dir.
  TestQueryPerformance._create_python_file: TestQueryPerformance#_create_python_file().
  TestQueryPerformance.test_query_simple_pattern_performance: TestQueryPerformance#test_query_simple_pattern_performance().
  TestQueryPerformance.test_query_complex_pattern_performance: TestQueryPerformance#test_query_complex_pattern_performance().
  TestQueryPerformance.test_query_with_filter_performance: TestQueryPerformance#test_query_with_filter_performance().
  TestQueryPerformance.test_query_custom_query_performance: TestQueryPerformance#test_query_custom_query_performance().
  TestQueryPerformance.test_query_summary_format_performance: TestQueryPerformance#test_query_summary_format_performance().
  TestQueryPerformance.test_query_json_format_performance: TestQueryPerformance#test_query_json_format_performance().
  TestQueryPerformance.test_query_with_max_count_performance: TestQueryPerformance#test_query_with_max_count_performance().
  TestQueryPerformance.test_query_repeated_performance: TestQueryPerformance#test_query_repeated_performance().
  TestQueryPerformance.test_query_different_languages_performance: TestQueryPerformance#test_query_different_languages_performance().
  TestQueryPerformance.test_query_multiple_files_performance: TestQueryPerformance#test_query_multiple_files_performance().
  TestQueryPerformance.teardown_method: TestQueryPerformance#teardown_method().
  pytestmark: pytestmark.
  TestQueryPerformance: TestQueryPerformance#
  TestQueryPerformance.setup_method: TestQueryPerformance#setup_method().
---
# Module: [`tests/benchmarks/test_query_performance.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py)

## Classes
### `TestQueryPerformance`
- def: [`tests/benchmarks/test_query_performance.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L19)
- doc: Tests for query performance.
- signature: `class TestQueryPerformance:`
- members:
  - `_create_python_file(self, content: str)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L32) — Create a Python file for testing.
  - `setup_method(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L22) — Set up test fixtures.
  - `teardown_method(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L26) — Clean up test fixtures.
  - `test_query_complex_pattern_performance(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L62) — Test performance of complex query pattern.
  - `test_query_custom_query_performance(self)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L150) — Test performance of custom tree-sitter query.
  - `test_query_different_languages_performance(self)` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L266) — Test performance of querying different languages.
  - `test_query_json_format_performance(self)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L196) — Test performance of JSON format output.
  - `test_query_multiple_files_performance(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L119) — Test performance of querying multiple files.
  - `test_query_repeated_performance(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L243) — Test performance of repeated queries on same file.
  - `test_query_simple_pattern_performance(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L39) — Test performance of simple query pattern.
  - `test_query_summary_format_performance(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L173) — Test performance of summary format output.
  - `test_query_with_filter_performance(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L95) — Test performance of query with filter.
  - `test_query_with_max_count_performance(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L219) — Test performance of query with max_count limit.
  - `temp_dir` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L24)
- uses (calls/refs, reference-scoped): [`QueryTool`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)

## Module values
- `pytestmark` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_query_performance.py#L16)

