---
title: 'Module: tree_sitter_analyzer/mcp/tools/uml_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/uml_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.uml_tool`/
symbols:
  CodeGraphUMLTool.execute: CodeGraphUMLTool#execute().
  CodeGraphUMLTool: CodeGraphUMLTool#
  CodeGraphUMLTool.get_tool_schema: CodeGraphUMLTool#get_tool_schema().
  CodeGraphUMLTool.validate_arguments: CodeGraphUMLTool#validate_arguments().
  CodeGraphUMLTool.get_tool_definition: CodeGraphUMLTool#get_tool_definition().
  _DEFAULT_CLASS_MAX_EDGES: _DEFAULT_CLASS_MAX_EDGES.
  logger: logger.
  _DEFAULT_MAX_EDGES: _DEFAULT_MAX_EDGES.
  _DEFAULT_PACKAGE_MAX_EDGES: _DEFAULT_PACKAGE_MAX_EDGES.
  _DEFAULT_COMPONENT_MAX_EDGES: _DEFAULT_COMPONENT_MAX_EDGES.
---
# Module: [`tree_sitter_analyzer/mcp/tools/uml_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py)

## Classes
### `CodeGraphUMLTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/uml_tool.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L28)
- doc: Export UML-style Mermaid diagrams from the CodeGraph cache.
- signature: `class CodeGraphUMLTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L182) — documented in [tree_sitter_analyzer-uml_export](../../../../concepts/tree_sitter_analyzer-uml_export.md)
  - `get_tool_definition(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L31)
  - `get_tool_schema(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L53)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L158)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`activity_diagram`](../../uml_export.md#UMLExporter.activity_diagram), [`build_response`](_response_builder.md#build_response), [`state_diagram`](../../uml_export.md#UMLExporter.state_diagram), [`metadata`](../../uml_export.md#UMLDiagram.metadata), [`class_diagram`](../../uml_export.md#UMLExporter.class_diagram), [`component_diagram`](../../uml_export.md#UMLExporter.component_diagram), [`package_diagram`](../../uml_export.md#UMLExporter.package_diagram), [`sequence_diagram`](../../uml_export.md#UMLExporter.sequence_diagram), [`edges`](../../uml_export.md#UMLDiagram.edges), [`build_error`](_response_builder.md#build_error), [`to_dict`](../../uml_export.md#UMLDiagram.to_dict), [`_validate_positive_int`](_validators.md#_validate_positive_int), [`uml_exporter`](codegraph_visualization_hub.md#CodeGraphVisualizationHub.uml_exporter), [`CodeGraphVisualizationHub`](codegraph_visualization_hub.md#CodeGraphVisualizationHub), [`_DEFAULT_CLASS_MAX_EDGES`](uml_tool.md#_DEFAULT_CLASS_MAX_EDGES), [`_DEFAULT_COMPONENT_MAX_EDGES`](uml_tool.md#_DEFAULT_COMPONENT_MAX_EDGES), [`_DEFAULT_PACKAGE_MAX_EDGES`](uml_tool.md#_DEFAULT_PACKAGE_MAX_EDGES)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_viz_facade`](viz_facade.md#build_viz_facade)  (36 test-only)

## Module values
- `_DEFAULT_CLASS_MAX_EDGES` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L19)
- `_DEFAULT_COMPONENT_MAX_EDGES` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L21)
- `_DEFAULT_MAX_EDGES` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L25)
- `_DEFAULT_PACKAGE_MAX_EDGES` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L20)
- `logger` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/uml_tool.py#L15)

