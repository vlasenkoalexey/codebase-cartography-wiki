---
title: 'Module: tests/unit/test_codegraph_pr_review_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_pr_review_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_pr_review_tool`/
symbols:
  TestFileReview.test_to_dict_with_details: TestFileReview#test_to_dict_with_details().
  TestPRReviewResult.test_to_dict: TestPRReviewResult#test_to_dict().
  TestHelpers.test_build_recommendations_api_changes: TestHelpers#test_build_recommendations_api_changes().
  TestFileReview.test_to_dict_minimal: TestFileReview#test_to_dict_minimal().
  TestCoverageToolMethods.test_build_recommendations_refactor: TestCoverageToolMethods#test_build_recommendations_refactor().
  _run: _run().
  _make_project: _make_project().
  TestPhantomEdgeFilter._make_func: TestPhantomEdgeFilter#_make_func().
  TestPhantomEdgeFilter.test_analyze_call_graph_impact_filters_phantoms: TestPhantomEdgeFilter#test_analyze_call_graph_impact_filters_phantoms().
  TestCoverageToolMethods.test_analyze_call_graph_impact_function_refs_exception: TestCoverageToolMethods#test_analyze_call_graph_impact_function_refs_exception().
  TestCoverageToolMethods.test_analyze_call_graph_impact_dedup_upstream: TestCoverageToolMethods#test_analyze_call_graph_impact_dedup_upstream().
  TestCoverageToolMethods.test_get_call_graph_uses_cache_if_available: TestCoverageToolMethods#test_get_call_graph_uses_cache_if_available().
  TestCoverageToolMethods.test_analyze_call_graph_impact_dedup_callee: TestCoverageToolMethods#test_analyze_call_graph_impact_dedup_callee().
  TestCoverageToolMethods.test_analyze_call_graph_impact_ambiguous_anchor_dropped: TestCoverageToolMethods#test_analyze_call_graph_impact_ambiguous_anchor_dropped().
  TestCoverageToolMethods.test_analyze_call_graph_impact_unknown_lang_file: TestCoverageToolMethods#test_analyze_call_graph_impact_unknown_lang_file().
  TestCodeGraphPRReviewTool.test_tool_definition: TestCodeGraphPRReviewTool#test_tool_definition().
  TestCodeGraphPRReviewTool.test_no_changes: TestCodeGraphPRReviewTool#test_no_changes().
  TestCodeGraphPRReviewTool.test_local_diff_review: TestCodeGraphPRReviewTool#test_local_diff_review().
  TestCodeGraphPRReviewTool.test_output_format_json: TestCodeGraphPRReviewTool#test_output_format_json().
  TestCodeGraphPRReviewTool.test_no_changed_files_only_reachable_with_valid_non_pr_mode: TestCodeGraphPRReviewTool#test_no_changed_files_only_reachable_with_valid_non_pr_mode().
  TestPhantomEdgeFilter.test_known_generic_callback_name_dropped: TestPhantomEdgeFilter#test_known_generic_callback_name_dropped().
  TestPhantomEdgeFilter.test_three_same_name_functions_in_one_file_not_ambiguous: TestPhantomEdgeFilter#test_three_same_name_functions_in_one_file_not_ambiguous().
  TestPhantomEdgeFilter.test_same_name_across_three_distinct_files_is_ambiguous: TestPhantomEdgeFilter#test_same_name_across_three_distinct_files_is_ambiguous().
  TestPhantomEdgeFilter.test_analyze_call_graph_impact_distinct_file_counting: TestPhantomEdgeFilter#test_analyze_call_graph_impact_distinct_file_counting().
  TestCoverageToolMethods.test_call_graph_initialized_true_after_set: TestCoverageToolMethods#test_call_graph_initialized_true_after_set().
  TestCoverageToolMethods.test_on_project_root_changed_resets_call_graph: TestCoverageToolMethods#test_on_project_root_changed_resets_call_graph().
  TestCoverageToolMethods.test_analyze_call_graph_impact_graph_build_exception: TestCoverageToolMethods#test_analyze_call_graph_impact_graph_build_exception().
  TestCoverageToolMethods.test_execute_skipped_file_no_language: TestCoverageToolMethods#test_execute_skipped_file_no_language().
  TestCoverageToolMethods.test_execute_skips_file_with_no_old_new_src: TestCoverageToolMethods#test_execute_skips_file_with_no_old_new_src().
  TestCoverageToolMethods.test_execute_api_change_detection: TestCoverageToolMethods#test_execute_api_change_detection().
  TestCoverageToolMethods.test_high_risk_changes_hunks_are_lean_no_ast_children: TestCoverageToolMethods#test_high_risk_changes_hunks_are_lean_no_ast_children().
  TestCoverageToolMethods.test_execute_pr_url_in_response: TestCoverageToolMethods#test_execute_pr_url_in_response().
  TestHelpers.test_branch_diff_uses_current_pr_base: TestHelpers#test_branch_diff_uses_current_pr_base().
  TestCodeGraphPRReviewTool.test_validate_bad_mode: TestCodeGraphPRReviewTool#test_validate_bad_mode().
  TestCodeGraphPRReviewTool.test_pr_url_invalid: TestCodeGraphPRReviewTool#test_pr_url_invalid().
  TestCodeGraphPRReviewTool.test_pr_url_gh_unavailable: TestCodeGraphPRReviewTool#test_pr_url_gh_unavailable().
  TestCodeGraphPRReviewTool.test_pr_mode_without_pr_url_fails_with_error: TestCodeGraphPRReviewTool#test_pr_mode_without_pr_url_fails_with_error().
  TestCodeGraphPRReviewTool.test_pr_mode_with_empty_pr_url_fails_with_error: TestCodeGraphPRReviewTool#test_pr_mode_with_empty_pr_url_fails_with_error().
  TestCodeGraphPRReviewTool.test_pr_mode_without_pr_url_has_recovery_hint: TestCodeGraphPRReviewTool#test_pr_mode_without_pr_url_has_recovery_hint().
  TestCodeGraphPRReviewTool.test_pr_mode_wrong_param_name_fails_not_empty_success: TestCodeGraphPRReviewTool#test_pr_mode_wrong_param_name_fails_not_empty_success().
  TestPhantomEdgeFilter.test_same_language_specific_name_kept: TestPhantomEdgeFilter#test_same_language_specific_name_kept().
  TestPhantomEdgeFilter.test_cross_language_phantom_dropped: TestPhantomEdgeFilter#test_cross_language_phantom_dropped().
  TestPhantomEdgeFilter.test_ambiguous_count_name_dropped: TestPhantomEdgeFilter#test_ambiguous_count_name_dropped().
  TestPhantomEdgeFilter.test_full_scenario_exact_pin: TestPhantomEdgeFilter#test_full_scenario_exact_pin().
  TestPhantomEdgeFilter.test_empty_language_passes_through: TestPhantomEdgeFilter#test_empty_language_passes_through().
  TestCoverageToolMethods.test_call_graph_initialized_false: TestCoverageToolMethods#test_call_graph_initialized_false().
  TestCoverageToolMethods.test_get_call_graph_no_project_root: TestCoverageToolMethods#test_get_call_graph_no_project_root().
  TestCoverageToolMethods.test_get_call_graph_public_alias: TestCoverageToolMethods#test_get_call_graph_public_alias().
  TestCoverageToolMethods.test_try_get_cache_no_project_root: TestCoverageToolMethods#test_try_get_cache_no_project_root().
  TestCoverageToolMethods.test_try_get_cache_exception_returns_none: TestCoverageToolMethods#test_try_get_cache_exception_returns_none().
  TestHelpers.test_risk_to_score: TestHelpers#test_risk_to_score().
  TestHelpers.test_score_to_risk: TestHelpers#test_score_to_risk().
  TestHelpers.test_compute_verdict: TestHelpers#test_compute_verdict().
  TestHelpers.test_parse_diff_files: TestHelpers#test_parse_diff_files().
  TestHelpers.test_build_recommendations_empty: TestHelpers#test_build_recommendations_empty().
  TestPhantomEdgeFilter.test_upstream_cpp_caller_of_c_header_kept: TestPhantomEdgeFilter#test_upstream_cpp_caller_of_c_header_kept().
  TestPhantomEdgeFilter.test_upstream_pure_c_caller_of_cpp_definition_dropped: TestPhantomEdgeFilter#test_upstream_pure_c_caller_of_cpp_definition_dropped().
  TestPhantomEdgeFilter.test_downstream_cpp_definition_called_from_c_header_dropped: TestPhantomEdgeFilter#test_downstream_cpp_definition_called_from_c_header_dropped().
  TestPhantomEdgeFilter.test_downstream_c_definition_called_from_cpp_caller_kept: TestPhantomEdgeFilter#test_downstream_c_definition_called_from_cpp_caller_kept().
  TestHelperUtilities.test_extract_file_diff_found: TestHelperUtilities#test_extract_file_diff_found().
  TestHelperUtilities.test_extract_file_diff_not_found_returns_empty: TestHelperUtilities#test_extract_file_diff_not_found_returns_empty().
  TestHelperUtilities.test_extract_old_new_from_diff_basic: TestHelperUtilities#test_extract_old_new_from_diff_basic().
  TestHelperUtilities.test_extract_old_new_no_newline_marker: TestHelperUtilities#test_extract_old_new_no_newline_marker().
  TestHelperUtilities.test_get_local_diff_no_project_root: TestHelperUtilities#test_get_local_diff_no_project_root().
  TestHelperUtilities.test_get_local_diff_subprocess_timeout: TestHelperUtilities#test_get_local_diff_subprocess_timeout().
  TestHelperUtilities.test_get_local_diff_file_not_found: TestHelperUtilities#test_get_local_diff_file_not_found().
  TestHelperUtilities.test_get_local_diff_nonzero_returncode: TestHelperUtilities#test_get_local_diff_nonzero_returncode().
  TestCoverageToolMethods.test_compute_verdict_fallback: TestCoverageToolMethods#test_compute_verdict_fallback().
  TestCoverageToolMethods.test_build_recommendations_large_blast_radius: TestCoverageToolMethods#test_build_recommendations_large_blast_radius().
  TestCoverageToolMethods.test_get_old_source_exception: TestCoverageToolMethods#test_get_old_source_exception().
  TestCoverageToolMethods.test_get_old_source_file_not_found: TestCoverageToolMethods#test_get_old_source_file_not_found().
  TestCoverageToolMethods.test_get_new_source_os_error: TestCoverageToolMethods#test_get_new_source_os_error().
  TestHelpers.fake_run: TestHelpers#fake_run().
  TestHelpers: TestHelpers#
  TestFileReview: TestFileReview#
  TestPRReviewResult: TestPRReviewResult#
  TestCodeGraphPRReviewTool: TestCodeGraphPRReviewTool#
  TestPhantomEdgeFilter: TestPhantomEdgeFilter#
  TestHelperUtilities: TestHelperUtilities#
  TestCoverageToolMethods: TestCoverageToolMethods#
