---
title: 'Module: tests/unit/mcp/test_change_impact_tool_git_and_verification.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_change_impact_tool_git_and_verification.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_change_impact_tool_git_and_verification`/
symbols:
  test_verification_strategy_recommends_focused_then_default_for_dirty_worktree: test_verification_strategy_recommends_focused_then_default_for_dirty_worktree().
  test_low_impact_profile_rewrites_focused_pytest_for_local_agents: test_low_impact_profile_rewrites_focused_pytest_for_local_agents().
  test_low_impact_profile_leaves_non_pytest_strategy_unchanged: test_low_impact_profile_leaves_non_pytest_strategy_unchanged().
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().
  test_build_test_plan_returns_sorted_runnable_tests: test_build_test_plan_returns_sorted_runnable_tests().
  test_diff_mode_includes_untracked_files: test_diff_mode_includes_untracked_files().
  test_diff_mode_deduplicates_untracked_paths: test_diff_mode_deduplicates_untracked_paths().
  test_diff_mode_accepts_scope_pathspecs: test_diff_mode_accepts_scope_pathspecs().
  test_staged_mode_keeps_staged_semantics: test_staged_mode_keeps_staged_semantics().
  test_diff_stat_mentions_untracked_files: test_diff_stat_mentions_untracked_files().
  test_code_change_with_runtime_fallback_uses_default_suite: test_code_change_with_runtime_fallback_uses_default_suite().
  test_verification_strategy_avoids_huge_focused_commands: test_verification_strategy_avoids_huge_focused_commands().
  test_non_pytest_default_verification_plan_uses_detected_runner: test_non_pytest_default_verification_plan_uses_detected_runner().
  test_change_impact_schema_accepts_resource_profile: test_change_impact_schema_accepts_resource_profile().
  test_low_impact_profile_caps_default_pytest_for_local_agents: test_low_impact_profile_caps_default_pytest_for_local_agents().
  test_low_impact_profile_leaves_docs_only_strategy_unchanged: test_low_impact_profile_leaves_docs_only_strategy_unchanged().
  test_build_pytest_command_quotes_paths: test_build_pytest_command_quotes_paths().
  test_build_pytest_command_falls_back_to_full_suite: test_build_pytest_command_falls_back_to_full_suite().
  test_docs_only_verification_plan_skips_pytest: test_docs_only_verification_plan_skips_pytest().
  test_requirements_txt_is_not_treated_as_docs_only: test_requirements_txt_is_not_treated_as_docs_only().
  test_code_change_verification_plan_uses_targeted_tests: test_code_change_verification_plan_uses_targeted_tests().
  test_code_change_verification_plan_falls_back_to_default_suite: test_code_change_verification_plan_falls_back_to_default_suite().
  test_mcp_default_resource_profile_is_local_low_impact: test_mcp_default_resource_profile_is_local_low_impact().
  test_low_impact_pytest_command_handles_pytest_binary_and_bad_shell_quote: test_low_impact_pytest_command_handles_pytest_binary_and_bad_shell_quote().
  test_low_impact_pytest_command_replaces_existing_worker_flags: test_low_impact_pytest_command_replaces_existing_worker_flags().
  test_build_file_impacts_without_graph_returns_fallback_rows: test_build_file_impacts_without_graph_returns_fallback_rows().
  test_no_changes_result_keeps_agent_scope_signal: test_no_changes_result_keeps_agent_scope_signal().
  test_agent_summary_only_response_omits_noisy_details: test_agent_summary_only_response_omits_noisy_details().
  test_build_test_plan_skips_when_disabled: test_build_test_plan_skips_when_disabled().
  test_cli_path_always_passes_resource_profile_explicitly: test_cli_path_always_passes_resource_profile_explicitly().
  test_low_impact_pytest_command_portable_on_windows: test_low_impact_pytest_command_portable_on_windows().
  test_diff_mode_includes_untracked_files.fake_run_git: test_diff_mode_includes_untracked_files().fake_run_git().
  test_diff_mode_deduplicates_untracked_paths.fake_run_git: test_diff_mode_deduplicates_untracked_paths().fake_run_git().
  test_diff_mode_accepts_scope_pathspecs.fake_run_git: test_diff_mode_accepts_scope_pathspecs().fake_run_git().
  test_staged_mode_keeps_staged_semantics.fake_run_git: test_staged_mode_keeps_staged_semantics().fake_run_git().
  test_diff_stat_mentions_untracked_files.fake_run_git: test_diff_stat_mentions_untracked_files().fake_run_git().
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents.FakeGraph: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().FakeGraph#
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents.FakeBlastRadius: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().FakeBlastRadius#
  test_build_test_plan_returns_sorted_runnable_tests.FakeGraph: test_build_test_plan_returns_sorted_runnable_tests().FakeGraph#
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents.FakeGraph.dependents_of: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().FakeGraph#dependents_of().
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents.FakeBlastRadius.__init__: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().FakeBlastRadius#__init__().
  FakeBlastRadius.graph: FakeBlastRadius#graph.
  test_build_file_impacts_with_graph_preserves_order_and_limits_dependents.FakeBlastRadius.forward: test_build_file_impacts_with_graph_preserves_order_and_limits_dependents().FakeBlastRadius#forward().
  test_build_test_plan_returns_sorted_runnable_tests.FakeGraph.nodes: test_build_test_plan_returns_sorted_runnable_tests().FakeGraph#nodes().
