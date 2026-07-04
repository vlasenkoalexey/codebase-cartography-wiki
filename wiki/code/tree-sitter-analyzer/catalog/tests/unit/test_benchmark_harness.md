---
title: 'Module: tests/unit/test_benchmark_harness.py'
type: catalog
provenance: extracted
module: tests/unit/test_benchmark_harness.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_benchmark_harness`/
symbols:
  TestRunIdUniqueness.test_run_record_with_session_id_validates_against_schema: TestRunIdUniqueness#test_run_record_with_session_id_validates_against_schema().
  TestCodeGraphCompareTSAAdapter.test_warm_index_rebuilds_when_db_is_empty: TestCodeGraphCompareTSAAdapter#test_warm_index_rebuilds_when_db_is_empty().
  TestCodeGraphCompareTSAAdapter.test_parse_tool_metrics_counts_mcp_calls_as_index_queries: TestCodeGraphCompareTSAAdapter#test_parse_tool_metrics_counts_mcp_calls_as_index_queries().
  TestRunRecordCostCacheColumns.test_runner_emits_cost_cache_columns_in_record: TestRunRecordCostCacheColumns#test_runner_emits_cost_cache_columns_in_record().
  TestRunIdUniqueness.test_session_id_uniquifies_raw_artifacts: TestRunIdUniqueness#test_session_id_uniquifies_raw_artifacts().
  TestRunRecordCostCacheColumns.test_run_record_defaults_keep_old_records_loadable: TestRunRecordCostCacheColumns#test_run_record_defaults_keep_old_records_loadable().
  TestRunRecordCostCacheColumns.test_run_record_accepts_real_cost_cache_columns: TestRunRecordCostCacheColumns#test_run_record_accepts_real_cost_cache_columns().
  TestCodeGraphCompareTSAAdapter.test_warm_index_skips_when_db_has_rows: TestCodeGraphCompareTSAAdapter#test_warm_index_skips_when_db_has_rows().
  _BENCH_DIR: _BENCH_DIR.
  TestCodeGraphCompareTSAAdapter.test_run_config_promotes_mcp_nav_context_first: TestCodeGraphCompareTSAAdapter#test_run_config_promotes_mcp_nav_context_first().
  TestCodeGraphCompareToolPolicy.test_tsa_arms_expose_mcp_tools_and_block_competitors: TestCodeGraphCompareToolPolicy#test_tsa_arms_expose_mcp_tools_and_block_competitors().
  TestCodeGraphCompareToolPolicy.test_tsa_mcp_config_pins_target_repo_as_project_root: TestCodeGraphCompareToolPolicy#test_tsa_mcp_config_pins_target_repo_as_project_root().
  TestCodeGraphComparePhases.test_smoke_phase_expands_to_one_question_dry_run_defaults: TestCodeGraphComparePhases#test_smoke_phase_expands_to_one_question_dry_run_defaults().
  TestCodeGraphComparePhases.test_pilot_phase_rejects_too_few_repeats: TestCodeGraphComparePhases#test_pilot_phase_rejects_too_few_repeats().
  TestCodeGraphCompareAnalysisGate.test_gate_flags_failed_and_low_quality_arms: TestCodeGraphCompareAnalysisGate#test_gate_flags_failed_and_low_quality_arms().
  TestCodeGraphCompareEvaluator.test_eval_prompt_renders_inputs_without_formatting_json_example: TestCodeGraphCompareEvaluator#test_eval_prompt_renders_inputs_without_formatting_json_example().
  TestCodeGraphCompareEvaluator.test_evaluate_all_accepts_current_run_schema: TestCodeGraphCompareEvaluator#test_evaluate_all_accepts_current_run_schema().
  TestCodeGraphCompareEvaluator.test_evaluate_run_marks_llm_fallback_as_not_evaluated: TestCodeGraphCompareEvaluator#test_evaluate_run_marks_llm_fallback_as_not_evaluated().
  TestRunRecordCostCacheColumns.test_runner_parses_real_cache_cost_from_claude_usage_block: TestRunRecordCostCacheColumns#test_runner_parses_real_cache_cost_from_claude_usage_block().
  TestRunRecordCostCacheColumns.test_runner_captures_codex_cache_hits: TestRunRecordCostCacheColumns#test_runner_captures_codex_cache_hits().
  tiny_repo: tiny_repo().
  TestScenarioRegistry: TestScenarioRegistry#
  TestScenarioRegistry.test_lists_four_scenarios: TestScenarioRegistry#test_lists_four_scenarios().
  TestScenarioRegistry.test_each_scenario_has_both_runners: TestScenarioRegistry#test_each_scenario_has_both_runners().
  TestRunCaseSchema: TestRunCaseSchema#
  TestRunCaseSchema.test_tsa_cold_start_returns_required_fields: TestRunCaseSchema#test_tsa_cold_start_returns_required_fields().
  TestRunCaseSchema.test_baseline_cold_start_returns_required_fields: TestRunCaseSchema#test_baseline_cold_start_returns_required_fields().
  TestRunCaseSchema.test_tsa_each_scenario_runs_without_crash: TestRunCaseSchema#test_tsa_each_scenario_runs_without_crash().
  TestRunCaseSchema.test_unknown_task_raises: TestRunCaseSchema#test_unknown_task_raises().
  TestRunCaseSchema.test_unknown_tool_raises: TestRunCaseSchema#test_unknown_tool_raises().
  TestJsonlRoundTrip: TestJsonlRoundTrip#
  TestJsonlRoundTrip.test_each_line_parses_as_json: TestJsonlRoundTrip#test_each_line_parses_as_json().
  TestJsonlRoundTrip.test_aggregate_json_has_rows_and_metadata: TestJsonlRoundTrip#test_aggregate_json_has_rows_and_metadata().
  TestTokenEstimation: TestTokenEstimation#
  TestTokenEstimation.test_empty_string_zero_tokens: TestTokenEstimation#test_empty_string_zero_tokens().
  TestTokenEstimation.test_short_string_clamps_to_one: TestTokenEstimation#test_short_string_clamps_to_one().
  TestTokenEstimation.test_long_string_scales_by_four_chars: TestTokenEstimation#test_long_string_scales_by_four_chars().
  TestCodeGraphCompareTSAAdapter: TestCodeGraphCompareTSAAdapter#
  TestCodeGraphCompareToolPolicy: TestCodeGraphCompareToolPolicy#
  TestCodeGraphCompareToolPolicy.test_tsa_prompt_is_mcp_index_first: TestCodeGraphCompareToolPolicy#test_tsa_prompt_is_mcp_index_first().
  TestCodeGraphComparePhases: TestCodeGraphComparePhases#
  TestCodeGraphCompareAnalysisGate: TestCodeGraphCompareAnalysisGate#
  TestCodeGraphCompareEvaluator: TestCodeGraphCompareEvaluator#
  TestRunIdUniqueness: TestRunIdUniqueness#
  TestRunRecordCostCacheColumns: TestRunRecordCostCacheColumns#
---
# Module: [`tests/unit/test_benchmark_harness.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py)

