---
title: 'Module: tree_sitter_analyzer/mcp/tools/symbol_body_inline.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/symbol_body_inline.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.symbol_body_inline`/
symbols:
  inline_neighbor_bodies: inline_neighbor_bodies().
  inline_search_summaries: inline_search_summaries().
  inline_symbol_body: inline_symbol_body().
  _body_for_record: _body_for_record().
  _record_span: _record_span().
  MAX_DEFINITION_LINES: MAX_DEFINITION_LINES.
  MAX_NEIGHBOR_LINES: MAX_NEIGHBOR_LINES.
  MAX_SUMMARY_LINES: MAX_SUMMARY_LINES.
  MAX_NEIGHBOR_BODIES: MAX_NEIGHBOR_BODIES.
  NEIGHBORS_DETERRENT: NEIGHBORS_DETERRENT.
  MAX_SUMMARY_BODIES: MAX_SUMMARY_BODIES.
  MAX_TOTAL_DEFINITION_LINES: MAX_TOTAL_DEFINITION_LINES.
  MAX_TOTAL_NEIGHBOR_LINES: MAX_TOTAL_NEIGHBOR_LINES.
  MAX_TOTAL_SUMMARY_LINES: MAX_TOTAL_SUMMARY_LINES.
  NAVIGATE_DETERRENT: NAVIGATE_DETERRENT.
  SEARCH_DETERRENT: SEARCH_DETERRENT.
---
# Module: [`tree_sitter_analyzer/mcp/tools/symbol_body_inline.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py)

## Functions
- `_body_for_record(project_root: str, cache: Any, record: dict[str, Any], per_body_cap: int, budget: list[int])` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L113) — Read one verbatim body for ``record`` honouring per-body + total caps.
- `_record_span(record: dict[str, Any], cache: Any)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L61) — Return a ``{name,file,line,end_line,class}`` def-span for ``record``.
- `inline_neighbor_bodies(project_root: str, cache: Any, neighbors: list[dict[str, Any]])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L147) — Attach a body (neighbour tier) to the top-N caller/callee records.
- `inline_search_summaries(project_root: str, cache: Any, results: list[dict[str, Any]])` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L175) — Attach a short body summary (summary tier) to the top search matches.
- `inline_symbol_body(project_root: str, cache: Any, record: dict[str, Any])` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L132) — Inline a single definition body (full tier) for ``nav navigate``.

## Module values
- `MAX_DEFINITION_LINES` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L39)
- `MAX_NEIGHBOR_BODIES` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L46)
- `MAX_NEIGHBOR_LINES` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L41)
- `MAX_SUMMARY_BODIES` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L48)
- `MAX_SUMMARY_LINES` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L43)
- `MAX_TOTAL_DEFINITION_LINES` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L51)
- `MAX_TOTAL_NEIGHBOR_LINES` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L52)
- `MAX_TOTAL_SUMMARY_LINES` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L53)
- `NAVIGATE_DETERRENT` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L204)
- `NEIGHBORS_DETERRENT` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L208)
- `SEARCH_DETERRENT` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_body_inline.py#L213)

