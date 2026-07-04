---
title: 'Module: tests/unit/mcp/tools/test_co_change.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_co_change.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_co_change`/
symbols:
  _sha: _sha().
  _make_git_log: _make_git_log().
  test_cli_co_change_execution_dispatches: test_cli_co_change_execution_dispatches().
  test_cli_test_map_execution_dispatches: test_cli_test_map_execution_dispatches().
  test_cli_co_change_execution_handles_exception: test_cli_co_change_execution_handles_exception().
  test_cli_co_change_json_output_format: test_cli_co_change_json_output_format().
  test_cli_co_change_returns_error_code_on_failure: test_cli_co_change_returns_error_code_on_failure().
  test_cli_test_map_with_file_path: test_cli_test_map_with_file_path().
  test_cli_co_change_toon_output_format: test_cli_co_change_toon_output_format().
  test_handle_nav_actions_returns_none_when_no_flags: test_handle_nav_actions_returns_none_when_no_flags().
  test_cli_co_change_routes_symbol_vs_path.make_ctx: test_cli_co_change_routes_symbol_vs_path().make_ctx().
  test_nav_facade_co_change_action_dispatches: test_nav_facade_co_change_action_dispatches().
  test_nav_facade_co_change_output_format_toon: test_nav_facade_co_change_output_format_toon().
  test_nav_facade_co_change_default_output_format_is_toon: test_nav_facade_co_change_default_output_format_is_toon().
  test_nav_facade_co_change_resolves_symbol_to_file_via_call_graph: test_nav_facade_co_change_resolves_symbol_to_file_via_call_graph().
  test_nav_facade_co_change_symbol_fallback_when_resolution_fails: test_nav_facade_co_change_symbol_fallback_when_resolution_fails().
  test_nav_facade_co_change_carries_candidates_below_threshold: test_nav_facade_co_change_carries_candidates_below_threshold().
  test_basic_coupling_exact_lift: test_basic_coupling_exact_lift().
  test_different_peers_get_different_lifts: test_different_peers_get_different_lifts().
  test_cache_hit_skips_subprocess: test_cache_hit_skips_subprocess().
  test_cache_key_includes_result_shaping_parameters: test_cache_key_includes_result_shaping_parameters().
  test_git_log_walks_from_head_explicitly: test_git_log_walks_from_head_explicitly().
  test_min_shared_filter_excludes_rare_peers: test_min_shared_filter_excludes_rare_peers().
  test_test_files_excluded_from_peers: test_test_files_excluded_from_peers().
  test_no_target_commits_returns_empty: test_no_target_commits_returns_empty().
  test_max_results_truncation: test_max_results_truncation().
  test_single_subprocess_structural_invariant: test_single_subprocess_structural_invariant().
  test_result_includes_agent_summary: test_result_includes_agent_summary().
  test_window_string_format: test_window_string_format().
  test_sorted_by_lift_descending: test_sorted_by_lift_descending().
  test_lift_uses_actual_commit_count_not_max_commits: test_lift_uses_actual_commit_count_not_max_commits().
  test_small_sample_guard_insufficient_history_next_step: test_small_sample_guard_insufficient_history_next_step().
  test_small_sample_guard_adequate_sample_may_say_safe: test_small_sample_guard_adequate_sample_may_say_safe().
  test_candidates_below_threshold_exact_count: test_candidates_below_threshold_exact_count().
  test_candidates_below_threshold_zero_when_no_peers_at_all: test_candidates_below_threshold_zero_when_no_peers_at_all().
  test_candidates_below_threshold_mixed_above_and_below: test_candidates_below_threshold_mixed_above_and_below().
  test_adequate_sample_filtered_candidates_next_step_says_filtered: test_adequate_sample_filtered_candidates_next_step_says_filtered().
  test_coupled_peers_small_sample_carries_caveat: test_coupled_peers_small_sample_carries_caveat().
  test_co_change_action_in_bespoke_map: test_co_change_action_in_bespoke_map().
  test_lru_cache_evicts_at_maxsize: test_lru_cache_evicts_at_maxsize().
  test_real_repo_co_change_under_2s: test_real_repo_co_change_under_2s().
  test_cli_co_change_routes_symbol_vs_path: test_cli_co_change_routes_symbol_vs_path().
  test_real_repo_co_change_under_2s._git: test_real_repo_co_change_under_2s()._git().
  test_no_git_repo_returns_empty: test_no_git_repo_returns_empty().
  test_git_log_failure_after_head_returns_empty: test_git_log_failure_after_head_returns_empty().
  test_nav_facade_co_change_requires_symbol_or_file_path: test_nav_facade_co_change_requires_symbol_or_file_path().
  test_nav_facade_schema_action_enum_includes_co_change: test_nav_facade_schema_action_enum_includes_co_change().
  test_nav_co_change_in_new_action_parity: test_nav_co_change_in_new_action_parity().
  test_cli_co_change_flag_exists: test_cli_co_change_flag_exists().
  test_nav_description_mentions_co_change: test_nav_description_mentions_co_change().
  test_server_instructions_mention_co_change: test_server_instructions_mention_co_change().
  test_cli_co_change_execution_dispatches._output_json: test_cli_co_change_execution_dispatches()._output_json().
  test_cli_test_map_execution_dispatches._output_json: test_cli_test_map_execution_dispatches()._output_json().
  test_cli_co_change_execution_handles_exception._capture_error: test_cli_co_change_execution_handles_exception()._capture_error().
  test_cli_co_change_json_output_format._capture_json: test_cli_co_change_json_output_format()._capture_json().
  test_cli_co_change_returns_error_code_on_failure._capture_json: test_cli_co_change_returns_error_code_on_failure()._capture_json().
  test_cli_test_map_with_file_path._capture_json: test_cli_test_map_with_file_path()._capture_json().
