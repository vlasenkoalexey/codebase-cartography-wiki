---
title: 'Module: tests/unit/mcp/test_file_health_response_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_file_health_response_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_file_health_response_coverage`/
symbols:
  TestBuildAgentSummary.test_critical_smell_preferred_over_warning: TestBuildAgentSummary#test_critical_smell_preferred_over_warning().
  TestBuildAgentSummary.test_empty_dimensions_returns_unknown: TestBuildAgentSummary#test_empty_dimensions_returns_unknown().
  TestBuildFileHealthResultIntegration.test_full_d_grade_flow: TestBuildFileHealthResultIntegration#test_full_d_grade_flow().
  _make_health: _make_health().
  TestBuildOptionalExtractionFields.test_d_grade_returns_next_action_and_plan: TestBuildOptionalExtractionFields#test_d_grade_returns_next_action_and_plan().
  TestBuildOptionalExtractionFields.test_f_grade_returns_fields: TestBuildOptionalExtractionFields#test_f_grade_returns_fields().
  TestBuildOptionalExtractionFields.test_a_grade_returns_empty: TestBuildOptionalExtractionFields#test_a_grade_returns_empty().
  TestBuildOptionalExtractionFields.test_no_long_methods_returns_no_extraction_plan: TestBuildOptionalExtractionFields#test_no_long_methods_returns_no_extraction_plan().
  TestBuildSignal.test_empty_dimensions_returns_no_data: TestBuildSignal#test_empty_dimensions_returns_no_data().
  TestBuildSignal.test_high_score_returns_healthy: TestBuildSignal#test_high_score_returns_healthy().
  TestBuildSignal.test_mid_score_uses_signal_map: TestBuildSignal#test_mid_score_uses_signal_map().
  TestBuildSignal.test_low_score_uses_signal_map: TestBuildSignal#test_low_score_uses_signal_map().
  TestBuildSignal.test_unknown_dimension_uses_fallback: TestBuildSignal#test_unknown_dimension_uses_fallback().
  TestBuildRecommendation.test_good_grade_no_smells: TestBuildRecommendation#test_good_grade_no_smells().
  TestBuildRecommendation.test_no_smells_with_grade_c: TestBuildRecommendation#test_no_smells_with_grade_c().
  TestBuildRecommendation.test_critical_smells_included: TestBuildRecommendation#test_critical_smells_included().
  TestBuildRecommendation.test_long_method_names_in_extraction: TestBuildRecommendation#test_long_method_names_in_extraction().
  TestLongMethodNames.test_extracts_names_from_detail: TestLongMethodNames#test_extracts_names_from_detail().
  TestLongMethodNames.test_skips_non_long_method_smells: TestLongMethodNames#test_skips_non_long_method_smells().
  TestLongMethodNames.test_skips_detail_without_quote: TestLongMethodNames#test_skips_detail_without_quote().
  TestSuggestNextAction.test_long_method_smell: TestSuggestNextAction#test_long_method_smell().
  TestSuggestNextAction.test_oversized_file_smell: TestSuggestNextAction#test_oversized_file_smell().
  TestSuggestNextAction.test_generic_smell: TestSuggestNextAction#test_generic_smell().
  TestBuildAgentNextAction.test_healthy_file_returns_noop: TestBuildAgentNextAction#test_healthy_file_returns_noop().
  TestBuildAgentNextAction.test_b_grade_with_smell_returns_medium: TestBuildAgentNextAction#test_b_grade_with_smell_returns_medium().
  TestBuildAgentNextAction.test_d_grade_returns_high_priority: TestBuildAgentNextAction#test_d_grade_returns_high_priority().
  TestBuildAgentNextAction.test_c_grade_with_smells_returns_medium: TestBuildAgentNextAction#test_c_grade_with_smells_returns_medium().
  TestBuildAgentNextAction.test_critical_smell_returns_high: TestBuildAgentNextAction#test_critical_smell_returns_high().
  TestBuildAgentNextAction.test_action_reason_without_smells: TestBuildAgentNextAction#test_action_reason_without_smells().
  TestWeakestDimensionScore.test_empty_dimensions: TestWeakestDimensionScore#test_empty_dimensions().
  TestWeakestDimensionScore.test_returns_lowest: TestWeakestDimensionScore#test_returns_lowest().
  TestFirstActionableSmell.test_empty_returns_none: TestFirstActionableSmell#test_empty_returns_none().
  TestFirstActionableSmell.test_critical_preferred: TestFirstActionableSmell#test_critical_preferred().
  TestFirstActionableSmell.test_first_when_no_critical: TestFirstActionableSmell#test_first_when_no_critical().
  TestHasRefactorTargetSmell.test_long_method_is_target: TestHasRefactorTargetSmell#test_long_method_is_target().
  TestHasRefactorTargetSmell.test_oversized_file_is_target: TestHasRefactorTargetSmell#test_oversized_file_is_target().
  TestHasRefactorTargetSmell.test_god_class_is_target: TestHasRefactorTargetSmell#test_god_class_is_target().
  TestHasRefactorTargetSmell.test_deep_nesting_is_target: TestHasRefactorTargetSmell#test_deep_nesting_is_target().
  TestHasRefactorTargetSmell.test_other_smell_is_not_target: TestHasRefactorTargetSmell#test_other_smell_is_not_target().
  TestBuildExtractionPlan.test_returns_none_when_no_long_methods: TestBuildExtractionPlan#test_returns_none_when_no_long_methods().
  TestBuildExtractionPlan.test_builds_plan_with_targets: TestBuildExtractionPlan#test_builds_plan_with_targets().
  TestBuildExtractionPlan.test_limits_to_three_targets: TestBuildExtractionPlan#test_limits_to_three_targets().
  TestBuildExtractionTarget.test_parses_detail_with_line_number: TestBuildExtractionTarget#test_parses_detail_with_line_number().
  TestBuildExtractionTarget.test_critical_severity_target: TestBuildExtractionTarget#test_critical_severity_target().
  TestBuildExtractionTarget.test_unknown_method_name: TestBuildExtractionTarget#test_unknown_method_name().
  TestFindFunctionEndLine.test_uses_analysis_functions: TestFindFunctionEndLine#test_uses_analysis_functions().
  TestFindFunctionEndLine.test_falls_back_to_file_read: TestFindFunctionEndLine#test_falls_back_to_file_read().
  TestFindFunctionEndLine.test_handles_missing_file: TestFindFunctionEndLine#test_handles_missing_file().
  TestFindFunctionEndLine.test_handles_start_beyond_file: TestFindFunctionEndLine#test_handles_start_beyond_file().
  TestBuildOptionalExtractionFields: TestBuildOptionalExtractionFields#
  TestBuildSignal: TestBuildSignal#
  TestBuildRecommendation: TestBuildRecommendation#
  TestLongMethodNames: TestLongMethodNames#
  TestSuggestNextAction: TestSuggestNextAction#
  TestBuildAgentNextAction: TestBuildAgentNextAction#
  TestBuildAgentSummary: TestBuildAgentSummary#
  TestWeakestDimensionScore: TestWeakestDimensionScore#
  TestFirstActionableSmell: TestFirstActionableSmell#
  TestHasRefactorTargetSmell: TestHasRefactorTargetSmell#
  TestBuildExtractionPlan: TestBuildExtractionPlan#
  TestBuildExtractionTarget: TestBuildExtractionTarget#
  TestFindFunctionEndLine: TestFindFunctionEndLine#
  TestBuildFileHealthResultIntegration: TestBuildFileHealthResultIntegration#
