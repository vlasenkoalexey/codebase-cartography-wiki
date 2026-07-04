---
title: 'Module: tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.dependency_analysis_tool`/
symbols:
  DependencyAnalysisTool.execute: DependencyAnalysisTool#execute().
  DependencyAnalysisTool: DependencyAnalysisTool#
  DependencyAnalysisTool._get_graph: DependencyAnalysisTool#_get_graph().
  _summary: _summary().
  DependencyAnalysisTool._resolve_file: DependencyAnalysisTool#_resolve_file().
  _attach_agent_summary: _attach_agent_summary().
  _file_deps: _file_deps().
  DependencyAnalysisTool._graph: DependencyAnalysisTool#_graph.
  DependencyAnalysisTool._on_project_root_changed: DependencyAnalysisTool#_on_project_root_changed().
  _cycles: _cycles().
  _deterministic_find_cycles: _deterministic_find_cycles().
  DependencyAnalysisTool._explain_fingerprint_delta: DependencyAnalysisTool#_explain_fingerprint_delta().
  DependencyAnalysisTool._cache_invalidated_reason: DependencyAnalysisTool#_cache_invalidated_reason.
  _deterministic_find_cycles.dfs: _deterministic_find_cycles().dfs().
  _blast_recommendation: _blast_recommendation().
  DependencyAnalysisTool._graph_fingerprint: DependencyAnalysisTool#_graph_fingerprint.
  _summary_mode_envelope: _summary_mode_envelope().
  DependencyAnalysisTool._normalize_mode: DependencyAnalysisTool#_normalize_mode().
  DependencyAnalysisTool._graph_built_at: DependencyAnalysisTool#_graph_built_at.
  DependencyAnalysisTool.validate_arguments: DependencyAnalysisTool#validate_arguments().
  _blast_radius_mode_envelope: _blast_radius_mode_envelope().
  logger: logger.
  DependencyAnalysisTool.get_tool_definition: DependencyAnalysisTool#get_tool_definition().
  DependencyAnalysisTool._MODE_ALIASES: DependencyAnalysisTool#_MODE_ALIASES.
  DependencyAnalysisTool.get_tool_schema: DependencyAnalysisTool#get_tool_schema().
  _cycles_mode_envelope: _cycles_mode_envelope().
  _file_deps_mode_envelope: _file_deps_mode_envelope().
  _blast_radius_next_step: _blast_radius_next_step().
  DependencyAnalysisTool.__init__: DependencyAnalysisTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py)

## Classes
### `DependencyAnalysisTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L21)
- doc: MCP Tool for project-level dependency analysis.
- signature: `class DependencyAnalysisTool(BaseMCPTool):`
- members:
  - `_normalize_mode(cls, mode: str)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L95) — Resolve aliases (e.g. ``full`` -> ``summary``).
  - `_resolve_file(self, file_path: str, graph: DependencyGraph)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L219) — Resolve file_path to a project-relative path that exists in the graph.
  - `execute(self, arguments: dict[str, Any])` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L163)
  - `get_tool_definition(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L99)
  - `get_tool_schema(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L118)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L154)
- protocol/private: `_MODE_ALIASES`[`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L92), `__init__`[`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L24), `_cache_invalidated_reason`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L32), `_explain_fingerprint_delta`[`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L65), `_get_graph`[`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L41), `_graph`[`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L25), `_graph_built_at`[`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L31), `_graph_fingerprint`[`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L30), `_on_project_root_changed`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L35)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`DependencyGraph`](../../project_graph.md#DependencyGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`compute_graph_fingerprint`](../../_graph_cache_fingerprint.md#compute_graph_fingerprint), [`file_count`](../../_graph_cache_fingerprint.md#GraphFingerprint.file_count), [`_summary`](dependency_analysis_tool.md#_summary), [`GraphFingerprint`](../../_graph_cache_fingerprint.md#GraphFingerprint), [`nodes`](../../project_graph.md#DependencyGraph.nodes), [`_attach_agent_summary`](dependency_analysis_tool.md#_attach_agent_summary), [`_file_deps`](dependency_analysis_tool.md#_file_deps), [`BlastRadius`](../../project_graph.md#BlastRadius), [`_cycles`](dependency_analysis_tool.md#_cycles), [`max_mtime_ns`](../../_graph_cache_fingerprint.md#GraphFingerprint.max_mtime_ns), [`has_node`](../../project_graph.md#DependencyGraph.has_node), [`_blast_recommendation`](dependency_analysis_tool.md#_blast_recommendation), [`analyze`](../../project_graph.md#BlastRadius.analyze), [`node_count`](../../project_graph.md#DependencyGraph.node_count)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_collect_forward_impact`](../../cli/commands/affected_command.md#_collect_forward_impact)  (14 test-only)

## Functions
- `_attach_agent_summary(result: dict[str, Any], mode: str, graph: DependencyGraph)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L505) — Mutate ``result`` in place to add summary_line + agent_summary.
- `_blast_radius_mode_envelope(result: dict[str, Any])` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L495) — Build ``(summary_line, next_step, verdict)`` for mode=blast_radius.
- `_blast_radius_next_step(forward: int)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L473) — Map ``forward`` count → ``(next_step, verdict)`` ladder for blast_radius.
- `_blast_recommendation(analysis: dict[str, Any])` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L403)
- `_cycles(graph: DependencyGraph)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L288)
- `_cycles_mode_envelope(result: dict[str, Any])` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L447) — Build ``(summary_line, next_step, verdict)`` for mode=cycles.
- `_deterministic_find_cycles(graph: DependencyGraph)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L321) — Enumerate elementary cycles in ``graph`` with a deterministic order.
- `_file_deps(graph: DependencyGraph, rel_path: str)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L389)
- `_file_deps_mode_envelope(result: dict[str, Any])` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L460) — Build ``(summary_line, next_step, verdict)`` for mode=file_deps.
- `_summary(graph: DependencyGraph)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L256)
- `_summary_mode_envelope(result: dict[str, Any], graph: DependencyGraph)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L417) — Build ``(summary_line, next_step, verdict)`` for mode=summary.
- `dfs(node: str)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L347)

## Module values
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.py#L18)

