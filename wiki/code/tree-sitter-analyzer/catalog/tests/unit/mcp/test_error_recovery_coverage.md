---
title: 'Module: tests/unit/mcp/test_error_recovery_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_error_recovery_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_error_recovery_coverage`/
symbols:
  _assert_canonical: _assert_canonical().
  TestBuildAgentFriendlyError.test_file_not_found_pattern: TestBuildAgentFriendlyError#test_file_not_found_pattern().
  TestBuildAgentFriendlyError.test_unsupported_language_pattern: TestBuildAgentFriendlyError#test_unsupported_language_pattern().
  TestBuildAgentFriendlyError.test_project_root_pattern: TestBuildAgentFriendlyError#test_project_root_pattern().
  TestBuildAgentFriendlyError.test_outside_boundary_pattern: TestBuildAgentFriendlyError#test_outside_boundary_pattern().
  TestBuildAgentFriendlyError.test_missing_parameter_pattern: TestBuildAgentFriendlyError#test_missing_parameter_pattern().
  TestBuildAgentFriendlyError.test_blast_radius_required_keeps_xref_guidance: TestBuildAgentFriendlyError#test_blast_radius_required_keeps_xref_guidance().
  TestBuildAgentFriendlyError.test_validation_error_pattern: TestBuildAgentFriendlyError#test_validation_error_pattern().
  TestBuildAgentFriendlyError.test_resource_exhausted_pattern: TestBuildAgentFriendlyError#test_resource_exhausted_pattern().
  TestBuildAgentFriendlyError.test_timeout_pattern: TestBuildAgentFriendlyError#test_timeout_pattern().
  TestBuildAgentFriendlyError.test_unknown_error_category: TestBuildAgentFriendlyError#test_unknown_error_category().
  TestBuildAgentFriendlyError.test_error_type_canonical_for_memory_error: TestBuildAgentFriendlyError#test_error_type_canonical_for_memory_error().
  TestBuildAgentFriendlyError.test_suggested_tool_with_file_not_found: TestBuildAgentFriendlyError#test_suggested_tool_with_file_not_found().
  TestBuildAgentFriendlyError.test_identifier_mirrored_from_arguments: TestBuildAgentFriendlyError#test_identifier_mirrored_from_arguments().
  TestEnsureCanonicalErrorEnvelope.test_adds_canonical_keys_to_minimal_dict: TestEnsureCanonicalErrorEnvelope#test_adds_canonical_keys_to_minimal_dict().
  TestBuildAgentFriendlyError.test_error_message_preserved: TestBuildAgentFriendlyError#test_error_message_preserved().
  TestEnsureCanonicalErrorEnvelope.test_preserves_existing_canonical_fields: TestEnsureCanonicalErrorEnvelope#test_preserves_existing_canonical_fields().
  TestEnsureCanonicalErrorEnvelope.test_skips_success_responses: TestEnsureCanonicalErrorEnvelope#test_skips_success_responses().
  TestEnsureCanonicalErrorEnvelope.test_hoists_verdict_to_top_level: TestEnsureCanonicalErrorEnvelope#test_hoists_verdict_to_top_level().
  TestEnsureCanonicalErrorEnvelope.test_preserves_tool_specific_top_level_verdict: TestEnsureCanonicalErrorEnvelope#test_preserves_tool_specific_top_level_verdict().
  TestEnsureCanonicalErrorEnvelope.test_na_placeholder_treated_as_missing_verdict: TestEnsureCanonicalErrorEnvelope#test_na_placeholder_treated_as_missing_verdict().
  TestSuccessEnvelopeNextStepMirror.test_top_level_next_step_mirrored_into_agent_summary: TestSuccessEnvelopeNextStepMirror#test_top_level_next_step_mirrored_into_agent_summary().
  TestSuccessEnvelopeNextStepMirror.test_existing_agent_summary_next_step_is_not_clobbered: TestSuccessEnvelopeNextStepMirror#test_existing_agent_summary_next_step_is_not_clobbered().
  TestSuccessEnvelopeNextStepMirror.test_no_next_step_anywhere_stays_empty_string: TestSuccessEnvelopeNextStepMirror#test_no_next_step_anywhere_stays_empty_string().
  TestSynthesizedSummaryLineIsVerdictAware.test_warn_verdict_does_not_say_ok: TestSynthesizedSummaryLineIsVerdictAware#test_warn_verdict_does_not_say_ok().
  TestSynthesizedSummaryLineIsVerdictAware.test_not_found_verdict_suffix: TestSynthesizedSummaryLineIsVerdictAware#test_not_found_verdict_suffix().
  TestSynthesizedSummaryLineIsVerdictAware.test_error_verdict_suffix: TestSynthesizedSummaryLineIsVerdictAware#test_error_verdict_suffix().
  TestSynthesizedSummaryLineIsVerdictAware.test_caution_review_unsafe_verdicts_are_not_ok: TestSynthesizedSummaryLineIsVerdictAware#test_caution_review_unsafe_verdicts_are_not_ok().
  TestSynthesizedSummaryLineIsVerdictAware.test_info_and_safe_verdicts_still_ok: TestSynthesizedSummaryLineIsVerdictAware#test_info_and_safe_verdicts_still_ok().
  TestSynthesizedSummaryLineIsVerdictAware.test_verdict_read_from_agent_summary_when_top_level_absent: TestSynthesizedSummaryLineIsVerdictAware#test_verdict_read_from_agent_summary_when_top_level_absent().
  TestSynthesizedSummaryLineIsVerdictAware.test_identifier_still_wins_over_verdict_suffix: TestSynthesizedSummaryLineIsVerdictAware#test_identifier_still_wins_over_verdict_suffix().
  TestSynthesizedSummaryLineIsVerdictAware.test_no_verdict_no_identifier_falls_back_to_ok: TestSynthesizedSummaryLineIsVerdictAware#test_no_verdict_no_identifier_falls_back_to_ok().
  TestBuildAgentFriendlyError: TestBuildAgentFriendlyError#
  TestEnsureCanonicalErrorEnvelope: TestEnsureCanonicalErrorEnvelope#
  TestSuccessEnvelopeNextStepMirror: TestSuccessEnvelopeNextStepMirror#
  TestSynthesizedSummaryLineIsVerdictAware: TestSynthesizedSummaryLineIsVerdictAware#
