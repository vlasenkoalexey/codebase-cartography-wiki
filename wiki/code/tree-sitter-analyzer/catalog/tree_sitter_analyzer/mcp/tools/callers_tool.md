---
title: 'Module: tree_sitter_analyzer/mcp/tools/callers_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/callers_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.callers_tool`/
symbols:
  CodeGraphCallersTool.execute: CodeGraphCallersTool#execute().
  CodeGraphCallersTool: CodeGraphCallersTool#
  CodeGraphCallersTool._inline_caller_bodies: CodeGraphCallersTool#_inline_caller_bodies().
  CodeGraphCallersTool._sql_native_callers: CodeGraphCallersTool#_sql_native_callers().
  CodeGraphCallersTool.__init__: CodeGraphCallersTool#__init__().
  logger: logger.
  CodeGraphCallersTool._on_project_root_changed: CodeGraphCallersTool#_on_project_root_changed().
  CodeGraphCallersTool._enrich_callers_with_resolution: CodeGraphCallersTool#_enrich_callers_with_resolution().
  CodeGraphCallersTool.get_tool_definition: CodeGraphCallersTool#get_tool_definition().
  CodeGraphCallersTool.get_tool_schema: CodeGraphCallersTool#get_tool_schema().
  CodeGraphCallersTool.validate_arguments: CodeGraphCallersTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/callers_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py)

## Classes
### `CodeGraphCallersTool`  ·  implements/extends BaseMCPTool, CodeGraphRelationToolMixin
- def: [`tree_sitter_analyzer/mcp/tools/callers_tool.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L31) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Tool for finding callers of a function (CodeGraph parity).
- signature: `class CodeGraphCallersTool(CodeGraphRelationToolMixin, BaseMCPTool):`
- members:
  - `_enrich_callers_with_resolution(callers: list[dict[str, Any]])` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L342) — Add callee_resolution and callee_resolved_file to graph-fallback results.
  - `_inline_caller_bodies(self, cache: Any, callers: list[dict[str, Any]])` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L255) — P2: attach a body to the top-N callers (in place). Returns deterrent.
  - `_sql_native_callers(self, cache: Any, func_name: str, file_path: str | None, include_activation: bool = False)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L282) — Use SQL-native callers query — O(k) instead of full graph build.
  - `execute(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L106) — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `get_tool_definition(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L41)
  - `get_tool_schema(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L59)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L101)
- protocol/private: `__init__`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L34), `_on_project_root_changed`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L38)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`callers_of`](../../call_graph.md#CallGraph.callers_of), [`_get_call_graph`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._get_call_graph), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`inline_neighbor_bodies`](symbol_body_inline.md#inline_neighbor_bodies), [`_try_get_cache`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._try_get_cache), [`_is_stale_resolution`](codegraph_relation_tool.md#_is_stale_resolution), [`project_root`](codegraph_relation_tool.md#CodeGraphRelationToolMixin.project_root), [`is_index_rebuilding`](index_rebuild_signal.md#is_index_rebuilding), [`classify_callee_resolution`](codegraph_relation_tool.md#classify_callee_resolution), [`_STALE_CACHE_WARNING`](codegraph_relation_tool.md#_STALE_CACHE_WARNING), [`_init_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._init_relation_state), [`_reset_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._reset_relation_state), [`_data_source`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._data_source), [`rebuild_in_progress_next_step`](index_rebuild_signal.md#rebuild_in_progress_next_step), [`logger`](callers_tool.md#logger), [`_cache_call_graph_built`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._cache_call_graph_built), [`_fetch_activation_map`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._fetch_activation_map), [`NEIGHBORS_DETERRENT`](symbol_body_inline.md#NEIGHBORS_DETERRENT)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`_try_ast_caller_count`](modification_guard_tool.md#ModificationGuardTool._try_ast_caller_count), [`_callers_route`](nav_facade.md#build_nav_facade._callers_route)  (38 test-only)

## Module values
- `logger` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/callers_tool.py#L28)

