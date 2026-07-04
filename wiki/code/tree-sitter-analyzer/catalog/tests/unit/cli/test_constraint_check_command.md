---
title: 'Module: tests/unit/cli/test_constraint_check_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_constraint_check_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_constraint_check_command`/
symbols:
  _v: _v().
  _APPLY_TOON: _APPLY_TOON.
  TestRunAndPersist.test_violations_table_cleared_before_insert: TestRunAndPersist#test_violations_table_cleared_before_insert().
  TestEvaluateWithExplicitFile.test_with_db_and_error_violations_returns_unsafe: TestEvaluateWithExplicitFile#test_with_db_and_error_violations_returns_unsafe().
  TestRunCheckConstraints.test_with_constraint_file_routes_to_evaluate_explicit: TestRunCheckConstraints#test_with_constraint_file_routes_to_evaluate_explicit().
  TestRunCheckConstraints.test_without_constraint_file_calls_asyncio_run: TestRunCheckConstraints#test_without_constraint_file_calls_asyncio_run().
  TestRunCheckConstraints.test_caution_verdict_returns_exit_2: TestRunCheckConstraints#test_caution_verdict_returns_exit_2().
  TestRunCheckConstraints.test_failure_result_returns_exit_1: TestRunCheckConstraints#test_failure_result_returns_exit_1().
  TestRunCheckConstraints.test_print_result_called_with_result_and_format: TestRunCheckConstraints#test_print_result_called_with_result_and_format().
  TestRunCheckConstraints.test_path_filter_passed_to_evaluate_explicit: TestRunCheckConstraints#test_path_filter_passed_to_evaluate_explicit().
  TestRunAndPersist.test_violations_persisted_to_db: TestRunAndPersist#test_violations_persisted_to_db().
  TestRunAndPersist.test_duplicate_pk_violations_do_not_crash_persist: TestRunAndPersist#test_duplicate_pk_violations_do_not_crash_persist().
  TestEvaluateWithExplicitFile.test_parse_error_returns_failure: TestEvaluateWithExplicitFile#test_parse_error_returns_failure().
  TestEvaluateWithExplicitFile.test_with_db_no_violations_returns_safe: TestEvaluateWithExplicitFile#test_with_db_no_violations_returns_safe().
  TestEvaluateWithExplicitFile.test_constraint_file_path_included_in_result: TestEvaluateWithExplicitFile#test_constraint_file_path_included_in_result().
  TestRunCheckConstraints.test_severity_min_defaults_to_warn_when_none: TestRunCheckConstraints#test_severity_min_defaults_to_warn_when_none().
  TestEvaluateWithExplicitFile._call: TestEvaluateWithExplicitFile#_call().
  TestFormatResponse.test_passes_payload_and_format_to_helper: TestFormatResponse#test_passes_payload_and_format_to_helper().
  TestLoadExplicit.test_non_canonical_name_stages_into_tempdir: TestLoadExplicit#test_non_canonical_name_stages_into_tempdir().
  TestLoadExplicit.test_non_canonical_creates_canonical_filename_in_tempdir: TestLoadExplicit#test_non_canonical_creates_canonical_filename_in_tempdir().
  TestLoadExplicit.test_non_canonical_content_is_copied: TestLoadExplicit#test_non_canonical_content_is_copied().
  TestRunAndPersist._db_with_edges: TestRunAndPersist#_db_with_edges().
  TestRunAndPersist.test_evaluate_exception_degrades_gracefully: TestRunAndPersist#test_evaluate_exception_degrades_gracefully().
  TestRunAndPersist.test_returns_edge_count_from_db: TestRunAndPersist#test_returns_edge_count_from_db().
  TestEvaluateWithExplicitFile.test_no_db_returns_safe_with_note: TestEvaluateWithExplicitFile#test_no_db_returns_safe_with_note().
  _PRINT_RESULT: _PRINT_RESULT.
  _RESOLVE_OFMT: _RESOLVE_OFMT.
  _ns: _ns().
  _EVALUATE: _EVALUATE.
  _LOAD_EXPLICIT: _LOAD_EXPLICIT.
  TestFilterViolations.test_no_path_filter_passes_all_at_or_above_severity: TestFilterViolations#test_no_path_filter_passes_all_at_or_above_severity().
  TestFilterViolations.test_severity_floor_excludes_lower_ranked: TestFilterViolations#test_severity_floor_excludes_lower_ranked().
  TestFilterViolations.test_empty_path_filter_skips_glob: TestFilterViolations#test_empty_path_filter_skips_glob().
  TestFilterViolations.test_returned_rows_are_dicts: TestFilterViolations#test_returned_rows_are_dicts().
  TestFilterViolations.test_row_contains_all_expected_keys: TestFilterViolations#test_row_contains_all_expected_keys().
  TestFilterViolations.test_unknown_severity_rank_treated_as_zero: TestFilterViolations#test_unknown_severity_rank_treated_as_zero().
  TestFilterViolations.test_min_severity_rank_zero_passes_everything: TestFilterViolations#test_min_severity_rank_zero_passes_everything().
  TestFormatResponse.test_returns_value_from_apply_toon: TestFormatResponse#test_returns_value_from_apply_toon().
  TestFailureEnvelope.test_success_is_false: TestFailureEnvelope#test_success_is_false().
  TestFailureEnvelope.test_verdict_is_caution: TestFailureEnvelope#test_verdict_is_caution().
  TestFailureEnvelope.test_error_message_included: TestFailureEnvelope#test_error_message_included().
  TestFailureEnvelope.test_violations_is_empty_list: TestFailureEnvelope#test_violations_is_empty_list().
  TestFailureEnvelope.test_rule_count_is_zero: TestFailureEnvelope#test_rule_count_is_zero().
  TestResolveOutputFormat.test_delegates_to_resolve_mcp_tool_format: TestResolveOutputFormat#test_delegates_to_resolve_mcp_tool_format().
  TestResolveOutputFormat.test_returns_toon_when_resolver_says_toon: TestResolveOutputFormat#test_returns_toon_when_resolver_says_toon().
  TestLoadExplicit.test_canonical_name_calls_load_constraints_on_parent: TestLoadExplicit#test_canonical_name_calls_load_constraints_on_parent().
  TestRunAndPersist.test_no_call_edges_table_returns_empty: TestRunAndPersist#test_no_call_edges_table_returns_empty().
  TestRunTool.test_builds_tool_and_returns_execute_coroutine: TestRunTool#test_builds_tool_and_returns_execute_coroutine().
  TestRunTool.test_passes_path_filter_and_severity: TestRunTool#test_passes_path_filter_and_severity().
  TestEvaluateWithExplicitFile.test_file_not_found_returns_failure: TestEvaluateWithExplicitFile#test_file_not_found_returns_failure().
  _LOAD_CONSTRAINTS: _LOAD_CONSTRAINTS.
  _ASYNCIO_RUN: _ASYNCIO_RUN.
  _RUN_AND_PERSIST: _RUN_AND_PERSIST.
  _EVAL_EXPLICIT: _EVAL_EXPLICIT.
  TestExitCodeFor.test_success_false_returns_1: TestExitCodeFor#test_success_false_returns_1().
  TestExitCodeFor.test_missing_success_returns_1: TestExitCodeFor#test_missing_success_returns_1().
  TestExitCodeFor.test_unsafe_verdict_returns_1: TestExitCodeFor#test_unsafe_verdict_returns_1().
  TestExitCodeFor.test_caution_verdict_returns_2: TestExitCodeFor#test_caution_verdict_returns_2().
  TestExitCodeFor.test_safe_verdict_returns_0: TestExitCodeFor#test_safe_verdict_returns_0().
  TestExitCodeFor.test_missing_verdict_defaults_to_safe_returns_0: TestExitCodeFor#test_missing_verdict_defaults_to_safe_returns_0().
  TestComputeVerdict.test_empty_rows_returns_safe: TestComputeVerdict#test_empty_rows_returns_safe().
  TestComputeVerdict.test_error_severity_returns_unsafe: TestComputeVerdict#test_error_severity_returns_unsafe().
  TestComputeVerdict.test_warn_severity_returns_caution: TestComputeVerdict#test_warn_severity_returns_caution().
  TestComputeVerdict.test_info_severity_returns_safe: TestComputeVerdict#test_info_severity_returns_safe().
  TestComputeVerdict.test_error_takes_priority_over_warn: TestComputeVerdict#test_error_takes_priority_over_warn().
  TestComputeVerdict.test_multiple_warns_no_error_returns_caution: TestComputeVerdict#test_multiple_warns_no_error_returns_caution().
  TestViolationsDDL.test_returns_string: TestViolationsDDL#test_returns_string().
  TestViolationsDDL.test_contains_table_name: TestViolationsDDL#test_contains_table_name().
  TestViolationsDDL.test_is_valid_sqlite: TestViolationsDDL#test_is_valid_sqlite().
  TestViolationsDDL.test_is_idempotent_if_not_exists: TestViolationsDDL#test_is_idempotent_if_not_exists().
  TestPrintResult.test_toon_prints_toon_content: TestPrintResult#test_toon_prints_toon_content().
  TestPrintResult.test_json_prints_json: TestPrintResult#test_json_prints_json().
  TestPrintResult.test_toon_missing_key_prints_empty_string: TestPrintResult#test_toon_missing_key_prints_empty_string().
  TestPrintResult.test_json_output_is_indented: TestPrintResult#test_json_output_is_indented().
  TestGetDefaultProjectRoot.test_returns_project_root_attr: TestGetDefaultProjectRoot#test_returns_project_root_attr().
  TestGetDefaultProjectRoot.test_falls_back_to_cwd_when_none: TestGetDefaultProjectRoot#test_falls_back_to_cwd_when_none().
  TestGetDefaultProjectRoot.test_falls_back_to_cwd_when_attr_missing: TestGetDefaultProjectRoot#test_falls_back_to_cwd_when_attr_missing().
  TestRunAndPersist.test_empty_call_edges_table_returns_empty: TestRunAndPersist#test_empty_call_edges_table_returns_empty().
  _RESOLVE_FMT: _RESOLVE_FMT.
  _CCT_CLS: _CCT_CLS.
  TestLoadExplicit.capture: TestLoadExplicit#capture().
  TestFormatResponse.capture: TestFormatResponse#capture().
  TestLoadExplicit.capture_and_check: TestLoadExplicit#capture_and_check().
  TestRunAndPersist._empty_db: TestRunAndPersist#_empty_db().
  TestExitCodeFor: TestExitCodeFor#
  TestComputeVerdict: TestComputeVerdict#
  TestFilterViolations: TestFilterViolations#
  TestViolationsDDL: TestViolationsDDL#
  TestFormatResponse: TestFormatResponse#
  TestFailureEnvelope: TestFailureEnvelope#
  TestResolveOutputFormat: TestResolveOutputFormat#
  TestPrintResult: TestPrintResult#
  TestGetDefaultProjectRoot: TestGetDefaultProjectRoot#
  TestLoadExplicit: TestLoadExplicit#
  TestRunAndPersist: TestRunAndPersist#
  TestRunTool: TestRunTool#
  TestEvaluateWithExplicitFile: TestEvaluateWithExplicitFile#
  TestRunCheckConstraints: TestRunCheckConstraints#