---
# Module: [`tests/unit/mcp/test_error_recovery_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py)

## Classes
### `TestBuildAgentFriendlyError`
- def: [`tests/unit/mcp/test_error_recovery_coverage.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L42)
- signature: `class TestBuildAgentFriendlyError:`
- members:
  - `test_blast_radius_required_keeps_xref_guidance(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L84)
  - `test_error_message_preserved(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L133)
  - `test_error_type_canonical_for_memory_error(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L144)
  - `test_file_not_found_pattern(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L43)
  - `test_identifier_mirrored_from_arguments(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L160)
  - `test_missing_parameter_pattern(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L72)
  - `test_outside_boundary_pattern(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L65)
  - `test_project_root_pattern(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L58)
  - `test_resource_exhausted_pattern(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L108)
  - `test_suggested_tool_with_file_not_found(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L153)
  - `test_timeout_pattern(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L115)
  - `test_unknown_error_category(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L122)
  - `test_unsupported_language_pattern(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L51)
  - `test_validation_error_pattern(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L101)
- uses (calls/refs, reference-scoped): [`build_agent_friendly_error`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#build_agent_friendly_error)  (1 test-only)

### `TestEnsureCanonicalErrorEnvelope`
- def: [`tests/unit/mcp/test_error_recovery_coverage.py:172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L172)
- doc: Tools that already return `{success: False, ...}` get the canonical
- signature: `class TestEnsureCanonicalErrorEnvelope:`
- members:
  - `test_adds_canonical_keys_to_minimal_dict(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L177)
  - `test_hoists_verdict_to_top_level(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L212) — Wave 1a: a tool that returns a bare {success: False} dict gets a
  - `test_na_placeholder_treated_as_missing_verdict(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L234) — The ``n/a`` post-hook placeholder must NOT be promoted to a
  - `test_preserves_existing_canonical_fields(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L188)
  - `test_preserves_tool_specific_top_level_verdict(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L220) — A tool that already set a more specific top-level verdict (e.g.
  - `test_skips_success_responses(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L205)
- uses (calls/refs, reference-scoped): [`ensure_canonical_error_envelope`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#ensure_canonical_error_envelope)  (1 test-only)

### `TestSuccessEnvelopeNextStepMirror`
- def: [`tests/unit/mcp/test_error_recovery_coverage.py:250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L250)
- doc: Wave 1b batch B (audit nav-03/04, search-05, project-03, viz-05, health-04):
- signature: `class TestSuccessEnvelopeNextStepMirror:`
- members:
  - `test_existing_agent_summary_next_step_is_not_clobbered(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L269)
  - `test_no_next_step_anywhere_stays_empty_string(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L279)
  - `test_top_level_next_step_mirrored_into_agent_summary(self)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L257)
- uses (calls/refs, reference-scoped): [`ensure_canonical_success_envelope`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#ensure_canonical_success_envelope)

### `TestSynthesizedSummaryLineIsVerdictAware`
- def: [`tests/unit/mcp/test_error_recovery_coverage.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L286)
- doc: #672/#678: when no summary_line / agent_summary.summary_line / identifier
- signature: `class TestSynthesizedSummaryLineIsVerdictAware:`
- members:
  - `test_caution_review_unsafe_verdicts_are_not_ok(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L310)
  - `test_error_verdict_suffix(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L305)
  - `test_identifier_still_wins_over_verdict_suffix(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L334)
  - `test_info_and_safe_verdicts_still_ok(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L322)
  - `test_no_verdict_no_identifier_falls_back_to_ok(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L341)
  - `test_not_found_verdict_suffix(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L300)
  - `test_verdict_read_from_agent_summary_when_top_level_absent(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L329)
  - `test_warn_verdict_does_not_say_ok(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L294)
- uses (calls/refs, reference-scoped): [`ensure_canonical_success_envelope`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#ensure_canonical_success_envelope)

## Functions
- `_assert_canonical(result: dict)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_error_recovery_coverage.py#L21) — Every error envelope must carry the 5 canonical keys.

