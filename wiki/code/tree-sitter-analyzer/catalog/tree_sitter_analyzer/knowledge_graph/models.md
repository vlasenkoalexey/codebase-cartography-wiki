---
title: 'Module: tree_sitter_analyzer/knowledge_graph/models.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/knowledge_graph/models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.knowledge_graph.models`/Knowledge
symbols:
  KnowledgeNode: Node#
  KnowledgeNode.id: Node#id.
  KnowledgeNode.kind: Node#kind.
  KnowledgeNode.label: Node#label.
  KnowledgeGraphSnapshot: GraphSnapshot#
  KnowledgeNode.file_path: Node#file_path.
  KnowledgeEdge: Edge#
  KnowledgeGraphSnapshot.stats: GraphSnapshot#stats.
  KnowledgeGraphSnapshot.edges: GraphSnapshot#edges.
  KnowledgeGraphSnapshot.nodes: GraphSnapshot#nodes.
  KnowledgeEdge.kind: Edge#kind.
  KnowledgeEdge.to_dict: Edge#to_dict().
  KnowledgeEdge.source: Edge#source.
  KnowledgeEdge.target: Edge#target.
  KnowledgeNode.to_dict: Node#to_dict().
  KnowledgeEdge.id: Edge#id.
  KnowledgeGraphSnapshot.to_dict: GraphSnapshot#to_dict().
  KnowledgeEdge.metadata: Edge#metadata.
  KnowledgeNode.language: Node#language.
  KnowledgeEdge.line: Edge#line.
  KnowledgeNode.metadata: Node#metadata.
  KnowledgeEdge.provenance: Edge#provenance.
---
# Module: [`tree_sitter_analyzer/knowledge_graph/models.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py)

## Classes
### `KnowledgeEdge`
- def: [`tree_sitter_analyzer/knowledge_graph/models.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L32)
- doc: A directed relationship between two knowledge graph nodes.
- signature: `class KnowledgeEdge:`
- members:
  - `to_dict(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L43)
  - `id` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L35)
  - `kind` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L38)
  - `line` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L39)
  - `metadata` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L41)
  - `provenance` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L40)
  - `source` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L36)
  - `target` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L37)
- used by: [`to_graphology`](exporters.md#to_graphology), [`write`](stores.md#LadybugKnowledgeGraphStore.write), [`build`](builder.md#KnowledgeGraphBuilder.build), [`aggregate_package_graph`](exporters.md#aggregate_package_graph), [`_add_markdown_links`](builder.md#KnowledgeGraphBuilder._add_markdown_links), [`_add_file_and_symbols`](builder.md#KnowledgeGraphBuilder._add_file_and_symbols), [`_select`](exporters.md#_select), [`_snapshot_from_payload`](../mcp/tools/knowledge_graph_tool.md#_snapshot_from_payload), [`_add_edge`](builder.md#KnowledgeGraphBuilder._add_edge), [`edges`](models.md#KnowledgeGraphSnapshot.edges), [`_add_existing_edge`](builder.md#KnowledgeGraphBuilder._add_existing_edge), [`to_dict`](models.md#KnowledgeGraphSnapshot.to_dict)  (8 test-only)

### `KnowledgeGraphSnapshot`
- def: [`tree_sitter_analyzer/knowledge_graph/models.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L56)
- doc: A materialized graph projection ready for JSON/Ladybug/Sigma export.
- signature: `class KnowledgeGraphSnapshot:`
- members:
  - `to_dict(self)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L63)
  - `edges` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L60)
  - `nodes` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L59)
  - `stats` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L61)
- uses (calls/refs, reference-scoped): [`KnowledgeNode`](models.md#KnowledgeNode), [`KnowledgeEdge`](models.md#KnowledgeEdge), [`to_dict`](models.md#KnowledgeEdge.to_dict), [`to_dict`](models.md#KnowledgeNode.to_dict)
- used by: [`to_graphology`](exporters.md#to_graphology), [`write`](stores.md#LadybugKnowledgeGraphStore.write), [`build`](builder.md#KnowledgeGraphBuilder.build), [`aggregate_package_graph`](exporters.md#aggregate_package_graph), [`_select`](exporters.md#_select), [`_snapshot_from_payload`](../mcp/tools/knowledge_graph_tool.md#_snapshot_from_payload), [`write`](stores.md#JsonKnowledgeGraphStore.write), [`summarize`](exporters.md#summarize)  (14 test-only)

### `KnowledgeNode`
- def: [`tree_sitter_analyzer/knowledge_graph/models.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L10)
- doc: A code, file, package, or markdown node in the knowledge graph.
- signature: `class KnowledgeNode:`
- members:
  - `to_dict(self)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L20)
  - `file_path` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L16)
  - `id` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L13)
  - `kind` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L14)
  - `label` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L15)
  - `language` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L17)
  - `metadata` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/models.py#L18)
- used by: [`to_graphology`](exporters.md#to_graphology), [`write`](stores.md#LadybugKnowledgeGraphStore.write), [`build`](builder.md#KnowledgeGraphBuilder.build), [`aggregate_package_graph`](exporters.md#aggregate_package_graph), [`_add_markdown_links`](builder.md#KnowledgeGraphBuilder._add_markdown_links), [`_add_file_and_symbols`](builder.md#KnowledgeGraphBuilder._add_file_and_symbols), [`_select`](exporters.md#_select), [`_snapshot_from_payload`](../mcp/tools/knowledge_graph_tool.md#_snapshot_from_payload), [`_add_placeholder_node`](builder.md#KnowledgeGraphBuilder._add_placeholder_node), [`nodes`](models.md#KnowledgeGraphSnapshot.nodes), [`_add_existing_edge`](builder.md#KnowledgeGraphBuilder._add_existing_edge), [`to_dict`](models.md#KnowledgeGraphSnapshot.to_dict), [`_package_by_file`](exporters.md#_package_by_file), [`_upsert_node`](builder.md#KnowledgeGraphBuilder._upsert_node), [`_node_size`](exporters.md#_node_size), [`_positions`](exporters.md#_positions)  (12 test-only)

