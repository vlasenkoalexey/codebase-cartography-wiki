---
title: 'Module: tests/integration/_test_phase7_security_stress_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_security_stress_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_security_stress_helpers`/
symbols:
  assert_concurrent_security_stress_results: assert_concurrent_security_stress_results().
  _build_concurrent_security_tasks: _build_concurrent_security_tasks().
  _build_normal_tasks: _build_normal_tasks().
  collect_concurrent_security_stress_results: collect_concurrent_security_stress_results().
  _build_path_traversal_tasks: _build_path_traversal_tasks().
  _build_malicious_query_tasks: _build_malicious_query_tasks().
  _build_concurrent_attack_results: _build_concurrent_attack_results().
  _split_concurrent_security_results: _split_concurrent_security_results().
  _assert_normal_tasks_survived: _assert_normal_tasks_survived().
  _assert_path_traversals_blocked: _assert_path_traversals_blocked().
  _assert_malicious_queries_safely_handled: _assert_malicious_queries_safely_handled().
  _assert_concurrent_security_stayed_responsive: _assert_concurrent_security_stayed_responsive().
  _print_concurrent_security_summary: _print_concurrent_security_summary().
  _build_concurrent_attack_result: _build_concurrent_attack_result().
---
# Module: [`tests/integration/_test_phase7_security_stress_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py)

## Functions
- `_assert_concurrent_security_stayed_responsive(execution_time: float)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L109)
- `_assert_malicious_queries_safely_handled(malicious_query_results: list[dict[str, Any]])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L97)
- `_assert_normal_tasks_survived(normal_results: list[dict[str, Any]])` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L72)
- `_assert_path_traversals_blocked(path_traversal_results: list[dict[str, Any]])` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L82)
- `_build_concurrent_attack_result(attack_type: str, result: Any)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L225)
- `_build_concurrent_attack_results(attack_tasks: list[tuple[str, Any]], results: Iterable[Any])` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L214)
- `_build_concurrent_security_tasks(secure_test_project: str, malicious_paths: Iterable[str], malicious_queries: Iterable[str])` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L139)
- `_build_malicious_query_tasks(search_tool: SearchContentTool, malicious_queries: Iterable[str], secure_test_project: str)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L173)
- `_build_normal_tasks(scale_tool: AnalyzeScaleTool, search_tool: SearchContentTool, secure_test_project: str)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L189)
- `_build_path_traversal_tasks(scale_tool: AnalyzeScaleTool, malicious_paths: Iterable[str])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L163)
- `_print_concurrent_security_summary(execution_time: float, successful_normal: list[dict[str, Any]], normal_results: list[dict[str, Any]], blocked_path_traversals: list[dict[str, Any]], path_traversal_results: list[dict[str, Any]], path_traversal_block_rate: float, safely_handled_queries: list[dict[str, Any]], malicious_query_results: list[dict[str, Any]])` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L115)
- `_split_concurrent_security_results(attack_results: list[dict[str, Any]])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L62)
- `assert_concurrent_security_stress_results(attack_results: list[dict[str, Any]], execution_time: float)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L34) — Assert and report the concurrent stress security expectations.
- `collect_concurrent_security_stress_results(secure_test_project: str, malicious_paths: Iterable[str], malicious_queries: Iterable[str])` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_stress_helpers.py#L13) — Run mixed normal and attack tasks concurrently.

