---
title: 'Module: tests/unit/test_ci_routing.py'
type: catalog
provenance: extracted
module: tests/unit/test_ci_routing.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ci_routing`/
symbols:
  CONFIG: CONFIG.
  test_docs_only_change_skips_matrix_runs_docs_check: test_docs_only_change_skips_matrix_runs_docs_check().
  test_readme_change_is_docs_only_but_docs_check_guards_counts: test_readme_change_is_docs_only_but_docs_check_guards_counts().
  test_docs_plus_code_change_runs_full_matrix: test_docs_plus_code_change_runs_full_matrix().
  test_empty_changeset_is_not_docs_only: test_empty_changeset_is_not_docs_only().
  test_ci_workflow_md_change_is_not_docs_only: test_ci_workflow_md_change_is_not_docs_only().
  test_sql_plugin_change_routes_sql_and_grammar: test_sql_plugin_change_routes_sql_and_grammar().
  test_workflow_change_forces_full_suite: test_workflow_change_forces_full_suite().
  test_regression_scope_is_narrow_when_only_api_changes: test_regression_scope_is_narrow_when_only_api_changes().
  test_multiple_regression_scopes_upgrade_to_all: test_multiple_regression_scopes_upgrade_to_all().
  PROJECT_ROOT: PROJECT_ROOT.
---
# Module: [`tests/unit/test_ci_routing.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py)

## Functions
- `test_ci_workflow_md_change_is_not_docs_only()` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L55) — A workflow/config change that happens to be docs-shaped still forces the
- `test_docs_only_change_skips_matrix_runs_docs_check()` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L11) — A pure docs change skips the heavy Win/macOS test matrix + build, and
- `test_docs_plus_code_change_runs_full_matrix()` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L37) — A change that touches BOTH docs and code is NOT docs-only — the full
- `test_empty_changeset_is_not_docs_only()` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L48) — An empty changed-file list must not be misclassified as docs-only.
- `test_multiple_regression_scopes_upgrade_to_all()` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L88)
- `test_readme_change_is_docs_only_but_docs_check_guards_counts()` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L29) — README.md is docs-only (skips the matrix) but docs-check runs the
- `test_regression_scope_is_narrow_when_only_api_changes()` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L81)
- `test_sql_plugin_change_routes_sql_and_grammar()` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L63)
- `test_workflow_change_forces_full_suite()` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L72)

## Module values
- `CONFIG` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L8)
- `PROJECT_ROOT` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ci_routing.py#L7)