---
# Module: [`tests/unit/cli/test_constraint_check_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py)

## Classes
### `TestComputeVerdict`
- def: [`tests/unit/cli/test_constraint_check_command.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L119)
- signature: `class TestComputeVerdict:`
- members:
  - `test_empty_rows_returns_safe(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L120)
  - `test_error_severity_returns_unsafe(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L123)
  - `test_error_takes_priority_over_warn(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L132)
  - `test_info_severity_returns_safe(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L129)
  - `test_multiple_warns_no_error_returns_caution(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L136)
  - `test_warn_severity_returns_caution(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L126)
- uses (calls/refs, reference-scoped): [`_compute_verdict`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_compute_verdict)

### `TestEvaluateWithExplicitFile`
- def: [`tests/unit/cli/test_constraint_check_command.py:595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L595)
- signature: `class TestEvaluateWithExplicitFile:`
- members:
  - `test_constraint_file_path_included_in_result(self, tmp_path)` — [`L655`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L655)
  - `test_file_not_found_returns_failure(self, tmp_path)` — [`L613`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L613)
  - `test_no_db_returns_safe_with_note(self, tmp_path)` — [`L630`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L630)
  - `test_parse_error_returns_failure(self, tmp_path)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L619)
  - `test_with_db_and_error_violations_returns_unsafe(self, tmp_path)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L668)
  - `test_with_db_no_violations_returns_safe(self, tmp_path)` — [`L640`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L640)
