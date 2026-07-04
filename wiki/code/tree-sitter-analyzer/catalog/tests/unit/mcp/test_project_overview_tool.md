---
title: 'Module: tests/unit/mcp/test_project_overview_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_project_overview_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_project_overview_tool`/
symbols:
  _write: _write().
  TestProjectOverviewExecute.test_execute_basic_json: TestProjectOverviewExecute#test_execute_basic_json().
  TestProjectOverviewExecute.test_execute_toon_format: TestProjectOverviewExecute#test_execute_toon_format().
  TestProjectOverviewExecute.test_execute_multi_language_project: TestProjectOverviewExecute#test_execute_multi_language_project().
  TestEdgeCases.test_max_depth_1: TestEdgeCases#test_max_depth_1().
  TestEdgeCases.test_unicode_filename: TestEdgeCases#test_unicode_filename().
  TestEdgeCases.test_all_supported_extensions: TestEdgeCases#test_all_supported_extensions().
  _run: _run().
  TestProjectOverviewExecute.test_execute_no_project_root_raises: TestProjectOverviewExecute#test_execute_no_project_root_raises().
  TestProjectOverviewExecute.test_execute_invalid_root_raises: TestProjectOverviewExecute#test_execute_invalid_root_raises().
  TestProjectOverviewExecute.test_execute_empty_project: TestProjectOverviewExecute#test_execute_empty_project().
  TestGitignoreSupport.test_load_gitignore_patterns_exists: TestGitignoreSupport#test_load_gitignore_patterns_exists().
  TestGitignoreSupport.test_load_gitignore_patterns_with_comments: TestGitignoreSupport#test_load_gitignore_patterns_with_comments().
  TestGitignoreSupport.test_is_ignored_by_gitignore_normalization: TestGitignoreSupport#test_is_ignored_by_gitignore_normalization().
  TestAddFileToScan.test_adds_source_file: TestAddFileToScan#test_adds_source_file().
  TestAddFileToScan.test_skips_unsupported_extension: TestAddFileToScan#test_skips_unsupported_extension().
  TestAddFileToScan.test_records_extension_even_for_unsupported: TestAddFileToScan#test_records_extension_even_for_unsupported().
  TestAddFileToScan.test_java_extension_mapped: TestAddFileToScan#test_java_extension_mapped().
  TestAddFileToScan.test_header_mapped_to_c: TestAddFileToScan#test_header_mapped_to_c().
  TestAddFileToScan.test_yaml_extensions_mapped: TestAddFileToScan#test_yaml_extensions_mapped().
  TestValidateArguments.test_validate_default_max_depth: TestValidateArguments#test_validate_default_max_depth().
  TestValidateArguments.test_validate_valid_max_depth: TestValidateArguments#test_validate_valid_max_depth().
  TestValidateArguments.test_validate_max_depth_zero_raises: TestValidateArguments#test_validate_max_depth_zero_raises().
  TestValidateArguments.test_validate_max_depth_too_large_raises: TestValidateArguments#test_validate_max_depth_too_large_raises().
  TestValidateArguments.test_validate_max_depth_string_raises: TestValidateArguments#test_validate_max_depth_string_raises().
  TestToolDefinition.test_get_tool_definition: TestToolDefinition#test_get_tool_definition().
  TestToolDefinition.test_get_tool_schema: TestToolDefinition#test_get_tool_schema().
  TestScanProject.test_scan_excludes_node_modules: TestScanProject#test_scan_excludes_node_modules().
  TestScanProject.test_scan_excludes_git: TestScanProject#test_scan_excludes_git().
  TestScanProject.test_scan_excludes_pytest_cache: TestScanProject#test_scan_excludes_pytest_cache().
  TestScanProject.test_scan_respects_max_depth: TestScanProject#test_scan_respects_max_depth().
  TestScanProject.test_scan_sorts_source_files_by_lines: TestScanProject#test_scan_sorts_source_files_by_lines().
  TestScanProject.test_scan_records_directory_tree: TestScanProject#test_scan_records_directory_tree().
  TestScanProject.test_scan_extension_distribution: TestScanProject#test_scan_extension_distribution().
  TestScanProject.test_scan_respects_gitignore: TestScanProject#test_scan_respects_gitignore().
  TestScanProject.test_scan_without_gitignore: TestScanProject#test_scan_without_gitignore().
  TestScanProject.test_scan_respects_multiple_gitignore_patterns: TestScanProject#test_scan_respects_multiple_gitignore_patterns().
  TestAddPathToScan.test_skips_excluded_dirs: TestAddPathToScan#test_skips_excluded_dirs().
  TestAddPathToScan.test_skips_deep_paths: TestAddPathToScan#test_skips_deep_paths().
  TestAddPathToScan.test_increments_dir_tree_for_directories: TestAddPathToScan#test_increments_dir_tree_for_directories().
  TestAddFileToScan.test_handles_binary_file_gracefully: TestAddFileToScan#test_handles_binary_file_gracefully().
  TestBuildResult.test_without_health: TestBuildResult#test_without_health().
  TestBuildResult.test_with_health_includes_smart_hint: TestBuildResult#test_with_health_includes_smart_hint().
  TestCountLines.test_counts_correctly: TestCountLines#test_counts_correctly().
  TestCountLines.test_empty_file: TestCountLines#test_empty_file().
  test_load_gitignore_unreadable_returns_none: test_load_gitignore_unreadable_returns_none().
  TestGitignoreSupport.test_load_gitignore_patterns_missing: TestGitignoreSupport#test_load_gitignore_patterns_missing().
  TestGitignoreSupport.test_is_ignored_by_gitignore_none_spec: TestGitignoreSupport#test_is_ignored_by_gitignore_none_spec().
  TestIncrement.test_new_key: TestIncrement#test_new_key().
  TestIncrement.test_existing_key: TestIncrement#test_existing_key().
  TestBuildBaseResult.test_languages_sorted_by_count: TestBuildBaseResult#test_languages_sorted_by_count().
  TestBuildBaseResult.test_largest_source_files_capped_at_15: TestBuildBaseResult#test_largest_source_files_capped_at_15().
  TestBuildHealthAlert.test_builds_alert: TestBuildHealthAlert#test_builds_alert().
  TestBuildHealthAlert.test_caps_at_5_files: TestBuildHealthAlert#test_caps_at_5_files().
  TestHealthOptInHint.test_hint_text: TestHealthOptInHint#test_hint_text().
  TestOverviewRisk.test_high_when_health_alert: TestOverviewRisk#test_high_when_health_alert().
  TestOverviewRisk.test_fallback_when_no_signals: TestOverviewRisk#test_fallback_when_no_signals().
  TestOverviewRisk.test_low_when_health_ok: TestOverviewRisk#test_low_when_health_ok().
  TestOverviewNextStep.test_with_health_alert: TestOverviewNextStep#test_with_health_alert().
  TestOverviewNextStep.test_without_health: TestOverviewNextStep#test_without_health().
  TestOverviewNextStep.test_healthy_project: TestOverviewNextStep#test_healthy_project().
  TestTopLanguage.test_empty: TestTopLanguage#test_empty().
  TestTopLanguage.test_returns_max: TestTopLanguage#test_returns_max().
  TestBuildToolRouting.test_contains_all_expected_tools: TestBuildToolRouting#test_contains_all_expected_tools().
  TestCountLines.test_nonexistent_returns_zero: TestCountLines#test_nonexistent_returns_zero().
  TestSuggestRefactorAction.test_large_prod_file: TestSuggestRefactorAction#test_large_prod_file().
  TestSuggestRefactorAction.test_test_file: TestSuggestRefactorAction#test_test_file().
  TestSuggestRefactorAction.test_markdown_file: TestSuggestRefactorAction#test_markdown_file().
  TestSuggestRefactorAction.test_small_prod_file: TestSuggestRefactorAction#test_small_prod_file().
  TestBuildSmartHint.test_all_healthy_hint: TestBuildSmartHint#test_all_healthy_hint().
  TestBuildSmartHint.test_unhealthy_hint: TestBuildSmartHint#test_unhealthy_hint().
  TestBuildSmartHint.test_empty_project: TestBuildSmartHint#test_empty_project().
  TestBuildSmartHint.test_language_to_extension_mapping: TestBuildSmartHint#test_language_to_extension_mapping().
  TestBuildSmartHint.test_language_to_extension_mapping_java: TestBuildSmartHint#test_language_to_extension_mapping_java().
  TestBuildAgentSummary.test_summary_fields: TestBuildAgentSummary#test_summary_fields().
  TestBuildAgentSummary.test_health_checked_flag: TestBuildAgentSummary#test_health_checked_flag().
  test_load_gitignore_only_comments_returns_none: test_load_gitignore_only_comments_returns_none().
  test_load_gitignore_unreadable_returns_none.boom: test_load_gitignore_unreadable_returns_none().boom().
  TestProjectOverviewExecute: TestProjectOverviewExecute#
  TestValidateArguments: TestValidateArguments#
  TestToolDefinition: TestToolDefinition#
  TestScanProject: TestScanProject#
  TestGitignoreSupport: TestGitignoreSupport#
  TestAddPathToScan: TestAddPathToScan#
  TestAddFileToScan: TestAddFileToScan#
  TestIncrement: TestIncrement#
  TestBuildResult: TestBuildResult#
  TestBuildBaseResult: TestBuildBaseResult#
  TestBuildHealthAlert: TestBuildHealthAlert#
  TestHealthOptInHint: TestHealthOptInHint#
  TestOverviewRisk: TestOverviewRisk#
  TestOverviewNextStep: TestOverviewNextStep#
  TestTopLanguage: TestTopLanguage#
  TestBuildToolRouting: TestBuildToolRouting#
  TestCountLines: TestCountLines#
  TestSuggestRefactorAction: TestSuggestRefactorAction#
  TestBuildSmartHint: TestBuildSmartHint#
  TestBuildAgentSummary: TestBuildAgentSummary#
  TestEdgeCases: TestEdgeCases#
