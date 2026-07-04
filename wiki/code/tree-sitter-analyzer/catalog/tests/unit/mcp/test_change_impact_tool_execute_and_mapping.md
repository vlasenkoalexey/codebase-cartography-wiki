---
title: 'Module: tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_change_impact_tool_execute_and_mapping`/
symbols:
  test_agent_summary_warns_for_unscoped_large_dirty_worktree: test_agent_summary_warns_for_unscoped_large_dirty_worktree().
  test_change_impact_result_uses_complete_mapped_tests_for_verification: test_change_impact_result_uses_complete_mapped_tests_for_verification().
  test_execute_forwards_scope_paths_to_git_readers: test_execute_forwards_scope_paths_to_git_readers().
  test_execute_strict_scope_mode_mutes_out_of_scope: test_execute_strict_scope_mode_mutes_out_of_scope().
  test_execute_strict_scope_mode_does_not_leak_into_toon: test_execute_strict_scope_mode_does_not_leak_into_toon().
  test_execute_default_scope_mode_lists_out_of_scope: test_execute_default_scope_mode_lists_out_of_scope().
  test_execute_exposes_verification_fields_for_agents: test_execute_exposes_verification_fields_for_agents().
  test_execute_adds_queue_ledger_for_scoped_dirty_worktree: test_execute_adds_queue_ledger_for_scoped_dirty_worktree().
  test_execute_test_only_diff_skips_expensive_analysis: test_execute_test_only_diff_skips_expensive_analysis().
  test_execute_supports_agent_summary_only: test_execute_supports_agent_summary_only().
  test_find_test_files_marks_docs_as_diff_check_only: test_find_test_files_marks_docs_as_diff_check_only().
  test_validate_arguments_rejects_invalid_mode: test_validate_arguments_rejects_invalid_mode().
  test_validate_arguments_accepts_valid_modes: test_validate_arguments_accepts_valid_modes().
  test_validate_arguments_accepts_missing_mode: test_validate_arguments_accepts_missing_mode().
  test_execute_no_changes_returns_no_changes_result: test_execute_no_changes_returns_no_changes_result().
  test_execute_no_changes_with_scope_paths: test_execute_no_changes_with_scope_paths().
  test_execute_no_changes_with_agent_summary_only: test_execute_no_changes_with_agent_summary_only().
  test_execute_no_changes_with_scope_and_agent_summary: test_execute_no_changes_with_scope_and_agent_summary().
  test_validate_arguments_rejects_bad_resource_profile: test_validate_arguments_rejects_bad_resource_profile().
  test_validate_arguments_rejects_bad_scope_mode: test_validate_arguments_rejects_bad_scope_mode().
  test_find_test_files_maps_fixture_files_to_related_tests: test_find_test_files_maps_fixture_files_to_related_tests().
  test_find_test_files_excludes_conftest_from_runnable_targets: test_find_test_files_excludes_conftest_from_runnable_targets().
  test_find_test_files_does_not_treat_source_test_prefix_as_test: test_find_test_files_does_not_treat_source_test_prefix_as_test().
  test_find_test_files_maps_python_plugin_internals_to_package_tests: test_find_test_files_maps_python_plugin_internals_to_package_tests().
  test_find_test_files_maps_extracted_analysis_modules_to_family_tests: test_find_test_files_maps_extracted_analysis_modules_to_family_tests().
  test_find_test_files_maps_refactoring_plan_builder_to_family_tests: test_find_test_files_maps_refactoring_plan_builder_to_family_tests().
  test_find_test_files_maps_extracted_search_content_modules_to_family_tests: test_find_test_files_maps_extracted_search_content_modules_to_family_tests().
  test_find_test_files_maps_find_and_grep_execution_to_family_tests: test_find_test_files_maps_find_and_grep_execution_to_family_tests().
  test_execute_test_only_diff_skips_expensive_analysis.fail_expensive_path: test_execute_test_only_diff_skips_expensive_analysis().fail_expensive_path().
  test_doc_drift_hints_absent_for_unrelated_files: test_doc_drift_hints_absent_for_unrelated_files().
  test_doc_drift_hints_cli_main_triggers_readme_count_check: test_doc_drift_hints_cli_main_triggers_readme_count_check().
  test_doc_drift_hints_tool_registry_triggers_readme_count_check: test_doc_drift_hints_tool_registry_triggers_readme_count_check().
  test_doc_drift_hints_facade_tool_triggers_doc_regen: test_doc_drift_hints_facade_tool_triggers_doc_regen().
  test_doc_drift_hints_util_file_not_treated_as_facade_tool: test_doc_drift_hints_util_file_not_treated_as_facade_tool().
  test_doc_drift_hints_argument_groups_file_triggers_readme_count_check: test_doc_drift_hints_argument_groups_file_triggers_readme_count_check().
  test_doc_drift_hints_facade_map_triggers_facade_doc_regen: test_doc_drift_hints_facade_map_triggers_facade_doc_regen().
  test_doc_drift_hints_tool_registry_triggers_both_checks: test_doc_drift_hints_tool_registry_triggers_both_checks().
  test_doc_drift_hints_appends_to_verification_steps: test_doc_drift_hints_appends_to_verification_steps().
  test_execute_exposes_verification_fields_for_agents.fail_graph: test_execute_exposes_verification_fields_for_agents().fail_graph().
  test_execute_forwards_scope_paths_to_git_readers.fake_changed_files: test_execute_forwards_scope_paths_to_git_readers().fake_changed_files().
  test_execute_forwards_scope_paths_to_git_readers.fake_diff_stat: test_execute_forwards_scope_paths_to_git_readers().fake_diff_stat().
  test_execute_adds_queue_ledger_for_scoped_dirty_worktree.fake_changed_files: test_execute_adds_queue_ledger_for_scoped_dirty_worktree().fake_changed_files().
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeGraph: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeGraph#
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeBlastRadius: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeBlastRadius#
  test_execute_strict_scope_mode_mutes_out_of_scope.fake_changed: test_execute_strict_scope_mode_mutes_out_of_scope().fake_changed().
  test_execute_strict_scope_mode_mutes_out_of_scope.fail_graph: test_execute_strict_scope_mode_mutes_out_of_scope().fail_graph().
  test_execute_strict_scope_mode_does_not_leak_into_toon.fake_changed: test_execute_strict_scope_mode_does_not_leak_into_toon().fake_changed().
  test_execute_strict_scope_mode_does_not_leak_into_toon.fail_graph: test_execute_strict_scope_mode_does_not_leak_into_toon().fail_graph().
  test_execute_default_scope_mode_lists_out_of_scope.fake_changed: test_execute_default_scope_mode_lists_out_of_scope().fake_changed().
  test_execute_default_scope_mode_lists_out_of_scope.fail_graph: test_execute_default_scope_mode_lists_out_of_scope().fail_graph().
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeGraph.nodes: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeGraph#nodes().
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeGraph.dependents_of: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeGraph#dependents_of().
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeBlastRadius.__init__: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeBlastRadius#__init__().
  FakeBlastRadius.graph: FakeBlastRadius#graph.
  test_change_impact_result_uses_complete_mapped_tests_for_verification.FakeBlastRadius.forward: test_change_impact_result_uses_complete_mapped_tests_for_verification().FakeBlastRadius#forward().
