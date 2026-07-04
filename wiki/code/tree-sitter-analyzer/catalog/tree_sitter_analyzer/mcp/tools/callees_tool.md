---
title: 'Module: tree_sitter_analyzer/mcp/tools/callees_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/callees_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.callees_tool`/
symbols:
  CodeGraphCalleesTool.execute: CodeGraphCalleesTool#execute().
  CodeGraphCalleesTool: CodeGraphCalleesTool#
  CodeGraphCalleesTool._enrich_graph_callees_with_activation: CodeGraphCalleesTool#_enrich_graph_callees_with_activation().
  CodeGraphCalleesTool._inline_callee_bodies: CodeGraphCalleesTool#_inline_callee_bodies().
  CodeGraphCalleesTool._sql_native_callees: CodeGraphCalleesTool#_sql_native_callees().
  CodeGraphCalleesTool._resolve_via_enhanced: CodeGraphCalleesTool#_resolve_via_enhanced().
  CodeGraphCalleesTool.__init__: CodeGraphCalleesTool#__init__().
  logger: logger.
  CodeGraphCalleesTool._on_project_root_changed: CodeGraphCalleesTool#_on_project_root_changed().
  CodeGraphCalleesTool._enrich_callees_with_resolution: CodeGraphCalleesTool#_enrich_callees_with_resolution().
  CodeGraphCalleesTool.get_tool_definition: CodeGraphCalleesTool#get_tool_definition().
  CodeGraphCalleesTool.get_tool_schema: CodeGraphCalleesTool#get_tool_schema().
  CodeGraphCalleesTool.validate_arguments: CodeGraphCalleesTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/callees_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py)

## Classes
### `CodeGraphCalleesTool`  ·  implements/extends BaseMCPTool, CodeGraphRelationToolMixin
- def: [`tree_sitter_analyzer/mcp/tools/callees_tool.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L31)
- doc: MCP Tool for finding callees of a function (CodeGraph parity).
- signature: `class CodeGraphCalleesTool(CodeGraphRelationToolMixin, BaseMCPTool):`
- members:
  - `_enrich_callees_with_resolution(self, callees: list[dict[str, Any]])` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L329) — Add callee_resolution and callee_resolved_file to graph-fallback results.
  - `_enrich_graph_callees_with_activation(self, callees: list[dict[str, Any]])` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L382) — Decorate graph-walk results with activation when SQL path missed.
  - `_inline_callee_bodies(self, cache: Any, callees: list[dict[str, Any]])` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L241) — P2: attach a body to the top-N callees (in place). Returns deterrent.
  - `_resolve_via_enhanced(self, cache: Any, func_name: str, file_path: str | None, activation_map: dict[tuple[str, int], dict[str, Any]])` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L341) — Fallback to query_callees_enhanced for cross-file resolution.
  - `_sql_native_callees(self, cache: Any, func_name: str, file_path: str | None, include_activation: bool = False)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L268) — Use SQL-native callees query — O(k) instead of full graph build.
  - `execute(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L106)
  - `get_tool_definition(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L41)
  - `get_tool_schema(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L59)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L101)
- protocol/private: `__init__`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L34), `_on_project_root_changed`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L38)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`callees_of`](../../call_graph.md#CallGraph.callees_of), [`_get_call_graph`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._get_call_graph), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`inline_neighbor_bodies`](symbol_body_inline.md#inline_neighbor_bodies), [`_try_get_cache`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._try_get_cache), [`_is_stale_resolution`](codegraph_relation_tool.md#_is_stale_resolution), [`project_root`](codegraph_relation_tool.md#CodeGraphRelationToolMixin.project_root), [`is_index_rebuilding`](index_rebuild_signal.md#is_index_rebuilding), [`classify_callee_resolution`](codegraph_relation_tool.md#classify_callee_resolution), [`_STALE_CACHE_WARNING`](codegraph_relation_tool.md#_STALE_CACHE_WARNING), [`_init_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._init_relation_state), [`_reset_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._reset_relation_state), [`_data_source`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._data_source), [`rebuild_in_progress_next_step`](index_rebuild_signal.md#rebuild_in_progress_next_step), [`logger`](callees_tool.md#logger), [`_activation_for`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._activation_for), [`_cache_call_graph_built`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._cache_call_graph_built), [`_fetch_activation_map`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._fetch_activation_map), [`NEIGHBORS_DETERRENT`](symbol_body_inline.md#NEIGHBORS_DETERRENT)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`_callees_route`](nav_facade.md#build_nav_facade._callees_route)  (32 test-only)

## Module values
- `logger` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callees_tool.py#L28)