---
# Module: [`tests/unit/mcp/test_file_health_response_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py)

## Classes
### `TestBuildAgentNextAction`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L139)
- signature: `class TestBuildAgentNextAction:`
- members:
  - `test_action_reason_without_smells(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L172)
  - `test_b_grade_with_smell_returns_medium(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L144)
  - `test_c_grade_with_smells_returns_medium(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L158)
  - `test_critical_smell_returns_high(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L165)
  - `test_d_grade_returns_high_priority(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L151)
  - `test_healthy_file_returns_noop(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L140)
- uses (calls/refs, reference-scoped): [`_build_agent_next_action`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_agent_next_action)

### `TestBuildAgentSummary`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L177)
- signature: `class TestBuildAgentSummary:`
- members:
  - `test_critical_smell_preferred_over_warning(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L185)
  - `test_empty_dimensions_returns_unknown(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L178)
- uses (calls/refs, reference-scoped): [`_build_agent_summary`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_agent_summary), [`_build_agent_next_action`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_agent_next_action)  (1 test-only)

### `TestBuildExtractionPlan`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L246)
- signature: `class TestBuildExtractionPlan:`
- members:
  - `test_builds_plan_with_targets(self, tmp_path)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L251)
  - `test_limits_to_three_targets(self, tmp_path)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L266)
  - `test_returns_none_when_no_long_methods(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L247)
- uses (calls/refs, reference-scoped): [`_build_extraction_plan`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_extraction_plan)

### `TestBuildExtractionTarget`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L278)
- signature: `class TestBuildExtractionTarget:`
- members:
  - `test_critical_severity_target(self, tmp_path)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L288)
  - `test_parses_detail_with_line_number(self, tmp_path)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L279)
  - `test_unknown_method_name(self, tmp_path)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L295)