---
# Module: [`tests/unit/mcp/tools/test_co_change.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py)

## Functions
- `_capture_error(msg: str)` — [`L1108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1108)
- `_capture_json(data: dict)` — [`L1157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1157)
- `_capture_json(data: dict)` — [`L1266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1266)
- `_capture_json(data: dict)` — [`L1319`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1319)
- `_git(*args: str)` — [`L833`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L833)
- `_make_git_log(commits: list[tuple[str, list[str]]])` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L33) — Build fake ``git log --pretty=format:%H --name-only`` output.
- `_output_json(data: dict)` — [`L899`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L899)
- `_output_json(data: dict)` — [`L963`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L963)
- `_sha(n: int)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L46) — Return a deterministic 40-hex SHA for test n.
- `make_ctx()` — [`L1713`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1713)
- `test_adequate_sample_filtered_candidates_next_step_says_filtered()` — [`L1585`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1585) — Adequate n=20, co_changed_files=[], candidates_below_threshold=3 ->
- `test_basic_coupling_exact_lift()` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L56) — Peer sharing 5 of 10 target commits, peer_commits=5 ->
- `test_cache_hit_skips_subprocess()` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L203) — Second call with same (project, file, HEAD) hits cache.
- `test_cache_key_includes_result_shaping_parameters()` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L234) — Changing max_commits/min_shared/max_results must trigger a fresh log walk.
- `test_candidates_below_threshold_exact_count()` — [`L1474`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1474) — Adequate sample (n=20) but peers below min_shared=3 -> candidates_below_threshold.
- `test_candidates_below_threshold_mixed_above_and_below()` — [`L1540`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1540) — peer_a cleared threshold (shared=5), peer_b filtered (shared=2).
- `test_candidates_below_threshold_zero_when_no_peers_at_all()` — [`L1517`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1517) — No peers at all -> candidates_below_threshold must be exactly 0.
- `test_cli_co_change_execution_dispatches(tmp_path: Path)` — [`L882`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L882) — --co-change FILE_OR_SYMBOL must route through handle_nav_actions and
- `test_cli_co_change_execution_handles_exception()` — [`L1096`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1096) — --co-change must handle exceptions gracefully and return error code 1.
- `test_cli_co_change_flag_exists()` — [`L600`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L600) — --co-change must be registered in the argument parser.
- `test_cli_co_change_json_output_format()` — [`L1145`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1145) — --co-change with output_format=json must call output_json (not print toon).
- `test_cli_co_change_returns_error_code_on_failure()` — [`L1254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1254) — --co-change with success=False in result must return error code 1.
- `test_cli_co_change_routes_symbol_vs_path()` — [`L1701`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1701) — Path-looking values -> file_path; bare names -> symbol.
- `test_cli_co_change_toon_output_format()` — [`L1204`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1204) — --co-change with output_format=toon must extract and print toon_content.
- `test_cli_test_map_execution_dispatches(tmp_path: Path)` — [`L947`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L947) — --test-map SYMBOL must route through handle_nav_actions and return a
- `test_cli_test_map_with_file_path()` — [`L1307`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1307) — --test-map --test-map-file should pass file_path to facade.
- `test_co_change_action_in_bespoke_map()` — [`L638`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L638) — co_change must be registered as a bespoke route (NOT action_map).
- `test_coupled_peers_small_sample_carries_caveat()` — [`L1672`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1672) — n=3 with a peer meeting min_shared=3 must lead with the caution.
- `test_different_peers_get_different_lifts()` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L86) — RFC two-peer differential proof:
- `test_git_log_failure_after_head_returns_empty()` — [`L176`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L176) — HEAD rev-parse succeeds but git log fails -> graceful empty result.
- `test_git_log_walks_from_head_explicitly()` — [`L275`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L275) — Detached worktrees must walk history reachable from HEAD, not a branch ref.
- `test_handle_nav_actions_returns_none_when_no_flags()` — [`L1366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1366) — handle_nav_actions returns None when neither --test-map nor --co-change set.
- `test_lift_uses_actual_commit_count_not_max_commits()` — [`L724`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L724) — lift denominator = actual parsed commits, NOT max_commits.
- `test_lru_cache_evicts_at_maxsize()` — [`L770`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L770) — Cache must not grow beyond _CO_CHANGE_CACHE_MAXSIZE entries.
- `test_max_results_truncation()` — [`L386`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L386) — When more peers than max_results -> truncated=True, list capped.
- `test_min_shared_filter_excludes_rare_peers()` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L300) — peer_b with shared=1 < min_shared=3 excluded; peer_a with shared=5 included.
- `test_nav_co_change_in_new_action_parity()` — [`L583`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L583) — nav_co_change lives in NEW_ACTION_PARITY with --co-change CLI flag.
- `test_nav_description_mentions_co_change()` — [`L614`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L614) — _NAV_DESCRIPTION must include co_change so agents can discover the action.
- `test_nav_facade_co_change_action_dispatches()` — [`L474`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L474) — nav execute({action: co_change, file_path: ...}) routes to _co_change_route.
- `test_nav_facade_co_change_carries_candidates_below_threshold()` — [`L1631`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1631) — nav facade co_change result must include candidates_below_threshold field.
- `test_nav_facade_co_change_default_output_format_is_toon()` — [`L542`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L542) — MCP house rule: default output_format for co_change is toon -- LOCKED sec.1.
- `test_nav_facade_co_change_output_format_toon()` — [`L513`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L513) — output_format=toon -> toon_content key present (TOON wrapper applied).
- `test_nav_facade_co_change_requires_symbol_or_file_path()` — [`L504`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L504) — co_change requires symbol OR file_path; missing both -> success=False.
- `test_nav_facade_co_change_resolves_symbol_to_file_via_call_graph()` — [`L1013`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1013) — When symbol= is given, attempt to resolve via call graph (lines 362-366).
- `test_nav_facade_co_change_symbol_fallback_when_resolution_fails()` — [`L1064`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1064) — When symbol resolution fails, fall back to treating symbol as file path.
- `test_nav_facade_schema_action_enum_includes_co_change()` — [`L570`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L570) — Schema action enum must include co_change so agents can discover it.
- `test_no_git_repo_returns_empty()` — [`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L158) — git exit code != 0 -> success=True, commits_analyzed=0, co_changed_files=[].
- `test_no_target_commits_returns_empty()` — [`L359`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L359) — File with no history -> success=True, commits_analyzed=0, empty list.
- `test_real_repo_co_change_under_2s(tmp_path: Path)` — [`L814`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L814) — Rule-11: _compute_co_change on a ~10-commit real git repo completes < 2.0 s.
- `test_result_includes_agent_summary()` — [`L448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L448) — co_change result must include agent_summary dict for downstream routing.
- `test_server_instructions_mention_co_change()` — [`L626`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L626) — MCP server instructions must document co_change.
- `test_single_subprocess_structural_invariant()` — [`L417`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L417) — RFC structural invariant: exactly 2 _run_git calls (rev-parse + single log).
- `test_small_sample_guard_adequate_sample_may_say_safe()` — [`L1438`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1438) — n=10 commits AND no candidates at all -> 'Safe to edit in isolation' IS allowed.
- `test_small_sample_guard_insufficient_history_next_step()` — [`L1401`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L1401) — n=3 commits -> next_step must contain 'insufficient history' and NOT 'Safe to edit'.
- `test_sorted_by_lift_descending()` — [`L674`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L674) — co_changed_files must be sorted by lift descending.
- `test_test_files_excluded_from_peers()` — [`L330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L330) — Test-file peers are excluded by default (co_change is about production coupling).
- `test_window_string_format()` — [`L650`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_co_change.py#L650) — result['window'] must be 'last N commits' where N == max_commits.

