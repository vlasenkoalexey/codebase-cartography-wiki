---
title: 'Module: tree_sitter_analyzer/mcp/tools/facade_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/facade_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.facade_tool`/
symbols:
  FacadeTool.execute: FacadeTool#execute().
  FacadeTool.action_map: FacadeTool#action_map.
  FacadeTool: FacadeTool#
  FacadeTool.bespoke_map: FacadeTool#bespoke_map.
  FacadeTool.get_tool_schema: FacadeTool#get_tool_schema().
  FacadeTool.get_tool_definition: FacadeTool#get_tool_definition().
  FacadeTool.register_bespoke_inner: FacadeTool#register_bespoke_inner().
  FacadeTool._bespoke_inners: FacadeTool#_bespoke_inners.
  FacadeTool._available_actions: FacadeTool#_available_actions().
  FacadeTool._project_args: FacadeTool#_project_args().
  FacadeTool.facade_name: FacadeTool#facade_name.
  FacadeTool.validate_arguments: FacadeTool#validate_arguments().
  FacadeTool._action_error: FacadeTool#_action_error().
  FacadeTool._inner_property_names: FacadeTool#_inner_property_names().
  FacadeTool.__init__: FacadeTool#__init__().
  FacadeTool._annotations: FacadeTool#_annotations.
  FacadeTool._description: FacadeTool#_description.
  FacadeTool._extra_public_params: FacadeTool#_extra_public_params.
  FacadeTool._clean_bespoke_args: FacadeTool#_clean_bespoke_args().
  FacadeTool._closest_action: FacadeTool#_closest_action().
  _CORE_FACADE_PARAMS._CORE_FACADE_PARAMS: _CORE_FACADE_PARAMS._CORE_FACADE_PARAMS.
  BespokeHandler: BespokeHandler.
  _FACADE_CONTROL_KEYS._FACADE_CONTROL_KEYS: _FACADE_CONTROL_KEYS._FACADE_CONTROL_KEYS.
  FacadeTool._on_project_root_changed: FacadeTool#_on_project_root_changed().
---
# Module: [`tree_sitter_analyzer/mcp/tools/facade_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py)

## Classes
### `FacadeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/facade_tool.py:108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L108) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: One MCP tool fanning `action` out to many inner tools.
- signature: `class FacadeTool(BaseMCPTool):`
- members:
  - `_action_error(self, message: str, suggestion: str | None = None)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L295) — Return a canonical error envelope listing available actions.
  - `_clean_bespoke_args(args: dict[str, Any])` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L265) — Strip facade control keys for a bespoke route (no schema projection).
  - `_closest_action(self, action: str)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L282) — Return the single closest valid action to ``action`` (a likely
  - `_inner_property_names(inner: BaseMCPTool)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L209) — Return the inner tool's declared top-level schema property names.
  - `_on_project_root_changed(self, project_root: str | None)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L184) — Forward the new project root to every held inner instance.
  - `_project_args(self, inner: BaseMCPTool, args: dict[str, Any])` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L223) — Project caller args onto the inner tool's schema whitelist.
  - `execute(self, arguments: dict[str, Any])` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L334) — Route ``arguments['action']`` to the matching inner / bespoke route. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_definition(self)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L417)
  - `get_tool_schema(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L366) — Slim public facade schema: ``action`` (required) + core shared params.
  - `register_bespoke_inner(self, inner: BaseMCPTool)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L167) — Register an inner instance reachable only via a bespoke closure (F5).
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L429) — A facade only requires a known ``action``; inner tools validate the
  - `action_map` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L150) — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `bespoke_map` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L151) — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `facade_name` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L149)
- protocol/private: `__init__`[`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L138), `_annotations`[`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L157), `_available_actions`[`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L279), `_bespoke_inners`[`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L155), `_description`[`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L156), `_extra_public_params`[`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L158)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`set_project_path`](base_tool.md#BaseMCPTool.set_project_path), [`_CORE_FACADE_PARAMS`](facade_tool.md#_CORE_FACADE_PARAMS._CORE_FACADE_PARAMS), [`BespokeHandler`](facade_tool.md#BespokeHandler), [`_FACADE_CONTROL_KEYS`](facade_tool.md#_FACADE_CONTROL_KEYS._FACADE_CONTROL_KEYS)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade), [`build_health_facade`](health_facade.md#build_health_facade), [`build_edit_facade`](edit_facade.md#build_edit_facade), [`build_viz_facade`](viz_facade.md#build_viz_facade), [`build_project_facade`](project_facade.md#build_project_facade), [`build_search_facade`](search_facade.md#build_search_facade), [`build_index_facade`](index_facade.md#build_index_facade)  (250 test-only)

## Module values
- `BespokeHandler` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L65)
- `_CORE_FACADE_PARAMS` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L89)
- `_FACADE_CONTROL_KEYS` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/facade_tool.py#L71)

