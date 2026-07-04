---
title: 'Module: tests/unit/mcp/test_security_scanner.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_security_scanner.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_security_scanner`/
symbols:
  test_file_health_does_not_report_test_asserts_as_prod_security_smell: test_file_health_does_not_report_test_asserts_as_prod_security_smell().
  test_python_asserts_are_reported_in_source_files: test_python_asserts_are_reported_in_source_files().
  test_python_asserts_are_not_reported_in_test_files: test_python_asserts_are_not_reported_in_test_files().
  test_test_files_still_report_other_security_issues: test_test_files_still_report_other_security_issues().
  test_python_eval_inside_string_or_comment_is_not_reported: test_python_eval_inside_string_or_comment_is_not_reported().
  test_python_hardcoded_secret_detection_still_scans_assignments: test_python_hardcoded_secret_detection_still_scans_assignments().
  test_scanner_rule_samples_do_not_report_as_security_issues: test_scanner_rule_samples_do_not_report_as_security_issues().
  test_python_runtime_security_constructs_are_still_reported: test_python_runtime_security_constructs_are_still_reported().
  _run: _run().
---
# Module: [`tests/unit/mcp/test_security_scanner.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py)

## Functions
- `_run(coro)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L12)
- `test_file_health_does_not_report_test_asserts_as_prod_security_smell(tmp_path)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L116)
- `test_python_asserts_are_not_reported_in_test_files()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L26)
- `test_python_asserts_are_reported_in_source_files()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L16)
- `test_python_eval_inside_string_or_comment_is_not_reported()` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L46)
- `test_python_hardcoded_secret_detection_still_scans_assignments()` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L66)
- `test_python_runtime_security_constructs_are_still_reported()` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L93)
- `test_scanner_rule_samples_do_not_report_as_security_issues()` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L76)
- `test_test_files_still_report_other_security_issues()` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_security_scanner.py#L36)

