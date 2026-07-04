---
title: 'Module: tree_sitter_analyzer/mcp/tools/project_health_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/project_health_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.project_health_tool`/
symbols:
  _build_project_health_result: _build_project_health_result().
  _compute_project_health_aggregates: _compute_project_health_aggregates().
  ProjectHealthTool: ProjectHealthTool#
  ProjectHealthTool.execute: ProjectHealthTool#execute().
  _build_project_agent_summary: _build_project_agent_summary().
  _build_agent_backlog_item: _build_agent_backlog_item().
  _build_agent_backlog: _build_agent_backlog().
  _top_refactoring_targets: _top_refactoring_targets().
  _file_action: _file_action().
  _estimate_seconds: _estimate_seconds().
  _is_agent_backlog_candidate: _is_agent_backlog_candidate().
  _weakest_dimension: _weakest_dimension().
  _file_details: _file_details().
  _is_non_actionable_sample_path: _is_non_actionable_sample_path().
  _GRADE_ORDER: _GRADE_ORDER.
  _ProjectHealthAggregates.grade_distribution: _ProjectHealthAggregates#grade_distribution.
  _ProjectHealthAggregates.worst: _ProjectHealthAggregates#worst.
  _ProjectHealthAggregates.weakest_dim: _ProjectHealthAggregates#weakest_dim.
  _ProjectHealthAggregates.files: _ProjectHealthAggregates#files.
  ProjectHealthTool.get_tool_definition: ProjectHealthTool#get_tool_definition().
  _visible_file_limit: _visible_file_limit().
  _average_dimensions: _average_dimensions().
  _scores_at_or_below_min_grade: _scores_at_or_below_min_grade().
  _attach_queue_head_fields: _attach_queue_head_fields().
  _AGENT_BACKLOG_LIMIT: _AGENT_BACKLOG_LIMIT.
  _ProjectHealthAggregates.dim_avgs: _ProjectHealthAggregates#dim_avgs.
  _ProjectHealthAggregates.agent_backlog: _ProjectHealthAggregates#agent_backlog.
  _build_project_recommendation: _build_project_recommendation().
  logger: logger.
  _ProjectHealthAggregates: _ProjectHealthAggregates#
  _ProjectHealthAggregates.grade_counts: _ProjectHealthAggregates#grade_counts.
  _ProjectHealthAggregates.signal_dims: _ProjectHealthAggregates#signal_dims.
  _ProjectHealthAggregates.visible_limit: _ProjectHealthAggregates#visible_limit.
  _numeric_dimensions: _numeric_dimensions().
  _project_risk: _project_risk().
  _project_risk_to_verdict: _project_risk_to_verdict().
  _AGENT_BACKLOG_EXCLUDED_SEGMENTS: _AGENT_BACKLOG_EXCLUDED_SEGMENTS.
  _AGENT_BACKLOG_EXCLUDED_FILENAMES: _AGENT_BACKLOG_EXCLUDED_FILENAMES.
  ProjectHealthTool.get_tool_schema: ProjectHealthTool#get_tool_schema().
  ProjectHealthTool.validate_arguments: ProjectHealthTool#validate_arguments().
  _normalize_max_files: _normalize_max_files().
  _coverage_status: _coverage_status().
  _project_summary_line: _project_summary_line().
  _project_summary_base: _project_summary_base().
  _project_queue_head: _project_queue_head().
  _project_signal: _project_signal().
  _recommended_cli_command: _recommended_cli_command().
  _agent_backlog_priority: _agent_backlog_priority().
  _agent_backlog_reason: _agent_backlog_reason().
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _GRADE_RECOMMENDATIONS: _GRADE_RECOMMENDATIONS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/project_health_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py)

