---
title: 'Module: tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.get_project_summary_tool`/
symbols:
  GetProjectSummaryTool._execute_json: GetProjectSummaryTool#_execute_json().
  GetProjectSummaryTool.execute: GetProjectSummaryTool#execute().
  GetProjectSummaryTool: GetProjectSummaryTool#
  GetProjectSummaryTool._execute_toon: GetProjectSummaryTool#_execute_toon().
  _build_project_summary_line: _build_project_summary_line().
  _emit_header_block: _emit_header_block().
  _make_quick_start: _make_quick_start().
  _emit_structure_block: _emit_structure_block().
  _top_code_languages: _top_code_languages().
  GetProjectSummaryTool._read_or_render_toon: GetProjectSummaryTool#_read_or_render_toon().
  GetProjectSummaryTool._append_custom_notes_if_needed: GetProjectSummaryTool#_append_custom_notes_if_needed().
  _format_toon: _format_toon().
  GetProjectSummaryTool.get_tool_definition: GetProjectSummaryTool#get_tool_definition().
  _append_subdir_lines: _append_subdir_lines().
  _toon_envelope: _toon_envelope().
  _NON_CODE_LANGUAGES._NON_CODE_LANGUAGES: _NON_CODE_LANGUAGES._NON_CODE_LANGUAGES.
  _DIR_COL._DIR_COL: _DIR_COL._DIR_COL.
  GetProjectSummaryTool.get_tool_schema: GetProjectSummaryTool#get_tool_schema().
  GetProjectSummaryTool.validate_arguments: GetProjectSummaryTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py)

## Classes
### `GetProjectSummaryTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py:201`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L201)
- doc: MCP tool that returns a persistent cross-session architecture overview.
- signature: `class GetProjectSummaryTool(BaseMCPTool):`
- members:
  - `_append_custom_notes_if_needed(text: str, manager: ProjectIndexManager, include_notes: bool)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L348) — Append ``custom_notes`` to the TOON text when the index has them.
  - `_execute_json(self, manager: ProjectIndexManager, project_root: str, force_refresh: bool, include_notes: bool)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L377) — JSON path — load (or build) the full index, attach the canonical envelope.
  - `_execute_toon(self, manager: ProjectIndexManager, project_root: str, force_refresh: bool, include_notes: bool)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L316) — TOON path — return the pre-rendered summary.toon when possible.
  - `_read_or_render_toon(manager: ProjectIndexManager, project_root: str, index: ProjectIndex, include_notes: bool)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L365) — Return TOON text — read pre-rendered file when present, else render now.
  - `execute(self, arguments: dict[str, Any])` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L292) — Load (or build) the project index and return a summary.
  - `get_tool_definition(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L255)
  - `get_tool_schema(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L204)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L289)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`ProjectIndexManager`](../utils/project_index/_manager.md#ProjectIndexManager), [`build`](../utils/project_index/_manager.md#ProjectIndexManager.build), [`load`](../utils/project_index/_manager.md#ProjectIndexManager.load), [`ProjectIndex`](../utils/project_index/_models.md#ProjectIndex), [`_build_project_summary_line`](get_project_summary_tool.md#_build_project_summary_line), [`render_toon`](../utils/project_index/_manager.md#ProjectIndexManager.render_toon), [`custom_notes`](../utils/project_index/_models.md#ProjectIndex.custom_notes), [`language_distribution`](../utils/project_index/_models.md#ProjectIndex.language_distribution), [`updated_at`](../utils/project_index/_models.md#ProjectIndex.updated_at), [`_make_quick_start`](get_project_summary_tool.md#_make_quick_start), [`file_count`](../utils/project_index/_models.md#ProjectIndex.file_count), [`entry_points`](../utils/project_index/_models.md#ProjectIndex.entry_points), [`module_descriptions`](../utils/project_index/_models.md#ProjectIndex.module_descriptions), [`readme_excerpt`](../utils/project_index/_models.md#ProjectIndex.readme_excerpt), [`key_files`](../utils/project_index/_models.md#ProjectIndex.key_files), [`top_level_structure`](../utils/project_index/_models.md#ProjectIndex.top_level_structure), [`critical_nodes`](../utils/project_index/_models.md#ProjectIndex.critical_nodes), [`project_root`](../utils/project_index/_models.md#ProjectIndex.project_root), [`TOON_FILE`](../utils/project_index/_manager.md#ProjectIndexManager.TOON_FILE), [`_toon_envelope`](get_project_summary_tool.md#_toon_envelope)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments)  (18 test-only)

## Functions
- `_append_subdir_lines(name: str, subdirs: list[dict[str, Any]], descs: dict[str, str], lines: list[str])` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L68) — Append described depth-2 subdirectories of ``name`` (up to 5).
- `_build_project_summary_line(idx: ProjectIndex | None, project_root: str)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L427) — Build the (summary_line, next_step) tuple for get_project_summary.
- `_emit_header_block(index: ProjectIndex, lines: list[str])` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L46) — Append the ``project`` / ``purpose`` / ``language`` / ``entry`` / ``config`` block.
- `_emit_structure_block(index: ProjectIndex, lines: list[str])` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L86) — Append the ``structure:`` block — up to 10 top-level dirs with descriptions.
- `_format_toon(index: ProjectIndex, age_hours: float, is_fresh: bool)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L116) — Render project summary as TOON-style structured text.
- `_make_quick_start(index: ProjectIndex)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L158) — Generate a one-line orientation sentence (≤100 chars).
- `_toon_envelope(resolved_fmt: str, text: str, summary_line: str, next_step: str)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L131) — Construct the canonical TOON-path envelope.
- `_top_code_languages(index: ProjectIndex)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L28) — Return up to top-3 real programming languages by file count.

## Module values
- `_DIR_COL` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L25)
- `_NON_CODE_LANGUAGES` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_project_summary_tool.py#L19)