---
# Module: [`tests/unit/test_codegraph_pr_review_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py)

## Classes
### `TestCodeGraphPRReviewTool`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L182)
- signature: `class TestCodeGraphPRReviewTool:`
- members:
  - `test_local_diff_review(self)` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L208)
  - `test_no_changed_files_only_reachable_with_valid_non_pr_mode(self)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L326) — The 'No changed files found' path must only trigger for non-pr modes
  - `test_no_changes(self)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L197)
  - `test_output_format_json(self)` — [`L272`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L272)
  - `test_pr_mode_with_empty_pr_url_fails_with_error(self)` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L295) — mode=pr with pr_url='' → same failure (typo scenario from issue #451).
  - `test_pr_mode_without_pr_url_fails_with_error(self)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L287) — mode=pr with missing pr_url → success:False, error naming the param.
  - `test_pr_mode_without_pr_url_has_recovery_hint(self)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L303) — Error response must carry a recovery_hint with a usage example.
  - `test_pr_mode_wrong_param_name_fails_not_empty_success(self)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L313) — After facade projects args, inner receives mode=pr without pr_url.
  - `test_pr_url_gh_unavailable(self)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L256)
  - `test_pr_url_invalid(self)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L250)
  - `test_tool_definition(self)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L183)
  - `test_validate_bad_mode(self)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L192)
- uses (calls/refs, reference-scoped): [`CodeGraphPRReviewTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.get_tool_definition), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.get_tool_schema), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.validate_arguments)  (2 test-only)