---
# Module: [`tests/unit/mcp/test_change_impact_tool_git_and_verification.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py)

## Classes
### `FakeBlastRadius`
- def: [`tests/unit/mcp/test_change_impact_tool_git_and_verification.py:594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L594)
- signature: `class FakeBlastRadius:`
- members:
  - `forward(self, file_path)` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L598)
  - `graph` — [`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L596)
- protocol/private: `__init__`[`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L595)
- used by: (1 test-only callers)

### `FakeGraph`
- def: [`tests/unit/mcp/test_change_impact_tool_git_and_verification.py:631`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L631)
- signature: `class FakeGraph:`
- members:
  - `dependents_of(self, file_path)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L591)
  - `nodes(self)` — [`L632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L632)
- used by: (1 test-only callers)

## Functions
- `fake_run_git(args, cwd=None)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L36)
- `fake_run_git(args, cwd=None)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L56)
- `fake_run_git(args, cwd=None)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L74)
- `fake_run_git(args, cwd=None)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L121)
- `fake_run_git(args, cwd=None)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L138)
- `test_agent_summary_only_response_omits_noisy_details()` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L520) — Agents can ask for only the compact decision surface.
- `test_build_file_impacts_with_graph_preserves_order_and_limits_dependents(monkeypatch)` — [`L585`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L585) — Graph-backed impact rows should be stable and bounded for agent output.
- `test_build_file_impacts_without_graph_returns_fallback_rows()` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L486) — Missing dependency graphs should still report each changed file.
- `test_build_pytest_command_falls_back_to_full_suite()` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L166) — No mapped tests should still produce a valid validation command.
- `test_build_pytest_command_quotes_paths()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L154) — Fast validation command should be directly runnable in a shell.
- `test_build_test_plan_returns_sorted_runnable_tests()` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L628) — Fallback auto-discovery markers should not become pytest targets.
- `test_build_test_plan_skips_when_disabled()` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L616) — Agents can request impact data without related test lookup.
- `test_change_impact_schema_accepts_resource_profile()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L14) — MCP callers need the same resource profile knob as the CLI.
- `test_cli_path_always_passes_resource_profile_explicitly()` — [`L654`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L654) — CLI builder must always set resource_profile so the MCP fallback never overrides it (#925 P2).
- `test_code_change_verification_plan_falls_back_to_default_suite()` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L447) — Code edits without mapped tests should keep the default-suite contract.
- `test_code_change_verification_plan_uses_targeted_tests()` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L198) — Code edits should recommend the narrow mapped pytest command.
- `test_code_change_with_runtime_fallback_uses_default_suite()` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L217) — Unmapped runtime files should not be hidden by other targeted tests.
- `test_diff_mode_accepts_scope_pathspecs(monkeypatch)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L70) — Agents can narrow noisy dirty worktrees to the current queue scope.
- `test_diff_mode_deduplicates_untracked_paths(monkeypatch)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L53) — Duplicate git output should not duplicate changed_files entries.
- `test_diff_mode_includes_untracked_files(monkeypatch)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L33) — Default diff mode should include untracked files in changed_files.
- `test_diff_stat_mentions_untracked_files(monkeypatch)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L135) — Diff stat should make untracked files visible to agents.
- `test_docs_only_verification_plan_skips_pytest()` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L171) — Docs-only edits should not send agents into the full test suite.
- `test_low_impact_profile_caps_default_pytest_for_local_agents(monkeypatch)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L320) — Unmapped runtime diffs still avoid xdist=auto on the local machine.
- `test_low_impact_profile_leaves_docs_only_strategy_unchanged()` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L347) — Docs-only changes should still avoid pytest entirely.
- `test_low_impact_profile_leaves_non_pytest_strategy_unchanged()` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L366) — Resource profile is pytest-specific and should not rewrite other runners.
- `test_low_impact_profile_rewrites_focused_pytest_for_local_agents(monkeypatch)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L279) — Local agents should get a nice/xdist-capped command without losing CI intent.
- `test_low_impact_pytest_command_handles_pytest_binary_and_bad_shell_quote(monkeypatch)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L389) — Command rewriting should be conservative for malformed shell strings.
- `test_low_impact_pytest_command_portable_on_windows(monkeypatch)` — [`L679`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L679) — #925 P2: _low_impact_pytest_command must not emit 'nice' on Windows.
- `test_low_impact_pytest_command_replaces_existing_worker_flags(monkeypatch)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L410) — Existing xdist settings should not survive the local-low-impact rewrite.
- `test_mcp_default_resource_profile_is_local_low_impact()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L24) — #731: MCP entrypoint defaults to local_low_impact without explicit arg.
- `test_no_changes_result_keeps_agent_scope_signal()` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L497) — Empty scoped diffs should still return a useful compact summary.
- `test_non_pytest_default_verification_plan_uses_detected_runner()` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L466) — Arbitrary-language projects should follow their own default test runner.
- `test_requirements_txt_is_not_treated_as_docs_only()` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L190) — Dependency manifests can affect execution even when they are .txt files.
- `test_staged_mode_keeps_staged_semantics(monkeypatch)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L117) — Staged mode should only report staged files.
- `test_verification_strategy_avoids_huge_focused_commands()` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L425) — Very broad diffs should not produce copy-paste hostile focused commands.
- `test_verification_strategy_recommends_focused_then_default_for_dirty_worktree()` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_change_impact_tool_git_and_verification.py#L244) — Agents should get an iteration command plus a queue-boundary command.

