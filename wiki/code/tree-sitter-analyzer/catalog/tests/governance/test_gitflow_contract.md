---
title: 'Module: tests/governance/test_gitflow_contract.py'
type: catalog
provenance: extracted
module: tests/governance/test_gitflow_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.governance.test_gitflow_contract`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  test_gitflow_documentation_is_present: test_gitflow_documentation_is_present().
  test_gitflow_guard_does_not_allow_bot_prs_to_main: test_gitflow_guard_does_not_allow_bot_prs_to_main().
  test_release_and_hotfix_prs_use_gitflow_branch_heads: test_release_and_hotfix_prs_use_gitflow_branch_heads().
  test_release_and_hotfix_finalize_prs_do_not_mask_closed_prs: test_release_and_hotfix_finalize_prs_do_not_mask_closed_prs().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/governance/test_gitflow_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py)

## Functions
- `test_gitflow_documentation_is_present()` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L34) — The GitFlow mandate must remain documented + machine-enforced.
- `test_gitflow_guard_does_not_allow_bot_prs_to_main()` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L78) — Bot branch shortcuts must not bypass the protected main release flow.
- `test_release_and_hotfix_finalize_prs_do_not_mask_closed_prs()` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L116) — A closed, unmerged finalize PR means the release/hotfix is not landed.
- `test_release_and_hotfix_prs_use_gitflow_branch_heads()` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L95) — Release/hotfix automation must open main PRs from GitFlow branches.

## Module values
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_gitflow_contract.py#L24)

