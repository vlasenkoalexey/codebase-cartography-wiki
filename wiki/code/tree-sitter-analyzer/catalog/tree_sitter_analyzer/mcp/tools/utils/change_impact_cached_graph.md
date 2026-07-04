---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.change_impact_cached_graph`/
symbols:
  load_cached_dependency_graph: load_cached_dependency_graph().
  _modules_from_import_text: _modules_from_import_text().
  CachedDependencyGraph.add_edge: CachedDependencyGraph#add_edge().
  _python_import_modules: _python_import_modules().
  _add_cached_import_edges: _add_cached_import_edges().
  _js_ts_import_modules: _js_ts_import_modules().
  CachedDependencyGraph: CachedDependencyGraph#
  _cached_index_rows: _cached_index_rows().
  CachedDependencyGraph.dependencies_of: CachedDependencyGraph#dependencies_of().
  CachedDependencyGraph.dependents_of: CachedDependencyGraph#dependents_of().
  _iter_cached_import_modules: _iter_cached_import_modules().
  CachedDependencyGraph._nodes: CachedDependencyGraph#_nodes.
  CachedDependencyGraph.edges: CachedDependencyGraph#edges().
  CachedDependencyGraph.nodes: CachedDependencyGraph#nodes().
  _java_import_modules: _java_import_modules().
  _rust_import_modules: _rust_import_modules().
  CachedDependencyGraph._edges: CachedDependencyGraph#_edges.
  CachedDependencyGraph.all_nodes: CachedDependencyGraph#all_nodes().
  CachedDependencyGraph.has_node: CachedDependencyGraph#has_node().
  CachedDependencyGraph.node_count: CachedDependencyGraph#node_count().
  CachedDependencyGraph.edge_count: CachedDependencyGraph#edge_count().
  _QUOTED_PATH_RE: _QUOTED_PATH_RE.
  CachedDependencyGraph._deps: CachedDependencyGraph#_deps.
  CachedDependencyGraph._dependents: CachedDependencyGraph#_dependents.
  logger: logger.
  _JS_FROM_RE: _JS_FROM_RE.
  _JS_IMPORT_RE: _JS_IMPORT_RE.
  _JS_REQUIRE_RE: _JS_REQUIRE_RE.
  _JAVA_IMPORT_RE: _JAVA_IMPORT_RE.
  _RUST_USE_RE: _RUST_USE_RE.
  CachedDependencyGraph.__init__: CachedDependencyGraph#__init__().
  CachedDependencyGraph.project_root: CachedDependencyGraph#project_root.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py)

## Classes
### `CachedDependencyGraph`
- def: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py:32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L32)
- doc: Small DependencyGraph-compatible wrapper backed by ASTCache rows.
- signature: `class CachedDependencyGraph:`
- members:
  - `add_edge(self, source: str, target: str)` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L42)
  - `all_nodes(self)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L52) — Return all nodes as frozenset — mirrors DependencyGraph.all_nodes().
  - `dependencies_of(self, file_rel: str)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L71)
  - `dependents_of(self, file_rel: str)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L74)
  - `edge_count(self)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L67) — Return the number of directed edges in the graph.
  - `edges(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L56)
  - `has_node(self, file_rel: str)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L59) — Return True if *file_rel* is a node in the graph (O(1) set lookup).
  - `node_count(self)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L63) — Return the number of nodes in the graph.
  - `nodes(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L49)
  - `project_root` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L36)
- protocol/private: `__init__`[`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L35), `_dependents`[`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L40), `_deps`[`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L39), `_edges`[`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L38), `_nodes`[`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L37)
- used by: [`load_cached_dependency_graph`](change_impact_cached_graph.md#load_cached_dependency_graph), [`_add_cached_import_edges`](change_impact_cached_graph.md#_add_cached_import_edges)  (5 test-only)

## Functions
- `_add_cached_import_edges(graph: CachedDependencyGraph, row: dict[str, Any], nodes: set[str])` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L125)
- `_cached_index_rows(cache: ASTCache)` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L114)
- `_iter_cached_import_modules(row: dict[str, Any])` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L141)
- `_java_import_modules(text: str)` — [`L200`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L200)
- `_js_ts_import_modules(text: str)` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L191)
- `_modules_from_import_text(text: str, language: str, source: str)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L157)
- `_python_import_modules(text: str, language: str, source: str)` — [`L177`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L177)
- `_rust_import_modules(text: str)` — [`L210`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L210)
- `load_cached_dependency_graph(project_root: str | None)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L78) — Return a dependency graph reconstructed from ``.ast-cache/index.db``.

## Module values
- `_JAVA_IMPORT_RE` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L27)
- `_JS_FROM_RE` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L24)
- `_JS_IMPORT_RE` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L25)
- `_JS_REQUIRE_RE` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L26)
- `_QUOTED_PATH_RE` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L28)
- `_RUST_USE_RE` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L29)
- `logger` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_cached_graph.py#L22)

