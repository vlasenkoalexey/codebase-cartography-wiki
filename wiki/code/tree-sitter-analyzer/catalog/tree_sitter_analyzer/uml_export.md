---
title: 'Module: tree_sitter_analyzer/uml_export.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/uml_export.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.uml_export`/
symbols:
  UMLExporter: UMLExporter#
  UMLExporter.activity_diagram: UMLExporter#activity_diagram().
  UMLExporter.state_diagram: UMLExporter#state_diagram().
  UMLDiagram.metadata: UMLDiagram#metadata.
  UMLExporter.class_diagram: UMLExporter#class_diagram().
  UMLEdge: UMLEdge#
  UMLExporter.package_diagram: UMLExporter#package_diagram().
  UMLExporter.component_diagram: UMLExporter#component_diagram().
  UMLExporter.sequence_diagram: UMLExporter#sequence_diagram().
  UMLDiagram.mermaid: UMLDiagram#mermaid.
  UMLDiagram.nodes: UMLDiagram#nodes.
  UMLDiagram: UMLDiagram#
  UMLDiagram.edges: UMLDiagram#edges.
  render_flowchart_mermaid: render_flowchart_mermaid().
  _safe_id: _safe_id().
  UMLDiagram.diagram_type: UMLDiagram#diagram_type.
  render_state_mermaid: render_state_mermaid().
  UMLEdge.source: UMLEdge#source.
  UMLEdge.target: UMLEdge#target.
  UMLDiagram.mermaid_type: UMLDiagram#mermaid_type.
  UMLDiagram.to_dict: UMLDiagram#to_dict().
  render_class_mermaid: render_class_mermaid().
  UMLExporter._activity_not_found_no_file: UMLExporter#_activity_not_found_no_file().
  _clamp_edges: _clamp_edges().
  UMLDiagram.truncated: UMLDiagram#truncated.
  _dedupe_edges_by_signature: _dedupe_edges_by_signature().
  UMLEdge.label: UMLEdge#label.
  UMLEdge.to_dict: UMLEdge#to_dict().
  render_sequence_mermaid: render_sequence_mermaid().
  _escape_label: _escape_label().
  _file_matches: _file_matches().
  UMLExporter._open_cache: UMLExporter#_open_cache().
  UMLEdge.weight: UMLEdge#weight.
  UMLExporter.project_root: UMLExporter#project_root.
  _ACTIVITY_NOT_FOUND_MERMAID: _ACTIVITY_NOT_FOUND_MERMAID.
  _is_neighbourhood: _is_neighbourhood().
  _package_name: _package_name().
  _component_name: _component_name().
  UMLExporter._resolve_function_file: UMLExporter#_resolve_function_file().
  _TRUNCATION_NOTE: _TRUNCATION_NOTE.
  UMLExporter._cache: UMLExporter#_cache.
  UMLExporter._last_activity_index_hits: UMLExporter#_last_activity_index_hits.
  _EXTERNAL_BASES: _EXTERNAL_BASES.
  UMLExporter.__init__: UMLExporter#__init__().
---
# Module: [`tree_sitter_analyzer/uml_export.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py)

## Classes
### `UMLDiagram`
- def: [`tree_sitter_analyzer/uml_export.py:65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L65) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- signature: `class UMLDiagram:`
- members:
  - `to_dict(self)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L74) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `diagram_type` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L66) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `edges` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L70) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `mermaid` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L68) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `mermaid_type` — [`L67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L67) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `metadata` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L72) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `nodes` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L69) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `truncated` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L71) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- uses (calls/refs, reference-scoped): [`UMLEdge`](uml_export.md#UMLEdge), [`to_dict`](uml_export.md#UMLEdge.to_dict)
- used by: [`activity_diagram`](uml_export.md#UMLExporter.activity_diagram), [`state_diagram`](uml_export.md#UMLExporter.state_diagram), [`class_diagram`](uml_export.md#UMLExporter.class_diagram), [`execute`](mcp/tools/uml_tool.md#CodeGraphUMLTool.execute), [`component_diagram`](uml_export.md#UMLExporter.component_diagram), [`package_diagram`](uml_export.md#UMLExporter.package_diagram), [`sequence_diagram`](uml_export.md#UMLExporter.sequence_diagram), [`_activity_not_found_no_file`](uml_export.md#UMLExporter._activity_not_found_no_file)  (76 test-only)

### `UMLEdge`
- def: [`tree_sitter_analyzer/uml_export.py:47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L47) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- signature: `class UMLEdge:`
- members:
  - `to_dict(self)` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L53)
  - `label` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L50)
  - `source` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L48)
  - `target` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L49)
  - `weight` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L51)
