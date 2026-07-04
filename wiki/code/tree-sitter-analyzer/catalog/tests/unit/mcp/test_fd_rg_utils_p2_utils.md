---
title: 'Module: tests/unit/mcp/test_fd_rg_utils_p2_utils.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_fd_rg_utils_p2_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_fd_rg_utils_p2_utils`/Test
symbols:
  TestParseRgJsonLinesToMatches.test_parse_hard_cap: ParseRgJsonLinesToMatches#test_parse_hard_cap().
  TestParseRgJsonLinesToMatches.test_parse_valid_json: ParseRgJsonLinesToMatches#test_parse_valid_json().
  TestParseRgJsonLinesToMatches.test_parse_multiple_lines: ParseRgJsonLinesToMatches#test_parse_multiple_lines().
  TestParseRgJsonLinesToMatches.test_parse_non_match_event: ParseRgJsonLinesToMatches#test_parse_non_match_event().
  TestParseRgJsonLinesToMatches.test_parse_invalid_json: ParseRgJsonLinesToMatches#test_parse_invalid_json().
  TestParseRgJsonLinesToMatches.test_parse_empty_lines: ParseRgJsonLinesToMatches#test_parse_empty_lines().
  TestParseRgJsonLinesToMatches.test_parse_with_submatches: ParseRgJsonLinesToMatches#test_parse_with_submatches().
  TestGroupMatchesByFile.test_group_empty_matches: GroupMatchesByFile#test_group_empty_matches().
  TestGroupMatchesByFile.test_group_single_file: GroupMatchesByFile#test_group_single_file().
  TestGroupMatchesByFile.test_group_multiple_files: GroupMatchesByFile#test_group_multiple_files().
  TestOptimizeMatchPaths.test_optimize_empty_matches: OptimizeMatchPaths#test_optimize_empty_matches().
  TestOptimizeMatchPaths.test_optimize_single_match: OptimizeMatchPaths#test_optimize_single_match().
  TestOptimizeMatchPaths.test_optimize_with_common_prefix: OptimizeMatchPaths#test_optimize_with_common_prefix().
  TestOptimizeMatchPaths.test_optimize_with_long_path: OptimizeMatchPaths#test_optimize_with_long_path().
  TestSummarizeSearchResults.test_summarize_empty_results: SummarizeSearchResults#test_summarize_empty_results().
  TestSummarizeSearchResults.test_summarize_single_file: SummarizeSearchResults#test_summarize_single_file().
  TestSummarizeSearchResults.test_summarize_multiple_files: SummarizeSearchResults#test_summarize_multiple_files().
  TestSummarizeSearchResults.test_summarize_with_max_files_limit: SummarizeSearchResults#test_summarize_with_max_files_limit().
  TestSummarizeSearchResults.test_summarize_truncates_long_lines: SummarizeSearchResults#test_summarize_truncates_long_lines().
  TestParseRgCountOutput.test_parse_valid_output: ParseRgCountOutput#test_parse_valid_output().
  TestParseRgCountOutput.test_parse_empty_output: ParseRgCountOutput#test_parse_empty_output().
  TestParseRgCountOutput.test_parse_with_whitespace_lines: ParseRgCountOutput#test_parse_with_whitespace_lines().
  TestParseRgCountOutput.test_parse_invalid_format: ParseRgCountOutput#test_parse_invalid_format().
  TestExtractFileListFromCountData.test_extract_file_list: ExtractFileListFromCountData#test_extract_file_list().
  TestCreateFileSummaryFromCountData.test_create_summary: CreateFileSummaryFromCountData#test_create_summary().
  TestSplitRootsForParallelProcessing.test_split_empty_roots: SplitRootsForParallelProcessing#test_split_empty_roots().
  TestSplitRootsForParallelProcessing.test_split_single_root: SplitRootsForParallelProcessing#test_split_single_root().
  TestSplitRootsForParallelProcessing.test_split_multiple_roots: SplitRootsForParallelProcessing#test_split_multiple_roots().
  TestSplitRootsForParallelProcessing.test_split_with_remainder: SplitRootsForParallelProcessing#test_split_with_remainder().
  TestRunParallelRgSearches.test_run_single_command: RunParallelRgSearches#test_run_single_command().
  TestRunParallelRgSearches.test_run_multiple_commands: RunParallelRgSearches#test_run_multiple_commands().
  TestRunParallelRgSearches.test_run_with_timeout: RunParallelRgSearches#test_run_with_timeout().
  TestMergeRgResults.test_merge_successful_results: MergeRgResults#test_merge_successful_results().
  TestMergeRgResults.test_merge_count_only_results: MergeRgResults#test_merge_count_only_results().
  TestMergeRgResults.test_merge_with_failure: MergeRgResults#test_merge_with_failure().
  TestNormalizeMaxFilesize.test_normalize_valid_size: NormalizeMaxFilesize#test_normalize_valid_size().
  TestNormalizeMaxFilesize.test_normalize_none: NormalizeMaxFilesize#test_normalize_none().
  TestNormalizeMaxFilesize.test_normalize_above_hard_cap: NormalizeMaxFilesize#test_normalize_above_hard_cap().
  TestNormalizeMaxFilesize.test_normalize_invalid_format: NormalizeMaxFilesize#test_normalize_invalid_format().
  TestConstants.test_max_results_hard_cap: Constants#test_max_results_hard_cap().
  TestConstants.test_default_results_limit: Constants#test_default_results_limit().
  TestConstants.test_default_rg_max_filesize: Constants#test_default_rg_max_filesize().
  TestConstants.test_rg_max_filesize_hard_cap_bytes: Constants#test_rg_max_filesize_hard_cap_bytes().
  TestConstants.test_default_rg_timeout_ms: Constants#test_default_rg_timeout_ms().
  TestConstants.test_rg_timeout_hard_cap_ms: Constants#test_rg_timeout_hard_cap_ms().
  TestParseRgJsonLinesToMatches: ParseRgJsonLinesToMatches#
  TestGroupMatchesByFile: GroupMatchesByFile#
  TestOptimizeMatchPaths: OptimizeMatchPaths#
  TestSummarizeSearchResults: SummarizeSearchResults#
  TestParseRgCountOutput: ParseRgCountOutput#
  TestExtractFileListFromCountData: ExtractFileListFromCountData#
  TestCreateFileSummaryFromCountData: CreateFileSummaryFromCountData#
  TestSplitRootsForParallelProcessing: SplitRootsForParallelProcessing#
  TestRunParallelRgSearches: RunParallelRgSearches#
  TestMergeRgResults: MergeRgResults#
  TestNormalizeMaxFilesize: NormalizeMaxFilesize#
  TestConstants: Constants#
