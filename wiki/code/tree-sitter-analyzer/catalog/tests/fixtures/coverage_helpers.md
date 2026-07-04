---
title: 'Module: tests/fixtures/coverage_helpers.py'
type: catalog
provenance: extracted
module: tests/fixtures/coverage_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.coverage_helpers`/
symbols:
  create_mock_node: create_mock_node().
  create_mock_query_result: create_mock_query_result().
  create_mock_node.child_by_field_name: create_mock_node().child_by_field_name().
  create_mock_parser: create_mock_parser().
  create_mock_analysis_result: create_mock_analysis_result().
  create_temp_code_file: create_temp_code_file().
  create_async_mock_tool: create_async_mock_tool().
  assert_coverage_improved: assert_coverage_improved().
  assert_coverage_threshold: assert_coverage_threshold().
  get_uncovered_lines_info: get_uncovered_lines_info().
  __all__: __all__.
---
# Module: [`tests/fixtures/coverage_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py)

## Functions
- `assert_coverage_improved(before_coverage: float, after_coverage: float, min_improvement: float = 5)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L216) — Assert that coverage has improved by at least the minimum amount.
- `assert_coverage_threshold(coverage: float, threshold: float = 80, module_name: str = "module")` — [`L242`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L242) — Assert that coverage meets or exceeds the threshold.
- `child_by_field_name(field_name: str)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L77)
- `create_async_mock_tool(return_value: Any = None)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L196) — Create an async mock MCP tool.
- `create_mock_analysis_result(file_path: str = "test.py", language: str = "python", elements: dict[str, list[dict[str, Any]]] | None = None, error: str | None = None)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L113) — Create a mock analysis result.
- `create_mock_node(type: str = "function_definition", text: str = "def foo():\n pass", start_point: tuple[int, int] = (0, 0), end_point: tuple[int, int] = (1, 8), children: list[Any] | None = None)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L42) — Create a mock tree-sitter node.
- `create_mock_parser(language: str = "python")` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L16) — Create a mock tree-sitter parser.
- `create_mock_query_result(captures: list[tuple[MagicMock, str]] | None = None)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L89) — Create mock query results.
- `create_temp_code_file(tmp_path: Path, filename: str, content: str, language: str = "python")` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L158) — Create a temporary code file for testing.
- `get_uncovered_lines_info(coverage_data: dict[str, Any])` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L267) — Extract and format information about uncovered lines.

## Module values
- `__all__` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/coverage_helpers.py#L291)