## Classes
### `ProjectHealthTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/project_health_tool.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L81)
- doc: MCP Tool that scores every source file and returns a project health report.
- signature: `class ProjectHealthTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L150)
  - `get_tool_definition(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L84)
  - `get_tool_schema(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L113)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L147)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`_build_project_health_result`](project_health_tool.md#_build_project_health_result), [`HealthScorer`](../../health_scorer.md#HealthScorer), [`score_project_with_stats`](../../health_scorer.md#HealthScorer.score_project_with_stats), [`_normalize_max_files`](project_health_tool.md#_normalize_max_files)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_health_facade`](health_facade.md#build_health_facade), [`_handle_health_check`](../../cli/special_commands.md#_handle_health_check)  (12 test-only)

### `_ProjectHealthAggregates`
- def: [`tree_sitter_analyzer/mcp/tools/project_health_tool.py:192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L192)
- doc: Pre-computed aggregates shared between health-result fields.
- signature: `class _ProjectHealthAggregates:`
- members:
  - `agent_backlog` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L208)
  - `dim_avgs` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L204)
  - `files` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L209)
  - `grade_counts` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L202)
  - `grade_distribution` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L203)
  - `signal_dims` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L205)
  - `visible_limit` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L210)
  - `weakest_dim` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L207)
  - `worst` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L206)
- used by: [`_build_project_health_result`](project_health_tool.md#_build_project_health_result), [`_compute_project_health_aggregates`](project_health_tool.md#_compute_project_health_aggregates)

## Functions
- `_agent_backlog_priority(grade: str)` — [`L737`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L737) — Return an execution priority for autonomous project-health backlogs.
- `_agent_backlog_reason(grade: str, weakest: str)` — [`L748`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L748) — Explain why project-health queued this file.
- `_attach_queue_head_fields(summary: dict[str, Any], queue_head: dict[str, Any], root: str)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L559) — Add queue-head pointers + next-step CLI hints to ``summary``.
- `_average_dimensions(scores: list[Any])` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L335) — Average health dimensions across a scored project.
- `_build_agent_backlog(scores: list[Any], limit: int = _AGENT_BACKLOG_LIMIT)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L458) — Build a machine-friendly backlog from project health scores.
- `_build_agent_backlog_item(score: Any)` — [`L695`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L695) — Build one project-health backlog item with MCP and CLI parity.
- `_build_project_agent_summary(*, root: str, total_files: int, grade_distribution: dict[str, int], weakest_dim: str, agent_backlog: list[dict[str, Any]], max_files: int = 20, actual_seconds: float | None = None)` — [`L579`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L579) — Build a compact project-level summary for autonomous agent loops.
- `_build_project_health_result(root: str, all_scores: list[Any], min_grade: str, max_files: int, actual_seconds: float | None = None, walk_stats: dict[str, Any] | None = None)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L243) — Build the JSON-ready project-health response.
- `_build_project_recommendation(grade_counts: Counter, weakest_dim: str, total: int)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L418)
- `_compute_project_health_aggregates(all_scores: list[Any], min_grade: str, max_files: int)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L213) — Pre-compute the aggregates that the response dict needs.
- `_coverage_status(dimensions: dict[str, float | None])` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L358) — Track whether project coverage data was available.
- `_estimate_seconds(total_files: int)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L26) — Return a rough wall-clock estimate so callers can size their timeouts.
- `_file_action(score: Any)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L440) — Suggest the next tool to call for a specific file.
- `_file_details(scores: list[Any], max_files: int)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L375) — Build detailed file health rows for project-health output.
- `_is_agent_backlog_candidate(score: Any)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L468) — Return whether a score should become an autonomous agent queue item.
- `_is_non_actionable_sample_path(file_path: str)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L475) — Skip demo fixtures and docs that are intentionally poor queue heads.
- `_normalize_max_files(value: Any)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L322) — Normalize user-provided project-health detail limit.
- `_numeric_dimensions(dimensions: dict[str, float | None])` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L349) — Keep only numeric dimensions for signal and comparison logic.
- `_project_queue_head(queue_head: dict[str, Any])` — [`L636`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L636) — Return the fields agents need before opening the next project item.
- `_project_risk(grade_distribution: dict[str, int])` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L662) — Convert project health distribution into a compact risk label.
- `_project_risk_to_verdict(risk: str)` — [`L673`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L673) — Map project-level risk to the cross-tool verdict vocabulary.
- `_project_signal(dim_signal: str, risk: str)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L648) — Return a project-level signal consistent with the grade-distribution risk.
- `_project_summary_base(*, summary_line: str, verdict: str, risk: str, total_files: int, grade_distribution: dict[str, int], weakest_dim: str, agent_backlog_count: int, estimated_seconds: float, actual_seconds: float | None, max_files: int)` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L514) — Build the always-present fields of the project_health agent_summary.
- `_project_summary_line(*, risk: str, total_files: int, grade_distribution: dict[str, int], agent_backlog_count: int, weakest_dim: str, estimated_seconds: float, actual_seconds: float | None)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L484) — Build the ``project_health risk=... files=... A=N B=N ...`` headline line.
- `_recommended_cli_command(grade: str, quoted_path: str)` — [`L728`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L728) — Return the CLI command matching the recommended MCP action.
- `_scores_at_or_below_min_grade(scores: list[Any], min_grade: str)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L363) — Return files whose grade is at or below the requested detail threshold.
- `_top_refactoring_targets(scores: list[Any], max_files: int = _AGENT_BACKLOG_LIMIT)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L398) — Build the compact top-refactoring target list.
- `_visible_file_limit(max_files: int)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L330) — Keep compact target/backlog lists aligned with the requested detail limit.
- `_weakest_dimension(dimensions: dict[str, float | None])` — [`L755`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L755) — Return the weakest dimension name, or an empty string when unavailable.

## Module values
- `_AGENT_BACKLOG_EXCLUDED_FILENAMES` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L72)
- `_AGENT_BACKLOG_EXCLUDED_SEGMENTS` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L71)
- `_AGENT_BACKLOG_LIMIT` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L69)
- `_EXCLUDE_DIRS` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L44)
- `_GRADE_ORDER` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L70)
- `_GRADE_RECOMMENDATIONS` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L185)
- `logger` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_health_tool.py#L20)

