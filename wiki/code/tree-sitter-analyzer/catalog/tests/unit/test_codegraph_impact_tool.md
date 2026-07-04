---
title: 'Module: tests/unit/test_codegraph_impact_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_impact_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_impact_tool`/
symbols:
  _make_func: _make_func().
  TestFunctionImpactListCap.test_direct_callers_capped_but_count_is_full: TestFunctionImpactListCap#test_direct_callers_capped_but_count_is_full().
  TestTransitiveCapFlag.test_capped_flag_absent_below_limit: TestTransitiveCapFlag#test_capped_flag_absent_below_limit().
  TestTransitiveCapFlag.test_capped_flag_present_at_limit: TestTransitiveCapFlag#test_capped_flag_present_at_limit().
  TestTransitiveCapFlag.test_callee_capped_flag_absent_below_limit: TestTransitiveCapFlag#test_callee_capped_flag_absent_below_limit().
  TestTransitiveCapFlag.test_callee_capped_flag_present_at_limit: TestTransitiveCapFlag#test_callee_capped_flag_present_at_limit().
  TestCodeGraphImpactTool.test_execute_risk_score: TestCodeGraphImpactTool#test_execute_risk_score().
  TestFunctionImpactListCap.test_small_lists_not_truncated: TestFunctionImpactListCap#test_small_lists_not_truncated().
  TestImpactTestPartition.test_partition_refs_splits_prod_and_test: TestImpactTestPartition#test_partition_refs_splits_prod_and_test().
  TestBlastRadiusSingularAlias.test_execute_singular_wraps_to_list: TestBlastRadiusSingularAlias#test_execute_singular_wraps_to_list().
  TestBlastRadiusUnknownSeedVerdict.test_unknown_seed_verdict_is_not_found: TestBlastRadiusUnknownSeedVerdict#test_unknown_seed_verdict_is_not_found().
  TestBlastRadiusUnknownSeedVerdict.test_unknown_seed_agent_summary_verdict_is_not_found: TestBlastRadiusUnknownSeedVerdict#test_unknown_seed_agent_summary_verdict_is_not_found().
  TestBlastRadiusUnknownSeedVerdict.test_unknown_seed_next_step_does_not_advise_edit: TestBlastRadiusUnknownSeedVerdict#test_unknown_seed_next_step_does_not_advise_edit().
  TestTransitiveCapFlag._graph_with_n_transitive_callers: TestTransitiveCapFlag#_graph_with_n_transitive_callers().
  TestTransitiveCapFlag._graph_with_n_transitive_callees: TestTransitiveCapFlag#_graph_with_n_transitive_callees().
  TestBlastRadiusUnknownSeedVerdict._make_tool: TestBlastRadiusUnknownSeedVerdict#_make_tool().
  TestTransitiveCallers.test_no_callers: TestTransitiveCallers#test_no_callers().
  TestTransitiveCallers.test_direct_callers: TestTransitiveCallers#test_direct_callers().
  TestTransitiveCallers.test_transitive_chain: TestTransitiveCallers#test_transitive_chain().
  TestTransitiveCallees.test_no_callees: TestTransitiveCallees#test_no_callees().
  TestTransitiveCallees.test_transitive_chain: TestTransitiveCallees#test_transitive_chain().
  TestRiskScore.test_low_risk: TestRiskScore#test_low_risk().
  TestRiskScore.test_high_risk_many_callers: TestRiskScore#test_high_risk_many_callers().
  TestRiskScore.test_critical_risk: TestRiskScore#test_critical_risk().
  TestBlastRadius.test_single_function_no_impact: TestBlastRadius#test_single_function_no_impact().
  TestBlastRadius.test_propagation: TestBlastRadius#test_propagation().
  TestBlastRadius.test_respects_depth: TestBlastRadius#test_respects_depth().
  TestCodeGraphImpactTool.test_tool_definition: TestCodeGraphImpactTool#test_tool_definition().
  TestCodeGraphImpactTool.test_validate_function_impact_missing_name: TestCodeGraphImpactTool#test_validate_function_impact_missing_name().
  TestCodeGraphImpactTool.test_validate_blast_radius_missing_names: TestCodeGraphImpactTool#test_validate_blast_radius_missing_names().
  TestCodeGraphImpactTool.test_validate_risk_score_missing_name: TestCodeGraphImpactTool#test_validate_risk_score_missing_name().
  TestCodeGraphImpactTool.test_validate_ok: TestCodeGraphImpactTool#test_validate_ok().
  TestImpactTestPartition.test_risk_score_excludes_test_callers: TestImpactTestPartition#test_risk_score_excludes_test_callers().
  TestImpactTestPartition.test_risk_score_all_prod_callers_score_60: TestImpactTestPartition#test_risk_score_all_prod_callers_score_60().
  TestImpactTestPartition.test_df16_scenario: TestImpactTestPartition#test_df16_scenario().
  TestImpactTestPartition.test_tests_bucket_always_present_when_zero: TestImpactTestPartition#test_tests_bucket_always_present_when_zero().
  TestImpactTestPartition.test_include_tests_false_omits_file_lists: TestImpactTestPartition#test_include_tests_false_omits_file_lists().
  TestImpactTestPartition.test_include_tests_true_adds_file_lists: TestImpactTestPartition#test_include_tests_true_adds_file_lists().
  TestImpactTestPartition.test_schema_declares_include_tests: TestImpactTestPartition#test_schema_declares_include_tests().
  TestImpactTestPartition.test_transitive_callers_filters_tests_by_default: TestImpactTestPartition#test_transitive_callers_filters_tests_by_default().
  TestImpactTestPartition.test_transitive_callers_include_tests_true: TestImpactTestPartition#test_transitive_callers_include_tests_true().
  TestImpactTestPartition.test_transitive_callees_filters_tests_by_default: TestImpactTestPartition#test_transitive_callees_filters_tests_by_default().
  TestImpactTestPartition.test_transitive_callees_include_tests_true: TestImpactTestPartition#test_transitive_callees_include_tests_true().
  TestBlastRadiusPropagation.test_transitive_caller_chain_propagates: TestBlastRadiusPropagation#test_transitive_caller_chain_propagates().
  TestBlastRadiusPropagation.test_four_direct_callers_are_all_counted: TestBlastRadiusPropagation#test_four_direct_callers_are_all_counted().
  TestBlastRadiusSingularAlias.test_validate_accepts_singular_function_name: TestBlastRadiusSingularAlias#test_validate_accepts_singular_function_name().
  TestBlastRadiusSingularAlias.test_validate_still_raises_when_both_absent: TestBlastRadiusSingularAlias#test_validate_still_raises_when_both_absent().
  TestBlastRadiusSingularAlias.test_schema_mentions_blast_radius_function_names: TestBlastRadiusSingularAlias#test_schema_mentions_blast_radius_function_names().
  TestBlastRadiusSingularAlias.test_schema_describes_singular_alias: TestBlastRadiusSingularAlias#test_schema_describes_singular_alias().
  TestBlastRadiusFileOnlyRecoveryHint.test_blast_radius_error_message_contains_xref_hint: TestBlastRadiusFileOnlyRecoveryHint#test_blast_radius_error_message_contains_xref_hint().
  TestBlastRadiusFileOnlyRecoveryHint.test_blast_radius_error_message_mentions_file_mode: TestBlastRadiusFileOnlyRecoveryHint#test_blast_radius_error_message_mentions_file_mode().
  TestBlastRadiusFileOnlyRecoveryHint.test_blast_radius_with_no_args_error_still_mentions_xref: TestBlastRadiusFileOnlyRecoveryHint#test_blast_radius_with_no_args_error_still_mentions_xref().
  TestFunctionImpactListCap._graph_with_n_direct_callers: TestFunctionImpactListCap#_graph_with_n_direct_callers().
  TestBlastRadiusUnknownSeedVerdict._mock_empty_graph: TestBlastRadiusUnknownSeedVerdict#_mock_empty_graph().
  TestRiskScore.test_unknown_function: TestRiskScore#test_unknown_function().
  TestImpactTestPartition.test_partition_refs_empty_list: TestImpactTestPartition#test_partition_refs_empty_list().
  TestImpactVerdictCriticalLevel.test_critical_level_is_caution_not_info: TestImpactVerdictCriticalLevel#test_critical_level_is_caution_not_info().
  TestImpactVerdictCriticalLevel.test_known_levels_unchanged: TestImpactVerdictCriticalLevel#test_known_levels_unchanged().
  TestImpactVerdictCriticalLevel.test_no_level_fallthrough_stays_info: TestImpactVerdictCriticalLevel#test_no_level_fallthrough_stays_info().
  TestTransitiveCallers: TestTransitiveCallers#
  TestTransitiveCallees: TestTransitiveCallees#
  TestRiskScore: TestRiskScore#
  TestBlastRadius: TestBlastRadius#
  TestCodeGraphImpactTool: TestCodeGraphImpactTool#
  TestFunctionImpactListCap: TestFunctionImpactListCap#
  TestImpactTestPartition: TestImpactTestPartition#
  TestBlastRadiusPropagation: TestBlastRadiusPropagation#
  TestBlastRadiusSingularAlias: TestBlastRadiusSingularAlias#
  TestTransitiveCapFlag: TestTransitiveCapFlag#
  TestBlastRadiusFileOnlyRecoveryHint: TestBlastRadiusFileOnlyRecoveryHint#
  TestBlastRadiusUnknownSeedVerdict: TestBlastRadiusUnknownSeedVerdict#
  TestImpactVerdictCriticalLevel: TestImpactVerdictCriticalLevel#
