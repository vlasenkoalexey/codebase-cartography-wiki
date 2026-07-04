---
title: 'Module: tests/unit/test_change_impact_response.py'
type: catalog
provenance: extracted
module: tests/unit/test_change_impact_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_change_impact_response`/
symbols:
  TestBuildChangeImpactResponse.test_full_response: TestBuildChangeImpactResponse#test_full_response().
  TestBuildChangeImpactResponse.test_full_response_exposes_low_impact_local_and_ci_commands: TestBuildChangeImpactResponse#test_full_response_exposes_low_impact_local_and_ci_commands().
  TestBuildChangeImpactResponse.test_empty_affected: TestBuildChangeImpactResponse#test_empty_affected().
  TestBuildAgentSummary.test_basic_summary: TestBuildAgentSummary#test_basic_summary().
  TestBuildAgentSummary.test_changed_preview_limited_to_5: TestBuildAgentSummary#test_changed_preview_limited_to_5().
  TestBuildAgentSummary.test_no_scope_hint_for_small_diff: TestBuildAgentSummary#test_no_scope_hint_for_small_diff().
  TestBuildAgentSummary.test_scope_hint_for_large_unscoped_diff: TestBuildAgentSummary#test_scope_hint_for_large_unscoped_diff().
  TestBuildAgentSummary.test_no_scope_hint_when_scoped: TestBuildAgentSummary#test_no_scope_hint_when_scoped().
  TestBuildAgentSummary.test_focused_test_command_included: TestBuildAgentSummary#test_focused_test_command_included().
  TestBuildAgentSummary.test_local_low_impact_summary_uses_local_command: TestBuildAgentSummary#test_local_low_impact_summary_uses_local_command().
  TestBuildAgentSummary.test_local_low_impact_summary_without_ci_command: TestBuildAgentSummary#test_local_low_impact_summary_without_ci_command().
  TestBuildAgentSummary.test_next_step_with_focused_test: TestBuildAgentSummary#test_next_step_with_focused_test().
  TestBuildAgentSummary.test_stop_condition_no_tests: TestBuildAgentSummary#test_stop_condition_no_tests().
  _make_verification: _make_verification().
  _make_strategy: _make_strategy().
  TestVerdictReconciliation782.test_compact_response_preserves_reconciled_verdict: TestVerdictReconciliation782#test_compact_response_preserves_reconciled_verdict().
  TestVerdictReconciliation782.test_compact_response_keeps_constraint_unsafe: TestVerdictReconciliation782#test_compact_response_keeps_constraint_unsafe().
  test_verdict_severity_rank_matches_journal_rank: test_verdict_severity_rank_matches_journal_rank().
  TestBuildNoChangesResult.test_basic_no_changes: TestBuildNoChangesResult#test_basic_no_changes().
  TestBuildNoChangesResult.test_scoped_mode: TestBuildNoChangesResult#test_scoped_mode().
  TestBuildNoChangesResult.test_unscoped_mode: TestBuildNoChangesResult#test_unscoped_mode().
  TestBuildAgentSummaryOnlyResponse.test_extracts_summary_fields: TestBuildAgentSummaryOnlyResponse#test_extracts_summary_fields().
  TestBuildAgentSummaryOnlyResponse.test_agent_summary_only_preserves_low_impact_fields: TestBuildAgentSummaryOnlyResponse#test_agent_summary_only_preserves_low_impact_fields().
  TestBuildAgentSummaryOnlyResponse.test_agent_summary_only_does_not_emit_contradictory_legacy_scalars: TestBuildAgentSummaryOnlyResponse#test_agent_summary_only_does_not_emit_contradictory_legacy_scalars().
  TestAttachQueueLedger.test_no_ledger_without_scope: TestAttachQueueLedger#test_no_ledger_without_scope().
  TestAttachQueueLedger.test_ledger_with_scope: TestAttachQueueLedger#test_ledger_with_scope().
  TestAttachQueueLedger.test_preview_limited_to_5: TestAttachQueueLedger#test_preview_limited_to_5().
  TestAttachQueueLedger.test_agent_summary_gets_scope_hint: TestAttachQueueLedger#test_agent_summary_gets_scope_hint().
  TestAttachQueueLedger.test_report_mode_is_default_and_keeps_out_of_scope_preview: TestAttachQueueLedger#test_report_mode_is_default_and_keeps_out_of_scope_preview().
  TestAttachQueueLedger.test_strict_mode_mutes_out_of_scope_preview: TestAttachQueueLedger#test_strict_mode_mutes_out_of_scope_preview().
  TestAttachQueueLedger.test_strict_scope_hint_does_not_bury_scoped_message: TestAttachQueueLedger#test_strict_scope_hint_does_not_bury_scoped_message().
  TestVerdictReconciliation782.test_changed_files_lift_top_level_to_review: TestVerdictReconciliation782#test_changed_files_lift_top_level_to_review().
  TestVerdictReconciliation782.test_constraint_escalation_is_not_downgraded: TestVerdictReconciliation782#test_constraint_escalation_is_not_downgraded().
  TestVerdictReconciliation782.test_no_changes_stays_benign_and_agrees: TestVerdictReconciliation782#test_no_changes_stays_benign_and_agrees().
  TestVerdictReconciliation782.test_reconcile_no_ops_when_a_verdict_is_missing: TestVerdictReconciliation782#test_reconcile_no_ops_when_a_verdict_is_missing().
  TestBuildNoChangesResult: TestBuildNoChangesResult#
  TestBuildAgentSummary: TestBuildAgentSummary#
  TestBuildAgentSummaryOnlyResponse: TestBuildAgentSummaryOnlyResponse#
  TestAttachQueueLedger: TestAttachQueueLedger#
  TestBuildChangeImpactResponse: TestBuildChangeImpactResponse#
  TestVerdictReconciliation782: TestVerdictReconciliation782#
---
# Module: [`tests/unit/test_change_impact_response.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py)

