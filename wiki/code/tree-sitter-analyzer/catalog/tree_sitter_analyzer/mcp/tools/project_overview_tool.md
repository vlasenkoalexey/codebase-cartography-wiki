---
title: 'Module: tree_sitter_analyzer/mcp/tools/project_overview_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/project_overview_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.project_overview_tool`/
symbols:
  ProjectOverviewTool: ProjectOverviewTool#
  ProjectOverviewTool.execute: ProjectOverviewTool#execute().
  _scan_project: _scan_project().
  _build_result: _build_result().
  _add_file_to_scan: _add_file_to_scan().
  _add_path_to_scan: _add_path_to_scan().
  _build_smart_hint: _build_smart_hint().
  _new_scan: _new_scan().
  _build_agent_summary: _build_agent_summary().
  _load_gitignore_patterns: _load_gitignore_patterns().
  _is_ignored_by_gitignore: _is_ignored_by_gitignore().
  _add_health_data: _add_health_data().
  _overview_risk: _overview_risk().
  _suggest_refactor_action: _suggest_refactor_action().
  _build_tool_routing: _build_tool_routing().
  ProjectOverviewTool.validate_arguments: ProjectOverviewTool#validate_arguments().
  _increment: _increment().
  _health_opt_in_hint: _health_opt_in_hint().
  _overview_risk_to_verdict: _overview_risk_to_verdict().
  _overview_next_step: _overview_next_step().
  _count_lines: _count_lines().
  _build_base_result: _build_base_result().
  _build_health_alert: _build_health_alert().
  _top_language: _top_language().
  logger: logger.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _is_language_count_excluded: _is_language_count_excluded().
  ProjectOverviewTool.get_tool_definition: ProjectOverviewTool#get_tool_definition().
  ProjectOverviewTool.get_tool_schema: ProjectOverviewTool#get_tool_schema().
  _score_health_entry: _score_health_entry().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  _SUPPORTED_EXTS: _SUPPORTED_EXTS.
  _LANGUAGE_TO_EXT: _LANGUAGE_TO_EXT.
  _LANGUAGE_COUNT_EXCLUDED_SEGMENTS._LANGUAGE_COUNT_EXCLUDED_SEGMENTS: _LANGUAGE_COUNT_EXCLUDED_SEGMENTS._LANGUAGE_COUNT_EXCLUDED_SEGMENTS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/project_overview_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py)

## Classes
### `ProjectOverviewTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/project_overview_tool.py:148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L148)
- doc: MCP Tool that gives AI agents a complete project portrait in one call.
- signature: `class ProjectOverviewTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L198) — Execute project scan and build result with optional health data.
  - `get_tool_definition(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L151) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L186) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L190) — Validate max_depth argument.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`_scan_project`](project_overview_tool.md#_scan_project), [`_build_result`](project_overview_tool.md#_build_result), [`TOOL_SCHEMA`](project_overview_tool.md#TOOL_SCHEMA.TOOL_SCHEMA)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases)  (23 test-only)

## Functions
- `_add_file_to_scan(scan: dict[str, Any], root: Path, path: Path)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L350) — Add one source or non-source file to scan accumulators.
- `_add_health_data(result: dict[str, Any], source_files: list[dict[str, Any]], root: Path)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L443) — Add health grades for top source files.
- `_add_path_to_scan(scan: dict[str, Any], root: Path, path: Path, max_depth: int, gitignore_spec: pathspec.PathSpec | None = None)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L314) — Add a path to project scan accumulators when it is in scope.
- `_build_agent_summary(result: dict[str, Any], include_health: bool)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L488) — Build a compact project-overview summary for first-hop agent decisions.
- `_build_base_result(root: Path, scan: dict[str, Any])` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L402) — Build the health-independent overview response.
- `_build_health_alert(unhealthy: list[dict[str, Any]])` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L483)
- `_build_result(root: Path, scan: dict[str, Any], include_health: bool)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L384) — Build the result dict from scan data.
- `_build_smart_hint(result: dict[str, Any])` — [`L724`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L724) — Build smart workflow hint from health and language data.
- `_build_tool_routing()` — [`L646`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L646) — Return the static MCP tool routing guide.
- `_count_lines(path: Path)` — [`L698`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L698) — Count lines in a file using UTF-8 encoding.
- `_health_opt_in_hint()` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L436)
- `_increment(counts: dict[str, int], key: str)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L380)
- `_is_ignored_by_gitignore(rel_path: str, gitignore_spec: pathspec.PathSpec | None)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L252) — Check if a relative path matches any gitignore patterns.
- `_is_language_count_excluded(rel_path: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L118) — True if ``rel_path`` should not influence language_distribution.
- `_load_gitignore_patterns(root: Path)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L224) — Load .gitignore patterns from the project root.
- `_new_scan()` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L304) — Return mutable scan accumulators.
- `_overview_next_step(result: dict[str, Any], include_health: bool)` — [`L627`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L627)
- `_overview_risk(result: dict[str, Any], include_health: bool)` — [`L552`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L552) — Infer project risk from observable signals (F11 fix).
- `_overview_risk_to_verdict(risk: str)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L525) — Map project-overview risk to the cross-tool verdict vocabulary.
- `_scan_project(root: Path, max_depth: int)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L272) — Walk the project tree and collect file/directory stats.
- `_score_health_entry(scorer: Any, root: Path, source_file: dict[str, Any])` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L461) — Score one source file for project overview health output.
- `_suggest_refactor_action(file_path: str, line_count: int, health: Any)` — [`L707`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L707) — Suggest refactoring action based on file type and size.
- `_top_language(language_distribution: dict[str, int])` — [`L640`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L640)

## Module values
- `TOOL_SCHEMA` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L124)
- `_EXCLUDE_DIRS` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L72)
- `_LANGUAGE_COUNT_EXCLUDED_SEGMENTS` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L89)
- `_LANGUAGE_TO_EXT` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L48)
- `_SUPPORTED_EXTS` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L20)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/project_overview_tool.py#L18)

