---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_visualize_tool`/
symbols:
  CodeGraphVisualizeTool.execute: CodeGraphVisualizeTool#execute().
  CodeGraphVisualizeTool: CodeGraphVisualizeTool#
  CodeGraphVisualizeTool._edges_function: CodeGraphVisualizeTool#_edges_function().
  CodeGraphVisualizeTool._edges_file: CodeGraphVisualizeTool#_edges_file().
  CodeGraphVisualizeTool._edges_full: CodeGraphVisualizeTool#_edges_full().
  CodeGraphVisualizeTool.validate_arguments: CodeGraphVisualizeTool#validate_arguments().
  _sigma_node_attributes: _sigma_node_attributes().
  CodeGraphVisualizeTool._get_call_graph: CodeGraphVisualizeTool#_get_call_graph().
  _mermaid_edge: _mermaid_edge().
  _build_sigma_graph: _build_sigma_graph().
  CodeGraphVisualizeTool.get_call_graph: CodeGraphVisualizeTool#get_call_graph().
  CodeGraphVisualizeTool.get_tool_schema: CodeGraphVisualizeTool#get_tool_schema().
  CodeGraphVisualizeTool.__init__: CodeGraphVisualizeTool#__init__().
  CodeGraphVisualizeTool._on_project_root_changed: CodeGraphVisualizeTool#_on_project_root_changed().
  CodeGraphVisualizeTool.get_tool_definition: CodeGraphVisualizeTool#get_tool_definition().
  _VISUALIZATION_FORMATS: _VISUALIZATION_FORMATS.
  logger: logger.
  _MAX_EDGES_DEFAULT: _MAX_EDGES_DEFAULT.
  _MAX_DEPTH_DEFAULT: _MAX_DEPTH_DEFAULT.
  CodeGraphVisualizeTool._visualization_hub: CodeGraphVisualizeTool#_visualization_hub.
  _package_from_path: _package_from_path().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py)

## Classes
### `CodeGraphVisualizeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L48)
- doc: MCP Tool for Mermaid call graph visualization (CodeGraph parity).
- signature: `class CodeGraphVisualizeTool(BaseMCPTool):`
- members:
  - `_edges_file(self, cg: CallGraph, file_path: str | None, max_edges: int)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L258) — Return (edges, truncated) for mode=file.
  - `_edges_full(self, cg: CallGraph, max_edges: int)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L231) — Return (edges, truncated) for mode=full.
  - `_edges_function(self, cg: CallGraph, function: str | None, file_path: str | None, depth: int, max_edges: int)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L287) — Return (edges, truncated) for mode=function.
  - `execute(self, arguments: dict[str, Any])` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L163)
  - `get_call_graph(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L61) — Public alias for _get_call_graph() — use this instead of patching _get_call_graph.
  - `get_tool_definition(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L65)
  - `get_tool_schema(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L85)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L143)
- protocol/private: `__init__`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L51), `_get_call_graph`[`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L58), `_on_project_root_changed`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L55), `_visualization_hub`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L52)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`FunctionRef`](../../call_graph.md#FunctionRef), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`build_error`](_response_builder.md#build_error), [`caller_refs_of`](../../call_graph.md#CallGraph.caller_refs_of), [`qualified_name`](../../call_graph.md#FunctionRef.qualified_name), [`callee_refs_of`](../../call_graph.md#CallGraph.callee_refs_of), [`resolve_targets`](../../call_graph.md#CallGraph.resolve_targets), [`safe_node_id`](codegraph_visualization_hub.md#safe_node_id), [`function_refs`](../../call_graph.md#CallGraph.function_refs), [`call_graph`](codegraph_visualization_hub.md#CodeGraphVisualizationHub.call_graph), [`render_call_flowchart`](codegraph_visualization_hub.md#render_call_flowchart), [`_build_sigma_graph`](codegraph_visualize_tool.md#_build_sigma_graph), [`_mermaid_edge`](codegraph_visualize_tool.md#_mermaid_edge), [`function_refs_in_file`](../../call_graph.md#CallGraph.function_refs_in_file), [`reset`](codegraph_visualization_hub.md#CodeGraphVisualizationHub.reset), [`CodeGraphVisualizationHub`](codegraph_visualization_hub.md#CodeGraphVisualizationHub), [`_VISUALIZATION_FORMATS`](codegraph_visualize_tool.md#_VISUALIZATION_FORMATS), [`_MAX_DEPTH_DEFAULT`](codegraph_visualize_tool.md#_MAX_DEPTH_DEFAULT), [`_MAX_EDGES_DEFAULT`](codegraph_visualize_tool.md#_MAX_EDGES_DEFAULT)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_viz_facade`](viz_facade.md#build_viz_facade)  (21 test-only)

## Functions
- `_build_sigma_graph(edges: list[tuple[FunctionRef, FunctionRef]])` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L354) — Build a Graphology-compatible graph payload for Sigma.js clients.
- `_mermaid_edge(edge: tuple[FunctionRef, FunctionRef])` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L344)
- `_package_from_path(file_path: str)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L431)
- `_sigma_node_attributes(ref: FunctionRef)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L412)

## Module values
- `_MAX_DEPTH_DEFAULT` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L44)
- `_MAX_EDGES_DEFAULT` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L43)
- `_VISUALIZATION_FORMATS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L45)
- `logger` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.py#L41)