---
# Module: [`tests/unit/mcp/test_project_overview_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py)

## Classes
### `TestAddFileToScan`
- def: [`tests/unit/mcp/test_project_overview_tool.py:325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L325)
- signature: `class TestAddFileToScan:`
- members:
  - `test_adds_source_file(self, tmp_path)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L326)
  - `test_handles_binary_file_gracefully(self, tmp_path)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L357)
  - `test_header_mapped_to_c(self, tmp_path)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L374)
  - `test_java_extension_mapped(self, tmp_path)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L366)
  - `test_records_extension_even_for_unsupported(self, tmp_path)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L349)
  - `test_skips_unsupported_extension(self, tmp_path)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L340)
  - `test_yaml_extensions_mapped(self, tmp_path)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L382)
- uses (calls/refs, reference-scoped): [`_add_file_to_scan`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_add_file_to_scan), [`_new_scan`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_new_scan)  (1 test-only)

### `TestAddPathToScan`
- def: [`tests/unit/mcp/test_project_overview_tool.py:294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L294)
- signature: `class TestAddPathToScan:`
- members:
  - `test_increments_dir_tree_for_directories(self, tmp_path)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L315)
  - `test_skips_deep_paths(self, tmp_path)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L305)
  - `test_skips_excluded_dirs(self, tmp_path)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L295)