---
# Module: [`tests/unit/test_codegraph_impact_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py)

## Classes
### `TestBlastRadius`
- def: [`tests/unit/test_codegraph_impact_tool.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L139)
- signature: `class TestBlastRadius:`
- members:
  - `test_propagation(self)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L150)
  - `test_respects_depth(self)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L164)
  - `test_single_function_no_impact(self)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L140)
- uses (calls/refs, reference-scoped): [`_blast_radius_for_functions`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_blast_radius_for_functions)  (1 test-only)

### `TestBlastRadiusFileOnlyRecoveryHint`
- def: [`tests/unit/test_codegraph_impact_tool.py:678`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L678)
- doc: #668: when blast_radius is called with file_path only (no function_names),
- signature: `class TestBlastRadiusFileOnlyRecoveryHint:`
- members:
  - `test_blast_radius_error_message_contains_xref_hint(self)` — [`L687`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L687) — validate_arguments raises; error message mentions 'xref'.
  - `test_blast_radius_error_message_mentions_file_mode(self)` — [`L697`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L697) — Error message must reference mode=file so the agent knows which xref mode.
  - `test_blast_radius_with_no_args_error_still_mentions_xref(self)` — [`L707`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L707) — Even with no file_path provided, the blast_radius error hints at xref.
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.validate_arguments)