### `TestCoverageToolMethods`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:867`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L867)
- doc: Cover CodeGraphPRReviewTool methods not exercised by main execute path.
- signature: `class TestCoverageToolMethods:`
- members:
  - `test_analyze_call_graph_impact_ambiguous_anchor_dropped(self)` — [`L1255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1255) — Anchor with ambiguous name (count >= threshold) → callers go to ambiguous_dropped.
  - `test_analyze_call_graph_impact_dedup_callee(self)` — [`L1229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1229) — Duplicate callee entries (same qualified_name) are deduplicated.
  - `test_analyze_call_graph_impact_dedup_upstream(self)` — [`L936`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L936) — Duplicate caller entries (same qualified_name) are deduplicated.
  - `test_analyze_call_graph_impact_function_refs_exception(self)` — [`L915`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L915) — If function_refs() raises, name_file_count stays empty (no crash).
  - `test_analyze_call_graph_impact_graph_build_exception(self)` — [`L904`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L904) — If graph.build() raises, returns empty stats (no crash).
  - `test_analyze_call_graph_impact_unknown_lang_file(self)` — [`L1305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1305) — Changed file with unknown extension → empty changed_langs → lang gate skips.
  - `test_build_recommendations_large_blast_radius(self)` — [`L971`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L971) — More than 5 upstream callers triggers the large-blast-radius recommendation.
  - `test_build_recommendations_refactor(self)` — [`L981`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L981) — Refactor files trigger the refactor recommendation.
  - `test_call_graph_initialized_false(self)` — [`L870`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L870)
  - `test_call_graph_initialized_true_after_set(self)` — [`L874`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L874)
  - `test_compute_verdict_fallback(self)` — [`L961`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L961) — Unknown risk falls through to REVIEW (fail-safe).
  - `test_execute_api_change_detection(self)` — [`L1108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1108) — API changes are captured in api_changes field.
  - `test_execute_pr_url_in_response(self)` — [`L1329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1329) — When pr_url is provided via gh path (mocked), it appears in the response.
  - `test_execute_skipped_file_no_language(self)` — [`L995`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L995) — Files without a recognised extension are counted in files_skipped.
  - `test_execute_skips_file_with_no_old_new_src(self)` — [`L1075`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1075) — Files with no old + new source are counted as skipped (both empty).
  - `test_get_call_graph_no_project_root(self)` — [`L879`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L879)
  - `test_get_call_graph_public_alias(self)` — [`L886`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L886) — get_call_graph() delegates to _get_call_graph().
  - `test_get_call_graph_uses_cache_if_available(self)` — [`L1064`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1064) — _get_call_graph uses CachedCallGraph when _try_get_cache returns a cache.
  - `test_get_new_source_os_error(self)` — [`L1038`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1038) — _get_new_source returns '' when file is unreadable.
  - `test_get_old_source_exception(self)` — [`L1018`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1018) — _get_old_source returns '' when subprocess raises TimeoutExpired.
  - `test_get_old_source_file_not_found(self)` — [`L1029`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1029) — _get_old_source returns '' when git binary missing.
  - `test_high_risk_changes_hunks_are_lean_no_ast_children(self)` — [`L1170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1170) — BUG A (Codex P2 #696 follow-up): high_risk_changes entries must NOT
  - `test_on_project_root_changed_resets_call_graph(self)` — [`L893`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L893)
  - `test_try_get_cache_exception_returns_none(self)` — [`L1047`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L1047) — _try_get_cache returns None when ASTCache import raises.
  - `test_try_get_cache_no_project_root(self)` — [`L899`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L899)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`CodeGraphPRReviewTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool), [`_analyze_call_graph_impact`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._analyze_call_graph_impact), [`_get_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._get_call_graph), [`_build_recommendations`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_build_recommendations), [`_try_get_cache`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._try_get_cache), [`FileReview`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview), [`_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._call_graph), [`file_path`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.file_path), [`_compute_verdict`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_compute_verdict), [`category_counts`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.category_counts), [`dominant_category`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.dominant_category), [`risk_level`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.risk_level), [`change_summary`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.change_summary), [`get_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.get_call_graph), [`hunk_count`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.hunk_count), [`language`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.language), [`_get_old_source`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_get_old_source), [`call_graph_initialized`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.call_graph_initialized), [`_on_project_root_changed`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._on_project_root_changed), [`_get_new_source`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_get_new_source)  (2 test-only)

