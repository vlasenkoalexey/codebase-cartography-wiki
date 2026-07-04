---
title: 'Module: tests/test_prs.py'
type: catalog
provenance: extracted
module: tests/test_prs.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_prs`/
symbols:
  make_pr: make_pr().
  TestClassify.test_ready: TestClassify#test_ready().
  TestClassify.test_ci_fail: TestClassify#test_ci_fail().
  TestClassify.test_changes_req: TestClassify#test_changes_req().
  TestClassify.test_draft: TestClassify#test_draft().
  TestClassify.test_stale: TestClassify#test_stale().
  TestClassify.test_draft_not_marked_stale: TestClassify#test_draft_not_marked_stale().
  TestClassify.test_pending: TestClassify#test_pending().
  TestClassify.test_wrong_base: TestClassify#test_wrong_base().
  TestComputePrImpact.test_matching_files_returns_correct_communities_and_count: TestComputePrImpact#test_matching_files_returns_correct_communities_and_count().
  TestComputePrImpact.test_matching_both_files: TestComputePrImpact#test_matching_both_files().
  TestComputePrImpact.test_empty_files_returns_empty: TestComputePrImpact#test_empty_files_returns_empty().
  TestComputePrImpact.test_no_matching_files_returns_empty: TestComputePrImpact#test_no_matching_files_returns_empty().
  TestFormatPrsText.test_contains_pr_metadata_and_count_header: TestFormatPrsText#test_contains_pr_metadata_and_count_header().
  TestComputePrImpact._make_graph: TestComputePrImpact#_make_graph().
  TestParseCi.test_empty_rollup_returns_none: TestParseCi#test_empty_rollup_returns_none().
  TestParseCi.test_failure_conclusion: TestParseCi#test_failure_conclusion().
  TestParseCi.test_cancelled_is_failure: TestParseCi#test_cancelled_is_failure().
  TestParseCi.test_timed_out_is_failure: TestParseCi#test_timed_out_is_failure().
  TestParseCi.test_in_progress_is_pending: TestParseCi#test_in_progress_is_pending().
  TestParseCi.test_success: TestParseCi#test_success().
  TestParseCi.test_mixed_success_and_failure_is_failure: TestParseCi#test_mixed_success_and_failure_is_failure().
  TestPathMatch.test_exact_match: TestPathMatch#test_exact_match().
  TestPathMatch.test_graph_path_longer_with_boundary: TestPathMatch#test_graph_path_longer_with_boundary().
  TestPathMatch.test_no_false_positive_on_partial_filename: TestPathMatch#test_no_false_positive_on_partial_filename().
  TestPathMatch.test_both_directions_work: TestPathMatch#test_both_directions_work().
  TestComputePrImpact.test_no_double_counting_when_basename_matches_multiple_paths: TestComputePrImpact#test_no_double_counting_when_basename_matches_multiple_paths().
  TestComputePrImpact.test_no_double_counting_same_graph_file_matched_by_two_pr_files: TestComputePrImpact#test_no_double_counting_same_graph_file_matched_by_two_pr_files().
  TestFetchWorktrees.test_normal_case_maps_branch_to_path: TestFetchWorktrees#test_normal_case_maps_branch_to_path().
  TestFetchWorktrees.test_detached_head_does_not_leak_into_next_record: TestFetchWorktrees#test_detached_head_does_not_leak_into_next_record().
  TestFetchWorktrees.test_empty_output_returns_empty_dict: TestFetchWorktrees#test_empty_output_returns_empty_dict().
  TestFetchWorktrees.test_nonzero_returncode_returns_empty_dict: TestFetchWorktrees#test_nonzero_returncode_returns_empty_dict().
  TestFetchWorktrees.test_subprocess_failure_returns_empty_dict: TestFetchWorktrees#test_subprocess_failure_returns_empty_dict().
  TestFormatPrsText.test_empty_pr_list: TestFormatPrsText#test_empty_pr_list().
  TestDetectDefaultBranch.test_gh_returns_main: TestDetectDefaultBranch#test_gh_returns_main().
  TestDetectDefaultBranch.test_falls_back_to_git_symbolic_ref: TestDetectDefaultBranch#test_falls_back_to_git_symbolic_ref().
  TestDetectDefaultBranch.test_both_fail_returns_main: TestDetectDefaultBranch#test_both_fail_returns_main().
  TestDetectDefaultBranch.test_gh_returns_empty_dict_falls_back: TestDetectDefaultBranch#test_gh_returns_empty_dict_falls_back().
  TestDetectDefaultBranch.test_git_timeout_returns_main: TestDetectDefaultBranch#test_git_timeout_returns_main().
  TestBuildCommunityLabels.test_basic_grouping: TestBuildCommunityLabels#test_basic_grouping().
  TestBuildCommunityLabels.test_top_n_capped: TestBuildCommunityLabels#test_top_n_capped().
  TestBuildCommunityLabels.test_no_community_field_skipped: TestBuildCommunityLabels#test_no_community_field_skipped().
  TestBuildCommunityLabels.test_empty_nodes: TestBuildCommunityLabels#test_empty_nodes().
  TestClassify: TestClassify#
  TestParseCi: TestParseCi#
  TestPathMatch: TestPathMatch#
  TestComputePrImpact: TestComputePrImpact#
  TestFetchWorktrees: TestFetchWorktrees#
  TestFormatPrsText: TestFormatPrsText#
  TestDetectDefaultBranch: TestDetectDefaultBranch#
  TestBuildCommunityLabels: TestBuildCommunityLabels#
---
# Module: [`tests/test_prs.py`](../../../../../raw/code/graphify/tests/test_prs.py)

## Classes
### `TestBuildCommunityLabels`
- def: [`tests/test_prs.py:379`](../../../../../raw/code/graphify/tests/test_prs.py#L379)
- signature: `class TestBuildCommunityLabels:`
- members:
  - `test_basic_grouping(self)` — [`L380`](../../../../../raw/code/graphify/tests/test_prs.py#L380)
  - `test_empty_nodes(self)` — [`L401`](../../../../../raw/code/graphify/tests/test_prs.py#L401)
  - `test_no_community_field_skipped(self)` — [`L397`](../../../../../raw/code/graphify/tests/test_prs.py#L397)
  - `test_top_n_capped(self)` — [`L392`](../../../../../raw/code/graphify/tests/test_prs.py#L392)
- uses (calls/refs, reference-scoped): [`build_community_labels`](../graphify/prs.md#build_community_labels)

### `TestClassify`
- def: [`tests/test_prs.py:57`](../../../../../raw/code/graphify/tests/test_prs.py#L57)
- signature: `class TestClassify:`
- members:
  - `test_changes_req(self)` — [`L66`](../../../../../raw/code/graphify/tests/test_prs.py#L66)
  - `test_ci_fail(self)` — [`L62`](../../../../../raw/code/graphify/tests/test_prs.py#L62)
  - `test_draft(self)` — [`L70`](../../../../../raw/code/graphify/tests/test_prs.py#L70)
  - `test_draft_not_marked_stale(self)` — [`L79`](../../../../../raw/code/graphify/tests/test_prs.py#L79)
  - `test_pending(self)` — [`L85`](../../../../../raw/code/graphify/tests/test_prs.py#L85)
  - `test_ready(self)` — [`L58`](../../../../../raw/code/graphify/tests/test_prs.py#L58)
  - `test_stale(self)` — [`L74`](../../../../../raw/code/graphify/tests/test_prs.py#L74)
  - `test_wrong_base(self)` — [`L89`](../../../../../raw/code/graphify/tests/test_prs.py#L89)
- uses (calls/refs, reference-scoped): [`_classify`](../graphify/prs.md#_classify)  (1 test-only)

### `TestComputePrImpact`
- def: [`tests/test_prs.py:153`](../../../../../raw/code/graphify/tests/test_prs.py#L153)
- signature: `class TestComputePrImpact:`
- members:
  - `_make_graph(self)` — [`L154`](../../../../../raw/code/graphify/tests/test_prs.py#L154) — 3 nodes across 2 communities, 2 distinct source files.
  - `test_empty_files_returns_empty(self)` — [`L176`](../../../../../raw/code/graphify/tests/test_prs.py#L176)
  - `test_matching_both_files(self)` — [`L168`](../../../../../raw/code/graphify/tests/test_prs.py#L168)
  - `test_matching_files_returns_correct_communities_and_count(self)` — [`L162`](../../../../../raw/code/graphify/tests/test_prs.py#L162)
  - `test_no_double_counting_same_graph_file_matched_by_two_pr_files(self)` — [`L198`](../../../../../raw/code/graphify/tests/test_prs.py#L198)
  - `test_no_double_counting_when_basename_matches_multiple_paths(self)` — [`L188`](../../../../../raw/code/graphify/tests/test_prs.py#L188)
  - `test_no_matching_files_returns_empty(self)` — [`L182`](../../../../../raw/code/graphify/tests/test_prs.py#L182)
- uses (calls/refs, reference-scoped): [`compute_pr_impact`](../graphify/prs.md#compute_pr_impact)

### `TestDetectDefaultBranch`
- def: [`tests/test_prs.py:333`](../../../../../raw/code/graphify/tests/test_prs.py#L333)
- signature: `class TestDetectDefaultBranch:`
- members:
  - `test_both_fail_returns_main(self)` — [`L350`](../../../../../raw/code/graphify/tests/test_prs.py#L350)
  - `test_falls_back_to_git_symbolic_ref(self)` — [`L341`](../../../../../raw/code/graphify/tests/test_prs.py#L341)
  - `test_gh_returns_empty_dict_falls_back(self)` — [`L359`](../../../../../raw/code/graphify/tests/test_prs.py#L359) — gh returns data but with no defaultBranchRef — should still fall back.
  - `test_gh_returns_main(self)` — [`L334`](../../../../../raw/code/graphify/tests/test_prs.py#L334)
  - `test_git_timeout_returns_main(self)` — [`L369`](../../../../../raw/code/graphify/tests/test_prs.py#L369)
- uses (calls/refs, reference-scoped): [`_detect_default_branch`](../graphify/prs.md#_detect_default_branch)

### `TestFetchWorktrees`
- def: [`tests/test_prs.py:211`](../../../../../raw/code/graphify/tests/test_prs.py#L211)
- signature: `class TestFetchWorktrees:`
- members:
  - `test_detached_head_does_not_leak_into_next_record(self)` — [`L233`](../../../../../raw/code/graphify/tests/test_prs.py#L233) — A detached HEAD (no branch line) must not associate its path with the
  - `test_empty_output_returns_empty_dict(self)` — [`L255`](../../../../../raw/code/graphify/tests/test_prs.py#L255)
  - `test_nonzero_returncode_returns_empty_dict(self)` — [`L263`](../../../../../raw/code/graphify/tests/test_prs.py#L263)
  - `test_normal_case_maps_branch_to_path(self)` — [`L212`](../../../../../raw/code/graphify/tests/test_prs.py#L212)
  - `test_subprocess_failure_returns_empty_dict(self)` — [`L271`](../../../../../raw/code/graphify/tests/test_prs.py#L271)
- uses (calls/refs, reference-scoped): [`fetch_worktrees`](../graphify/prs.md#fetch_worktrees)

### `TestFormatPrsText`
- def: [`tests/test_prs.py:282`](../../../../../raw/code/graphify/tests/test_prs.py#L282)
- signature: `class TestFormatPrsText:`
- members:
  - `test_contains_pr_metadata_and_count_header(self)` — [`L283`](../../../../../raw/code/graphify/tests/test_prs.py#L283)
  - `test_empty_pr_list(self)` — [`L325`](../../../../../raw/code/graphify/tests/test_prs.py#L325)
- uses (calls/refs, reference-scoped): [`format_prs_text`](../graphify/prs.md#format_prs_text)  (1 test-only)

### `TestParseCi`
- def: [`tests/test_prs.py:97`](../../../../../raw/code/graphify/tests/test_prs.py#L97)
- signature: `class TestParseCi:`
- members:
  - `test_cancelled_is_failure(self)` — [`L105`](../../../../../raw/code/graphify/tests/test_prs.py#L105)
  - `test_empty_rollup_returns_none(self)` — [`L98`](../../../../../raw/code/graphify/tests/test_prs.py#L98)
  - `test_failure_conclusion(self)` — [`L101`](../../../../../raw/code/graphify/tests/test_prs.py#L101)
  - `test_in_progress_is_pending(self)` — [`L113`](../../../../../raw/code/graphify/tests/test_prs.py#L113)
  - `test_mixed_success_and_failure_is_failure(self)` — [`L121`](../../../../../raw/code/graphify/tests/test_prs.py#L121)
  - `test_success(self)` — [`L117`](../../../../../raw/code/graphify/tests/test_prs.py#L117)
  - `test_timed_out_is_failure(self)` — [`L109`](../../../../../raw/code/graphify/tests/test_prs.py#L109)
- uses (calls/refs, reference-scoped): [`_parse_ci`](../graphify/prs.md#_parse_ci)

### `TestPathMatch`
- def: [`tests/test_prs.py:131`](../../../../../raw/code/graphify/tests/test_prs.py#L131)
- signature: `class TestPathMatch:`
- members:
  - `test_both_directions_work(self)` — [`L144`](../../../../../raw/code/graphify/tests/test_prs.py#L144)
  - `test_exact_match(self)` — [`L132`](../../../../../raw/code/graphify/tests/test_prs.py#L132)
  - `test_graph_path_longer_with_boundary(self)` — [`L135`](../../../../../raw/code/graphify/tests/test_prs.py#L135)
  - `test_no_false_positive_on_partial_filename(self)` — [`L139`](../../../../../raw/code/graphify/tests/test_prs.py#L139)
- uses (calls/refs, reference-scoped): [`_path_match`](../graphify/prs.md#_path_match)

## Functions
- `make_pr(number: int = 1, title: str = "Test PR", branch: str = "feature", base_branch: str = "v8", author: str = "alice", is_draft: bool = False, review_decision: str = "", ci_status: str = "SUCCESS", updated_at: datetime | None = None, expected_base: str = "v8")` — [`L26`](../../../../../raw/code/graphify/tests/test_prs.py#L26) — Build a minimal PRInfo with sensible defaults.