## Classes
### `TestCodeGraphCompareAnalysisGate`
- def: [`tests/unit/test_benchmark_harness.py:394`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L394)
- signature: `class TestCodeGraphCompareAnalysisGate:`
- members:
  - `test_gate_flags_failed_and_low_quality_arms(self)` — [`L395`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L395)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCodeGraphCompareEvaluator`
- def: [`tests/unit/test_benchmark_harness.py:428`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L428)
- signature: `class TestCodeGraphCompareEvaluator:`
- members:
  - `test_eval_prompt_renders_inputs_without_formatting_json_example(self)` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L429)
  - `test_evaluate_all_accepts_current_run_schema(self, tmp_path: Path)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L441)
  - `test_evaluate_run_marks_llm_fallback_as_not_evaluated(self, tmp_path: Path)` — [`L502`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L502)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestCodeGraphComparePhases`
- def: [`tests/unit/test_benchmark_harness.py:354`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L354)
- signature: `class TestCodeGraphComparePhases:`
- members:
  - `test_pilot_phase_rejects_too_few_repeats(self)` — [`L377`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L377)
  - `test_smoke_phase_expands_to_one_question_dry_run_defaults(self)` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L355)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCodeGraphCompareTSAAdapter`
- def: [`tests/unit/test_benchmark_harness.py:212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L212)
- signature: `class TestCodeGraphCompareTSAAdapter:`
- members:
  - `test_parse_tool_metrics_counts_mcp_calls_as_index_queries(self)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L251)
  - `test_run_config_promotes_mcp_nav_context_first(self, tmp_path: Path)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L273)
  - `test_warm_index_rebuilds_when_db_is_empty(self, tmp_path: Path)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L213)
  - `test_warm_index_skips_when_db_has_rows(self, tmp_path: Path)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L232)
- uses (calls/refs, reference-scoped): (13 test-only callers)

### `TestCodeGraphCompareToolPolicy`
- def: [`tests/unit/test_benchmark_harness.py:282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L282)
- signature: `class TestCodeGraphCompareToolPolicy:`
- members:
  - `test_tsa_arms_expose_mcp_tools_and_block_competitors(self)` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L283)
  - `test_tsa_mcp_config_pins_target_repo_as_project_root(self, tmp_path: Path)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L327) — The TSA MCP server must get --project-root <target repo>.
  - `test_tsa_prompt_is_mcp_index_first(self)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L310)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestJsonlRoundTrip`
- def: [`tests/unit/test_benchmark_harness.py:160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L160)
- signature: `class TestJsonlRoundTrip:`
- members:
  - `test_aggregate_json_has_rows_and_metadata(self, tiny_repo: Path, tmp_path: Path)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L181)
  - `test_each_line_parses_as_json(self, tiny_repo: Path, tmp_path: Path)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L161)

