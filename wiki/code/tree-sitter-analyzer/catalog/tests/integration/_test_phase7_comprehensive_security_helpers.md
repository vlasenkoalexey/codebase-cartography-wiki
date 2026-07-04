---
title: 'Module: tests/integration/_test_phase7_comprehensive_security_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_comprehensive_security_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_comprehensive_security_helpers`/
symbols:
  collect_comprehensive_security_checks: collect_comprehensive_security_checks().
  assert_comprehensive_security_checks: assert_comprehensive_security_checks().
  _collect_path_traversal_checks: _collect_path_traversal_checks().
  _collect_path_traversal_check: _collect_path_traversal_check().
  _collect_normal_query_checks: _collect_normal_query_checks().
  _collect_normal_query_check: _collect_normal_query_check().
  _collect_normal_search_check: _collect_normal_search_check().
  PATH_TRAVERSAL_CHECKS: PATH_TRAVERSAL_CHECKS.
  NORMAL_QUERY_CHECKS: NORMAL_QUERY_CHECKS.
  _print_comprehensive_security_summary: _print_comprehensive_security_summary().
  _assert_path_traversal_protection: _assert_path_traversal_protection().
  _assert_relevant_security_score: _assert_relevant_security_score().
---
# Module: [`tests/integration/_test_phase7_comprehensive_security_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py)

## Functions
- `_assert_path_traversal_protection(security_checks: list[dict[str, Any]])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L87)
- `_assert_relevant_security_score(security_checks: list[dict[str, Any]], security_score: float)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L103)
- `_collect_normal_query_check(search_tool: SearchContentTool, query: str, secure_test_project: str)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L165)
- `_collect_normal_query_checks(search_tool: SearchContentTool, queries: Iterable[str], secure_test_project: str)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L154)
- `_collect_normal_search_check(search_tool: SearchContentTool, secure_test_project: str)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L201)
- `_collect_path_traversal_check(scale_tool: AnalyzeScaleTool, attack_path: str)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L132)
- `_collect_path_traversal_checks(scale_tool: AnalyzeScaleTool, attack_paths: Iterable[str])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L122)
- `_print_comprehensive_security_summary(total_checks: int, blocked_checks: list[dict[str, Any]], failed_checks: list[dict[str, Any]], security_score: float)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L69)
- `assert_comprehensive_security_checks(security_checks: list[dict[str, Any]])` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L48) — Assert and report comprehensive security validation results.
- `collect_comprehensive_security_checks(secure_test_project: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L23) — Run the mixed checks used by the comprehensive security test.

## Module values
- `NORMAL_QUERY_CHECKS` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L16)
- `PATH_TRAVERSAL_CHECKS` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_comprehensive_security_helpers.py#L11)

