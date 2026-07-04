---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.change_impact_verification`/
symbols:
  _build_verification_plan: _build_verification_plan().
  AUTO_DISCOVER_TEST_HINT: AUTO_DISCOVER_TEST_HINT.
  _build_pytest_command: _build_pytest_command().
  DOCS_ONLY_TEST_HINT: DOCS_ONLY_TEST_HINT.
  _requires_pytest: _requires_pytest().
  _has_runtime_auto_discovery: _has_runtime_auto_discovery().
  _is_docs_only_change: _is_docs_only_change().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py)

## Functions
- `_build_pytest_command(tests_to_run: list[str])` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L18) — Build a copy-pasteable fast validation command.
- `_build_verification_plan(changed_files: list[str], tests_to_run: list[str], test_mapping: dict[str, list[str]] | None = None, default_test_command: DefaultTestCommand = PYTEST_COMMAND)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L46) — Build the smallest recommended verification command for the diff.
- `_has_runtime_auto_discovery(test_mapping: dict[str, list[str]])` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L100) — Return True when runtime changes lack a targeted test mapping.
- `_is_docs_only_change(path: str)` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L30) — Return True for documentation-only files that do not need pytest.
- `_requires_pytest(changed_files: list[str])` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L23) — Return False for changes that cannot affect executable behavior.

## Module values
- `AUTO_DISCOVER_TEST_HINT` — [`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L14)
- `DOCS_ONLY_TEST_HINT` — [`L15`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_verification.py#L15)