- uses (calls/refs, reference-scoped): [`_add_path_to_scan`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_add_path_to_scan), [`_new_scan`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_new_scan)

### `TestBuildAgentSummary`
- def: [`tests/unit/mcp/test_project_overview_tool.py:661`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L661)
- signature: `class TestBuildAgentSummary:`
- members:
  - `test_health_checked_flag(self)` — [`L677`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L677)
  - `test_summary_fields(self)` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L662)
- uses (calls/refs, reference-scoped): [`_build_agent_summary`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_agent_summary)

### `TestBuildBaseResult`
- def: [`tests/unit/mcp/test_project_overview_tool.py:443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L443)
- signature: `class TestBuildBaseResult:`
- members:
  - `test_languages_sorted_by_count(self, tmp_path)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L444)
  - `test_largest_source_files_capped_at_15(self, tmp_path)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L459)
- uses (calls/refs, reference-scoped): [`_build_base_result`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_base_result)

### `TestBuildHealthAlert`
- def: [`tests/unit/mcp/test_project_overview_tool.py:480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L480)
- signature: `class TestBuildHealthAlert:`
- members:
  - `test_builds_alert(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L481)
  - `test_caps_at_5_files(self)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L491)
- uses (calls/refs, reference-scoped): [`_build_health_alert`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_health_alert)

