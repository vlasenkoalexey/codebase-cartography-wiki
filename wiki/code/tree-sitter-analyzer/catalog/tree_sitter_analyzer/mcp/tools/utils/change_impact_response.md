---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.change_impact_response`/
symbols:
  build_agent_summary: build_agent_summary().
  build_change_impact_response: build_change_impact_response().
  apply_scope_validation: apply_scope_validation().
  AgentSummaryContext.changed_files: AgentSummaryContext#changed_files.
  build_agent_summary_only_response: build_agent_summary_only_response().
  attach_queue_ledger: attach_queue_ledger().
  AgentSummaryContext: AgentSummaryContext#
  AgentSummaryContext.risk: AgentSummaryContext#risk.
  AgentSummaryContext.scope_paths: AgentSummaryContext#scope_paths.
  AgentSummaryContext.verification: AgentSummaryContext#verification.
  AgentSummaryContext.strategy: AgentSummaryContext#strategy.
  AgentSummaryContext.affected_count: AgentSummaryContext#affected_count.
  AgentSummaryContext.tests_to_run_count: AgentSummaryContext#tests_to_run_count.
  build_no_changes_result: build_no_changes_result().
  CHANGE_IMPACT_PREVIEW_LIMIT: CHANGE_IMPACT_PREVIEW_LIMIT.
  ChangeImpactResponseContext: ChangeImpactResponseContext#
  ChangeImpactResponseContext.affected: ChangeImpactResponseContext#affected.
  ChangeImpactResponseContext.risk: ChangeImpactResponseContext#risk.
  ChangeImpactResponseContext.visible_tests: ChangeImpactResponseContext#visible_tests.
  ChangeImpactResponseContext.all_tests: ChangeImpactResponseContext#all_tests.
  ChangeImpactResponseContext.test_mapping: ChangeImpactResponseContext#test_mapping.
  ChangeImpactResponseContext.request: ChangeImpactResponseContext#request.
  ChangeImpactResponseContext.file_impacts: ChangeImpactResponseContext#file_impacts.
  ChangeImpactResponseContext.verification: ChangeImpactResponseContext#verification.
  ChangeImpactResponseContext.strategy: ChangeImpactResponseContext#strategy.
  ChangeImpactResponseContext.agent_summary: ChangeImpactResponseContext#agent_summary.
  _reconcile_envelope_verdict: _reconcile_envelope_verdict().
  _VERDICT_SEVERITY._VERDICT_SEVERITY: _VERDICT_SEVERITY._VERDICT_SEVERITY.
  LARGE_DIRTY_DIFF_THRESHOLD: LARGE_DIRTY_DIFF_THRESHOLD.
  _effective_verification_command: _effective_verification_command().
  CHANGE_IMPACT_VERDICT_CLEAN: CHANGE_IMPACT_VERDICT_CLEAN.
  CHANGE_IMPACT_VERDICT_REVIEW: CHANGE_IMPACT_VERDICT_REVIEW.
  CHANGE_IMPACT_VERDICT_WARN: CHANGE_IMPACT_VERDICT_WARN.
  _change_impact_risk_to_verdict: _change_impact_risk_to_verdict().
  _queue_ledger_handoff: _queue_ledger_handoff().
  _agent_next_step: _agent_next_step().
  _agent_stop_condition: _agent_stop_condition().
  _resolve_changed_count: _resolve_changed_count().
  _augment_summary_line: _augment_summary_line().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py)

## Classes
### `AgentSummaryContext`
- def: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py:98`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L98)
- members:
  - `affected_count` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L106)
  - `changed_files` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L102)
  - `risk` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L101)
  - `scope_paths` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L103)
  - `strategy` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L105)
  - `tests_to_run_count` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L107)
  - `verification` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L104)
