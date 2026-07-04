---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_response`/
symbols:
  format_search_response: format_search_response().
  apply_limits: apply_limits().
  DEFAULT_CONTENT_LISTED_CAP: DEFAULT_CONTENT_LISTED_CAP.
  _format_match_response: _format_match_response().
  _resolve_real_total: _resolve_real_total().
  determine_requested_format: determine_requested_format().
  _parse_limited_matches: _parse_limited_matches().
  _respond_files_with_matches: _respond_files_with_matches().
  logger: logger.
  RECOUNT_BUDGET_MS: RECOUNT_BUDGET_MS.
  ToonApplier: ToonApplier.
  ToonFormatter: ToonFormatter.
  resolve_max_count: resolve_max_count().
  build_rg_args: build_rg_args().
  _parent_dir: _parent_dir().
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_response.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py)

## Functions
- `_format_match_response(matches: list[dict[str, Any]], truncated: bool, elapsed_ms: int, output_format: str, cache_key: str | None, arguments: dict[str, Any], cache: Any, file_output_manager: Any, fd_rg_utils: Any, attach_toon: ToonFormatter, apply_toon: ToonApplier, real_total: int | None = None, total_count_known: bool = True)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L265) — Dispatch parsed matches to grouped, summary, or full response mode.
- `_parent_dir(file_path: str)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L245) — Return the parent directory of a file path (mirrors _prepare_search_roots).
- `_parse_limited_matches(arguments: dict[str, Any], out: bytes, fd_rg_utils: Any)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L252) — Parse rg JSON output and apply match limits/path optimization.
- `_resolve_real_total(*, truncated: bool, displayed_count: int, rg_args: dict[str, Any] | None, roots: list[str] | None, files: list[str] | None, fd_rg_utils: Any)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L171) — Return (real_total, total_count_known) for a search response.
- `_respond_files_with_matches(out: bytes, elapsed_ms: int, cache_key: str | None, arguments: dict[str, Any], cache: Any, output_format: str, apply_toon: ToonApplier)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L327) — Parse rg --files-with-matches plain-text output into a file list.
- `apply_limits(matches: list[dict[str, Any]], arguments: dict[str, Any], fd_rg_utils: Any)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L363) — Truncate matches to user max_count, default cap, or hard cap.
- `build_rg_args(arguments: dict[str, Any], max_count: int | None, no_ignore: bool)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L56) — Build shared ripgrep command keyword arguments.
- `determine_requested_format(arguments: dict[str, Any])` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L35) — Return the requested search response mode.
- `format_search_response(arguments: dict[str, Any], output_format: str, out: bytes, elapsed_ms: int, cache_key: str | None, *, cache: Any, file_output_manager: Any, fd_rg_utils: Any, attach_toon: ToonFormatter, apply_toon: ToonApplier, rg_args: dict[str, Any] | None = None, roots: list[str] | None = None, files: list[str] | None = None)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L101) — Dispatch successful rg output to the requested response mode.
- `resolve_max_count(arguments: dict[str, Any], fd_rg_utils: Any)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L48) — Clamp user-specified max_count to safe bounds.

## Module values
- `DEFAULT_CONTENT_LISTED_CAP` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L29)
- `RECOUNT_BUDGET_MS` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L23)
- `ToonApplier` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L32)
- `ToonFormatter` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L31)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response.py#L18)

