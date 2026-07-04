---
title: 'Module: tests/integration/_test_phase7_sensitive_exposure_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_sensitive_exposure_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_sensitive_exposure_helpers`/
symbols:
  _check_sensitive_exposure_pattern: _check_sensitive_exposure_pattern().
  collect_sensitive_exposure_results: collect_sensitive_exposure_results().
  _build_sensitive_exposure_result: _build_sensitive_exposure_result().
  _matches_are_sanitized: _matches_are_sanitized().
  create_sensitive_data_patterns: create_sensitive_data_patterns().
  UNSANITIZED_SECRET_FRAGMENTS: UNSANITIZED_SECRET_FRAGMENTS.
---
# Module: [`tests/integration/_test_phase7_sensitive_exposure_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py)

## Functions
- `_build_sensitive_exposure_result(pattern: str, result: dict[str, Any])` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L75)
- `_check_sensitive_exposure_pattern(search_tool: SearchContentTool, pattern: str, secure_test_project: str)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L51)
- `_matches_are_sanitized(matches: Iterable[dict[str, Any]])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L96)
- `collect_sensitive_exposure_results(search_tool: SearchContentTool, sensitive_patterns: Iterable[str], secure_test_project: str)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L31) — Search sensitive patterns and verify matches are sanitized.
- `create_sensitive_data_patterns()` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L17) — Return patterns that should not expose raw sensitive fixture data.

## Module values
- `UNSANITIZED_SECRET_FRAGMENTS` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_sensitive_exposure_helpers.py#L8)