### `TestFileReview`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L130)
- signature: `class TestFileReview:`
- members:
  - `test_to_dict_minimal(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L131)
  - `test_to_dict_with_details(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L146)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.to_dict), [`FileReview`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview), [`file_path`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.file_path), [`category_counts`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.category_counts), [`dominant_category`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.dominant_category), [`risk_level`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.risk_level), [`change_summary`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.change_summary), [`hunk_count`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.hunk_count), [`language`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.language), [`high_risk_hunks`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.high_risk_hunks)

### `TestHelperUtilities`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:804`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L804)
- doc: Cover standalone helper functions not exercised by the E2E path.
- signature: `class TestHelperUtilities:`
- members:
  - `test_extract_file_diff_found(self)` — [`L807`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L807)
  - `test_extract_file_diff_not_found_returns_empty(self)` — [`L824`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L824)
  - `test_extract_old_new_from_diff_basic(self)` — [`L830`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L830)
  - `test_extract_old_new_no_newline_marker(self)` — [`L836`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L836) — '\' continuation lines (e.g. '\ No newline at end of file') are skipped.
  - `test_get_local_diff_file_not_found(self)` — [`L853`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L853)
  - `test_get_local_diff_no_project_root(self)` — [`L842`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L842)
  - `test_get_local_diff_nonzero_returncode(self)` — [`L858`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L858)
  - `test_get_local_diff_subprocess_timeout(self)` — [`L846`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L846)