- protocol/private: `_call`[`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L596)
- uses (calls/refs, reference-scoped): [`_evaluate_with_explicit_file`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_evaluate_with_explicit_file), [`ConstraintParseError`](../../../tree_sitter_analyzer/constraints/parser.md#ConstraintParseError)  (4 test-only)

### `TestExitCodeFor`
- def: [`tests/unit/cli/test_constraint_check_command.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L93)
- signature: `class TestExitCodeFor:`
- members:
  - `test_caution_verdict_returns_2(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L103)
  - `test_missing_success_returns_1(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L97)
  - `test_missing_verdict_defaults_to_safe_returns_0(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L109)
  - `test_safe_verdict_returns_0(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L106)
  - `test_success_false_returns_1(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L94)
  - `test_unsafe_verdict_returns_1(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L100)
- uses (calls/refs, reference-scoped): [`_exit_code_for`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_exit_code_for)

### `TestFailureEnvelope`
- def: [`tests/unit/cli/test_constraint_check_command.py:262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L262)
- signature: `class TestFailureEnvelope:`
- members:
  - `test_error_message_included(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L273)
  - `test_rule_count_is_zero(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L283)
  - `test_success_is_false(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L263)
  - `test_verdict_is_caution(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L268)
  - `test_violations_is_empty_list(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L278)
- uses (calls/refs, reference-scoped): [`_failure_envelope`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_failure_envelope)  (1 test-only)

### `TestFilterViolations`
- def: [`tests/unit/cli/test_constraint_check_command.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L146)
- signature: `class TestFilterViolations:`
- members:
  - `test_empty_path_filter_skips_glob(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L163)
  - `test_min_severity_rank_zero_passes_everything(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L200)
  - `test_no_path_filter_passes_all_at_or_above_severity(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L147)
  - `test_returned_rows_are_dicts(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L168)
  - `test_row_contains_all_expected_keys(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L172)
  - `test_severity_floor_excludes_lower_ranked(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L152)
  - `test_unknown_severity_rank_treated_as_zero(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L195)
- uses (calls/refs, reference-scoped): [`_filter_violations`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_filter_violations)  (1 test-only)

### `TestFormatResponse`
- def: [`tests/unit/cli/test_constraint_check_command.py:235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L235)
- signature: `class TestFormatResponse:`
- members:
  - `capture(p, fmt)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L247)
  - `test_passes_payload_and_format_to_helper(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L243)
  - `test_returns_value_from_apply_toon(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L236)
- uses (calls/refs, reference-scoped): [`_format_response`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_format_response)  (1 test-only)

### `TestGetDefaultProjectRoot`
- def: [`tests/unit/cli/test_constraint_check_command.py:341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L341)
- signature: `class TestGetDefaultProjectRoot:`
- members:
  - `test_falls_back_to_cwd_when_attr_missing(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L350)
  - `test_falls_back_to_cwd_when_none(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L346)
  - `test_returns_project_root_attr(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L342)
- uses (calls/refs, reference-scoped): [`get_default_project_root`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#get_default_project_root)

### `TestLoadExplicit`
- def: [`tests/unit/cli/test_constraint_check_command.py:359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L359)
- signature: `class TestLoadExplicit:`
- members:
  - `capture(root: str)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L373)
  - `capture_and_check(root: str)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L387)
  - `test_canonical_name_calls_load_constraints_on_parent(self, tmp_path)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L360)
  - `test_non_canonical_content_is_copied(self, tmp_path)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L395)
  - `test_non_canonical_creates_canonical_filename_in_tempdir(self, tmp_path)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L383)
  - `test_non_canonical_name_stages_into_tempdir(self, tmp_path)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L368)
- uses (calls/refs, reference-scoped): [`_load_explicit`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_load_explicit)  (1 test-only)

### `TestPrintResult`
- def: [`tests/unit/cli/test_constraint_check_command.py:314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L314)
- signature: `class TestPrintResult:`
- members:
  - `test_json_output_is_indented(self, capsys)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L330)
  - `test_json_prints_json(self, capsys)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L320)
  - `test_toon_missing_key_prints_empty_string(self, capsys)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L326)
  - `test_toon_prints_toon_content(self, capsys)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L315)
