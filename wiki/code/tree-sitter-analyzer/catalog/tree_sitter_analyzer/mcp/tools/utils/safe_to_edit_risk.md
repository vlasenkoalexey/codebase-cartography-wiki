---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.safe_to_edit_risk`/
symbols:
  compute_risk: compute_risk().
  build_checklist: build_checklist().
  _test_instructions: _test_instructions().
  RiskFactor: RiskFactor.
  _add_downstream_factor: _add_downstream_factor().
  _add_health_factor: _add_health_factor().
  _add_test_factor: _add_test_factor().
  _add_init_factor: _add_init_factor().
  _add_edit_type_factor: _add_edit_type_factor().
  _add_dependency_factor: _add_dependency_factor().
  build_checklist._strip_number: build_checklist()._strip_number().
  _classify_risk: _classify_risk().
  _risk_instruction: _risk_instruction().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py)

## Functions
- `_add_dependency_factor(factors: list[RiskFactor], dep_count: int)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L227) — Add risk for files with a broad interaction surface.
- `_add_downstream_factor(factors: list[RiskFactor], forward_count: int)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L77) — Add downstream blast-radius risk.
- `_add_edit_type_factor(factors: list[RiskFactor], edit_type: str, forward_count: int)` — [`L167`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L167) — Add risk based on the planned edit type.
- `_add_health_factor(factors: list[RiskFactor], health_grade: str)` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L109) — Add risk for files that are already fragile.
- `_add_init_factor(factors: list[RiskFactor], is_init_file: bool)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L153) — Add risk for package boundary files.
- `_add_test_factor(factors: list[RiskFactor], has_tests: bool)` — [`L132`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L132) — Add risk or confidence based on nearby tests.
- `_classify_risk(score: int)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L241) — Map numeric risk score to safe/caution/dangerous.
- `_risk_instruction(risk: str)` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L250) — Return the first checklist item for a risk level.
- `_strip_number(text: str)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L71)
- `_test_instructions(has_tests: bool, test_files: list[str], project_root: str | Path | None)` — [`L259`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L259) — Return checklist items for test coverage.
- `build_checklist(risk: str, downstream_count: int, has_tests: bool, test_files: list[str], edit_type: str, health_grade: str = "", file_path: str = "", project_root: str | Path | None = None)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L34) — Build a pre-edit checklist for the AI agent.
- `compute_risk(forward_count: int, dep_count: int, health_grade: str, has_tests: bool, edit_type: str, is_init_file: bool)` — [`L12`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L12) — Compute risk level and contributing factors.

## Module values
- `RiskFactor` — [`L9`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.py#L9)

