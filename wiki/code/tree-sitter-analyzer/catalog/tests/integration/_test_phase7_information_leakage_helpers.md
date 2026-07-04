---
title: 'Module: tests/integration/_test_phase7_information_leakage_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_information_leakage_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_information_leakage_helpers`/
symbols:
  _build_result_leakage_summary: _build_result_leakage_summary().
  create_information_leakage_test_cases: create_information_leakage_test_cases().
  _build_exception_leakage_summary: _build_exception_leakage_summary().
  _collect_information_leakage_result: _collect_information_leakage_result().
  collect_information_leakage_results: collect_information_leakage_results().
  _contains_any: _contains_any().
  _truncate_error_message: _truncate_error_message().
  SENSITIVE_ERROR_FRAGMENTS: SENSITIVE_ERROR_FRAGMENTS.
  SENSITIVE_EXCEPTION_FRAGMENTS: SENSITIVE_EXCEPTION_FRAGMENTS.
  SENSITIVE_PATH_FRAGMENTS: SENSITIVE_PATH_FRAGMENTS.
---
# Module: [`tests/integration/_test_phase7_information_leakage_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py)

## Functions
- `_build_exception_leakage_summary(description: str, exc: Exception)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L103)
- `_build_result_leakage_summary(description: str, result: dict[str, Any])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L84)
- `_collect_information_leakage_result(test_case: dict[str, Any])` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L74)
- `_contains_any(value: str, fragments: Iterable[str])` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L121)
- `_truncate_error_message(error_message: str)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L125)
- `collect_information_leakage_results(error_test_cases: Iterable[dict[str, Any]])` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L64) — Execute error cases and summarize leakage safety.
- `create_information_leakage_test_cases(secure_test_project: str)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L38) — Return tool calls that should not leak sensitive path details.

## Module values
- `SENSITIVE_ERROR_FRAGMENTS` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L10)
- `SENSITIVE_EXCEPTION_FRAGMENTS` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L23)
- `SENSITIVE_PATH_FRAGMENTS` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_information_leakage_helpers.py#L31)

