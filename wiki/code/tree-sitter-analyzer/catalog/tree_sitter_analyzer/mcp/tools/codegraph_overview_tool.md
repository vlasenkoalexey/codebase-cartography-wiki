---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_overview_tool`/
symbols:
  CodeGraphOverviewTool.execute: CodeGraphOverviewTool#execute().
  _find_entry_points: _find_entry_points().
  _find_hub_functions: _find_hub_functions().
  _compute_depth_distribution: _compute_depth_distribution().
  _find_dead_code: _find_dead_code().
  CodeGraphOverviewTool._get_call_graph: CodeGraphOverviewTool#_get_call_graph().
  _compute_module_coupling: _compute_module_coupling().
  CodeGraphOverviewTool: CodeGraphOverviewTool#
  CodeGraphOverviewTool._try_get_cache: CodeGraphOverviewTool#_try_get_cache().
  CodeGraphOverviewTool.get_call_graph: CodeGraphOverviewTool#get_call_graph().
  _compute_depth_distribution._chain_depth: _compute_depth_distribution()._chain_depth().
  CodeGraphOverviewTool._call_graph: CodeGraphOverviewTool#_call_graph.
  CodeGraphOverviewTool.__init__: CodeGraphOverviewTool#__init__().
  CodeGraphOverviewTool.call_graph_initialized: CodeGraphOverviewTool#call_graph_initialized().
  logger: logger.
  CodeGraphOverviewTool._on_project_root_changed: CodeGraphOverviewTool#_on_project_root_changed().
  CodeGraphOverviewTool.get_tool_definition: CodeGraphOverviewTool#get_tool_definition().
  _HUB_CALLER_FILE_SAMPLE_LIMIT: _HUB_CALLER_FILE_SAMPLE_LIMIT.
  CodeGraphOverviewTool.get_tool_schema: CodeGraphOverviewTool#get_tool_schema().
  CodeGraphOverviewTool.validate_arguments: CodeGraphOverviewTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py)

## Classes
### `CodeGraphOverviewTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L26)
- doc: MCP Tool for project-wide call graph intelligence (CodeGraph parity).
- signature: `class CodeGraphOverviewTool(BaseMCPTool):`
- members:
  - `call_graph_initialized(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L67) — True if the call graph has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L126)
  - `get_call_graph(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L62) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `get_tool_definition(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L71)
  - `get_tool_schema(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L89)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L123)
- protocol/private: `__init__`[`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L29), `_call_graph`[`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L30), `_get_call_graph`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L51), `_on_project_root_changed`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L33), `_try_get_cache`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L36)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`summary`](../../call_graph.md#CallGraph.summary), [`_find_entry_points`](codegraph_overview_tool.md#_find_entry_points), [`_find_hub_functions`](codegraph_overview_tool.md#_find_hub_functions), [`_compute_depth_distribution`](codegraph_overview_tool.md#_compute_depth_distribution), [`_find_dead_code`](codegraph_overview_tool.md#_find_dead_code), [`_compute_module_coupling`](codegraph_overview_tool.md#_compute_module_coupling)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade)  (5 test-only)

## Functions
- `_chain_depth(func: Any)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L283)
- `_compute_depth_distribution(graph: CallGraph)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L270) — Compute a bounded call depth distribution across all functions.
- `_compute_module_coupling(graph: CallGraph, limit: int)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L333) — Files with the most cross-file calls (high coupling).
- `_find_dead_code(graph: CallGraph, limit: int)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L251) — Functions with zero callers AND zero callees (dead code candidates).
- `_find_entry_points(graph: CallGraph, limit: int)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L203) — Functions with zero callers = public API surface.
- `_find_hub_functions(graph: CallGraph, limit: int)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L224) — Functions called by many others (high fan-in).

## Module values
- `_HUB_CALLER_FILE_SAMPLE_LIMIT` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L23)
- `logger` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.py#L21)

