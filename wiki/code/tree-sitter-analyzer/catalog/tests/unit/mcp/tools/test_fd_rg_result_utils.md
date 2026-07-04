---
title: 'Module: tests/unit/mcp/tools/test_fd_rg_result_utils.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_fd_rg_result_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_fd_rg_result_utils`/
symbols:
  _rg_match_event: _rg_match_event().
  TestParseRgJsonLinesToMatches.test_single_match: TestParseRgJsonLinesToMatches#test_single_match().
  TestParseRgJsonLinesToMatches.test_skips_non_match_events: TestParseRgJsonLinesToMatches#test_skips_non_match_events().
  TestParseRgJsonLinesToMatches.test_multiple_matches: TestParseRgJsonLinesToMatches#test_multiple_matches().
  TestParseRgJsonLinesToMatches.test_hard_cap_enforced: TestParseRgJsonLinesToMatches#test_hard_cap_enforced().
  TestParseRgJsonLinesToMatches.test_line_normalization: TestParseRgJsonLinesToMatches#test_line_normalization().
  TestParseRgJsonLinesToMatches.test_unicode_handling: TestParseRgJsonLinesToMatches#test_unicode_handling().
  TestParseRgJsonLinesToMatches.test_empty_input: TestParseRgJsonLinesToMatches#test_empty_input().
  TestParseRgJsonLinesToMatches.test_whitespace_only: TestParseRgJsonLinesToMatches#test_whitespace_only().
  TestParseRgJsonLinesToMatches.test_invalid_json_line: TestParseRgJsonLinesToMatches#test_invalid_json_line().
  TestParseRgJsonLinesToMatches.test_missing_path_text_skipped: TestParseRgJsonLinesToMatches#test_missing_path_text_skipped().
  TestParseRgJsonLinesToMatches.test_missing_data_skipped: TestParseRgJsonLinesToMatches#test_missing_data_skipped().
  TestParseRgJsonLinesToMatches.test_invalid_utf8_replaced: TestParseRgJsonLinesToMatches#test_invalid_utf8_replaced().
  TestGroupMatchesByFile.test_empty_input: TestGroupMatchesByFile#test_empty_input().
  TestGroupMatchesByFile.test_single_match: TestGroupMatchesByFile#test_single_match().
  TestGroupMatchesByFile.test_multiple_files: TestGroupMatchesByFile#test_multiple_files().
  TestGroupMatchesByFile.test_fallback_keys: TestGroupMatchesByFile#test_fallback_keys().
  TestOptimizeMatchPaths.test_empty_input: TestOptimizeMatchPaths#test_empty_input().
  TestOptimizeMatchPaths.test_common_prefix_removed: TestOptimizeMatchPaths#test_common_prefix_removed().
  TestOptimizeMatchPaths.test_no_common_prefix: TestOptimizeMatchPaths#test_no_common_prefix().
  TestOptimizeMatchPaths.test_deep_path_shortened: TestOptimizeMatchPaths#test_deep_path_shortened().
  TestOptimizeMatchPaths.test_no_file_key: TestOptimizeMatchPaths#test_no_file_key().
  TestSummarizeSearchResults.test_empty_input: TestSummarizeSearchResults#test_empty_input().
  TestSummarizeSearchResults.test_single_file: TestSummarizeSearchResults#test_single_file().
  TestSummarizeSearchResults.test_max_files_limit: TestSummarizeSearchResults#test_max_files_limit().
  TestSummarizeSearchResults.test_line_truncation: TestSummarizeSearchResults#test_line_truncation().
  TestSummarizeSearchResults.test_empty_text_uses_count_fallback: TestSummarizeSearchResults#test_empty_text_uses_count_fallback().
  TestSummarizeSearchResults.test_remaining_lines_budget: TestSummarizeSearchResults#test_remaining_lines_budget().
  TestSummarizeSearchResults.test_summary_text_few_files: TestSummarizeSearchResults#test_summary_text_few_files().
  TestSummarizeSearchResults.test_summary_text_many_files: TestSummarizeSearchResults#test_summary_text_many_files().
  TestExtractFileListFromCountData.test_basic: TestExtractFileListFromCountData#test_basic().
  TestExtractFileListFromCountData.test_empty: TestExtractFileListFromCountData#test_empty().
  TestExtractFileListFromCountData.test_only_total: TestExtractFileListFromCountData#test_only_total().
  TestCreateFileSummaryFromCountData.test_basic: TestCreateFileSummaryFromCountData#test_basic().
  TestCreateFileSummaryFromCountData.test_missing_total: TestCreateFileSummaryFromCountData#test_missing_total().
  TestCreateFileSummaryFromCountData.test_empty: TestCreateFileSummaryFromCountData#test_empty().
  _rg_summary_event: _rg_summary_event().
  TestParseRgJsonLinesToMatches: TestParseRgJsonLinesToMatches#
  TestGroupMatchesByFile: TestGroupMatchesByFile#
  TestOptimizeMatchPaths: TestOptimizeMatchPaths#
  TestSummarizeSearchResults: TestSummarizeSearchResults#
  TestExtractFileListFromCountData: TestExtractFileListFromCountData#
  TestCreateFileSummaryFromCountData: TestCreateFileSummaryFromCountData#
