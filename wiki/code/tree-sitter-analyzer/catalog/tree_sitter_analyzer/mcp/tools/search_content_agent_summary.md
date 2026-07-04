---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_agent_summary`/
symbols:
  build_agent_summary: build_agent_summary().
  _build_summary_line: _build_summary_line().
  SearchAgentSummaryInput.file_count: SearchAgentSummaryInput#file_count.
  SearchAgentSummaryInput.arguments: SearchAgentSummaryInput#arguments.
  SearchAgentSummaryInput.mode: SearchAgentSummaryInput#mode.
  SearchAgentSummaryInput: SearchAgentSummaryInput#
  SearchAgentSummaryInput.truncated: SearchAgentSummaryInput#truncated.
  SearchAgentSummaryInput.count: SearchAgentSummaryInput#count.
  SearchAgentSummaryInput.elapsed_ms: SearchAgentSummaryInput#elapsed_ms.
  SearchAgentSummaryInput.total_matches: SearchAgentSummaryInput#total_matches.
  count_match_files: count_match_files().
  _short_query: _short_query().
  _search_summary_risk: _search_summary_risk().
  _search_summary_next_step: _search_summary_next_step().
  _search_summary_suggested_tool: _search_summary_suggested_tool().
  _search_summary_stop_condition: _search_summary_stop_condition().
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py)

## Classes
### `SearchAgentSummaryInput`
- def: [`tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L10)
- doc: Inputs needed to summarize one search_content response.
- signature: `class SearchAgentSummaryInput:`
- members:
  - `arguments` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L13)
  - `count` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L15)
  - `elapsed_ms` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L17)
  - `file_count` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L18)
  - `mode` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L14)
  - `total_matches` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L19)
  - `truncated` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L16)
- used by: [`respond_full`](search_content_response_modes.md#respond_full), [`build_agent_summary`](search_content_agent_summary.md#build_agent_summary), [`respond_grouped`](search_content_response_modes.md#respond_grouped), [`respond_summary`](search_content_response_modes.md#respond_summary), [`respond_count_only`](search_content_response_modes.md#respond_count_only), [`_build_summary_line`](search_content_agent_summary.md#_build_summary_line)

## Functions
- `_build_summary_line(context: SearchAgentSummaryInput, *, match_total: int)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L64) — Build a one-line human/agent-readable digest.
- `_search_summary_next_step(risk: str, mode: str, match_total: int, file_count: int | None)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L94)
- `_search_summary_risk(match_total: int, truncated: bool)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L86)
- `_search_summary_stop_condition(risk: str, mode: str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L125)
- `_search_summary_suggested_tool(risk: str, mode: str, file_count: int | None)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L113)
- `_short_query(query: Any, limit: int = 120)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L79)
- `build_agent_summary(context: SearchAgentSummaryInput)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L22) — Build a compact search summary for immediate agent decisions.
- `count_match_files(matches: list[dict[str, Any]])` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_agent_summary.py#L74) — Return the number of unique files represented by search matches.

