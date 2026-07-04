---
title: 'Module: tests/integration/_test_phase7_security_policy_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_security_policy_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_security_policy_helpers`/
symbols:
  _execute_security_policy_case: _execute_security_policy_case().
  _run_security_policy_case: _run_security_policy_case().
  collect_security_policy_results: collect_security_policy_results().
  assert_security_policy_consistency_results: assert_security_policy_consistency_results().
  create_security_policy_test_cases: create_security_policy_test_cases().
  _build_security_policy_result: _build_security_policy_result().
  _print_inconsistent_security_policy_results: _print_inconsistent_security_policy_results().
---
# Module: [`tests/integration/_test_phase7_security_policy_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py)

## Functions
- `_build_security_policy_result(tool_name: str, test_case: dict[str, Any], blocked: bool, result_label: str | None = None)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L137)
- `_execute_security_policy_case(tool: Any, test_data: str)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L117)
- `_print_inconsistent_security_policy_results(inconsistent_results: list[dict[str, Any]])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L84)
- `_run_security_policy_case(tool: Any, tool_name: str, test_case: dict[str, Any])` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L95)
- `assert_security_policy_consistency_results(policy_results: list[dict[str, Any]])` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L60) — Assert and report security policy consistency across tools.
- `collect_security_policy_results(tools: Iterable[Any], test_cases: Iterable[dict[str, Any]])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L43) — Run path-policy cases across tools and report consistency.
- `create_security_policy_test_cases()` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_policy_helpers.py#L17) — Return common path-policy cases shared across MCP tools.

