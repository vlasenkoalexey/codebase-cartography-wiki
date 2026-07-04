---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_visualization_hub`/
symbols:
  safe_node_id: safe_node_id().
  query_flow_uml_facet: query_flow_uml_facet().
  CodeGraphVisualizationHub.call_graph: CodeGraphVisualizationHub#call_graph().
  render_call_flowchart: render_call_flowchart().
  _dedupe_uml_edges: _dedupe_uml_edges().
  CodeGraphVisualizationHub.cache: CodeGraphVisualizationHub#cache().
  CodeGraphVisualizationHub.uml_exporter: CodeGraphVisualizationHub#uml_exporter().
  short_label: short_label().
  CodeGraphVisualizationHub._call_graph: CodeGraphVisualizationHub#_call_graph.
  CodeGraphVisualizationHub.reset: CodeGraphVisualizationHub#reset().
  CodeGraphVisualizationHub.project_root: CodeGraphVisualizationHub#project_root.
  _query_symbol_key: _query_symbol_key().
  _query_display_name: _query_display_name().
  CodeGraphVisualizationHub: CodeGraphVisualizationHub#
  CodeGraphVisualizationHub._cache: CodeGraphVisualizationHub#_cache.
  CodeGraphVisualizationHub.__init__: CodeGraphVisualizationHub#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py)

## Classes
### `CodeGraphVisualizationHub`
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L154)
- doc: Shared cache/bootstrap layer for visualization-oriented MCP wrappers.
- signature: `class CodeGraphVisualizationHub:`
- members:
  - `cache(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L167)
  - `call_graph(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L174)
  - `reset(self, project_root: str | None)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L162)
  - `uml_exporter(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L188)
  - `project_root` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L158)
- protocol/private: `__init__`[`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L157), `_cache`[`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L160), `_call_graph`[`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L159)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`UMLExporter`](../../uml_export.md#UMLExporter), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`ensure_indexed`](../utils/auto_index_guard.md#ensure_indexed)
- used by: [`execute`](uml_tool.md#CodeGraphUMLTool.execute), [`_get_call_graph`](codegraph_visualize_tool.md#CodeGraphVisualizeTool._get_call_graph), [`__init__`](codegraph_visualize_tool.md#CodeGraphVisualizeTool.__init__), [`_on_project_root_changed`](codegraph_visualize_tool.md#CodeGraphVisualizeTool._on_project_root_changed)  (1 test-only)

## Functions
- `_dedupe_uml_edges(edges: list[UMLEdge])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L144)
- `_query_display_name(symbol: dict[str, Any] | None, fallback: str)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L134)
- `_query_symbol_key(symbol: dict[str, Any])` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L130)
- `query_flow_uml_facet(*, symbols: list[dict[str, Any]], current: list[dict[str, Any]], relationships: dict[str, dict[str, list[dict[str, Any]]]], direction: str, max_edges: int)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L65) — Build the codegraph_query ``uml`` facet from chain state primitives.
- `render_call_flowchart(edges: list[tuple[str, str, str, str]], direction: str = "TD")` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L27) — Render call-graph edge tuples as a Mermaid flowchart.
- `safe_node_id(name: str, file_path: str)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L14) — Build a Mermaid-safe node id for call-graph visualization nodes.
- `short_label(name: str, file_path: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.py#L20) — Build a compact label that preserves both file and function context.