### `TestBuildResult`
- def: [`tests/unit/mcp/test_project_overview_tool.py:405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L405)
- signature: `class TestBuildResult:`
- members:
  - `test_with_health_includes_smart_hint(self, tmp_path)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L428)
  - `test_without_health(self, tmp_path)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L406)
- uses (calls/refs, reference-scoped): [`_build_result`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_result), [`_new_scan`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_new_scan)

### `TestBuildSmartHint`
- def: [`tests/unit/mcp/test_project_overview_tool.py:605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L605)
- signature: `class TestBuildSmartHint:`
- members:
  - `test_all_healthy_hint(self)` — [`L606`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L606)
  - `test_empty_project(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L626)
  - `test_language_to_extension_mapping(self)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L635)
  - `test_language_to_extension_mapping_java(self)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L648)
  - `test_unhealthy_hint(self)` — [`L615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L615)
- uses (calls/refs, reference-scoped): [`_build_smart_hint`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_smart_hint)

### `TestBuildToolRouting`
- def: [`tests/unit/mcp/test_project_overview_tool.py:545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L545)
- signature: `class TestBuildToolRouting:`
- members:
  - `test_contains_all_expected_tools(self)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L546)
- uses (calls/refs, reference-scoped): [`_build_tool_routing`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_tool_routing)

### `TestCountLines`
- def: [`tests/unit/mcp/test_project_overview_tool.py:561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L561)
- signature: `class TestCountLines:`
- members:
  - `test_counts_correctly(self, tmp_path)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L562)
  - `test_empty_file(self, tmp_path)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L566)
  - `test_nonexistent_returns_zero(self, tmp_path)` — [`L570`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L570)
- uses (calls/refs, reference-scoped): [`_count_lines`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_count_lines)  (1 test-only)

### `TestEdgeCases`
- def: [`tests/unit/mcp/test_project_overview_tool.py:687`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L687)
- signature: `class TestEdgeCases:`
- members:
  - `test_all_supported_extensions(self, tmp_path)` — [`L705`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L705)
  - `test_max_depth_1(self, tmp_path)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L688)
  - `test_unicode_filename(self, tmp_path)` — [`L697`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L697)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute)  (2 test-only)

### `TestGitignoreSupport`
- def: [`tests/unit/mcp/test_project_overview_tool.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L251)
- signature: `class TestGitignoreSupport:`
- members:
  - `test_is_ignored_by_gitignore_none_spec(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L279) — Test that None spec never ignores anything.
  - `test_is_ignored_by_gitignore_normalization(self, tmp_path)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L283) — Test path normalization with backslashes.
  - `test_load_gitignore_patterns_exists(self, tmp_path)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L252) — Test loading .gitignore when it exists.
  - `test_load_gitignore_patterns_missing(self, tmp_path)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L263) — Test loading .gitignore when it doesn't exist.
  - `test_load_gitignore_patterns_with_comments(self, tmp_path)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L269) — Test that comments and empty lines are skipped.
- uses (calls/refs, reference-scoped): [`_load_gitignore_patterns`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_load_gitignore_patterns), [`_is_ignored_by_gitignore`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_is_ignored_by_gitignore)  (1 test-only)

### `TestHealthOptInHint`
- def: [`tests/unit/mcp/test_project_overview_tool.py:497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L497)
- signature: `class TestHealthOptInHint:`
- members:
  - `test_hint_text(self)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L498)
- uses (calls/refs, reference-scoped): [`_health_opt_in_hint`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_health_opt_in_hint)

