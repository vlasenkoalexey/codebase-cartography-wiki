---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_response_modes.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_response_modes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_response_modes`/
symbols:
  respond_full: respond_full().
  respond_grouped: respond_grouped().
  respond_summary: respond_summary().
  respond_count_only: respond_count_only().
  respond_total_only: respond_total_only().
  _resolved_case_sensitive: _resolved_case_sensitive().
  ToonFormatter: ToonFormatter.
  create_count_only_cache_key: create_count_only_cache_key().
  _attach_total_count_metadata: _attach_total_count_metadata().
  ToonApplier: ToonApplier.
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_response_modes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py)

## Functions
- `_attach_total_count_metadata(result: dict[str, Any], *, displayed_count: int, real_total: int | None, total_count_known: bool, truncated: bool)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L318) — Attach H2 fix metadata for total_count under truncation.
- `_resolved_case_sensitive(arguments: dict[str, Any])` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L21) — Echo the actually-honored case mode as a strict bool (N1).
- `create_count_only_cache_key(cache: Any, arguments: dict[str, Any])` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L36) — Create a count_only_matches cache key from a total_only query.
- `respond_count_only(out: bytes, elapsed_ms: int, output_format: str, cache_key: str | None, arguments: dict[str, Any], cache: Any, fd_rg_utils: Any, attach_toon: ToonFormatter)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L88) — Return per-file match counts.
- `respond_full(matches: list[dict[str, Any]], truncated: bool, elapsed_ms: int, output_format: str, cache_key: str | None, arguments: dict[str, Any], cache: Any, file_output_manager: Any, fd_rg_utils: Any, apply_toon: ToonApplier, real_total: int | None = None, total_count_known: bool = True)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L241) — Return full match details with optional next steps.
- `respond_grouped(matches: list[dict[str, Any]], truncated: bool, elapsed_ms: int, output_format: str, cache_key: str | None, arguments: dict[str, Any], cache: Any, file_output_manager: Any, fd_rg_utils: Any, attach_toon: ToonFormatter, real_total: int | None = None, total_count_known: bool = True)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L132) — Return matches organized by file.
- `respond_summary(matches: list[dict[str, Any]], truncated: bool, elapsed_ms: int, output_format: str, cache_key: str | None, arguments: dict[str, Any], cache: Any, file_output_manager: Any, fd_rg_utils: Any, attach_toon: ToonFormatter, real_total: int | None = None, total_count_known: bool = True)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L184) — Return aggregated search statistics.
- `respond_total_only(out: bytes, elapsed_ms: int, cache_key: str | None, arguments: dict[str, Any], cache: Any, fd_rg_utils: Any)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L54) — Return only the total match count.

## Module values
- `ToonApplier` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L33)
- `ToonFormatter` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_response_modes.py#L32)

