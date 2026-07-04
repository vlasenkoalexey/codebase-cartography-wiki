---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/verification_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/verification_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.verification_command`/
symbols:
  DefaultTestCommand: DefaultTestCommand#
  detect_default_test_command: detect_default_test_command().
  build_test_command: build_test_command().
  DefaultTestCommand.runner: DefaultTestCommand#runner.
  PYTEST_COMMAND: PYTEST_COMMAND.
  DefaultTestCommand.command: DefaultTestCommand#command.
  _node_test_command: _node_test_command().
  PYTEST_DEFAULT_COMMAND: PYTEST_DEFAULT_COMMAND.
  _package_json_has_test_script: _package_json_has_test_script().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/verification_command.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py)

## Classes
### `DefaultTestCommand`
- def: [`tree_sitter_analyzer/mcp/tools/utils/verification_command.py:13`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L13)
- doc: Default test command detected for a project root.
- signature: `class DefaultTestCommand:`
- members:
  - `command` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L17)
  - `runner` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L16)
- used by: [`_build_verification_plan`](change_impact_verification.md#_build_verification_plan), [`build_agent_workflow`](safe_to_edit_helpers.md#build_agent_workflow), [`_build_verification_strategy`](change_impact_analysis.md#_build_verification_strategy), [`detect_default_test_command`](verification_command.md#detect_default_test_command), [`build_test_command`](verification_command.md#build_test_command), [`PYTEST_COMMAND`](verification_command.md#PYTEST_COMMAND), [`_test_instructions`](safe_to_edit_risk.md#_test_instructions), [`_node_test_command`](verification_command.md#_node_test_command)  (9 test-only)

## Functions
- `_node_test_command(root: Path)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L83) — Choose the local Node package manager's test command.
- `_package_json_has_test_script(package_json: Path)` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L73) — Return True when package.json has a non-empty scripts.test entry.
- `build_test_command(default_command: DefaultTestCommand, tests_to_run: list[str])` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L53) — Build a verification command, using targeted tests when the runner supports it.
- `detect_default_test_command(project_root: str | Path | None)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L24) — Detect a directly runnable default test command for a project root.

## Module values
- `PYTEST_COMMAND` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L21)
- `PYTEST_DEFAULT_COMMAND` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/verification_command.py#L20)