### `TestBlastRadiusPropagation`
- def: [`tests/unit/test_codegraph_impact_tool.py:481`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L481)
- doc: #656: blast_radius must propagate transitively, not just return the seed.
- signature: `class TestBlastRadiusPropagation:`
- members:
  - `test_four_direct_callers_are_all_counted(self)` — [`L507`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L507) — seed with 4 direct callers: total_affected_functions == 5 (seed + 4).
  - `test_transitive_caller_chain_propagates(self)` — [`L491`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L491) — Seed←B←C: total_affected_functions == 3 (seed + 2 transitive callers).
- uses (calls/refs, reference-scoped): [`_blast_radius_for_functions`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_blast_radius_for_functions)  (1 test-only)

### `TestBlastRadiusSingularAlias`
- def: [`tests/unit/test_codegraph_impact_tool.py:532`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L532)
- doc: #657: blast_radius should accept function_name (singular) and wrap it.
- signature: `class TestBlastRadiusSingularAlias:`
- members:
  - `test_execute_singular_wraps_to_list(self)` — [`L548`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L548) — execute with function_name=X for blast_radius passes [X] to blast fn.
  - `test_schema_describes_singular_alias(self)` — [`L576`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L576) — function_name schema description must mention blast_radius alias.
  - `test_schema_mentions_blast_radius_function_names(self)` — [`L569`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L569) — Schema description for function_names must reference blast_radius mode.
  - `test_validate_accepts_singular_function_name(self)` — [`L535`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L535) — validate_arguments must NOT raise when function_name (singular) is given.
  - `test_validate_still_raises_when_both_absent(self)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L541) — validate_arguments must still raise when neither name form is provided.
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.execute), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.validate_arguments), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.get_tool_schema)  (1 test-only)

### `TestBlastRadiusUnknownSeedVerdict`
- def: [`tests/unit/test_codegraph_impact_tool.py:721`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L721)
- doc: blast_radius with an unresolved seed must yield verdict=NOT_FOUND and
- signature: `class TestBlastRadiusUnknownSeedVerdict:`
- members:
  - `test_unknown_seed_agent_summary_verdict_is_not_found(self, tmp_path)` — [`L767`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L767) — agent_summary.verdict for unknown seed must be 'NOT_FOUND', not 'INFO'.
  - `test_unknown_seed_next_step_does_not_advise_edit(self, tmp_path)` — [`L786`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L786) — blast_radius unknown seed must NOT tell caller to 'proceed with edit'.
  - `test_unknown_seed_verdict_is_not_found(self, tmp_path)` — [`L749`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L749) — blast_radius with unresolved seed → verdict == 'NOT_FOUND', not 'INFO'.
- protocol/private: `_make_tool`[`L735`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L735), `_mock_empty_graph`[`L738`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L738)
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.execute)

### `TestCodeGraphImpactTool`
- def: [`tests/unit/test_codegraph_impact_tool.py:178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L178)
- signature: `class TestCodeGraphImpactTool:`
- members:
  - `test_execute_risk_score(self)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L207)
  - `test_tool_definition(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L179)
  - `test_validate_blast_radius_missing_names(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L190)
  - `test_validate_function_impact_missing_name(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L185)
  - `test_validate_ok(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L200)
  - `test_validate_risk_score_missing_name(self)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L195)
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.execute), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.validate_arguments), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.get_tool_definition)  (1 test-only)

