---
title: 'Module: tree_sitter_analyzer/mcp/tools/query_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.query_helpers`/
symbols:
  handle_query_output: handle_query_output().
  build_query_agent_summary: build_query_agent_summary().
  _validate_string_arg: _validate_string_arg().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  format_summary: format_summary().
  extract_name_from_content: extract_name_from_content().
  validate_query_arguments: validate_query_arguments().
  _format_capture_item: _format_capture_item().
  _build_suppress_envelope: _build_suppress_envelope().
  _save_query_output: _save_query_output().
  build_next_steps: build_next_steps().
  _query_risk_and_step: _query_risk_and_step().
  _risk_to_verdict: _risk_to_verdict().
  _NAME_PATTERNS: _NAME_PATTERNS.
  _copy_agent_summary_to: _copy_agent_summary_to().
---
# Module: [`tree_sitter_analyzer/mcp/tools/query_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py)

## Functions
- `_build_suppress_envelope(formatted: dict[str, Any], file_path: str, language: str, query: str | None)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L329) — Build the minimal suppress envelope returned when suppress_output=True.
- `_copy_agent_summary_to(source: dict[str, Any], target: dict[str, Any])` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L314) — Copy agent_summary (and summary_line) from source dict into target envelope.
- `_format_capture_item(item: dict[str, Any])` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L172) — Build a single summary entry for one query-result item.
- `_query_risk_and_step(count: int, file_path: str, truncated: bool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L94) — Return (risk, next_step) based on query result count and truncation status.
- `_risk_to_verdict(risk: str)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L126) — Map risk level to canonical verdict string (low→INFO, medium→CAUTION, high→REVIEW).
- `_save_query_output(formatted: dict[str, Any], output_file: str, file_path: str, query: str | None, output_format: str, file_output_manager: Any)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L356) — Save formatted query output to a file and record metadata in formatted.
- `_validate_string_arg(arguments: dict[str, Any], key: str, *, non_empty: bool = False, allowed: list[str] | None = None)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L272) — Raise ValueError if ``key`` is present but fails type/value constraints.
- `build_next_steps(results: list[dict[str, Any]], file_path: str, query_used: str)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L233) — Build actionable next-step suggestions based on query results.
- `build_query_agent_summary(*, file_path: str, language: str, query: str, count: int, elapsed_ms: float, truncated: bool)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L135) — Build a compact agent summary for a query_code response.
- `extract_name_from_content(content: str)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L220) — Extract name from code content using common declaration patterns.
- `format_summary(results: list[dict[str, Any]], query_type: str, language: str)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L187) — Format query results as a summary grouped by capture name.
- `handle_query_output(formatted: dict[str, Any], arguments: dict[str, Any], file_path: str, language: str, query: str | None, file_output_manager: Any)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L384) — Handle file output and suppress logic for query results.
- `validate_query_arguments(arguments: dict[str, Any])` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L293) — Validate file_path/symbol, query_key/query_string, and format options.

## Module values
- `TOOL_SCHEMA` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L12)
- `_NAME_PATTERNS` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_helpers.py#L211)