---
# Module: [`tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py)

## Classes
### `FakeBlastRadius`
- def: [`tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L268)
- signature: `class FakeBlastRadius:`
- members:
  - `forward(self, file_path)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L272)
  - `graph` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L270)
- protocol/private: `__init__`[`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L269)
- used by: (1 test-only callers)

### `FakeGraph`
- def: [`tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py:258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L258)
- signature: `class FakeGraph:`
- members:
  - `dependents_of(self, file_path)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L265)
  - `nodes(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L259)
- used by: (1 test-only callers)

## Functions
- `fail_expensive_path(*args, **kwargs)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L213)
- `fail_graph(project_root)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L27)
- `fail_graph(project_root)` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L662)
- `fail_graph(project_root)` — [`L705`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L705)
- `fail_graph(project_root)` — [`L748`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L748)
- `fake_changed(mode, project_root, scope_paths=None)` — [`L646`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L646)
- `fake_changed(mode, project_root, scope_paths=None)` — [`L692`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L692)
- `fake_changed(mode, project_root, scope_paths=None)` — [`L735`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L735)
- `fake_changed_files(mode, project_root, scope_paths=None)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L79)
- `fake_changed_files(mode, project_root, scope_paths=None)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L119)
- `fake_diff_stat(mode, project_root, scope_paths=None)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L83)
- `test_agent_summary_warns_for_unscoped_large_dirty_worktree()` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L303) — The compact summary should tell agents to scope very noisy diffs.
- `test_change_impact_result_uses_complete_mapped_tests_for_verification(monkeypatch)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L255) — Display limits must not silently drop tests from the runnable command.
- `test_doc_drift_hints_absent_for_unrelated_files()` — [`L776`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L776) — No doc_drift_checks when changed files don't touch CLI or MCP tools.
- `test_doc_drift_hints_appends_to_verification_steps()` — [`L885`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L885) — doc-drift checks must appear in verification_steps, not just doc_drift_checks (P2 #924).
- `test_doc_drift_hints_argument_groups_file_triggers_readme_count_check()` — [`L840`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L840) — Adding a flag in cli/argument_groups/*.py must trigger README-count check (P2 #924).
- `test_doc_drift_hints_cli_main_triggers_readme_count_check()` — [`L786`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L786) — Changing cli_main.py must append the README-count test to doc_drift_checks.
- `test_doc_drift_hints_facade_map_triggers_facade_doc_regen()` — [`L856`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L856) — Changing facade_map.py must trigger facade-actions.md regen (P2 #924).
- `test_doc_drift_hints_facade_tool_triggers_doc_regen()` — [`L813`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L813) — Changing a facade tool must append the facade-actions.md regen step.
- `test_doc_drift_hints_tool_registry_triggers_both_checks()` — [`L869`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L869) — _tool_registry.py drives both README counts and facade-actions.md (P2 #924).
- `test_doc_drift_hints_tool_registry_triggers_readme_count_check()` — [`L800`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L800) — Changing _tool_registry.py must also append the README-count test.
- `test_doc_drift_hints_util_file_not_treated_as_facade_tool()` — [`L828`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L828) — Files under mcp/tools/utils/ must NOT trigger facade-actions regen.
- `test_execute_adds_queue_ledger_for_scoped_dirty_worktree(monkeypatch)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L116) — Scoped change-impact should report dirty files outside the queue.
- `test_execute_default_scope_mode_lists_out_of_scope(monkeypatch)` — [`L731`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L731) — Default scope_mode=report keeps today's behavior: out-of-scope dirty
- `test_execute_exposes_verification_fields_for_agents(monkeypatch)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L14) — The MCP tool output must include the command agents should run next.
- `test_execute_forwards_scope_paths_to_git_readers(monkeypatch)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L75) — MCP callers should get queue-scoped impact without post-filtering noise.
- `test_execute_no_changes_returns_no_changes_result(monkeypatch)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L554) — execute should return no-changes result when nothing is dirty.
- `test_execute_no_changes_with_agent_summary_only(monkeypatch)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L597) — No-changes agent-summary-only should omit full details.
- `test_execute_no_changes_with_scope_and_agent_summary(monkeypatch)` — [`L617`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L617) — Combined scope + agent-summary-only on empty diff should work.
- `test_execute_no_changes_with_scope_paths(monkeypatch)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L573) — No-changes result should reflect scope filtering when scope_paths given.
- `test_execute_strict_scope_mode_does_not_leak_into_toon(monkeypatch)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L688) — #8: under TOON output, strict mode must NOT serialize an out-of-scope
- `test_execute_strict_scope_mode_mutes_out_of_scope(monkeypatch)` — [`L642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L642) — #8: scope_mode=strict threads through execute and mutes the out-of-scope
- `test_execute_supports_agent_summary_only(monkeypatch)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L161) — MCP callers can avoid the large changed/affected/test mapping payload.
- `test_execute_test_only_diff_skips_expensive_analysis(monkeypatch)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L200) — Changed test files are exact targets; no graph/cache walk is needed.
- `test_find_test_files_does_not_treat_source_test_prefix_as_test()` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L382) — Source modules named test_*.py are not direct pytest targets.
- `test_find_test_files_excludes_conftest_from_runnable_targets()` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L372) — conftest.py can affect tests, but should not appear as a pytest target.
- `test_find_test_files_maps_extracted_analysis_modules_to_family_tests()` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L415) — Extracted analysis modules should map to their parent tool tests.
- `test_find_test_files_maps_extracted_search_content_modules_to_family_tests()` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L459) — Search content helper modules should stay on targeted search tests.
- `test_find_test_files_maps_find_and_grep_execution_to_family_tests()` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L494) — Execution helper modules should stay on targeted find_and_grep tests.
- `test_find_test_files_maps_fixture_files_to_related_tests()` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L356) — Fixture edits should run tests that name the fixture domain.
- `test_find_test_files_maps_python_plugin_internals_to_package_tests()` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L397) — Language plugin internals should map to package-level test files.
- `test_find_test_files_maps_refactoring_plan_builder_to_family_tests()` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L443) — The precise-plan builder should not force auto-discovery.
- `test_find_test_files_marks_docs_as_diff_check_only()` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L343) — Docs changes should not appear as pytest auto-discovery work.
- `test_validate_arguments_accepts_missing_mode()` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L536) — validate_arguments must pass when mode key is absent.
- `test_validate_arguments_accepts_valid_modes()` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L529) — validate_arguments must accept diff, staged, and branch.
- `test_validate_arguments_rejects_bad_resource_profile()` — [`L542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L542) — Invalid resource_profile values should fail at the tool boundary.
- `test_validate_arguments_rejects_bad_scope_mode()` — [`L764`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L764) — #8: invalid scope_mode is rejected with an actionable message.
- `test_validate_arguments_rejects_invalid_mode()` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_execute_and_mapping.py#L517) — validate_arguments must raise ValueError for unknown modes.