- uses (calls/refs, reference-scoped): [`_get_local_diff`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_get_local_diff), [`_extract_file_diff`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_extract_file_diff), [`_extract_old_new_from_diff`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_extract_old_new_from_diff)

### `TestHelpers`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L41)
- signature: `class TestHelpers:`
- members:
  - `fake_run(cmd, **kwargs)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L86)
  - `test_branch_diff_uses_current_pr_base(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L83)
  - `test_build_recommendations_api_changes(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L116)
  - `test_build_recommendations_empty(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L111)
  - `test_compute_verdict(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L55)
  - `test_parse_diff_files(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L65)
  - `test_risk_to_score(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L42)
  - `test_score_to_risk(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L49)
- uses (calls/refs, reference-scoped): [`_build_recommendations`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_build_recommendations), [`_get_local_diff`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_get_local_diff), [`FileReview`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview), [`file_path`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.file_path), [`_compute_verdict`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_compute_verdict), [`_risk_to_score`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_risk_to_score), [`category_counts`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.category_counts), [`dominant_category`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.dominant_category), [`risk_level`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.risk_level), [`_score_to_risk`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_score_to_risk), [`change_summary`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.change_summary), [`hunk_count`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.hunk_count), [`language`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#FileReview.language), [`_parse_diff_files`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_parse_diff_files)

### `TestPRReviewResult`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L162)
- signature: `class TestPRReviewResult:`
- members:
  - `test_to_dict(self)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L163)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.to_dict), [`file_reviews`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.file_reviews), [`PRReviewResult`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult), [`affected_functions`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.affected_functions), [`api_changes`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.api_changes), [`files_reviewed`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.files_reviewed), [`files_skipped`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.files_skipped), [`overall_risk`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.overall_risk), [`overall_verdict`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.overall_verdict), [`recommendations`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#PRReviewResult.recommendations)

### `TestPhantomEdgeFilter`
- def: [`tests/unit/test_codegraph_pr_review_tool.py:347`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L347)
- doc: RED-first tests for _filter_affected_by_language (Issue #450).
- signature: `class TestPhantomEdgeFilter:`
- members:
  - `test_ambiguous_count_name_dropped(self)` — [`L407`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L407) — A same-language edge whose bare name exists in ≥ threshold files is
  - `test_analyze_call_graph_impact_distinct_file_counting(self)` — [`L663`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L663) — Integration: _analyze_call_graph_impact uses distinct-file counting.
  - `test_analyze_call_graph_impact_filters_phantoms(self)` — [`L733`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L733) — End-to-end: _analyze_call_graph_impact populates stats fields
  - `test_cross_language_phantom_dropped(self)` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L392) — A swift phantom for a kotlin change must be dropped (cross-language gate).
  - `test_downstream_c_definition_called_from_cpp_caller_kept(self)` — [`L567`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L567) — Downstream edge: changed cpp file calls a c definition (c header).
  - `test_downstream_cpp_definition_called_from_c_header_dropped(self)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L546) — Downstream edge: changed c file calls a cpp definition.
  - `test_empty_language_passes_through(self)` — [`L488`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L488) — An edge with empty/unknown language must not be dropped (unknown > wrong).
  - `test_full_scenario_exact_pin(self)` — [`L447`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L447) — Integration scenario: kotlin change with real caller + swift phantom
  - `test_known_generic_callback_name_dropped(self)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L427) — A name in _KNOWN_GENERIC_CALLBACK_NAMES is dropped even below count threshold.
  - `test_same_language_specific_name_kept(self)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L378) — A same-language upstream edge with a specific (non-generic) name must survive.
  - `test_same_name_across_three_distinct_files_is_ambiguous(self)` — [`L629`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L629) — Same name in 3 different files → distinct-file count == 3
  - `test_three_same_name_functions_in_one_file_not_ambiguous(self)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L592) — 3 refs of the same name all from ONE file → distinct-file count == 1
  - `test_upstream_cpp_caller_of_c_header_kept(self)` — [`L505`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L505) — Upstream edge: C++ caller calls into a changed .h (indexed as 'c').
  - `test_upstream_pure_c_caller_of_cpp_definition_dropped(self)` — [`L526`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L526) — Upstream edge: pure-C caller calls into a changed .cpp definition.
- protocol/private: `_make_func`[`L363`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L363)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CodeGraphPRReviewTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool), [`_analyze_call_graph_impact`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._analyze_call_graph_impact), [`_filter_affected_by_language`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_filter_affected_by_language), [`_KNOWN_GENERIC_CALLBACK_NAMES`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_KNOWN_GENERIC_CALLBACK_NAMES._KNOWN_GENERIC_CALLBACK_NAMES), [`_AMBIGUOUS_NAME_FILE_THRESHOLD`](../../tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.md#_AMBIGUOUS_NAME_FILE_THRESHOLD)  (1 test-only)

## Functions
- `_make_project(*files: tuple[str, str])` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L32)
- `_run(tool: CodeGraphPRReviewTool, args: dict)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_pr_review_tool.py#L28)