### `TestRunCaseSchema`
- def: [`tests/unit/test_benchmark_harness.py:111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L111)
- signature: `class TestRunCaseSchema:`
- members:
  - `test_baseline_cold_start_returns_required_fields(self, tiny_repo: Path)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L119)
  - `test_tsa_cold_start_returns_required_fields(self, tiny_repo: Path)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L112)
  - `test_tsa_each_scenario_runs_without_crash(self, tiny_repo: Path, task: str, extra: dict)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L135)
  - `test_unknown_task_raises(self, tiny_repo: Path)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L146)
  - `test_unknown_tool_raises(self, tiny_repo: Path)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L150)

### `TestRunIdUniqueness`
- def: [`tests/unit/test_benchmark_harness.py:541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L541)
- doc: Raw benchmark artifacts must survive re-runs: a per-invocation session_id
- signature: `class TestRunIdUniqueness:`
- members:
  - `test_run_record_with_session_id_validates_against_schema(self, tmp_path)` — [`L581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L581) — Codex P2 #332: the new session_id field must NOT break RunRecord's
  - `test_session_id_uniquifies_raw_artifacts(self, tmp_path)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L546)
- uses (calls/refs, reference-scoped): (7 test-only callers)

### `TestRunRecordCostCacheColumns`
- def: [`tests/unit/test_benchmark_harness.py:613`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L613)
- doc: The benchmark must record the provider's REAL cache/cost accounting so a
- signature: `class TestRunRecordCostCacheColumns:`
- members:
  - `test_run_record_accepts_real_cost_cache_columns(self)` — [`L653`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L653)
  - `test_run_record_defaults_keep_old_records_loadable(self)` — [`L620`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L620)
  - `test_runner_captures_codex_cache_hits(self)` — [`L710`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L710) — Codex reports prompt-cache hits as `cached_input_tokens`, not Claude's
  - `test_runner_emits_cost_cache_columns_in_record(self, tmp_path)` — [`L723`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L723)
  - `test_runner_parses_real_cache_cost_from_claude_usage_block(self)` — [`L687`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L687) — The runner must pull cache_read/creation, total_cost_usd and num_turns
- uses (calls/refs, reference-scoped): (11 test-only callers)

### `TestScenarioRegistry`
- def: [`tests/unit/test_benchmark_harness.py:85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L85)
- signature: `class TestScenarioRegistry:`
- members:
  - `test_each_scenario_has_both_runners(self, task: str)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L99)
  - `test_lists_four_scenarios(self)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L86)

### `TestTokenEstimation`
- def: [`tests/unit/test_benchmark_harness.py:199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L199)
- signature: `class TestTokenEstimation:`
- members:
  - `test_empty_string_zero_tokens(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L200)
  - `test_long_string_scales_by_four_chars(self)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L206)
  - `test_short_string_clamps_to_one(self)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L203)

## Functions
- `tiny_repo(tmp_path: Path)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L44) — Create a 3-file Python project. Returns the repo root.

## Module values
- `_BENCH_DIR` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_benchmark_harness.py#L23)

