---
title: 'Module: tests/integration/_test_phase7_malicious_query_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_malicious_query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_malicious_query_helpers`/
symbols:
  _execute_malicious_query: _execute_malicious_query().
  _run_malicious_query: _run_malicious_query().
  collect_malicious_query_results: collect_malicious_query_results().
  _collect_tool_malicious_query_results: _collect_tool_malicious_query_results().
  _build_query_result: _build_query_result().
  _preview_query: _preview_query().
---
# Module: [`tests/integration/_test_phase7_malicious_query_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py)

## Functions
- `_build_query_result(tool_name: str, malicious_query: str, execution_time: float, result: dict[str, Any])` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L128)
- `_collect_tool_malicious_query_results(tool: Any, malicious_queries: Iterable[str], secure_test_project: str)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L34)
- `_execute_malicious_query(tool: Any, malicious_query: str, secure_test_project: str)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L89)
- `_preview_query(malicious_query: str)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L145)
- `_run_malicious_query(tool: Any, tool_name: str, malicious_query: str, secure_test_project: str)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L55)
- `collect_malicious_query_results(search_tools: Iterable[Any], malicious_queries: Iterable[str], secure_test_project: str)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_malicious_query_helpers.py#L14) — Run every malicious query against each search tool.