---
# Module: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py)

## Classes
### `TestCreateFileSummaryFromCountData`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L241)
- signature: `class TestCreateFileSummaryFromCountData:`
- members:
  - `test_basic(self)` — [`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L242)
  - `test_empty(self)` — [`L256`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L256)
  - `test_missing_total(self)` — [`L251`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L251)
- uses (calls/refs, reference-scoped): [`create_file_summary_from_count_data`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#create_file_summary_from_count_data)

### `TestExtractFileListFromCountData`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L228)
- signature: `class TestExtractFileListFromCountData:`
- members:
  - `test_basic(self)` — [`L229`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L229)
  - `test_empty(self)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L234)
  - `test_only_total(self)` — [`L237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L237)
- uses (calls/refs, reference-scoped): [`extract_file_list_from_count_data`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#extract_file_list_from_count_data)

### `TestGroupMatchesByFile`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L113)
- signature: `class TestGroupMatchesByFile:`
- members:
  - `test_empty_input(self)` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L114)
  - `test_fallback_keys(self)` — [`L138`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L138)
  - `test_multiple_files(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L128)
  - `test_single_match(self)` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L120)
- uses (calls/refs, reference-scoped): [`group_matches_by_file`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#group_matches_by_file)

### `TestOptimizeMatchPaths`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:145`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L145)
- signature: `class TestOptimizeMatchPaths:`
- members:
  - `test_common_prefix_removed(self)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L152)
  - `test_deep_path_shortened(self)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L166)
  - `test_empty_input(self)` — [`L146`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L146)
  - `test_no_common_prefix(self)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L161)
  - `test_no_file_key(self)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L171)
- uses (calls/refs, reference-scoped): [`optimize_match_paths`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#optimize_match_paths)

### `TestParseRgJsonLinesToMatches`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L39)
- signature: `class TestParseRgJsonLinesToMatches:`
- members:
  - `test_empty_input(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L40)
  - `test_hard_cap_enforced(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L90)
  - `test_invalid_json_line(self)` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L61)
  - `test_invalid_utf8_replaced(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L107)
  - `test_line_normalization(self)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L97)
  - `test_missing_data_skipped(self)` — [`L85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L85)
  - `test_missing_path_text_skipped(self)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L77)
  - `test_multiple_matches(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L65)
  - `test_single_match(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L46)
  - `test_skips_non_match_events(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L57)
  - `test_unicode_handling(self)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L102)
  - `test_whitespace_only(self)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L43)
- uses (calls/refs, reference-scoped): [`parse_rg_json_lines_to_matches`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#parse_rg_json_lines_to_matches)  (2 test-only)

### `TestSummarizeSearchResults`
- def: [`tests/unit/mcp/tools/test_fd_rg_result_utils.py:177`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L177)
- signature: `class TestSummarizeSearchResults:`
- members:
  - `test_empty_input(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L178)
  - `test_empty_text_uses_count_fallback(self)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L205)
  - `test_line_truncation(self)` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L198)
  - `test_max_files_limit(self)` — [`L192`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L192)
  - `test_remaining_lines_budget(self)` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L211)
  - `test_single_file(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L185)
  - `test_summary_text_few_files(self)` — [`L217`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L217)
  - `test_summary_text_many_files(self)` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L222)
- uses (calls/refs, reference-scoped): [`summarize_search_results`](../../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#summarize_search_results)

## Functions
- `_rg_match_event(file_path: str, line_number: int, text: str, submatches: list | None = None)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L18)
- `_rg_summary_event()` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_fd_rg_result_utils.py#L33)

