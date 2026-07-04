---
title: 'Module: tree_sitter_analyzer/mcp/tools/trace_impact_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/trace_impact_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.trace_impact_tool`/
symbols:
  TraceImpactTool.execute: TraceImpactTool#execute().
  TraceImpactTool: TraceImpactTool#
  _filter_comment_docstring_matches: _filter_comment_docstring_matches().
  _is_symbol_only_in_strings: _is_symbol_only_in_strings().
  _file_non_code_lines: _file_non_code_lines().
  _build_trace_impact_result: _build_trace_impact_result().
  TraceImpactTool._detect_language_filter: TraceImpactTool#_detect_language_filter().
  _get_impact_level: _get_impact_level().
  TraceImpactTool._get_extensions_for_language: TraceImpactTool#_get_extensions_for_language().
  _python_non_code_lines: _python_non_code_lines().
  TraceImpactTool.validate_arguments: TraceImpactTool#validate_arguments().
  TraceImpactTool.get_tool_definition: TraceImpactTool#get_tool_definition().
  TraceImpactTool.language_detector: TraceImpactTool#language_detector.
  logger: logger.
  _filter_source_matches: _filter_source_matches().
  _is_source_file: _is_source_file().
  _build_trace_impact_globs: _build_trace_impact_globs().
  _build_not_found_response: _build_not_found_response().
  TraceImpactTool.get_tool_schema: TraceImpactTool#get_tool_schema().
  TraceImpactTool._resolve_search_roots: TraceImpactTool#_resolve_search_roots().
  _SOURCE_EXT_GLOBS._SOURCE_EXT_GLOBS: _SOURCE_EXT_GLOBS._SOURCE_EXT_GLOBS.
  TraceImpactTool.__init__: TraceImpactTool#__init__().
  _PY_LIKE_EXTS: _PY_LIKE_EXTS.
  _C_LIKE_EXTS: _C_LIKE_EXTS.
  _PY_TRIPLE_QUOTE_RE: _PY_TRIPLE_QUOTE_RE.
  _c_like_non_code_lines: _c_like_non_code_lines().
  _classify_rg_error: _classify_rg_error().
  _truncate_for_display: _truncate_for_display().
  _matches_to_usages: _matches_to_usages().
  _verdict_and_next_step_for_impact: _verdict_and_next_step_for_impact().
  _trace_impact_base_envelope: _trace_impact_base_envelope().
  _trace_impact_apply_conditional_fields: _trace_impact_apply_conditional_fields().
  _TRACE_IMPACT_DESCRIPTION._TRACE_IMPACT_DESCRIPTION: _TRACE_IMPACT_DESCRIPTION._TRACE_IMPACT_DESCRIPTION.
  _TRACE_IMPACT_INPUT_SCHEMA._TRACE_IMPACT_INPUT_SCHEMA: _TRACE_IMPACT_INPUT_SCHEMA._TRACE_IMPACT_INPUT_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/trace_impact_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py)