- uses (calls/refs, reference-scoped): [`_print_result`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_print_result)

### `TestResolveOutputFormat`
- def: [`tests/unit/cli/test_constraint_check_command.py:294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L294)
- signature: `class TestResolveOutputFormat:`
- members:
  - `test_delegates_to_resolve_mcp_tool_format(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L295)
  - `test_returns_toon_when_resolver_says_toon(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L302)
- uses (calls/refs, reference-scoped): [`_resolve_output_format`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_resolve_output_format)  (1 test-only)

### `TestRunAndPersist`
- def: [`tests/unit/cli/test_constraint_check_command.py:417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L417)
- signature: `class TestRunAndPersist:`
- members:
  - `test_duplicate_pk_violations_do_not_crash_persist(self, tmp_path)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L504) — Regression for #544: two violations with the same PK must not crash.
  - `test_empty_call_edges_table_returns_empty(self, tmp_path)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L446)
  - `test_evaluate_exception_degrades_gracefully(self, tmp_path)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L456)
  - `test_no_call_edges_table_returns_empty(self, tmp_path)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L439)
  - `test_returns_edge_count_from_db(self, tmp_path)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L474)
  - `test_violations_persisted_to_db(self, tmp_path)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L463)
  - `test_violations_table_cleared_before_insert(self, tmp_path)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L480)
- protocol/private: `_db_with_edges`[`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L423), `_empty_db`[`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L418)
- uses (calls/refs, reference-scoped): [`_run_and_persist`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_run_and_persist), [`EDGE_STORE_SCHEMA`](../../../tree_sitter_analyzer/graph/edge_store.md#EDGE_STORE_SCHEMA), [`_violations_ddl`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_violations_ddl)  (2 test-only)

### `TestRunCheckConstraints`
- def: [`tests/unit/cli/test_constraint_check_command.py:696`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L696)
- signature: `class TestRunCheckConstraints:`
- members:
  - `test_caution_verdict_returns_exit_2(self, tmp_path)` — [`L717`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L717)
  - `test_failure_result_returns_exit_1(self, tmp_path)` — [`L726`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L726)
  - `test_path_filter_passed_to_evaluate_explicit(self, tmp_path)` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L758)
  - `test_print_result_called_with_result_and_format(self, tmp_path)` — [`L749`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L749)
  - `test_severity_min_defaults_to_warn_when_none(self, tmp_path)` — [`L735`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L735)
  - `test_with_constraint_file_routes_to_evaluate_explicit(self, tmp_path)` — [`L697`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L697)
  - `test_without_constraint_file_calls_asyncio_run(self, tmp_path)` — [`L707`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L707)
- uses (calls/refs, reference-scoped): [`run_check_constraints`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#run_check_constraints)  (5 test-only)

### `TestRunTool`
- def: [`tests/unit/cli/test_constraint_check_command.py:560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L560)
- signature: `class TestRunTool:`
- members:
  - `test_builds_tool_and_returns_execute_coroutine(self, tmp_path)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L561)
  - `test_passes_path_filter_and_severity(self, tmp_path)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L575)
