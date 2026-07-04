---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._pagerank`/
symbols:
  compute_pagerank: compute_pagerank().
  collect_critical_nodes: collect_critical_nodes().
  _pagerank_iterate: _pagerank_iterate().
  _pagerank_top_n_rows: _pagerank_top_n_rows().
  logger: logger.
  _pagerank_build_graph: _pagerank_build_graph().
  _pagerank_step: _pagerank_step().
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py)

## Functions
- `_pagerank_build_graph(edges: list[tuple[str, str]])` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L51) — Build the adjacency lists used by ``compute_pagerank``.
- `_pagerank_iterate(out_edges: dict[str, set[str]], node_list: list[str], alpha: float, max_iter: int)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L72) — Run power iteration until convergence (or ``max_iter``).
- `_pagerank_step(scores: dict[str, float], node_list: list[str], out_edges: dict[str, Any], dangling: set[str], alpha: float, n: int)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L96) — Run one power-iteration step of PageRank.
- `_pagerank_top_n_rows(scores: dict[str, float], inbound: dict[str, int], top_n: int)` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L126) — Filter stdlib blocklist + take ``top_n`` highest-score rows.
- `collect_critical_nodes(all_files: list[str], extract_edges_fn: Any)` — [`L162`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L162) — Run PageRank over the call graph; skip test paths.
- `compute_pagerank(edges: list[tuple[str, str]], top_n: int = 10, alpha: float = 0.85, max_iter: int = 100)` — [`L19`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L19) — Compute PageRank on the call graph and return top_n nodes.

## Module values
- `logger` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_pagerank.py#L16)