### `TestIncrement`
- def: [`tests/unit/mcp/test_project_overview_tool.py:393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L393)
- signature: `class TestIncrement:`
- members:
  - `test_existing_key(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L399)
  - `test_new_key(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L394)
- uses (calls/refs, reference-scoped): [`_increment`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_increment)

### `TestOverviewNextStep`
- def: [`tests/unit/mcp/test_project_overview_tool.py:517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L517)
- signature: `class TestOverviewNextStep:`
- members:
  - `test_healthy_project(self)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L526)
  - `test_with_health_alert(self)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L518)
  - `test_without_health(self)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L522)
- uses (calls/refs, reference-scoped): [`_overview_next_step`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_overview_next_step)

### `TestOverviewRisk`
- def: [`tests/unit/mcp/test_project_overview_tool.py:503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L503)
- signature: `class TestOverviewRisk:`
- members:
  - `test_fallback_when_no_signals(self)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L507)
  - `test_high_when_health_alert(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L504)
  - `test_low_when_health_ok(self)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L513)
- uses (calls/refs, reference-scoped): [`_overview_risk`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_overview_risk)

### `TestProjectOverviewExecute`
- def: [`tests/unit/mcp/test_project_overview_tool.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L44)
- signature: `class TestProjectOverviewExecute:`
- members:
  - `test_execute_basic_json(self, tmp_path)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L45)
  - `test_execute_empty_project(self, tmp_path)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L84)
  - `test_execute_invalid_root_raises(self, tmp_path)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L79)
  - `test_execute_multi_language_project(self, tmp_path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L94)
  - `test_execute_no_project_root_raises(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L74)
  - `test_execute_toon_format(self, tmp_path)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L62)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute)  (2 test-only)

### `TestScanProject`
- def: [`tests/unit/mcp/test_project_overview_tool.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L150)
- signature: `class TestScanProject:`
- members:
  - `test_scan_excludes_git(self, tmp_path)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L159)
  - `test_scan_excludes_node_modules(self, tmp_path)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L151)
  - `test_scan_excludes_pytest_cache(self, tmp_path)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L168)
  - `test_scan_extension_distribution(self, tmp_path)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L201)
  - `test_scan_records_directory_tree(self, tmp_path)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L193)
  - `test_scan_respects_gitignore(self, tmp_path)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L210) — Verify that overview respects .gitignore exclusions (#445).
  - `test_scan_respects_max_depth(self, tmp_path)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L176)
  - `test_scan_respects_multiple_gitignore_patterns(self, tmp_path)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L238) — Verify that multiple .gitignore patterns work correctly.
  - `test_scan_sorts_source_files_by_lines(self, tmp_path)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L184)
  - `test_scan_without_gitignore(self, tmp_path)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L228) — Verify that scanning works when no .gitignore exists.
- uses (calls/refs, reference-scoped): [`_scan_project`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_scan_project)  (1 test-only)

### `TestSuggestRefactorAction`
- def: [`tests/unit/mcp/test_project_overview_tool.py:574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L574)
- signature: `class TestSuggestRefactorAction:`
- members:
  - `test_large_prod_file(self)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L575)
  - `test_markdown_file(self)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L591)
  - `test_small_prod_file(self)` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L598)
  - `test_test_file(self)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L584)
- uses (calls/refs, reference-scoped): [`_suggest_refactor_action`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_suggest_refactor_action)

### `TestToolDefinition`
- def: [`tests/unit/mcp/test_project_overview_tool.py:135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L135)
- signature: `class TestToolDefinition:`
- members:
  - `test_get_tool_definition(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L136)
  - `test_get_tool_schema(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L143)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.get_tool_schema)

### `TestTopLanguage`
- def: [`tests/unit/mcp/test_project_overview_tool.py:537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L537)
- signature: `class TestTopLanguage:`
- members:
  - `test_empty(self)` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L538)
  - `test_returns_max(self)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L541)
- uses (calls/refs, reference-scoped): [`_top_language`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_top_language)

### `TestValidateArguments`
- def: [`tests/unit/mcp/test_project_overview_tool.py:110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L110)
- signature: `class TestValidateArguments:`
- members:
  - `test_validate_default_max_depth(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L111)
  - `test_validate_max_depth_string_raises(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L129)
  - `test_validate_max_depth_too_large_raises(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L124)
  - `test_validate_max_depth_zero_raises(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L119)
  - `test_validate_valid_max_depth(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L115)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.validate_arguments)

## Functions
- `_run(coro)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L33)
- `_write(tmp_path, rel, content, encoding="utf-8")` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L37)
- `boom(path, *a, **kw)` — [`L755`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L755)
- `test_load_gitignore_only_comments_returns_none(tmp_path)` — [`L734`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L734) — A .gitignore with only comments/blank lines compiles to None.
- `test_load_gitignore_unreadable_returns_none(tmp_path, monkeypatch)` — [`L744`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_overview_tool.py#L744) — A .gitignore that raises on read degrades gracefully to None.

