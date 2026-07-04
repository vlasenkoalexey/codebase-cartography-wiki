---
title: 'Module: tree_sitter_analyzer/mcp/tools/find_and_grep_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/find_and_grep_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.find_and_grep_response`/
symbols:
  FindAndGrepRespondMixin._respond_grouped: FindAndGrepRespondMixin#_respond_grouped().
  FindAndGrepRespondMixin._respond_full: FindAndGrepRespondMixin#_respond_full().
  FindAndGrepRespondMixin._respond_summary: FindAndGrepRespondMixin#_respond_summary().
  FindAndGrepRespondMixin: FindAndGrepRespondMixin#
  FindAndGrepRespondMixin.file_output_manager: FindAndGrepRespondMixin#file_output_manager.
  _attach_total_count_metadata: _attach_total_count_metadata().
  _build_next_steps: _build_next_steps().
---
# Module: [`tree_sitter_analyzer/mcp/tools/find_and_grep_response.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py)

## Classes
### `FindAndGrepRespondMixin`
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_response.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L20)
- doc: Build response payloads for grouped, summary, and full match modes.
- signature: `class FindAndGrepRespondMixin:`
- members:
  - `_respond_full(self, arguments: dict[str, Any], matches: list[dict[str, Any]], meta: dict[str, Any], output_format: str, *, real_total: int | None = None, total_count_known: bool = True)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L112) — Return full match results with optional next_steps.
  - `_respond_grouped(self, arguments: dict[str, Any], matches: list[dict[str, Any]], meta: dict[str, Any], *, real_total: int | None = None, total_count_known: bool = True)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L25) — Return matches grouped by file path.
  - `_respond_summary(self, arguments: dict[str, Any], matches: list[dict[str, Any]], meta: dict[str, Any], *, real_total: int | None = None, total_count_known: bool = True)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L69) — Return a summary-only response without full match data.
  - `file_output_manager` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L23)
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`FindAndGrepTool`](find_and_grep_tool.md#FindAndGrepTool), [`build_agent_summary_from_meta`](find_and_grep_agent_summary.md#build_agent_summary_from_meta), [`normalize_envelope`](search_envelope.md#normalize_envelope), [`summarize_search_results`](fd_rg_result_utils.md#summarize_search_results), [`attach_toon_content_to_response`](../utils/format_helper.md#attach_toon_content_to_response), [`handle_output`](find_and_grep_helpers.md#handle_output), [`group_matches_by_file`](fd_rg_result_utils.md#group_matches_by_file), [`count_match_files`](find_and_grep_agent_summary.md#count_match_files), [`_attach_total_count_metadata`](find_and_grep_response.md#_attach_total_count_metadata), [`_build_next_steps`](find_and_grep_response.md#_build_next_steps)
- used by: [`FindAndGrepTool`](find_and_grep_tool.md#FindAndGrepTool), [`_execute_full_match_mode`](find_and_grep_tool.md#FindAndGrepTool._execute_full_match_mode)

## Functions
- `_attach_total_count_metadata(result: dict[str, Any], *, displayed_count: int, real_total: int | None, total_count_known: bool, truncated: bool)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L163) — Attach H2-style ``total_count_known``/``total_count_at_least`` flags.
- `_build_next_steps(matches: list[dict[str, Any]])` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_response.py#L189) — Build next_steps suggestions for AI agents.