### `TestFunctionImpactListCap`
- def: [`tests/unit/test_codegraph_impact_tool.py:228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L228)
- doc: Wave 1b (audit nav-08): function_impact must cap the EMITTED caller/callee
- signature: `class TestFunctionImpactListCap:`
- members:
  - `test_direct_callers_capped_but_count_is_full(self)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L247)
  - `test_small_lists_not_truncated(self)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L256)
- protocol/private: `_graph_with_n_direct_callers`[`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L233)
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`_function_impact`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._function_impact), [`_MAX_LISTED`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_MAX_LISTED)  (1 test-only)

### `TestImpactTestPartition`
- def: [`tests/unit/test_codegraph_impact_tool.py:265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L265)
- doc: RFC-0014 Phase A: DF-16 test-noise partition for nav action=impact.
- signature: `class TestImpactTestPartition:`
- members:
  - `test_df16_scenario(self)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L320) — DF-16: 16 test + 2 prod callers → partitioned score == 0, level 'low'.
  - `test_include_tests_false_omits_file_lists(self)` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L361) — Default (include_tests=False): tests bucket has counts only, no file lists.
  - `test_include_tests_true_adds_file_lists(self)` — [`L375`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L375) — include_tests=True: file lists appear, sorted and deduplicated.
  - `test_partition_refs_empty_list(self)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L278) — Empty list → both buckets empty.
  - `test_partition_refs_splits_prod_and_test(self)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L268) — _partition_refs correctly classifies by is_test_file path.
  - `test_risk_score_all_prod_callers_score_60(self)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L302) — 12 prod callers from 12 distinct files → score==60 exactly.
  - `test_risk_score_excludes_test_callers(self)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L284) — 12 test + 1 prod caller → fan_in=1, score=0, level='low'.
  - `test_schema_declares_include_tests(self)` — [`L398`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L398) — include_tests must be in schema properties (P1-2: _project_args whitelist).
  - `test_tests_bucket_always_present_when_zero(self)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L348) — tests dict always present; both counts == 0 for isolated function.
  - `test_transitive_callees_filters_tests_by_default(self)` — [`L439`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L439) — _compute_transitive_callees(include_tests=False) excludes test-file entries.
  - `test_transitive_callees_include_tests_true(self)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L456) — _compute_transitive_callees(include_tests=True) includes test-file entries.
  - `test_transitive_callers_filters_tests_by_default(self)` — [`L406`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L406) — _compute_transitive_callers(include_tests=False) excludes test-file entries.
  - `test_transitive_callers_include_tests_true(self)` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L423) — _compute_transitive_callers(include_tests=True) includes test-file entries.
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`_compute_risk_score`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_risk_score), [`_compute_transitive_callers`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_transitive_callers), [`_compute_transitive_callees`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_transitive_callees), [`_partition_refs`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_partition_refs), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.get_tool_schema)  (1 test-only)