- uses (calls/refs, reference-scoped): [`_build_extraction_target`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_extraction_target)

### `TestBuildFileHealthResultIntegration`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L330)
- signature: `class TestBuildFileHealthResultIntegration:`
- members:
  - `test_full_d_grade_flow(self, tmp_path)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L331)
- uses (calls/refs, reference-scoped): [`build_file_health_result`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#build_file_health_result)  (1 test-only)

### `TestBuildOptionalExtractionFields`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L30)
- signature: `class TestBuildOptionalExtractionFields:`
- members:
  - `test_a_grade_returns_empty(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L46)
  - `test_d_grade_returns_next_action_and_plan(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L31)
  - `test_f_grade_returns_fields(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L39)
  - `test_no_long_methods_returns_no_extraction_plan(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L50)
- uses (calls/refs, reference-scoped): [`_build_optional_extraction_fields`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_optional_extraction_fields)

### `TestBuildRecommendation`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L77)
- signature: `class TestBuildRecommendation:`
- members:
  - `test_critical_smells_included(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L87)
  - `test_good_grade_no_smells(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L78)
  - `test_long_method_names_in_extraction(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L96)
  - `test_no_smells_with_grade_c(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L82)
- uses (calls/refs, reference-scoped): [`_build_recommendation`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_recommendation)

### `TestBuildSignal`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L57)
- signature: `class TestBuildSignal:`
- members:
  - `test_empty_dimensions_returns_no_data(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L58)
  - `test_high_score_returns_healthy(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L61)
  - `test_low_score_uses_signal_map(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L68)
  - `test_mid_score_uses_signal_map(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L64)
  - `test_unknown_dimension_uses_fallback(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L72)
- uses (calls/refs, reference-scoped): [`_build_signal`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_build_signal)

### `TestFindFunctionEndLine`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L303)
- signature: `class TestFindFunctionEndLine:`
- members:
  - `test_falls_back_to_file_read(self, tmp_path)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L313)
  - `test_handles_missing_file(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L319)
  - `test_handles_start_beyond_file(self, tmp_path)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L323)
  - `test_uses_analysis_functions(self, tmp_path)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L304)
- uses (calls/refs, reference-scoped): [`_find_function_end_line`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_find_function_end_line)

### `TestFirstActionableSmell`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L208)
- signature: `class TestFirstActionableSmell:`
- members:
  - `test_critical_preferred(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L212)
  - `test_empty_returns_none(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L209)
  - `test_first_when_no_critical(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L220)
- uses (calls/refs, reference-scoped): [`_first_actionable_smell`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_first_actionable_smell)

### `TestHasRefactorTargetSmell`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L229)
- signature: `class TestHasRefactorTargetSmell:`
- members:
  - `test_deep_nesting_is_target(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L239)
  - `test_god_class_is_target(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L236)
  - `test_long_method_is_target(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L230)
  - `test_other_smell_is_not_target(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L242)
  - `test_oversized_file_is_target(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L233)
- uses (calls/refs, reference-scoped): [`_has_refactor_target_smell`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_has_refactor_target_smell)

### `TestLongMethodNames`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L106)
- signature: `class TestLongMethodNames:`
- members:
  - `test_extracts_names_from_detail(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L107)
  - `test_skips_detail_without_quote(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L117)
  - `test_skips_non_long_method_smells(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L113)
- uses (calls/refs, reference-scoped): [`_long_method_names`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_long_method_names)

### `TestSuggestNextAction`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L122)
- signature: `class TestSuggestNextAction:`
- members:
  - `test_generic_smell(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L133)
  - `test_long_method_smell(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L123)
  - `test_oversized_file_smell(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L128)
- uses (calls/refs, reference-scoped): [`_suggest_next_action`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_suggest_next_action)

### `TestWeakestDimensionScore`
- def: [`tests/unit/mcp/test_file_health_response_coverage.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L196)
- signature: `class TestWeakestDimensionScore:`
- members:
  - `test_empty_dimensions(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L197)
  - `test_returns_lowest(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L202)
- uses (calls/refs, reference-scoped): [`_weakest_dimension_score`](../../../tree_sitter_analyzer/mcp/tools/utils/file_health_response.md#_weakest_dimension_score)

## Functions
- `_make_health(grade: str, total: float, dimensions: dict[str, float])` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_response_coverage.py#L26)

