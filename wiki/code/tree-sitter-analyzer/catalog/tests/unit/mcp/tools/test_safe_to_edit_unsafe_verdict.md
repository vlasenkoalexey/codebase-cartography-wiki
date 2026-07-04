---
title: 'Module: tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_safe_to_edit_unsafe_verdict`/
symbols:
  TestSafeToEditConstraintIntegration.test_safe_to_edit_emits_UNSAFE_on_error_violation: TestSafeToEditConstraintIntegration#test_safe_to_edit_emits_UNSAFE_on_error_violation().
  TestSafeToEditConstraintIntegration.test_summary_line_matches_escalated_verdict: TestSafeToEditConstraintIntegration#test_summary_line_matches_escalated_verdict().
  TestSafeToEditConstraintIntegration.test_recommendation_matches_escalated_verdict: TestSafeToEditConstraintIntegration#test_recommendation_matches_escalated_verdict().
  TestSafeToEditConstraintIntegration.test_safe_to_edit_emits_CAUTION_on_warn_violation: TestSafeToEditConstraintIntegration#test_safe_to_edit_emits_CAUTION_on_warn_violation().
  TestChangeImpactConstraintIntegration.test_change_impact_includes_constraint_violations_field: TestChangeImpactConstraintIntegration#test_change_impact_includes_constraint_violations_field().
  TARGET_FILE_REL: TARGET_FILE_REL.
  _make_safe_to_edit_tool: _make_safe_to_edit_tool().
  _scaffold_min_project: _scaffold_min_project().
  _make_change_impact_tool: _make_change_impact_tool().
  _run: _run().
  _init_violations_db: _init_violations_db().
  _seed_violation: _seed_violation().
  _stage_dogfood_constraints: _stage_dogfood_constraints().
  TestSafeToEditConstraintIntegration: TestSafeToEditConstraintIntegration#
  TestChangeImpactConstraintIntegration: TestChangeImpactConstraintIntegration#
---
# Module: [`tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py)

## Classes
### `TestChangeImpactConstraintIntegration`
- def: [`tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py:327`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L327)
- doc: analyze_change_impact must expose `constraint_violations`.
- signature: `class TestChangeImpactConstraintIntegration:`
- members:
  - `test_change_impact_includes_constraint_violations_field(self, tmp_path: Path)` — [`L330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L330) — When the diff touches a forbidden caller, surface the violation.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.execute)  (7 test-only)

### `TestSafeToEditConstraintIntegration`
- def: [`tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py:163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L163)
- doc: An error-severity violation on the target file must promote verdict.
- signature: `class TestSafeToEditConstraintIntegration:`
- members:
  - `test_recommendation_matches_escalated_verdict(self, tmp_path: Path)` — [`L255`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L255) — #1027: ``recommendation`` must agree with the escalated ``verdict``.
  - `test_safe_to_edit_emits_CAUTION_on_warn_violation(self, tmp_path: Path)` — [`L291`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L291) — Only warn-severity → CAUTION (not the legacy ``REVIEW``).
  - `test_safe_to_edit_emits_UNSAFE_on_error_violation(self, tmp_path: Path)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L166) — Pre-existing error-severity violation → safe_to_edit returns UNSAFE.
  - `test_summary_line_matches_escalated_verdict(self, tmp_path: Path)` — [`L219`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L219) — #781: an escalated verdict must reach the summary_line too.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.md#SafeToEditTool.execute)  (7 test-only)

## Functions
- `_init_violations_db(db_path: Path)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L67)
- `_make_change_impact_tool(project_root: Path)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L149)
- `_make_safe_to_edit_tool(project_root: Path)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L141)
- `_run(coro)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L45)
- `_scaffold_min_project(tmp_path: Path)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L49) — Create the minimum directory shape the SafeToEditTool needs.
- `_seed_violation(db_path: Path, *, rule_id: str, caller_file: str, severity: str, callee_file: str = "tree_sitter_analyzer/cli/y.py", caller_line: int = 1)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L91)
- `_stage_dogfood_constraints(project: Path)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L125) — Drop a minimal architectural-constraints.yml so the loader has rules.

## Module values
- `TARGET_FILE_REL` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_unsafe_verdict.py#L42)