- used by: [`activity_diagram`](uml_export.md#UMLExporter.activity_diagram), [`state_diagram`](uml_export.md#UMLExporter.state_diagram), [`class_diagram`](uml_export.md#UMLExporter.class_diagram), [`component_diagram`](uml_export.md#UMLExporter.component_diagram), [`package_diagram`](uml_export.md#UMLExporter.package_diagram), [`sequence_diagram`](uml_export.md#UMLExporter.sequence_diagram), [`edges`](uml_export.md#UMLDiagram.edges), [`render_flowchart_mermaid`](uml_export.md#render_flowchart_mermaid), [`to_dict`](uml_export.md#UMLDiagram.to_dict), [`render_class_mermaid`](uml_export.md#render_class_mermaid), [`query_flow_uml_facet`](mcp/tools/codegraph_visualization_hub.md#query_flow_uml_facet), [`_clamp_edges`](uml_export.md#_clamp_edges), [`_dedupe_edges_by_signature`](uml_export.md#_dedupe_edges_by_signature), [`_dedupe_uml_edges`](mcp/tools/codegraph_visualization_hub.md#_dedupe_uml_edges)  (27 test-only)

### `UMLExporter`
- def: [`tree_sitter_analyzer/uml_export.py:320`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L320) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- doc: Build Mermaid UML-style diagrams from existing CodeGraph indexes.
- signature: `class UMLExporter:`
- members:
  - `_activity_not_found_no_file(self, function_name: str)` — [`L373`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L373) — Return a descriptive NOT_FOUND when index lookup for *function_name* fails. — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `_resolve_function_file(self, function_name: str)` — [`L334`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L334) — Look up *function_name* in the AST index and return a unique file path.
  - `activity_diagram(self, function_name: str, file_path: str | None = None, max_nodes: int = 50)` — [`L647`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L647) — Build a structural control-flow graph for *function_name*. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `class_diagram(self, max_edges: int = 80, include_external_bases: bool = True, *, file_path: str | None = None, class_name: str | None = None, include_tests: bool = False)` — [`L409`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L409) — Build a class inheritance diagram. — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `component_diagram(self, max_edges: int = 120)` — [`L559`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L559) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `package_diagram(self, max_edges: int = 200, package_depth: int = 2)` — [`L528`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L528) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `sequence_diagram(self, source: str, target: str, max_depth: int = 8, max_paths: int = 3, max_hops: int = 12)` — [`L588`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L588) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `state_diagram(self, *, class_name: str | None = None, file_path: str | None = None, max_nodes: int = 50)` — [`L805`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L805) — Build a stateDiagram-v2 from an enum/match-driven FSM (P2-B, RFC-0015). — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `project_root` — [`L324`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L324)
- protocol/private: `__init__`[`L323`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L323), `_cache`[`L325`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L325), `_last_activity_index_hits`[`L366`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L366), `_open_cache`[`L327`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L327)
- uses (calls/refs, reference-scoped): [`ASTCache`](ast_cache.md#ASTCache), [`build_activity_cfg`](uml_activity.md#build_activity_cfg), [`build_state_result`](uml_state.md#build_state_result), [`metadata`](uml_export.md#UMLDiagram.metadata), [`UMLEdge`](uml_export.md#UMLEdge), [`build`](import_graph.md#ImportGraph.build), [`nodes`](uml_activity.md#ActivityCFG.nodes), [`ClassHierarchy`](class_hierarchy.md#ClassHierarchy), [`mermaid`](uml_export.md#UMLDiagram.mermaid), [`nodes`](uml_export.md#UMLDiagram.nodes), [`find_path`](call_path.md#CallPathFinder.find_path), [`UMLDiagram`](uml_export.md#UMLDiagram), [`edges`](uml_export.md#UMLDiagram.edges), [`CallPathFinder`](call_path.md#CallPathFinder), [`render_flowchart_mermaid`](uml_export.md#render_flowchart_mermaid), [`_safe_id`](uml_export.md#_safe_id), [`build`](class_hierarchy.md#ClassHierarchy.build), [`diagram_type`](uml_export.md#UMLDiagram.diagram_type), [`error`](uml_state.md#StateResult.error), [`render_state_mermaid`](uml_export.md#render_state_mermaid), [`transitions`](uml_state.md#StateResult.transitions), [`source`](uml_export.md#UMLEdge.source), [`target`](uml_export.md#UMLEdge.target), [`mermaid_type`](uml_export.md#UMLDiagram.mermaid_type), [`render_class_mermaid`](uml_export.md#render_class_mermaid), [`states`](uml_state.md#StateResult.states), [`_clamp_edges`](uml_export.md#_clamp_edges), [`to_dict`](call_path.md#CallPathResult.to_dict), [`source`](uml_state.md#StateTransition.source), [`target`](uml_state.md#StateTransition.target), [`node_id`](uml_activity.md#CFGNode.node_id), [`truncated`](uml_export.md#UMLDiagram.truncated), [`_dedupe_edges_by_signature`](uml_export.md#_dedupe_edges_by_signature), [`edges`](import_graph.md#ImportGraphResult.edges), [`ImportGraph`](import_graph.md#ImportGraph), [`render_sequence_mermaid`](uml_export.md#render_sequence_mermaid), [`truncated`](uml_activity.md#ActivityCFG.truncated), [`edges`](uml_activity.md#ActivityCFG.edges), [`_escape_label`](uml_export.md#_escape_label), [`error`](uml_activity.md#ActivityCFG.error)  (+16 more; 1 test-only)
- used by: [`execute`](mcp/tools/uml_tool.md#CodeGraphUMLTool.execute), [`uml_exporter`](mcp/tools/codegraph_visualization_hub.md#CodeGraphVisualizationHub.uml_exporter)  (67 test-only)

## Functions
- `_clamp_edges(edges: Iterable[UMLEdge], max_edges: int)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L133)
- `_component_name(file_path: str)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L120)
- `_dedupe_edges_by_signature(edges: Iterable[UMLEdge])` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L155) — Deduplicate edges that share (source, target, label), preserving order.
- `_escape_label(label: str)` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L95) — Sanitise a Mermaid node/edge label.
- `_file_matches(cls_file: str, filter_path: str | None)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L281) — Return True when *cls_file* matches *filter_path*.
- `_is_neighbourhood(child: str, cls: dict[str, Any], center: str | None, all_classes: list[dict[str, Any]])` — [`L294`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L294) — Return True when *child* is in the neighbourhood of *center*.
- `_package_name(file_path: str, max_depth: int = 2)` — [`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L110)
- `_safe_id(name: str)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L88)
- `render_class_mermaid(nodes: Iterable[str], edges: Iterable[UMLEdge], truncated: bool = False)` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L175)
- `render_flowchart_mermaid(nodes: Iterable[str], edges: Iterable[UMLEdge], direction: str = "LR")` — [`L196`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L196)
- `render_sequence_mermaid(paths: list[dict[str, Any]], max_hops: int)` — [`L253`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L253)
- `render_state_mermaid(states: list[str], transitions: list[Any], truncated: bool = False)` — [`L220`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L220) — Render a Mermaid stateDiagram-v2 from states and transitions.

## Module values
- `_ACTIVITY_NOT_FOUND_MERMAID` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L43)
- `_EXTERNAL_BASES` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L18)
- `_TRUNCATION_NOTE` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_export.py#L35)

