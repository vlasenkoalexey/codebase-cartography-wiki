---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_impact_tool`/
symbols:
  CodeGraphImpactTool: CodeGraphImpactTool#
  _compute_risk_score: _compute_risk_score().
  CodeGraphImpactTool._function_impact: CodeGraphImpactTool#_function_impact().
  _compute_transitive_callers: _compute_transitive_callers().
  CodeGraphImpactTool._call_graph: CodeGraphImpactTool#_call_graph.
  _compute_transitive_callees: _compute_transitive_callees().
  CodeGraphImpactTool.execute: CodeGraphImpactTool#execute().
  _blast_radius_for_functions: _blast_radius_for_functions().
  _MAX_TRANSITIVE: _MAX_TRANSITIVE.
  _MAX_LISTED: _MAX_LISTED.
  CodeGraphImpactTool._get_call_graph: CodeGraphImpactTool#_get_call_graph().
  CodeGraphImpactTool._try_get_cache: CodeGraphImpactTool#_try_get_cache().
  _partition_refs: _partition_refs().
  CodeGraphImpactTool.validate_arguments: CodeGraphImpactTool#validate_arguments().
  CodeGraphImpactTool.get_call_graph: CodeGraphImpactTool#get_call_graph().
  _impact_verdict: _impact_verdict().
  CodeGraphImpactTool.__init__: CodeGraphImpactTool#__init__().
  CodeGraphImpactTool.get_tool_schema: CodeGraphImpactTool#get_tool_schema().
  CodeGraphImpactTool.get_tool_definition: CodeGraphImpactTool#get_tool_definition().
  logger: logger.
  CodeGraphImpactTool._on_project_root_changed: CodeGraphImpactTool#_on_project_root_changed().
  CodeGraphImpactTool.call_graph_initialized: CodeGraphImpactTool#call_graph_initialized().
  _MAX_DEPTH: _MAX_DEPTH.
  _compute_risk_score._norm: _compute_risk_score()._norm().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py)

## Classes
### `CodeGraphImpactTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L330)
- doc: MCP Tool for function-level blast radius analysis (CodeGraph parity).
- signature: `class CodeGraphImpactTool(BaseMCPTool):`
- members:
  - `call_graph_initialized(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L371) — True if the call graph has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L476)
  - `get_call_graph(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L366) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `get_tool_definition(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L375)
  - `get_tool_schema(self)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L397)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L459)
- protocol/private: `__init__`[`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L333), `_call_graph`[`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L334), `_function_impact`[`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L611), `_get_call_graph`[`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L355), `_on_project_root_changed`[`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L337), `_try_get_cache`[`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L340)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`FunctionRef`](../../call_graph.md#FunctionRef), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`_compute_risk_score`](codegraph_impact_tool.md#_compute_risk_score), [`callees_of`](../../call_graph.md#CallGraph.callees_of), [`callers_of`](../../call_graph.md#CallGraph.callers_of), [`_compute_transitive_callers`](codegraph_impact_tool.md#_compute_transitive_callers), [`_compute_transitive_callees`](codegraph_impact_tool.md#_compute_transitive_callees), [`_blast_radius_for_functions`](codegraph_impact_tool.md#_blast_radius_for_functions), [`resolve_targets`](../../call_graph.md#CallGraph.resolve_targets), [`_MAX_LISTED`](codegraph_impact_tool.md#_MAX_LISTED), [`_MAX_TRANSITIVE`](codegraph_impact_tool.md#_MAX_TRANSITIVE), [`_impact_verdict`](codegraph_impact_tool.md#_impact_verdict)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`_test_map_route`](nav_facade.md#build_nav_facade._test_map_route), [`_co_change_route`](nav_facade.md#build_nav_facade._co_change_route)  (51 test-only)

## Functions
- `_blast_radius_for_functions(graph: CallGraph, function_names: list[str], file_path: str | None = None, depth: int = 5)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L257)
- `_compute_risk_score(graph: CallGraph, func_name: str, file_path: str | None = None, include_tests: bool = False)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L115)
- `_compute_transitive_callees(graph: CallGraph, func_name: str, file_path: str | None = None, max_depth: int = _MAX_DEPTH, include_tests: bool = False)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L84)
- `_compute_transitive_callers(graph: CallGraph, func_name: str, file_path: str | None = None, max_depth: int = _MAX_DEPTH, include_tests: bool = False)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L53)
- `_impact_verdict(result: dict[str, Any])` — [`L672`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L672) — Map embedded risk level to canonical verdict.
- `_norm(p: str | None)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L147)
- `_partition_refs(refs: list[FunctionRef])` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L39) — Split refs into (production, test) using the canonical is_test_file.

## Module values
- `_MAX_DEPTH` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L30)
- `_MAX_LISTED` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L36)
- `_MAX_TRANSITIVE` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L29)
- `logger` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_impact_tool.py#L27)

