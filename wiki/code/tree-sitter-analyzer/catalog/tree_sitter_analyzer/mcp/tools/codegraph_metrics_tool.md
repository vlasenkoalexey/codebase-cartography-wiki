---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_metrics_tool`/
symbols:
  CodeGraphMetricsTool.execute: CodeGraphMetricsTool#execute().
  CodeGraphMetricsTool._collect_call_graph_metrics: CodeGraphMetricsTool#_collect_call_graph_metrics().
  CodeGraphMetricsTool: CodeGraphMetricsTool#
  CodeGraphMetricsTool._collect_health_metrics: CodeGraphMetricsTool#_collect_health_metrics().
  CodeGraphMetricsTool._get_cache: CodeGraphMetricsTool#_get_cache().
  CodeGraphMetricsTool._collect_route_metrics: CodeGraphMetricsTool#_collect_route_metrics().
  CodeGraphMetricsTool._collect_complexity_metrics: CodeGraphMetricsTool#_collect_complexity_metrics().
  CodeGraphMetricsTool._cache: CodeGraphMetricsTool#_cache.
  logger: logger.
  CodeGraphMetricsTool.__init__: CodeGraphMetricsTool#__init__().
  CodeGraphMetricsTool._on_project_root_changed: CodeGraphMetricsTool#_on_project_root_changed().
  CodeGraphMetricsTool.get_tool_definition: CodeGraphMetricsTool#get_tool_definition().
  CodeGraphMetricsTool.get_tool_schema: CodeGraphMetricsTool#get_tool_schema().
  CodeGraphMetricsTool.validate_arguments: CodeGraphMetricsTool#validate_arguments().
  CodeGraphMetricsTool._collect_cache_metrics: CodeGraphMetricsTool#_collect_cache_metrics().
  CodeGraphMetricsTool._build_suggestions: CodeGraphMetricsTool#_build_suggestions().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py)

## Classes
### `CodeGraphMetricsTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L35)
- doc: MCP Tool for aggregated project intelligence metrics.
- signature: `class CodeGraphMetricsTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L128)
  - `get_tool_definition(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L61)
  - `get_tool_schema(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L86)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L117)
- protocol/private: `__init__`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L38), `_build_suggestions`[`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L386), `_cache`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L39), `_collect_cache_metrics`[`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L197), `_collect_call_graph_metrics`[`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L213), `_collect_complexity_metrics`[`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L278), `_collect_health_metrics`[`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L350), `_collect_route_metrics`[`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L333), `_get_cache`[`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L45), `_on_project_root_changed`[`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L42)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`FunctionRef`](../../call_graph.md#FunctionRef), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`RouteDetector`](../../route_detector.md#RouteDetector), [`analyze_project_heatmap`](../../complexity_heatmap.md#analyze_project_heatmap), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`HealthScorer`](../../health_scorer.md#HealthScorer), [`build`](../../call_graph.md#CachedCallGraph.build), [`ensure_indexed`](../utils/auto_index_guard.md#ensure_indexed), [`all_functions`](../../call_graph.md#CallGraph.all_functions), [`file_path`](../../health_scorer.md#HealthScore.file_path), [`total`](../../health_scorer.md#HealthScore.total), [`grade`](../../health_scorer.md#HealthScore.grade), [`score_project`](../../health_scorer.md#HealthScorer.score_project), [`summary`](../../route_detector.md#RouteDetector.summary), [`call_edges`](../../call_graph.md#CallGraph.call_edges)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_project_facade`](project_facade.md#build_project_facade), [`run_codegraph_metrics`](../../cli/commands/codegraph_index_commands.md#run_codegraph_metrics)  (7 test-only)

## Module values
- `logger` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.py#L32)

