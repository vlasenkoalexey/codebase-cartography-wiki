---
title: 'Module: tree_sitter_analyzer/mcp/tools/modification_guard_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/modification_guard_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.modification_guard_tool`/
symbols:
  ModificationGuardTool.execute: ModificationGuardTool#execute().
  ModificationGuardTool: ModificationGuardTool#
  ModificationGuardTool._trace_impact_tool: ModificationGuardTool#_trace_impact_tool.
  ModificationGuardTool._try_ast_caller_count: ModificationGuardTool#_try_ast_caller_count().
  MODIFICATION_TYPES.MODIFICATION_TYPES: MODIFICATION_TYPES.MODIFICATION_TYPES.
  ModificationGuardTool._run_trace_impact: ModificationGuardTool#_run_trace_impact().
  ModificationGuardTool._apply_pagerank_boost: ModificationGuardTool#_apply_pagerank_boost().
  ModificationGuardTool.validate_arguments: ModificationGuardTool#validate_arguments().
  ModificationGuardTool.get_tool_definition: ModificationGuardTool#get_tool_definition().
  _build_agent_summary: _build_agent_summary().
  ModificationGuardTool._build_initial_result: ModificationGuardTool#_build_initial_result().
  _format_modification_summary_line: _format_modification_summary_line().
  _load_critical_nodes: _load_critical_nodes().
  ModificationGuardTool.get_tool_schema: ModificationGuardTool#get_tool_schema().
  ModificationGuardTool._build_not_found_result: ModificationGuardTool#_build_not_found_result().
  logger: logger.
  CRITICAL_NODES_FILE: CRITICAL_NODES_FILE.
  _next_step_for_verdict: _next_step_for_verdict().
  _aggregate_callers_by_file: _aggregate_callers_by_file().
  _build_proceed_recommendation: _build_proceed_recommendation().
  _guard_impact_badge: _guard_impact_badge().
  _guard_impact_guidance: _guard_impact_guidance().
  _build_required_actions: _build_required_actions().
  _VERDICT_MAP._VERDICT_MAP: _VERDICT_MAP._VERDICT_MAP.
  _VERDICT_BOOST._VERDICT_BOOST: _VERDICT_BOOST._VERDICT_BOOST.
  _VERDICT_TO_RISK._VERDICT_TO_RISK: _VERDICT_TO_RISK._VERDICT_TO_RISK.
  ModificationGuardTool.__init__: ModificationGuardTool#__init__().
  ModificationGuardTool._on_project_root_changed: ModificationGuardTool#_on_project_root_changed().
---
# Module: [`tree_sitter_analyzer/mcp/tools/modification_guard_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py)

## Classes
### `ModificationGuardTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/modification_guard_tool.py:292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L292)
- doc: MCP tool for pre-modification safety checks.
- signature: `class ModificationGuardTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L300) — Initialize the modification guard tool.
  - `_apply_pagerank_boost(self, result: dict[str, Any], symbol: str, safety_verdict: str)` — [`L643`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L643) — PageRank: stamp architecture_* fields + boost verdict for top-10 nodes.
  - `_build_initial_result(*, symbol: str, modification_type: str, impact: dict[str, Any], impact_level: str, total_callers: int, callers_by_file: dict[str, int], safety_verdict: str, required_actions: list[Any], proceed_recommendation: str, ast_caller_count: int | None = None)` — [`L599`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L599) — Canonical safety report — incl. ``count`` alias + ``verdict`` alias.
  - `_build_not_found_result(symbol: str, modification_type: str)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L530) — Wave 1b (audit edit-08): envelope for a symbol unknown to the index.
  - `_on_project_root_changed(self, project_root: str | None)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L314) — Propagate the project-root change to the inner trace_impact tool.
  - `_run_trace_impact(self, symbol: str, file_path: str | None)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L564) — Call trace_impact, propagating project_root + file_path when set.
  - `_try_ast_caller_count(self, symbol: str, file_path: str | None)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L576) — Best-effort AST caller count for guard/callers count reconciliation.
  - `execute(self, arguments: dict[str, Any])` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L450) — Execute the modification guard tool.
  - `get_tool_definition(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L360) — Get the MCP tool definition for modification_guard.
  - `get_tool_schema(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L329)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L417) — Validate input arguments.
- protocol/private: `_trace_impact_tool`[`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L311)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`execute`](callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](callers_tool.md#CodeGraphCallersTool), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`execute`](trace_impact_tool.md#TraceImpactTool.execute), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`TraceImpactTool`](trace_impact_tool.md#TraceImpactTool), [`_get_impact_level`](trace_impact_tool.md#_get_impact_level), [`MODIFICATION_TYPES`](modification_guard_tool.md#MODIFICATION_TYPES.MODIFICATION_TYPES), [`_build_agent_summary`](modification_guard_tool.md#_build_agent_summary), [`_format_modification_summary_line`](modification_guard_tool.md#_format_modification_summary_line), [`_load_critical_nodes`](modification_guard_tool.md#_load_critical_nodes), [`_VERDICT_BOOST`](modification_guard_tool.md#_VERDICT_BOOST._VERDICT_BOOST), [`_VERDICT_MAP`](modification_guard_tool.md#_VERDICT_MAP._VERDICT_MAP), [`_aggregate_callers_by_file`](modification_guard_tool.md#_aggregate_callers_by_file), [`_build_proceed_recommendation`](modification_guard_tool.md#_build_proceed_recommendation), [`_build_required_actions`](modification_guard_tool.md#_build_required_actions), [`_guard_impact_badge`](modification_guard_tool.md#_guard_impact_badge), [`_guard_impact_guidance`](modification_guard_tool.md#_guard_impact_guidance)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (31 test-only)

## Functions
- `_aggregate_callers_by_file(usages: list[dict[str, Any]])` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L138) — Count usages grouped by their ``file`` field.
- `_build_agent_summary(*, symbol: str, modification_type: str, safety_verdict: str, total_callers: int, summary_line: str, proceed_recommendation: str, architecture_rank: int | None)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L60) — Compose the agent_summary block for modification_guard responses.
- `_build_proceed_recommendation(symbol: str, modification_type: str, safety_verdict: str, total_callers: int)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L147) — Verdict-specific advice string the agent reads to decide next step.
- `_build_required_actions(symbol: str, modification_type: str, impact_level: str, total_callers: int)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L238) — Build a list of required actions based on impact level and modification type.
- `_format_modification_summary_line(symbol: str, total_callers: int, final_verdict: str, result: dict[str, Any])` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L172) — One-line headline with optional architecture rank + PageRank score.
- `_guard_impact_badge(impact: dict[str, Any], total_callers: int)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L204) — Render guard impact with the correct unit for its trace-derived count.
- `_guard_impact_guidance(impact: dict[str, Any], total_callers: int)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L212) — Render guard guidance without calling trace occurrences AST callers.
- `_load_critical_nodes(project_root: str | None)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L223) — Load critical_nodes.json from the project cache, if it exists.
- `_next_step_for_verdict(*, safety_verdict: str, symbol: str, modification_type: str, total_callers: int, architecture_rank: int | None)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L104) — Return one concrete next action keyed by the safety verdict.

## Module values
- `CRITICAL_NODES_FILE` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L57)
- `MODIFICATION_TYPES` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L55)
- `_VERDICT_BOOST` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L33)
- `_VERDICT_MAP` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L25)
- `_VERDICT_TO_RISK` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L43)
- `logger` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/modification_guard_tool.py#L22)

