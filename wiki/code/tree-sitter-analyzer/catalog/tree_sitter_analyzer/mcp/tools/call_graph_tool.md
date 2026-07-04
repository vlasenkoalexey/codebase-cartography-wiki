---
title: 'Module: tree_sitter_analyzer/mcp/tools/call_graph_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/call_graph_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.call_graph_tool`/
symbols:
  CodeGraphCallTool.execute: CodeGraphCallTool#execute().
  CodeGraphCallTool._get_call_graph: CodeGraphCallTool#_get_call_graph().
  CodeGraphCallTool: CodeGraphCallTool#
  _attach_call_graph_envelope: _attach_call_graph_envelope().
  _maybe_bare_name_hint: _maybe_bare_name_hint().
  CodeGraphCallTool._on_project_root_changed: CodeGraphCallTool#_on_project_root_changed().
  CodeGraphCallTool._call_graph: CodeGraphCallTool#_call_graph.
  CodeGraphCallTool.get_call_graph: CodeGraphCallTool#get_call_graph().
  CodeGraphCallTool._explain_fingerprint_delta: CodeGraphCallTool#_explain_fingerprint_delta().
  CodeGraphCallTool._cache_invalidated_reason: CodeGraphCallTool#_cache_invalidated_reason.
  CodeGraphCallTool._call_graph_fingerprint: CodeGraphCallTool#_call_graph_fingerprint.
  CodeGraphCallTool.validate_arguments: CodeGraphCallTool#validate_arguments().
  CodeGraphCallTool.call_graph_initialized: CodeGraphCallTool#call_graph_initialized().
  CodeGraphCallTool._call_graph_built_at: CodeGraphCallTool#_call_graph_built_at.
  _apply_call_graph_agent_summary: _apply_call_graph_agent_summary().
  CodeGraphCallTool._build_callers_response: CodeGraphCallTool#_build_callers_response().
  CodeGraphCallTool._build_callees_response: CodeGraphCallTool#_build_callees_response().
  CodeGraphCallTool._build_chain_response: CodeGraphCallTool#_build_chain_response().
  CodeGraphCallTool._VALID_MODES: CodeGraphCallTool#_VALID_MODES.
  logger: logger.
  CodeGraphCallTool.get_tool_definition: CodeGraphCallTool#get_tool_definition().
  _SYMBOL_RESOLVING_MODES: _SYMBOL_RESOLVING_MODES.
  _result_is_empty_for_mode: _result_is_empty_for_mode().
  _call_graph_summary_line: _call_graph_summary_line().
  CodeGraphCallTool.get_tool_schema: CodeGraphCallTool#get_tool_schema().
  CodeGraphCallTool._FILE_PATH_MODES: CodeGraphCallTool#_FILE_PATH_MODES.
  CodeGraphCallTool._build_all_functions_response: CodeGraphCallTool#_build_all_functions_response().
  CodeGraphCallTool._build_file_impact_response: CodeGraphCallTool#_build_file_impact_response().
  CodeGraphCallTool._build_functions_in_file_response: CodeGraphCallTool#_build_functions_in_file_response().
  CodeGraphCallTool.__init__: CodeGraphCallTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/call_graph_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py)

## Classes
### `CodeGraphCallTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/call_graph_tool.py:242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L242)
- doc: MCP Tool for function-level call graph analysis.
- signature: `class CodeGraphCallTool(BaseMCPTool):`
- members:
  - `_build_all_functions_response(graph: Any)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L451) — M7: mode-named ``all_functions`` key + ``functions`` deprecated alias.
  - `_build_callees_response(graph: Any, arguments: dict[str, Any])` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L484) — Return callees of ``function_name`` with H2 ``function_indexed`` echo.
  - `_build_callers_response(graph: Any, arguments: dict[str, Any])` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L463) — Return callers of ``function_name`` with H2 ``function_indexed`` echo.
  - `_build_chain_response(graph: Any, arguments: dict[str, Any])` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L505) — Return the full call-chain DAG up to ``depth``.
  - `_build_file_impact_response(graph: Any, arguments: dict[str, Any])` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L526) — Return upstream/downstream impact summary for a file.
  - `_build_functions_in_file_response(graph: Any, arguments: dict[str, Any])` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L539) — Return all functions defined in the given file.
  - `_explain_fingerprint_delta(old: GraphFingerprint | None, new: GraphFingerprint)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L297) — Best-effort human-readable reason the cache was invalidated.
  - `call_graph_initialized(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L292) — True if the call graph has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L400) — Dispatch call-graph queries by ``mode``.
  - `get_call_graph(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L287) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `get_tool_definition(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L312)
  - `get_tool_schema(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L335)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L387)
- protocol/private: `_FILE_PATH_MODES`[`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L385), `_VALID_MODES`[`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L376), `__init__`[`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L245), `_cache_invalidated_reason`[`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L252), `_call_graph`[`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L246), `_call_graph_built_at`[`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L251), `_call_graph_fingerprint`[`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L250), `_get_call_graph`[`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L261), `_on_project_root_changed`[`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L255)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`compute_graph_fingerprint`](../../_graph_cache_fingerprint.md#compute_graph_fingerprint), [`file_count`](../../_graph_cache_fingerprint.md#GraphFingerprint.file_count), [`summary`](../../call_graph.md#CallGraph.summary), [`GraphFingerprint`](../../_graph_cache_fingerprint.md#GraphFingerprint), [`_attach_call_graph_envelope`](call_graph_tool.md#_attach_call_graph_envelope), [`_maybe_bare_name_hint`](call_graph_tool.md#_maybe_bare_name_hint), [`max_mtime_ns`](../../_graph_cache_fingerprint.md#GraphFingerprint.max_mtime_ns)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`_callees_route`](nav_facade.md#build_nav_facade._callees_route), [`_callers_route`](nav_facade.md#build_nav_facade._callers_route)  (8 test-only)

## Functions
- `_apply_call_graph_agent_summary(result: dict[str, Any], summary_line: str, mode: str, is_not_found: bool)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L111) — Populate ``result['agent_summary']`` with next_step + verdict + summary_line.
- `_attach_call_graph_envelope(result: dict[str, Any])` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L162) — Populate the canonical agent_summary + summary_line for call_graph.
- `_call_graph_summary_line(result: dict[str, Any], mode: str, func: str)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L60) — Build the per-mode ``summary_line`` for call_graph responses.
- `_maybe_bare_name_hint(graph: CallGraph, func_name: str, hit_count: int, mode: str)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L202) — Return a hint string when a qualified ``Class.method`` lookup returns
- `_result_is_empty_for_mode(result: dict[str, Any], mode: str)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L27) — Return True when the response represents a not-found lookup.

## Module values
- `_SYMBOL_RESOLVING_MODES` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L24)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_graph_tool.py#L18)