- uses (calls/refs, reference-scoped): [`_run_tool`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_run_tool)  (1 test-only)

### `TestViolationsDDL`
- def: [`tests/unit/cli/test_constraint_check_command.py:211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L211)
- signature: `class TestViolationsDDL:`
- members:
  - `test_contains_table_name(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L215)
  - `test_is_idempotent_if_not_exists(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L223)
  - `test_is_valid_sqlite(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L218)
  - `test_returns_string(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L212)
- uses (calls/refs, reference-scoped): [`_violations_ddl`](../../../tree_sitter_analyzer/cli/commands/constraint_check_command.md#_violations_ddl)

## Functions
- `_ns(**kwargs: object)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L688)
- `_v(severity: str = "error", rule_id: str = "R1", caller_file: str = "a.py", caller_name: str = "foo", caller_line: int = 10, callee_name: str = "bar", callee_file: str = "b.py", detected_at: int | None = None)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L66)

## Module values
- `_APPLY_TOON` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L31)
- `_ASYNCIO_RUN` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L49)
- `_CCT_CLS` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L56)
- `_EVALUATE` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L38)
- `_EVAL_EXPLICIT` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L45)
- `_LOAD_CONSTRAINTS` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L35)
- `_LOAD_EXPLICIT` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L39)
- `_PRINT_RESULT` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L50)
- `_RESOLVE_FMT` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L34)
- `_RESOLVE_OFMT` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L53)
- `_RUN_AND_PERSIST` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_constraint_check_command.py#L42)

