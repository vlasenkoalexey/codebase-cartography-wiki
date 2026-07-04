---
title: 'Module: tests/governance/test_postmortem_guards.py'
type: catalog
provenance: extracted
module: tests/governance/test_postmortem_guards.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.governance.test_postmortem_guards`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  test_readme_counts_match_registry: test_readme_counts_match_registry().
  test_postmortem_v1_13_doc_exists: test_postmortem_v1_13_doc_exists().
  test_agents_md_documents_v1_13_anti_patterns: test_agents_md_documents_v1_13_anti_patterns().
  test_check_ps_ascii_script_is_present_and_pre_commit_wired: test_check_ps_ascii_script_is_present_and_pre_commit_wired().
  test_actionlint_is_wired_into_pre_commit: test_actionlint_is_wired_into_pre_commit().
  test_no_powershell_blocks_contain_non_ascii: test_no_powershell_blocks_contain_non_ascii().
  test_skips_have_tracking_references: test_skips_have_tracking_references().
  test_python_version_floor_is_consistent: test_python_version_floor_is_consistent().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/governance/test_postmortem_guards.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py)

## Functions
- `test_actionlint_is_wired_into_pre_commit()` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L106) — actionlint catches the failure class behind PR #138 — dead
- `test_agents_md_documents_v1_13_anti_patterns()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L70) — AGENTS.md must surface the v1.13 anti-patterns so they hit any
- `test_check_ps_ascii_script_is_present_and_pre_commit_wired()` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L87) — The non-ASCII PowerShell guard must remain wired into pre-commit.
- `test_no_powershell_blocks_contain_non_ascii()` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L120) — End-to-end check at test time, complementing the pre-commit hook.
- `test_postmortem_v1_13_doc_exists()` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L39) — The v1.13 postmortem is the source of truth for the anti-patterns
- `test_python_version_floor_is_consistent()` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L237) — The repo's Python floor must be expressed coherently across
- `test_readme_counts_match_registry()` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L278) — README headline numbers must match the actual registry counts.
- `test_skips_have_tracking_references()` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L165) — Every ``pytest.skip``/``pytest.mark.skipif`` MUST carry a tracking

## Module values
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_postmortem_guards.py#L24)