---
# Module: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py)

## Classes
### `TestConstants`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L447)
- doc: Tests for module constants.
- signature: `class TestConstants:`
- members:
  - `test_default_results_limit(self)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L454) — Test DEFAULT_RESULTS_LIMIT constant.
  - `test_default_rg_max_filesize(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L458) — Test DEFAULT_RG_MAX_FILESIZE constant.
  - `test_default_rg_timeout_ms(self)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L466) — Test DEFAULT_RG_TIMEOUT_MS constant.
  - `test_max_results_hard_cap(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L450) — Test MAX_RESULTS_HARD_CAP constant.
  - `test_rg_max_filesize_hard_cap_bytes(self)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L462) — Test RG_MAX_FILESIZE_HARD_CAP_BYTES constant.
  - `test_rg_timeout_hard_cap_ms(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L470) — Test RG_TIMEOUT_HARD_CAP_MS constant.
- uses (calls/refs, reference-scoped): [`MAX_RESULTS_HARD_CAP`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#MAX_RESULTS_HARD_CAP), [`DEFAULT_RESULTS_LIMIT`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#DEFAULT_RESULTS_LIMIT), [`DEFAULT_RG_MAX_FILESIZE`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#DEFAULT_RG_MAX_FILESIZE), [`DEFAULT_RG_TIMEOUT_MS`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#DEFAULT_RG_TIMEOUT_MS), [`RG_MAX_FILESIZE_HARD_CAP_BYTES`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#RG_MAX_FILESIZE_HARD_CAP_BYTES), [`RG_TIMEOUT_HARD_CAP_MS`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#RG_TIMEOUT_HARD_CAP_MS)

### `TestCreateFileSummaryFromCountData`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L257)
- doc: Tests for create_file_summary_from_count_data function.
- signature: `class TestCreateFileSummaryFromCountData:`
- members:
  - `test_create_summary(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L260) — Test creating file summary from count data.
- uses (calls/refs, reference-scoped): [`create_file_summary_from_count_data`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#create_file_summary_from_count_data)

### `TestExtractFileListFromCountData`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L240)
- doc: Tests for extract_file_list_from_count_data function.
- signature: `class TestExtractFileListFromCountData:`
- members:
  - `test_extract_file_list(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L243) — Test extracting file list from count data.
- uses (calls/refs, reference-scoped): [`extract_file_list_from_count_data`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#extract_file_list_from_count_data)

### `TestGroupMatchesByFile`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L74)
- doc: Tests for group_matches_by_file function.
- signature: `class TestGroupMatchesByFile:`
- members:
  - `test_group_empty_matches(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L77) — Test grouping empty matches.
  - `test_group_multiple_files(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L96) — Test grouping matches from multiple files.
  - `test_group_single_file(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L84) — Test grouping matches from single file.
- uses (calls/refs, reference-scoped): [`group_matches_by_file`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#group_matches_by_file)

### `TestMergeRgResults`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L385)
- doc: Tests for merge_rg_results function.
- signature: `class TestMergeRgResults:`
- members:
  - `test_merge_count_only_results(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L399) — Test merging count-only results.
  - `test_merge_successful_results(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L388) — Test merging successful results.
  - `test_merge_with_failure(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L410) — Test merging with a failure.
- uses (calls/refs, reference-scoped): [`merge_rg_results`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#merge_rg_results)

### `TestNormalizeMaxFilesize`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L423)
- doc: Tests for normalize_max_filesize function.
- signature: `class TestNormalizeMaxFilesize:`
- members:
  - `test_normalize_above_hard_cap(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L436) — Test normalizing size above hard cap.
  - `test_normalize_invalid_format(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L441) — Test normalizing invalid format.
  - `test_normalize_none(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L431) — Test normalizing None.
  - `test_normalize_valid_size(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L426) — Test normalizing valid size.
- uses (calls/refs, reference-scoped): [`normalize_max_filesize`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#normalize_max_filesize)

### `TestOptimizeMatchPaths`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L110)
- doc: Tests for optimize_match_paths function.
- signature: `class TestOptimizeMatchPaths:`
- members:
  - `test_optimize_empty_matches(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L113) — Test optimizing empty matches.
  - `test_optimize_single_match(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L118) — Test optimizing single match.
  - `test_optimize_with_common_prefix(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L126) — Test optimizing with common prefix.
  - `test_optimize_with_long_path(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L138) — Test optimizing with long path.
- uses (calls/refs, reference-scoped): [`optimize_match_paths`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#optimize_match_paths)

### `TestParseRgCountOutput`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L208)
- doc: Tests for parse_rg_count_output function.
- signature: `class TestParseRgCountOutput:`
- members:
  - `test_parse_empty_output(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L219) — Test parsing empty output.
  - `test_parse_invalid_format(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L232) — Test that invalid format lines are skipped.
  - `test_parse_valid_output(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L211) — Test parsing valid count output.
  - `test_parse_with_whitespace_lines(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L224) — Test that whitespace lines are skipped.
- uses (calls/refs, reference-scoped): [`parse_rg_count_output`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#parse_rg_count_output)

### `TestParseRgJsonLinesToMatches`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L16)
- doc: Tests for parse_rg_json_lines_to_matches function.
- signature: `class TestParseRgJsonLinesToMatches:`
- members:
  - `test_parse_empty_lines(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L48) — Test that empty lines are skipped.
  - `test_parse_hard_cap(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L62) — Test that results are capped at hard limit.
  - `test_parse_invalid_json(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L42) — Test that invalid JSON is skipped.
  - `test_parse_multiple_lines(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L28) — Test parsing multiple JSON lines.
  - `test_parse_non_match_event(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L36) — Test that non-match events are skipped.
  - `test_parse_valid_json(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L19) — Test parsing valid JSON output.
  - `test_parse_with_submatches(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L54) — Test parsing with submatches.
- uses (calls/refs, reference-scoped): [`parse_rg_json_lines_to_matches`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#parse_rg_json_lines_to_matches), [`MAX_RESULTS_HARD_CAP`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#MAX_RESULTS_HARD_CAP)

### `TestRunParallelRgSearches`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L312)
- doc: Tests for run_parallel_rg_searches function.
- signature: `class TestRunParallelRgSearches:`
- members:
  - `test_run_multiple_commands(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L339) — Test running multiple commands.
  - `test_run_single_command(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L316) — Test running single command.
  - `test_run_with_timeout(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L363) — Test running with timeout.
- uses (calls/refs, reference-scoped): [`run_parallel_rg_searches`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#run_parallel_rg_searches)

### `TestSplitRootsForParallelProcessing`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L275)
- doc: Tests for split_roots_for_parallel_processing function.
- signature: `class TestSplitRootsForParallelProcessing:`
- members:
  - `test_split_empty_roots(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L278) — Test splitting empty roots.
  - `test_split_multiple_roots(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L291) — Test splitting multiple roots.
  - `test_split_single_root(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L283) — Test splitting single root.
  - `test_split_with_remainder(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L297) — Test splitting with remainder.
- uses (calls/refs, reference-scoped): [`split_roots_for_parallel_processing`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#split_roots_for_parallel_processing)

### `TestSummarizeSearchResults`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_utils.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L152)
- doc: Tests for summarize_search_results function.
- signature: `class TestSummarizeSearchResults:`
- members:
  - `test_summarize_empty_results(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L155) — Test summarizing empty results.
  - `test_summarize_multiple_files(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L175) — Test summarizing multiple files.
  - `test_summarize_single_file(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L163) — Test summarizing single file.
  - `test_summarize_truncates_long_lines(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L195) — Test that long lines are truncated.
  - `test_summarize_with_max_files_limit(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_utils.py#L186) — Test summarizing with max files limit.
- uses (calls/refs, reference-scoped): [`summarize_search_results`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#summarize_search_results)

