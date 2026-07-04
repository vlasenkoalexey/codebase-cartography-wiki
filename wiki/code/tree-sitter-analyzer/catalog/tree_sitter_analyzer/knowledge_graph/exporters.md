---
title: 'Module: tree_sitter_analyzer/knowledge_graph/exporters.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/knowledge_graph/exporters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.knowledge_graph.exporters`/
symbols:
  to_graphology: to_graphology().
  aggregate_package_graph: aggregate_package_graph().
  _select: _select().
  summarize: summarize().
  _package_by_file: _package_by_file().
  _positions: _positions().
  _node_size: _node_size().
  _file_from_node_id: _file_from_node_id().
  _LOD_KINDS._LOD_KINDS: _LOD_KINDS._LOD_KINDS.
  _node_color: _node_color().
  _stable_edge_id: _stable_edge_id().
---
# Module: [`tree_sitter_analyzer/knowledge_graph/exporters.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py)

## Functions
- `_file_from_node_id(node_id: str)` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L222)
- `_node_color(kind: str)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L197)
- `_node_size(node: KnowledgeNode)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L186)
- `_package_by_file(nodes: list[KnowledgeNode])` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L208)
- `_positions(nodes: list[KnowledgeNode])` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L170)
- `_select(snapshot: KnowledgeGraphSnapshot, lod: str, focus: str | None, max_nodes: int, max_edges: int)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L136)
- `_stable_edge_id(source: str, target: str, kind: str)` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L230)
- `aggregate_package_graph(snapshot: KnowledgeGraphSnapshot)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L92) — Aggregate file/symbol/doc edges to package-level dependencies.
- `summarize(snapshot: KnowledgeGraphSnapshot)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L80) — Compact summary for TOON/MCP agents.
- `to_graphology(snapshot: KnowledgeGraphSnapshot, *, lod: str = "file", focus: str | None = None, max_nodes: int = 10000, max_edges: int = 50000)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L20) — Return Graphology JSON suitable for Sigma.js/Obsidian-like viewers.

## Module values
- `_LOD_KINDS` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/exporters.py#L12)

