---
title: 'Module: tree_sitter_analyzer/knowledge_graph/stores.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/knowledge_graph/stores.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.knowledge_graph.stores`/
symbols:
  LadybugKnowledgeGraphStore.write: LadybugKnowledgeGraphStore#write().
  JsonKnowledgeGraphStore.write: JsonKnowledgeGraphStore#write().
  JsonKnowledgeGraphStore.path: JsonKnowledgeGraphStore#path.
  JsonKnowledgeGraphStore: JsonKnowledgeGraphStore#
  JsonKnowledgeGraphStore.status: JsonKnowledgeGraphStore#status().
  LadybugKnowledgeGraphStore.status: LadybugKnowledgeGraphStore#status().
  LadybugKnowledgeGraphStore: LadybugKnowledgeGraphStore#
  LadybugUnavailableError: LadybugUnavailableError#
  LadybugKnowledgeGraphStore.path: LadybugKnowledgeGraphStore#path.
  JsonKnowledgeGraphStore.read: JsonKnowledgeGraphStore#read().
  JsonKnowledgeGraphStore.exists: JsonKnowledgeGraphStore#exists().
  LadybugKnowledgeGraphStore._import_ladybug: LadybugKnowledgeGraphStore#_import_ladybug().
  LadybugKnowledgeGraphStore.__init__: LadybugKnowledgeGraphStore#__init__().
  LadybugKnowledgeGraphStore.available: LadybugKnowledgeGraphStore#available().
  JsonKnowledgeGraphStore.project_root: JsonKnowledgeGraphStore#project_root.
  LadybugKnowledgeGraphStore.project_root: LadybugKnowledgeGraphStore#project_root.
  LadybugKnowledgeGraphStore._create_schema: LadybugKnowledgeGraphStore#_create_schema().
  LadybugKnowledgeGraphStore._clear: LadybugKnowledgeGraphStore#_clear().
  JsonKnowledgeGraphStore.__init__: JsonKnowledgeGraphStore#__init__().
---
# Module: [`tree_sitter_analyzer/knowledge_graph/stores.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py)

## Classes
### `JsonKnowledgeGraphStore`
- def: [`tree_sitter_analyzer/knowledge_graph/stores.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L15)
- doc: Small JSON sidecar used by CLI/MCP and browser exports.
- signature: `class JsonKnowledgeGraphStore:`
- members:
  - `exists(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L39)
  - `read(self)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L35)
  - `status(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L42)
  - `write(self, snapshot: KnowledgeGraphSnapshot)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L26)
  - `path` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L20)
  - `project_root` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L19)
- protocol/private: `__init__`[`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L18)
- uses (calls/refs, reference-scoped): [`KnowledgeGraphSnapshot`](models.md#KnowledgeGraphSnapshot), [`to_dict`](models.md#KnowledgeGraphSnapshot.to_dict)
- used by: [`execute`](../mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool.execute), [`execute`](../mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeGraphTool.execute)  (4 test-only)

### `LadybugKnowledgeGraphStore`
- def: [`tree_sitter_analyzer/knowledge_graph/stores.py:58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L58)
- doc: Optional LadybugDB mirror for fast Cypher graph traversals.
- signature: `class LadybugKnowledgeGraphStore:`
- members:
  - `available()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L70)
  - `status(self)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L115)
  - `write(self, snapshot: KnowledgeGraphSnapshot)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L73)
  - `path` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L63)
  - `project_root` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L62)
- protocol/private: `__init__`[`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L61), `_clear`[`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L152), `_create_schema`[`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L139), `_import_ladybug`[`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L129)
- uses (calls/refs, reference-scoped): [`id`](models.md#KnowledgeNode.id), [`kind`](models.md#KnowledgeNode.kind), [`label`](models.md#KnowledgeNode.label), [`KnowledgeGraphSnapshot`](models.md#KnowledgeGraphSnapshot), [`file_path`](models.md#KnowledgeNode.file_path), [`edges`](models.md#KnowledgeGraphSnapshot.edges), [`nodes`](models.md#KnowledgeGraphSnapshot.nodes), [`kind`](models.md#KnowledgeEdge.kind), [`source`](models.md#KnowledgeEdge.source), [`target`](models.md#KnowledgeEdge.target), [`id`](models.md#KnowledgeEdge.id), [`metadata`](models.md#KnowledgeEdge.metadata), [`language`](models.md#KnowledgeNode.language), [`line`](models.md#KnowledgeEdge.line), [`LadybugUnavailableError`](stores.md#LadybugUnavailableError), [`metadata`](models.md#KnowledgeNode.metadata), [`provenance`](models.md#KnowledgeEdge.provenance)
- used by: [`execute`](../mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool.execute)  (2 test-only)

### `LadybugUnavailableError`  ·  implements/extends RuntimeError
- def: [`tree_sitter_analyzer/knowledge_graph/stores.py:54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/stores.py#L54)
- doc: Raised when the optional Ladybug package is not installed.
- signature: `class LadybugUnavailableError(RuntimeError):`
- used by: [`execute`](../mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool.execute), [`_import_ladybug`](stores.md#LadybugKnowledgeGraphStore._import_ladybug)  (2 test-only)