## Classes
### `TraceImpactTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/trace_impact_tool.py:786`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L786)
- doc: MCP tool for tracing the impact of code changes by finding all usage sites of a symbol.
- signature: `class TraceImpactTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L794`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L794) — Initialize the trace impact tool.
  - `_detect_language_filter(self, file_path: str | None)` — [`L980`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L980) — Detect language from ``file_path`` and return (language, extensions).
  - `_get_extensions_for_language(self, language: str)` — [`L1000`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L1000) — Get file extensions for a given language.
  - `_resolve_search_roots(self, project_root_arg: str | None)` — [`L966`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L966) — Compute the project root list for ripgrep.
  - `execute(self, arguments: dict[str, Any])` — [`L882`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L882) — Execute the trace impact tool.
  - `get_tool_definition(self)` — [`L807`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L807) — Get the MCP tool definition for trace_impact.
  - `get_tool_schema(self)` — [`L804`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L804)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L828`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L828) — Validate input arguments.
  - `language_detector` — [`L802`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L802)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`build_rg_command`](fd_rg_utils.md#build_rg_command), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`LanguageDetector`](../../language_detector.md#LanguageDetector), [`parse_rg_json_lines_to_matches`](fd_rg_result_utils.md#parse_rg_json_lines_to_matches), [`run_command_capture`](fd_rg_utils.md#run_command_capture), [`_filter_comment_docstring_matches`](trace_impact_tool.md#_filter_comment_docstring_matches), [`_build_trace_impact_result`](trace_impact_tool.md#_build_trace_impact_result), [`EXTENSION_MAPPING`](../../language_detector.md#LanguageDetector.EXTENSION_MAPPING), [`logger`](trace_impact_tool.md#logger), [`_build_not_found_response`](trace_impact_tool.md#_build_not_found_response), [`_build_trace_impact_globs`](trace_impact_tool.md#_build_trace_impact_globs), [`_filter_source_matches`](trace_impact_tool.md#_filter_source_matches), [`_TRACE_IMPACT_DESCRIPTION`](trace_impact_tool.md#_TRACE_IMPACT_DESCRIPTION._TRACE_IMPACT_DESCRIPTION), [`_TRACE_IMPACT_INPUT_SCHEMA`](trace_impact_tool.md#_TRACE_IMPACT_INPUT_SCHEMA._TRACE_IMPACT_INPUT_SCHEMA), [`_classify_rg_error`](trace_impact_tool.md#_classify_rg_error), [`_matches_to_usages`](trace_impact_tool.md#_matches_to_usages), [`_truncate_for_display`](trace_impact_tool.md#_truncate_for_display)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_trace_impact_tool`](modification_guard_tool.md#ModificationGuardTool._trace_impact_tool), [`_run_trace_impact`](modification_guard_tool.md#ModificationGuardTool._run_trace_impact)  (31 test-only)

## Functions
- `_build_not_found_response(symbol: str, language: str | None)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L477) — M11: ripgrep returned zero matches → NOT_FOUND envelope.
- `_build_trace_impact_globs(language_extensions: list[str], exclude_patterns: list[str])` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L405) — Build (include_globs, exclude_globs) for ripgrep.
- `_build_trace_impact_result(*, symbol: str, language: str | None, file_path: str | None, usages: list[dict[str, Any]], source_total: int, true_total: int, truncated: bool, max_results: int)` — [`L649`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L649) — Compose the canonical trace_impact success envelope.
- `_c_like_non_code_lines(text: str)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L258) — Return 1-based line numbers that are ``//`` comments or inside ``/* */`` blocks.
- `_classify_rg_error(rc: int, stderr: bytes | None)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L437) — Map ripgrep exit code to an error envelope, or ``None`` on success/no-match.
- `_file_non_code_lines(file_path: str)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L292) — Read ``file_path`` once and compute the set of comment/docstring lines.
- `_filter_comment_docstring_matches(matches: list[dict[str, Any]], symbol: str = "")` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L315) — Drop hits whose line is inside a comment, docstring, import, or string.
- `_filter_source_matches(matches: list[dict[str, Any]])` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L43) — H4 fix: drop hits whose file extension is not in ``_SOURCE_EXTS``.
- `_get_impact_level(count: int)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L358) — Return a severity dict for a given caller count.
- `_is_source_file(file_path: str)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L59) — Return ``True`` if ``file_path`` ends with a known source extension.
- `_is_symbol_only_in_strings(line: str, symbol: str)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L162) — Return True if every occurrence of ``symbol`` in ``line`` is inside an
- `_matches_to_usages(matches: list[Any])` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L525) — Convert rg matches to usage dicts with both ``file``/``file_path`` aliases.
- `_python_non_code_lines(text: str)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L98)
- `_trace_impact_apply_conditional_fields(result: dict[str, Any], *, impact_level: str, source_total: int, true_total: int, language: str | None, file_path: str | None, truncated: bool, max_results: int)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L608) — Mutate ``result`` with optional fields based on signal flags.
- `_trace_impact_base_envelope(*, symbol: str, impact: dict[str, Any], source_total: int, true_total: int, usages: list[dict[str, Any]], summary_line: str, verdict: str, next_step: str)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L560) — Build the always-present canonical fields of the trace_impact envelope.
- `_truncate_for_display(source_matches: list[Any], max_results: int)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L516) — Display-cap source matches without affecting impact-level count.
- `_verdict_and_next_step_for_impact(level: str, total_count: int)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L543) — K5: map impact level (magnitude vocab) → (verdict, next_step) (safety vocab).

## Module values
- `_C_LIKE_EXTS` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L74)
- `_PY_LIKE_EXTS` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L73)
- `_PY_TRIPLE_QUOTE_RE` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L95)
- `_SOURCE_EXT_GLOBS` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L40)
- `_TRACE_IMPACT_DESCRIPTION` — [`L700`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L700)
- `_TRACE_IMPACT_INPUT_SCHEMA` — [`L726`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L726)
- `logger` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/trace_impact_tool.py#L32)