## Classes
### `TestAttachQueueLedger`
- def: [`tests/unit/test_change_impact_response.py:370`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L370)
- doc: Tests for attach_queue_ledger.
- signature: `class TestAttachQueueLedger:`
- members:
  - `test_agent_summary_gets_scope_hint(self)` — [`L410`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L410)
  - `test_ledger_with_scope(self)` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L384)
  - `test_no_ledger_without_scope(self)` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L373)
  - `test_preview_limited_to_5(self)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L399)
  - `test_report_mode_is_default_and_keeps_out_of_scope_preview(self)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L421) — Default ``scope_mode`` (report) preserves today's behavior: the
  - `test_strict_mode_mutes_out_of_scope_preview(self)` — [`L438`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L438) — ``scope_mode='strict'`` fully mutes the out-of-scope dirty file list
  - `test_strict_scope_hint_does_not_bury_scoped_message(self)` — [`L458`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L458) — In strict mode the scope_hint leads with the scoped queue and clearly
- uses (calls/refs, reference-scoped): [`attach_queue_ledger`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#attach_queue_ledger)

### `TestBuildAgentSummary`
- def: [`tests/unit/test_change_impact_response.py:58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L58)
- doc: Tests for build_agent_summary.
- signature: `class TestBuildAgentSummary:`
- members:
  - `test_basic_summary(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L61)
  - `test_changed_preview_limited_to_5(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L78)
  - `test_focused_test_command_included(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L131)
  - `test_local_low_impact_summary_uses_local_command(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L144)
  - `test_local_low_impact_summary_without_ci_command(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L187)
  - `test_next_step_with_focused_test(self)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L215)
  - `test_no_scope_hint_for_small_diff(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L91)
  - `test_no_scope_hint_when_scoped(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L118)
  - `test_scope_hint_for_large_unscoped_diff(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L104)
  - `test_stop_condition_no_tests(self)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L228)
- uses (calls/refs, reference-scoped): [`build_agent_summary`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#build_agent_summary), [`changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.changed_files), [`AgentSummaryContext`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext), [`risk`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.risk), [`scope_paths`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.scope_paths), [`affected_count`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.affected_count), [`strategy`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.strategy), [`tests_to_run_count`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.tests_to_run_count), [`verification`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#AgentSummaryContext.verification)  (2 test-only)

### `TestBuildAgentSummaryOnlyResponse`
- def: [`tests/unit/test_change_impact_response.py:242`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L242)
- doc: Tests for build_agent_summary_only_response.
- signature: `class TestBuildAgentSummaryOnlyResponse:`
- members:
  - `test_agent_summary_only_does_not_emit_contradictory_legacy_scalars(self)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L334) — Compact mode must not expose stale top-level fields that fight summary.
  - `test_agent_summary_only_preserves_low_impact_fields(self)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L271)
  - `test_extracts_summary_fields(self)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L245)
- uses (calls/refs, reference-scoped): [`build_agent_summary_only_response`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#build_agent_summary_only_response)

### `TestBuildChangeImpactResponse`
- def: [`tests/unit/test_change_impact_response.py:475`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L475)
- doc: Tests for build_change_impact_response.
- signature: `class TestBuildChangeImpactResponse:`
- members:
  - `test_empty_affected(self)` — [`L550`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L550)
  - `test_full_response(self)` — [`L478`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L478)
  - `test_full_response_exposes_low_impact_local_and_ci_commands(self)` — [`L508`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L508)
- uses (calls/refs, reference-scoped): [`build_change_impact_response`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#build_change_impact_response), [`ChangeImpactResponseContext`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext), [`affected`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.affected), [`all_tests`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.all_tests), [`risk`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.risk), [`test_mapping`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.test_mapping), [`visible_tests`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.visible_tests), [`agent_summary`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.agent_summary), [`file_impacts`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.file_impacts), [`request`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.request), [`strategy`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.strategy), [`verification`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#ChangeImpactResponseContext.verification)  (2 test-only)

### `TestBuildNoChangesResult`
- def: [`tests/unit/test_change_impact_response.py:39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L39)
- doc: Tests for build_no_changes_result.
- signature: `class TestBuildNoChangesResult:`
- members:
  - `test_basic_no_changes(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L42)
  - `test_scoped_mode(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L49)
  - `test_unscoped_mode(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L53)
- uses (calls/refs, reference-scoped): [`build_no_changes_result`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#build_no_changes_result)

### `TestVerdictReconciliation782`
- def: [`tests/unit/test_change_impact_response.py:575`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L575)
- doc: #782: top-level verdict and agent_summary.verdict must agree (more
- signature: `class TestVerdictReconciliation782:`
- members:
  - `test_changed_files_lift_top_level_to_review(self)` — [`L581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L581)
  - `test_compact_response_keeps_constraint_unsafe(self)` — [`L630`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L630)
  - `test_compact_response_preserves_reconciled_verdict(self)` — [`L616`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L616)
  - `test_constraint_escalation_is_not_downgraded(self)` — [`L589`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L589)
  - `test_no_changes_stays_benign_and_agrees(self)` — [`L601`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L601)
  - `test_reconcile_no_ops_when_a_verdict_is_missing(self)` — [`L606`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L606)
- uses (calls/refs, reference-scoped): [`apply_scope_validation`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#apply_scope_validation), [`build_agent_summary_only_response`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_response.md#build_agent_summary_only_response)

## Functions
- `_make_strategy(**overrides)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L29)
- `_make_verification(**overrides)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L15)
- `test_verdict_severity_rank_matches_journal_rank()` — [`L643`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_response.py#L643) — #782 drift guard: the locally-duplicated severity rank must stay

