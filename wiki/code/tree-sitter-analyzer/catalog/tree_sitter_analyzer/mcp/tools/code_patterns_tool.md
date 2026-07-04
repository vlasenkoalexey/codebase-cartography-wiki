---
title: 'Module: tree_sitter_analyzer/mcp/tools/code_patterns_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/code_patterns_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.code_patterns_tool`/
symbols:
  CodePatternsTool.execute: CodePatternsTool#execute().
  CodePatternsTool: CodePatternsTool#
  CodePatternsTool._collect_patterns: CodePatternsTool#_collect_patterns().
  _detect_smells: _detect_smells().
  _detect_anti_patterns: _detect_anti_patterns().
  _SEVERITY_ORDER: _SEVERITY_ORDER.
  _detect_security: _detect_security().
  _build_summary: _build_summary().
  _syntax_error_response: _syntax_error_response().
  CodePatternsTool.get_tool_schema: CodePatternsTool#get_tool_schema().
  CodePatternsTool.validate_arguments: CodePatternsTool#validate_arguments().
  CodePatternsTool.get_tool_definition: CodePatternsTool#get_tool_definition().
  _filter_and_sort_patterns: _filter_and_sort_patterns().
  _build_code_patterns_response: _build_code_patterns_response().
  _dedup_security_mirror: _dedup_security_mirror().
  _is_security_mirror_smell: _is_security_mirror_smell().
  _empty_file_response: _empty_file_response().
  logger: logger.
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/code_patterns_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py)

## Classes
### `CodePatternsTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/code_patterns_tool.py:84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L84)
- doc: Detect code patterns, anti-patterns, and security issues in a file.
- signature: `class CodePatternsTool(BaseMCPTool):`
- members:
  - `_collect_patterns(self, resolved: str, language: str | None, categories: list[str])` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L165) — Run the 3 category detectors per ``categories``, then G4-dedup.
  - `execute(self, arguments: dict[str, Any])` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L119) — Scan a file for code-quality patterns. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_definition(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L90)
  - `get_tool_schema(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L87)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L109)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`_detect_anti_patterns`](code_patterns_tool.md#_detect_anti_patterns), [`_detect_smells`](code_patterns_tool.md#_detect_smells), [`_SEVERITY_ORDER`](code_patterns_tool.md#_SEVERITY_ORDER), [`_detect_security`](code_patterns_tool.md#_detect_security), [`_syntax_error_response`](code_patterns_tool.md#_syntax_error_response), [`_build_code_patterns_response`](code_patterns_tool.md#_build_code_patterns_response), [`_dedup_security_mirror`](code_patterns_tool.md#_dedup_security_mirror), [`_empty_file_response`](code_patterns_tool.md#_empty_file_response), [`_filter_and_sort_patterns`](code_patterns_tool.md#_filter_and_sort_patterns), [`TOOL_SCHEMA`](code_patterns_tool.md#TOOL_SCHEMA.TOOL_SCHEMA)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_health_facade`](health_facade.md#build_health_facade)  (43 test-only)

## Functions
- `_build_code_patterns_response(*, file_path: str, language: str | None, filtered: list[dict[str, Any]])` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L195) — Assemble the canonical code_patterns envelope from a filtered findings list.
- `_build_summary(patterns: list[dict[str, Any]])` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L490)
- `_dedup_security_mirror(patterns: list[dict[str, Any]])` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L269) — Remove duplicate findings across smell / security / anti-pattern passes.
- `_detect_anti_patterns(file_path: str, language: str)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L475) — Wrap shared ``detect_anti_patterns`` and stamp ``category=anti_patterns``.
- `_detect_security(file_path: str, language: str)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L438)
- `_detect_smells(file_path: str, language: str, project_root: str | None = None)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L368)
- `_empty_file_response(resolved: str, file_path: str, output_format: str)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L509) — Pol2 (round-21): mirror ``file_health_tool._empty_file_response``.
- `_filter_and_sort_patterns(patterns: list[dict[str, Any]], min_sev: int)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L184) — Drop patterns below ``min_sev`` and sort the rest by severity descending.
- `_is_security_mirror_smell(pattern: dict[str, Any], security_keys: set[tuple[int | None, str]])` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L341) — Return True when ``pattern`` is the smell-side mirror of a security finding.
- `_syntax_error_response(resolved: str, file_path: str, language: str | None, output_format: str)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L580) — M3 (round-26): short-circuit when tree-sitter reports a syntax error.

## Module values
- `TOOL_SCHEMA` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L49)
- `_SEVERITY_ORDER` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L81)
- `__all__` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L36)
- `logger` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/code_patterns_tool.py#L47)

