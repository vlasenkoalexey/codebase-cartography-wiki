---
title: 'Module: scripts/test_mastery_scan.py'
type: catalog
provenance: extracted
module: scripts/test_mastery_scan.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.test_mastery_scan`/
symbols:
  scan: scan().
  main: main().
  count_assertions: count_assertions().
  PROJECT_ROOT: PROJECT_ROOT.
  GATES: GATES.
  _is_counted_call: _is_counted_call().
  count_test_functions: count_test_functions().
  is_auxiliary_test_file: is_auxiliary_test_file().
  print_report: print_report().
---
# Module: [`scripts/test_mastery_scan.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py)

## Functions
- `_is_counted_call(node: ast.Call)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L33) — Return True if an AST Call node counts as an assertion.
- `count_assertions(filepath: Path)` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L41) — Count assert/test statements in a test file — includes AST assert nodes + mock.assert_* calls.
- `count_test_functions(filepath: Path)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L56) — Count test functions and test methods using AST traversal.
- `is_auxiliary_test_file(relative_path: str, assertions: int, tests: int)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L74) — Skip helper-heavy test files from low-density checks.
- `main()` — [`L284`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L284)
- `print_report(data: dict[str, Any])` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L218) — Print formatted report.
- `scan()` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L103) — Full test suite scan.

## Module values
- `GATES` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L23)
- `PROJECT_ROOT` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/scripts/test_mastery_scan.py#L20)

