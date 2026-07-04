---
title: 'Module: tree_sitter_analyzer/mcp/tools/change_impact_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/change_impact_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.change_impact_tool`/
symbols:
  ChangeImpactTool.execute: ChangeImpactTool#execute().
  ChangeImpactTool._execute_pr_analysis: ChangeImpactTool#_execute_pr_analysis().
  ChangeImpactTool: ChangeImpactTool#
  ChangeImpactTool._finalize_pr_result: ChangeImpactTool#_finalize_pr_result().
  _enrich_with_journal_decisions: _enrich_with_journal_decisions().
  ChangeImpactTool.validate_arguments: ChangeImpactTool#validate_arguments().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  _canonicalize_change_impact_verdict: _canonicalize_change_impact_verdict().
  _JOURNAL_VERDICT_RANK._JOURNAL_VERDICT_RANK: _JOURNAL_VERDICT_RANK._JOURNAL_VERDICT_RANK.
  _scope_paths_invalid: _scope_paths_invalid().
  ChangeImpactTool.get_tool_schema: ChangeImpactTool#get_tool_schema().
  _pr_invalid_url_envelope: _pr_invalid_url_envelope().
  _pr_gh_unavailable_envelope: _pr_gh_unavailable_envelope().
  ChangeImpactTool.get_tool_definition: ChangeImpactTool#get_tool_definition().
  _resolve_scope_path: _resolve_scope_path().
---
# Module: [`tree_sitter_analyzer/mcp/tools/change_impact_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py)

## Classes
### `ChangeImpactTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/change_impact_tool.py:277`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L277)
- doc: Analyze the impact of code changes using git diff + dependency graph.
- signature: `class ChangeImpactTool(BaseMCPTool):`
- members:
  - `_execute_pr_analysis(self, pr_url: str, include_tests: bool, output_format: str, scope_paths: list[str], agent_summary_only: bool, *, scope_mode: str = "report", resource_profile: str = "default", compact_only: bool = False)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L459) — Analyze a GitHub PR's diff via gh CLI.
  - `_finalize_pr_result(result: dict[str, Any], *, parsed: Any, scope_paths: list[str], scope_paths_invalid: Any, changed_files: list[str], agent_summary_only: bool, output_format: str, scope_mode: str = "report", compact_only: bool = False)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L536) — Attach PR metadata + queue ledger + scope validation, mirror, and TOON.
  - `execute(self, arguments: dict[str, Any])` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L348) — Analyze git diff + dependency graph for change impact. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_definition(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L284) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L280) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L327) — Validate mode + scope_mode arguments.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`_build_change_impact_result`](utils/change_impact_analysis.md#_build_change_impact_result), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`parse_pr_url`](../../pr_url.md#parse_pr_url), [`changed_files`](utils/change_impact_analysis.md#ChangeImpactRequest.changed_files), [`apply_scope_validation`](utils/change_impact_response.md#apply_scope_validation), [`_get_changed_files`](utils/change_impact_git.md#_get_changed_files), [`project_root`](utils/change_impact_analysis.md#ChangeImpactRequest.project_root), [`attach_queue_ledger`](utils/change_impact_response.md#attach_queue_ledger), [`build_agent_summary_only_response`](utils/change_impact_response.md#build_agent_summary_only_response), [`ChangeImpactRequest`](utils/change_impact_analysis.md#ChangeImpactRequest), [`fetch_pr_changed_files`](../../pr_url.md#fetch_pr_changed_files), [`fetch_pr_diff_stat`](../../pr_url.md#fetch_pr_diff_stat), [`_enrich_with_journal_decisions`](change_impact_tool.md#_enrich_with_journal_decisions), [`_get_diff_stat`](utils/change_impact_git.md#_get_diff_stat), [`check_gh_available`](../../pr_url.md#check_gh_available), [`build_no_changes_result`](utils/change_impact_response.md#build_no_changes_result), [`include_tests`](utils/change_impact_analysis.md#ChangeImpactRequest.include_tests), [`mode`](utils/change_impact_analysis.md#ChangeImpactRequest.mode), [`diff_stat`](utils/change_impact_analysis.md#ChangeImpactRequest.diff_stat), [`resource_profile`](utils/change_impact_analysis.md#ChangeImpactRequest.resource_profile), [`TOOL_SCHEMA`](change_impact_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`agent_summary_only`](utils/change_impact_analysis.md#ChangeImpactRequest.agent_summary_only), [`scope_paths`](utils/change_impact_analysis.md#ChangeImpactRequest.scope_paths), [`_canonicalize_change_impact_verdict`](change_impact_tool.md#_canonicalize_change_impact_verdict), [`_scope_paths_invalid`](change_impact_tool.md#_scope_paths_invalid), [`_pr_gh_unavailable_envelope`](change_impact_tool.md#_pr_gh_unavailable_envelope), [`_pr_invalid_url_envelope`](change_impact_tool.md#_pr_invalid_url_envelope)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (33 test-only)

## Functions
- `_canonicalize_change_impact_verdict(result: dict[str, Any])` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L38) — Fold both verdict surfaces back to the shared legal vocabulary.
- `_enrich_with_journal_decisions(result: dict[str, Any], project_root: str | None, changed_files: list[str])` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L82) — Phase 3 (r37fG): surface related decision_journal entries.
- `_pr_gh_unavailable_envelope(parsed: Any, output_format: str)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L263) — Pre-flight failure envelope when ``gh`` CLI is missing or unauthenticated.
- `_pr_invalid_url_envelope(pr_url: str, output_format: str)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L246) — Pre-flight failure envelope when ``pr_url`` cannot be parsed.
- `_resolve_scope_path(project_root: str | None, raw: str)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L145) — Resolve a user-supplied scope path against the project root.
- `_scope_paths_invalid(project_root: str | None, scope_paths: list[str])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L160) — Return the subset of ``scope_paths`` that do not exist on disk.

## Module values
- `TOOL_SCHEMA` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L173)
- `_JOURNAL_VERDICT_RANK` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/change_impact_tool.py#L70)

