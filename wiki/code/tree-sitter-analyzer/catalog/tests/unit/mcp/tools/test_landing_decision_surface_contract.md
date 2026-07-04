---
title: 'Module: tests/unit/mcp/tools/test_landing_decision_surface_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_landing_decision_surface_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_landing_decision_surface_contract`/
symbols:
  TestLandingDecisionSurfaceVerdict.test_project_overview_has_verdict: TestLandingDecisionSurfaceVerdict#test_project_overview_has_verdict().
  TestLandingDecisionSurfaceVerdict.test_project_health_has_verdict: TestLandingDecisionSurfaceVerdict#test_project_health_has_verdict().
  TestLandingDecisionSurfaceVerdict.test_change_impact_has_verdict: TestLandingDecisionSurfaceVerdict#test_change_impact_has_verdict().
  TestLandingDecisionSurfaceVerdict.test_agent_workflow_has_verdict: TestLandingDecisionSurfaceVerdict#test_agent_workflow_has_verdict().
  TestLandingDecisionSurfaceVerdict.test_agent_skills_has_verdict: TestLandingDecisionSurfaceVerdict#test_agent_skills_has_verdict().
  _assert_canonical_verdict: _assert_canonical_verdict().
  TestLandingAgentSummaryMirror.test_project_health_mirrors_verdict: TestLandingAgentSummaryMirror#test_project_health_mirrors_verdict().
  TestLandingAgentSummaryMirror.test_change_impact_mirrors_verdict: TestLandingAgentSummaryMirror#test_change_impact_mirrors_verdict().
  _run: _run().
  _LEGAL_VERDICTS: _LEGAL_VERDICTS.
  tiny_project: tiny_project().
  TestLandingDecisionSurfaceVerdict: TestLandingDecisionSurfaceVerdict#
  TestLandingAgentSummaryMirror: TestLandingAgentSummaryMirror#
---
# Module: [`tests/unit/mcp/tools/test_landing_decision_surface_contract.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py)

## Classes
### `TestLandingAgentSummaryMirror`
- def: [`tests/unit/mcp/tools/test_landing_decision_surface_contract.py:125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L125)
- doc: When agent_summary is present, verdict must mirror at both surfaces.
- signature: `class TestLandingAgentSummaryMirror:`
- members:
  - `test_change_impact_mirrors_verdict(self, tiny_project: Path)` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L148)
  - `test_project_health_mirrors_verdict(self, tiny_project: Path)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L133)
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.execute), [`ChangeImpactTool`](../../../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool), [`ProjectHealthTool`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool.execute)  (1 test-only)

### `TestLandingDecisionSurfaceVerdict`
- def: [`tests/unit/mcp/tools/test_landing_decision_surface_contract.py:69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L69)
- doc: Each tool tsa-landing reads MUST emit a verdict.
- signature: `class TestLandingDecisionSurfaceVerdict:`
- members:
  - `test_agent_skills_has_verdict(self, tiny_project: Path)` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L115)
  - `test_agent_workflow_has_verdict(self, tiny_project: Path)` — [`L99`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L99)
  - `test_change_impact_has_verdict(self, tiny_project: Path)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L90)
  - `test_project_health_has_verdict(self, tiny_project: Path)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L81)
  - `test_project_overview_has_verdict(self, tiny_project: Path)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L72)
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.execute), [`ChangeImpactTool`](../../../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool), [`ProjectOverviewTool`](../../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/agent_workflow_tool.md#AgentWorkflowTool.execute), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute), [`ProjectHealthTool`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool.execute), [`AgentWorkflowTool`](../../../../tree_sitter_analyzer/mcp/tools/agent_workflow_tool.md#AgentWorkflowTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/agent_skills_tool.md#AgentSkillsTool.execute), [`AgentSkillsTool`](../../../../tree_sitter_analyzer/mcp/tools/agent_skills_tool.md#AgentSkillsTool)  (2 test-only)

## Functions
- `_assert_canonical_verdict(result: dict, tool_name: str)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L51) — A landing-tool result must have a canonical verdict at top-level.
- `_run(coro)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L45)
- `tiny_project(tmp_path: Path)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L37) — A 1-file project sufficient for every landing tool to run.

## Module values
- `_LEGAL_VERDICTS` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_landing_decision_surface_contract.py#L31)

