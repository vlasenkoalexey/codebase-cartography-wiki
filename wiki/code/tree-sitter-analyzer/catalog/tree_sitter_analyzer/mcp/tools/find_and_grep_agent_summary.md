---
title: 'Module: tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.find_and_grep_agent_summary`/
symbols:
  build_agent_summary: build_agent_summary().
  build_agent_summary_from_meta: build_agent_summary_from_meta().
  _build_summary_line: _build_summary_line().
  FindAndGrepSummaryInput.arguments: FindAndGrepSummaryInput#arguments.
  FindAndGrepSummaryInput.mode: FindAndGrepSummaryInput#mode.
  FindAndGrepSummaryInput.searched_file_count: FindAndGrepSummaryInput#searched_file_count.
  FindAndGrepSummaryInput.file_count: FindAndGrepSummaryInput#file_count.
  FindAndGrepSummaryInput.truncated: FindAndGrepSummaryInput#truncated.
  count_match_files: count_match_files().
  _short_query: _short_query().
  FindAndGrepSummaryInput: FindAndGrepSummaryInput#
  FindAndGrepSummaryInput.count: FindAndGrepSummaryInput#count.
  FindAndGrepSummaryInput.total_matches: FindAndGrepSummaryInput#total_matches.
  FindAndGrepSummaryInput.fd_elapsed_ms: FindAndGrepSummaryInput#fd_elapsed_ms.
  FindAndGrepSummaryInput.rg_elapsed_ms: FindAndGrepSummaryInput#rg_elapsed_ms.
  _find_and_grep_summary_risk: _find_and_grep_summary_risk().
  _find_and_grep_summary_next_step: _find_and_grep_summary_next_step().
  _find_and_grep_summary_suggested_tool: _find_and_grep_summary_suggested_tool().
  _find_and_grep_summary_stop_condition: _find_and_grep_summary_stop_condition().
---
# Module: [`tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py)

## Classes
### `FindAndGrepSummaryInput`
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L10)
- doc: Inputs needed to summarize one find_and_grep response.
- signature: `class FindAndGrepSummaryInput:`
- members:
  - `arguments` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L13)
  - `count` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L15)
  - `fd_elapsed_ms` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L17)
  - `file_count` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L20)
  - `mode` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L14)
  - `rg_elapsed_ms` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L18)
  - `searched_file_count` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L19)
  - `total_matches` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L21)
  - `truncated` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L16)
- used by: [`build_agent_summary`](find_and_grep_agent_summary.md#build_agent_summary), [`build_agent_summary_from_meta`](find_and_grep_agent_summary.md#build_agent_summary_from_meta), [`_build_summary_line`](find_and_grep_agent_summary.md#_build_summary_line)

## Functions
- `_build_summary_line(context: FindAndGrepSummaryInput, *, match_total: int)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L72) — Build a one-line human/agent-readable digest.
- `_find_and_grep_summary_next_step(risk: str, mode: str, match_total: int, file_count: int | None)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L143)
- `_find_and_grep_summary_risk(match_total: int, searched_file_count: int, truncated: bool)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L133)
- `_find_and_grep_summary_stop_condition(risk: str, mode: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L172)
- `_find_and_grep_summary_suggested_tool(risk: str, mode: str, file_count: int | None)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L160)
- `_short_query(query: Any, limit: int = 120)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L126)
- `build_agent_summary(context: FindAndGrepSummaryInput)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L24) — Build a compact fd+rg summary for immediate agent decisions.
- `build_agent_summary_from_meta(arguments: dict[str, Any], *, mode: str, count: int, meta: dict[str, Any], file_count: int | None = None, total_matches: int | None = None)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L89) — Build an agent summary from the shared find_and_grep meta block.
- `count_match_files(matches: list[dict[str, Any]])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_agent_summary.py#L114) — Return the number of unique files represented by matches.

