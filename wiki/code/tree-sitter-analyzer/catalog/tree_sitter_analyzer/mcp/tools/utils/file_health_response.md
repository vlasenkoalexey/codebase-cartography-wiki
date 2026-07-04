---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/file_health_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/file_health_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.file_health_response`/
symbols:
  build_file_health_result: build_file_health_result().
  _build_signal: _build_signal().
  _build_agent_summary: _build_agent_summary().
  _build_agent_next_action: _build_agent_next_action().
  _apply_smell_penalty: _apply_smell_penalty().
  _build_base_health_result: _build_base_health_result().
  _build_optional_extraction_fields: _build_optional_extraction_fields().
  _build_refactor_agent_action: _build_refactor_agent_action().
  _build_recommendation: _build_recommendation().
  _find_function_end_line: _find_function_end_line().
  _build_extraction_plan: _build_extraction_plan().
  _build_extraction_target: _build_extraction_target().
  _has_refactor_target_smell: _has_refactor_target_smell().
  _long_method_names: _long_method_names().
  _suggest_next_action: _suggest_next_action().
  _first_actionable_smell: _first_actionable_smell().
  _weakest_dimension_score: _weakest_dimension_score().
  _project_smell_type: _project_smell_type().
  _grade_from_score: _grade_from_score().
  _health_next_step: _health_next_step().
  _health_verification_command: _health_verification_command().
  _health_stop_condition: _health_stop_condition().
  _file_health_cli_command: _file_health_cli_command().
  _SIGNAL_MAP: _SIGNAL_MAP.
  _MAX_SMELL_PENALTY: _MAX_SMELL_PENALTY.
  _GRADE_THRESHOLDS: _GRADE_THRESHOLDS.
  _build_noop_agent_action: _build_noop_agent_action().
  _refactor_cli_command: _refactor_cli_command().
  _agent_action_reason: _agent_action_reason().
  _agent_action_priority: _agent_action_priority().
  _add_target_location_summary: _add_target_location_summary().
  _SMELL_SCORE_PENALTY._SMELL_SCORE_PENALTY: _SMELL_SCORE_PENALTY._SMELL_SCORE_PENALTY.
  _SMELL_SEVERITY_PENALTY._SMELL_SEVERITY_PENALTY: _SMELL_SEVERITY_PENALTY._SMELL_SEVERITY_PENALTY.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/file_health_response.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py)

## Functions
- `_add_target_location_summary(summary: dict[str, Any], target: dict[str, Any])` — [`L462`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L462) — Attach compact location details for the first actionable smell.
- `_agent_action_priority(grade: str, smells: list[dict[str, Any]])` — [`L408`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L408) — Return a coarse priority for autonomous agents.
- `_agent_action_reason(grade: str, weakest_dimension: str, smells: list[dict[str, Any]])` — [`L396`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L396) — Explain why the structured action is being recommended.
- `_apply_smell_penalty(health: Any, smells: list[dict[str, Any]])` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L198) — Return (adjusted_total, adjusted_grade) after K9 smell penalties.
- `_build_agent_next_action(file_path: str, grade: str, dimensions: dict[str, float], smells: list[dict[str, Any]])` — [`L336`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L336) — Build a structured next action that agents can execute directly.
- `_build_agent_summary(file_path: str, health: Any, smells: list[dict[str, Any]], action: dict[str, Any], adjusted_total: float | None = None, adjusted_grade: str | None = None)` — [`L419`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L419) — Build the compact first-read health decision summary for agents.
- `_build_base_health_result(file_path: str, health: Any, smells: list[dict[str, Any]], action: dict[str, Any])` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L101) — Build the common file-health response fields.
- `_build_extraction_plan(file_path: str, smells: list[dict[str, Any]], resolved_path: str, analysis: Any)` — [`L523`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L523) — Build a structured extraction plan for D/F grade files.
- `_build_extraction_target(smell: dict[str, Any], resolved_path: str, analysis: Any)` — [`L556`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L556) — Build one extraction target from a long-method smell.
- `_build_noop_agent_action()` — [`L350`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L350) — Build the action payload for files that need no immediate work.
- `_build_optional_extraction_fields(file_path: str, grade: str, smells: list[dict[str, Any]], resolved: str, analysis: Any)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L240) — Build D/F-only next action and extraction plan fields.
- `_build_recommendation(grade: str, dimensions: dict[str, float], smells: list[dict[str, Any]])` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L274) — Build a human-readable recommendation based on grade and smells.
- `_build_refactor_agent_action(file_path: str, grade: str, weakest_dimension: str, smells: list[dict[str, Any]])` — [`L361`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L361) — Build the action payload for files that need focused cleanup.
- `_build_signal(dimensions: dict[str, float])` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L258) — Build a concise signal string identifying the weakest dimension.
- `_file_health_cli_command(file_path: str)` — [`L388`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L388) — Build the CLI command for re-running file health.
- `_find_function_end_line(file_path: str, start_line: int, analysis: Any)` — [`L573`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L573) — Find the end line of a function using tree-sitter elements, with fallback.
- `_first_actionable_smell(smells: list[dict[str, Any]])` — [`L509`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L509) — Return the first smell worth surfacing in a compact summary.
- `_grade_from_score(score: float)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L232) — Mirror ``HealthScore.grade`` so adjusted scores get a fresh letter.
- `_has_refactor_target_smell(smells: list[dict[str, Any]])` — [`L517`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L517) — Return whether refactoring_suggestions is likely to produce concrete targets.
- `_health_next_step(action: dict[str, Any], smells: list[dict[str, Any]])` — [`L482`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L482) — Return the immediate next step for a health report.
- `_health_stop_condition(action: dict[str, Any], file_path: str)` — [`L499`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L499) — Describe when a health-driven edit queue can close.
- `_health_verification_command(action: dict[str, Any], file_path: str)` — [`L491`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L491) — Return the primary command that verifies a health-driven edit.
- `_long_method_names(smells: list[dict[str, Any]])` — [`L307`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L307) — Extract long-method names from smell detail strings.
- `_project_smell_type(smells: list[dict[str, Any]])` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L68) — H6 fix: ensure every smell carries a ``type`` field.
- `_refactor_cli_command(file_path: str)` — [`L380`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L380) — Build the CLI command for refactoring suggestions.
- `_suggest_next_action(file_path: str, smells: list[dict[str, Any]])` — [`L316`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L316) — Suggest the next action for D/F grade files.
- `_weakest_dimension_score(dimensions: dict[str, float])` — [`L474`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L474) — Return the lowest health dimension and score for compact summaries.
- `build_file_health_result(file_path: str, health: Any, smells: list[dict[str, Any]], resolved: str, analysis: Any)` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L31) — Build the result dict from health data, smells, and optional extraction plan.

## Module values
- `_GRADE_THRESHOLDS` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L190)
- `_MAX_SMELL_PENALTY` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L189)
- `_SIGNAL_MAP` — [`L12`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L12)
- `_SMELL_SCORE_PENALTY` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L178)
- `_SMELL_SEVERITY_PENALTY` — [`L182`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_response.py#L182)