### `TestImpactVerdictCriticalLevel`
- def: [`tests/unit/test_codegraph_impact_tool.py:810`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L810)
- doc: _compute_risk_score emits 4 levels (critical&gt;=60, high&gt;=40, medium&gt;=20,
- signature: `class TestImpactVerdictCriticalLevel:`
- members:
  - `test_critical_level_is_caution_not_info(self)` — [`L821`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L821)
  - `test_known_levels_unchanged(self)` — [`L824`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L824)
  - `test_no_level_fallthrough_stays_info(self)` — [`L830`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L830)
- uses (calls/refs, reference-scoped): [`_impact_verdict`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_impact_verdict)

### `TestRiskScore`
- def: [`tests/unit/test_codegraph_impact_tool.py:91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L91)
- signature: `class TestRiskScore:`
- members:
  - `test_critical_risk(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L124)
  - `test_high_risk_many_callers(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L110)
  - `test_low_risk(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L99)
  - `test_unknown_function(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L92)
- uses (calls/refs, reference-scoped): [`_compute_risk_score`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_risk_score)  (1 test-only)

### `TestTransitiveCallees`
- def: [`tests/unit/test_codegraph_impact_tool.py:70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L70)
- signature: `class TestTransitiveCallees:`
- members:
  - `test_no_callees(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L71)
  - `test_transitive_chain(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L79)
- uses (calls/refs, reference-scoped): [`_compute_transitive_callees`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_transitive_callees)  (1 test-only)

### `TestTransitiveCallers`
- def: [`tests/unit/test_codegraph_impact_tool.py:31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L31)
- signature: `class TestTransitiveCallers:`
- members:
  - `test_direct_callers(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L40)
  - `test_no_callers(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L32)
  - `test_transitive_chain(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L52)
- uses (calls/refs, reference-scoped): [`_compute_transitive_callers`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_compute_transitive_callers)  (1 test-only)

### `TestTransitiveCapFlag`
- def: [`tests/unit/test_codegraph_impact_tool.py:590`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L590)
- doc: #658: transitive_caller_count == _MAX_TRANSITIVE must expose is_capped flag.
- signature: `class TestTransitiveCapFlag:`
- members:
  - `_graph_with_n_transitive_callees(self, n: int)` — [`L633`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L633) — Return a mock graph whose callee BFS yields exactly n unique callees.
  - `_graph_with_n_transitive_callers(self, n: int)` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L593) — Return a mock graph whose BFS yields exactly n unique callers.
  - `test_callee_capped_flag_absent_below_limit(self)` — [`L650`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L650) — transitive_callee_count_is_capped absent when callee count < _MAX_TRANSITIVE.
  - `test_callee_capped_flag_present_at_limit(self)` — [`L661`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L661) — transitive_callee_count_is_capped: True when count == _MAX_TRANSITIVE.
  - `test_capped_flag_absent_below_limit(self)` — [`L611`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L611) — transitive_count_is_capped absent when caller count < _MAX_TRANSITIVE.
  - `test_capped_flag_present_at_limit(self)` — [`L622`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L622) — transitive_count_is_capped: True when transitive_caller_count == _MAX_TRANSITIVE.
- uses (calls/refs, reference-scoped): [`CodeGraphImpactTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool), [`_function_impact`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._function_impact), [`to_dict`](../../tree_sitter_analyzer/call_graph.md#FunctionRef.to_dict), [`_MAX_TRANSITIVE`](../../tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.md#_MAX_TRANSITIVE)  (1 test-only)

## Functions
- `_make_func(name: str, file: str = "a.py", line: int = 1)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_impact_tool.py#L22)

