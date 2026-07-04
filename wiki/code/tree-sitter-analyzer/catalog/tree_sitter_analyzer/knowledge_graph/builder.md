---
title: 'Module: tree_sitter_analyzer/knowledge_graph/builder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/knowledge_graph/builder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.knowledge_graph.builder`/
symbols:
  KnowledgeGraphBuilder.build: KnowledgeGraphBuilder#build().
  KnowledgeGraphBuilder._add_markdown_links: KnowledgeGraphBuilder#_add_markdown_links().
  KnowledgeGraphBuilder._add_file_and_symbols: KnowledgeGraphBuilder#_add_file_and_symbols().
  KnowledgeGraphBuilder._add_placeholder_node: KnowledgeGraphBuilder#_add_placeholder_node().
  KnowledgeGraphBuilder._add_edge: KnowledgeGraphBuilder#_add_edge().
  KnowledgeGraphBuilder._add_existing_edge: KnowledgeGraphBuilder#_add_existing_edge().
  KnowledgeGraphBuilder._upsert_node: KnowledgeGraphBuilder#_upsert_node().
  KnowledgeGraphBuilder: KnowledgeGraphBuilder#
  _iter_markdown_files: _iter_markdown_files().
  KnowledgeGraphBuilder.project_root: KnowledgeGraphBuilder#project_root.
  _nullable_int: _nullable_int().
  _as_int: _as_int().
  _json_obj: _json_obj().
  _resolve_project_ref: _resolve_project_ref().
  KnowledgeGraphBuilder._package_node_id: KnowledgeGraphBuilder#_package_node_id().
  _DEFAULT_DOC_PATTERNS: _DEFAULT_DOC_PATTERNS.
  _SKIP_DIRS: _SKIP_DIRS.
  _edge_id: _edge_id().
  KnowledgeGraphBuilder.__init__: KnowledgeGraphBuilder#__init__().
---
# Module: [`tree_sitter_analyzer/knowledge_graph/builder.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py)

## Classes
### `KnowledgeGraphBuilder`
- def: [`tree_sitter_analyzer/knowledge_graph/builder.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L22)
- doc: Project graph builder backed by the existing AST cache and edge store.
- signature: `class KnowledgeGraphBuilder:`
- members:
  - `build(self, *, include_docs: bool = True, doc_patterns: list[str] | None = None, max_nodes: int = 100000, max_edges: int = 500000)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L28) — Build a capped whole-project graph projection from persisted indexes. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `project_root` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L26)
- protocol/private: `__init__`[`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L25), `_add_edge`[`L272`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L272), `_add_existing_edge`[`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L163), `_add_file_and_symbols`[`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L94), `_add_markdown_links`[`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L188), `_add_placeholder_node`[`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L243), `_package_node_id`[`L297`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L297), `_upsert_node`[`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L265)
- uses (calls/refs, reference-scoped): [`ASTCache`](../ast_cache.md#ASTCache), [`close`](../ast_cache.md#ASTCache.close), [`get_conn`](../ast_cache.md#ASTCache.get_conn), [`symbol_node`](../graph/edge_store.md#symbol_node), [`KnowledgeNode`](models.md#KnowledgeNode), [`id`](models.md#KnowledgeNode.id), [`extract_file_refs`](../doc_sync.md#extract_file_refs), [`kind`](models.md#KnowledgeNode.kind), [`parse_node_id`](../graph/edge_store.md#parse_node_id), [`label`](models.md#KnowledgeNode.label), [`KnowledgeGraphSnapshot`](models.md#KnowledgeGraphSnapshot), [`name`](../graph/edge_store.md#NodeRef.name), [`file_path`](models.md#KnowledgeNode.file_path), [`KnowledgeEdge`](models.md#KnowledgeEdge), [`stats`](models.md#KnowledgeGraphSnapshot.stats), [`edges`](models.md#KnowledgeGraphSnapshot.edges), [`nodes`](models.md#KnowledgeGraphSnapshot.nodes), [`file_path`](../graph/edge_store.md#NodeRef.file_path), [`kind`](models.md#KnowledgeEdge.kind), [`source`](models.md#KnowledgeEdge.source), [`target`](models.md#KnowledgeEdge.target), [`id`](models.md#KnowledgeEdge.id), [`line`](../graph/edge_store.md#NodeRef.line), [`path`](../doc_sync.md#DocRef.path), [`file_node`](../graph/edge_store.md#file_node), [`metadata`](models.md#KnowledgeEdge.metadata), [`_iter_markdown_files`](builder.md#_iter_markdown_files), [`language`](models.md#KnowledgeNode.language), [`line`](models.md#KnowledgeEdge.line), [`line`](../doc_sync.md#DocRef.line), [`metadata`](models.md#KnowledgeNode.metadata), [`provenance`](models.md#KnowledgeEdge.provenance), [`_nullable_int`](builder.md#_nullable_int), [`_as_int`](builder.md#_as_int), [`_json_obj`](builder.md#_json_obj), [`_resolve_project_ref`](builder.md#_resolve_project_ref), [`_DEFAULT_DOC_PATTERNS`](builder.md#_DEFAULT_DOC_PATTERNS), [`_edge_id`](builder.md#_edge_id)
- used by: [`execute`](../mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool.execute)  (4 test-only)

## Functions
- `_as_int(value: Any, default: int)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L328)
- `_edge_id(source: str, target: str, kind: str, line: int | None)` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L304)
- `_iter_markdown_files(project_root: str, patterns: list[str])` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L333)
- `_json_obj(raw: str | None)` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L309)
- `_nullable_int(value: Any)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L319)
- `_resolve_project_ref(path: str, doc_file: str, project_root: str)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L346)

## Module values
- `_DEFAULT_DOC_PATTERNS` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L18)
- `_SKIP_DIRS` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/knowledge_graph/builder.py#L19)

