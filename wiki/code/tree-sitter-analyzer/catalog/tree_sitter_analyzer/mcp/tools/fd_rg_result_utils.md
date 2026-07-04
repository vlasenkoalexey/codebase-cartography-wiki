---
title: 'Module: tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.fd_rg_result_utils`/
symbols:
  summarize_search_results: summarize_search_results().
  parse_rg_json_lines_to_matches: parse_rg_json_lines_to_matches().
  optimize_match_paths: optimize_match_paths().
  group_matches_by_file: group_matches_by_file().
  create_file_summary_from_count_data: create_file_summary_from_count_data().
  extract_file_list_from_count_data: extract_file_list_from_count_data().
  _collect_top_files: _collect_top_files().
  _optimize_file_path: _optimize_file_path().
  _MAX_RESULTS_HARD_CAP: _MAX_RESULTS_HARD_CAP.
  _group_matches_by_file: _group_matches_by_file().
  _build_sample_lines: _build_sample_lines().
---
# Module: [`tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py)

## Functions
- `_build_sample_lines(file_matches: list[dict[str, Any]], remaining_lines: int)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L176) — Return ``(sample_lines, lines_consumed)`` for up to 3 matches.
- `_collect_top_files(file_groups: dict[str, list[dict[str, Any]]], common_prefix: str, max_files: int, max_total_lines: int)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L203) — Build the ``top_files`` rows ordered by descending match count.
- `_group_matches_by_file(matches: list[dict[str, Any]])` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L155) — Group matches by file path; return ``(groups, common_prefix)``.
- `_optimize_file_path(file_path: str, common_prefix: str = "")` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L136) — Optimize file path for token efficiency by removing common prefixes and shortening.
- `create_file_summary_from_count_data(count_data: dict[str, int])` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L281) — Create a file summary structure from count data.
- `extract_file_list_from_count_data(count_data: dict[str, int])` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L275) — Extract file list from count data, excluding the special __total__ key.
- `group_matches_by_file(matches: list[dict[str, Any]])` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L76) — Group matches by file to eliminate file path duplication.
- `optimize_match_paths(matches: list[dict[str, Any]])` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L111) — Optimize file paths in match results to reduce token consumption.
- `parse_rg_json_lines_to_matches(stdout_bytes: bytes)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L19) — Parse ripgrep JSON event stream and keep only match events.
- `summarize_search_results(matches: list[dict[str, Any]], max_files: int = 10, max_total_lines: int = 50)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L232) — Summarize search results to reduce context size while preserving key information.

## Module values
- `_MAX_RESULTS_HARD_CAP` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.py#L15)