- used by: [`_build_change_impact_result`](change_impact_analysis.md#_build_change_impact_result), [`_build_test_only_change_impact_result`](change_impact_analysis.md#_build_test_only_change_impact_result), [`build_agent_summary`](change_impact_response.md#build_agent_summary)  (11 test-only)

### `ChangeImpactResponseContext`
- def: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py:111`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L111)
- doc: Computed parts for assembling a change-impact response.
- signature: `class ChangeImpactResponseContext:`
- members:
  - `affected` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L116)
  - `agent_summary` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L123)
  - `all_tests` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L119)
  - `file_impacts` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L117)
  - `request` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L114)
  - `risk` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L115)
  - `strategy` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L121)
  - `test_mapping` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L122)
  - `verification` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L120)
  - `visible_tests` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L118)
- used by: [`_build_change_impact_result`](change_impact_analysis.md#_build_change_impact_result), [`_build_test_only_change_impact_result`](change_impact_analysis.md#_build_test_only_change_impact_result), [`build_change_impact_response`](change_impact_response.md#build_change_impact_response)  (3 test-only)

## Functions
- `_agent_next_step(verification: dict[str, Any], strategy: dict[str, Any])` — [`L432`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L432) — Return one concise next action for agent decision-making.
- `_agent_stop_condition(risk: str, verification: dict[str, Any], strategy: dict[str, Any])` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L451) — Describe when the current edit queue can be considered closed.
- `_augment_summary_line(result: dict[str, Any], agent_summary: dict[str, Any], scope_paths_invalid: list[str])` — [`L577`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L577) — Append a ``scope_invalid=N`` token to both summary_line surfaces.
- `_change_impact_risk_to_verdict(risk: str)` — [`L156`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L156) — Map change-impact risk to canonical verdict vocabulary (CLAUDE.md).
- `_effective_verification_command(verification: dict[str, Any], strategy: dict[str, Any])` — [`L485`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L485) — Return the command the local agent should run for this response.
- `_queue_ledger_handoff(scope_paths: list[str], scoped_changed_files: list[str], out_of_scope: list[str], verification_command: str)` — [`L348`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L348) — Build one compact queue handoff sentence.
- `_reconcile_envelope_verdict(result: dict[str, Any], agent_summary: dict[str, Any])` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L73) — Force top-level ``verdict`` and ``agent_summary["verdict"]`` to agree.
- `_resolve_changed_count(result: dict[str, Any], agent_summary: dict[str, Any])` — [`L555`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L555) — Best-effort lookup of ``changed_count`` across response shapes.
- `apply_scope_validation(result: dict[str, Any], scope_paths_invalid: list[str])` — [`L497`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L497) — H8 / J11: surface nonexistent scope paths and a content-aware verdict.
- `attach_queue_ledger(result: dict[str, Any], *, mode: str, scope_paths: list[str] | None, scoped_changed_files: list[str], workspace_changed_files: list[str], scope_mode: str = "report")` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L274) — Attach a lightweight scoped dirty-worktree ledger for agent handoffs.
- `build_agent_summary(context: AgentSummaryContext)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L221) — Build the compact decision surface agents need from change-impact.
- `build_agent_summary_only_response(result: dict[str, Any])` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L170) — Return a compact change-impact response for agent decision loops.
- `build_change_impact_response(context: ChangeImpactResponseContext)` — [`L363`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L363) — Assemble the final response without mixing computation and formatting.
- `build_no_changes_result(mode: str, scope_paths: list[str] | None = None)` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L126) — Build a stable empty-diff response.

## Module values
- `CHANGE_IMPACT_PREVIEW_LIMIT` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L17)
- `CHANGE_IMPACT_VERDICT_CLEAN` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L50)
- `CHANGE_IMPACT_VERDICT_REVIEW` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L51)
- `CHANGE_IMPACT_VERDICT_WARN` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L52)
- `LARGE_DIRTY_DIFF_THRESHOLD` — [`L8`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L8)
- `_VERDICT_SEVERITY` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_response.py#L61)

