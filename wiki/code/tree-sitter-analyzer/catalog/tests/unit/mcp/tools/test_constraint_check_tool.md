---
title: 'Module: tests/unit/mcp/tools/test_constraint_check_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_constraint_check_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_constraint_check_tool`/
symbols:
  TestConstraintCheckVerdict.test_check_constraints_returns_violation_list: TestConstraintCheckVerdict#test_check_constraints_returns_violation_list().
  TestConstraintCheckVerdict.test_check_constraints_verdict_unsafe_when_error_severity: TestConstraintCheckVerdict#test_check_constraints_verdict_unsafe_when_error_severity().
  TestConstraintCheckVerdict.test_check_constraints_verdict_caution_when_only_warn: TestConstraintCheckVerdict#test_check_constraints_verdict_caution_when_only_warn().
  TestConstraintCheckFiltering.test_path_filter_narrows_results: TestConstraintCheckFiltering#test_path_filter_narrows_results().
  TestConstraintCheckVerdict.test_check_constraints_verdict_safe_when_no_violations: TestConstraintCheckVerdict#test_check_constraints_verdict_safe_when_no_violations().
  _make_tool: _make_tool().
  _run: _run().
  _init_violations_db: _init_violations_db().
  _seed_violation: _seed_violation().
  _stage_minimal_constraints: _stage_minimal_constraints().
  TestConstraintCheckVerdict: TestConstraintCheckVerdict#
  TestConstraintCheckFiltering: TestConstraintCheckFiltering#
---
# Module: [`tests/unit/mcp/tools/test_constraint_check_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py)

## Classes
### `TestConstraintCheckFiltering`
- def: [`tests/unit/mcp/tools/test_constraint_check_tool.py:265`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L265)
- doc: Optional `path_filter` narrows results by caller-file glob.
- signature: `class TestConstraintCheckFiltering:`
- members:
  - `test_path_filter_narrows_results(self, tmp_path: Path)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L268) — Filter is applied against ``caller_file`` and respects ``**``.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/constraint_check_tool.md#ConstraintCheckTool.execute)  (5 test-only)

### `TestConstraintCheckVerdict`
- def: [`tests/unit/mcp/tools/test_constraint_check_tool.py:160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L160)
- doc: Map violations to canonical verdict vocabulary.
- signature: `class TestConstraintCheckVerdict:`
- members:
  - `test_check_constraints_returns_violation_list(self, tmp_path: Path)` — [`L163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L163) — Happy path: at least one violation surfaces with a rule_count >= 1.
  - `test_check_constraints_verdict_caution_when_only_warn(self, tmp_path: Path)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L216) — Only warn-severity violations → ``CAUTION`` (not ``UNSAFE``).
  - `test_check_constraints_verdict_safe_when_no_violations(self, tmp_path: Path)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L239) — Constraints loaded, zero violations → ``SAFE``.
  - `test_check_constraints_verdict_unsafe_when_error_severity(self, tmp_path: Path)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L188) — Error-severity violation must escalate to ``UNSAFE``.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/constraint_check_tool.md#ConstraintCheckTool.execute)  (5 test-only)

## Functions
- `_init_violations_db(db_path: Path)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L52) — Create the ``ast_constraint_violations`` table per spec.
- `_make_tool(project_root: Path)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L144) — Construct ``ConstraintCheckTool`` bound to ``project_root``.
- `_run(coro)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L47) — Drive a coroutine to completion under pytest's per-test event loop.
- `_seed_violation(db_path: Path, *, rule_id: str, caller_file: str, callee_file: str, severity: str, caller_line: int = 1, callee_name: str = "callee_fn", caller_name: str = "caller_fn")` — [`L82`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L82) — Insert a single synthetic violation row.
- `_stage_minimal_constraints(project: Path)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_constraint_check_tool.py#L123) — Write a 1-rule architectural-constraints.yml into the project.

