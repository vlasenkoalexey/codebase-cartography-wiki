---
title: 'Module: tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.refactoring_suggestions_tool`/
symbols:
  RefactoringSuggestionsTool.execute: RefactoringSuggestionsTool#execute().
  RefactoringSuggestionsTool._build_suggestions_for_source: RefactoringSuggestionsTool#_build_suggestions_for_source().
  RefactoringSuggestionsTool: RefactoringSuggestionsTool#
  RefactoringSuggestionsTool._check_language_mismatch: RefactoringSuggestionsTool#_check_language_mismatch().
  _surface_security_and_anti_patterns: _surface_security_and_anti_patterns().
  RefactoringSuggestionsTool._read_source_or_error: RefactoringSuggestionsTool#_read_source_or_error().
  RefactoringSuggestionsTool._echo_detected_language: RefactoringSuggestionsTool#_echo_detected_language().
  _collect_security_and_anti_pattern_findings: _collect_security_and_anti_pattern_findings().
  RefactoringSuggestionsTool.get_tool_schema: RefactoringSuggestionsTool#get_tool_schema().
  _finding_to_refactor_suggestion: _finding_to_refactor_suggestion().
  logger: logger.
  RefactoringSuggestionsTool.get_tool_definition: RefactoringSuggestionsTool#get_tool_definition().
  _PATTERN_RULES._PATTERN_RULES: _PATTERN_RULES._PATTERN_RULES.
  _EXTRACTABLE_PATTERNS._EXTRACTABLE_PATTERNS: _EXTRACTABLE_PATTERNS._EXTRACTABLE_PATTERNS.
  _REFACTOR_SEVERITY_MAP._REFACTOR_SEVERITY_MAP: _REFACTOR_SEVERITY_MAP._REFACTOR_SEVERITY_MAP.
  RefactoringSuggestionsTool.validate_arguments: RefactoringSuggestionsTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py)

## Classes
### `RefactoringSuggestionsTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L97)
- doc: MCP Tool that provides concrete refactoring suggestions for source files.
- signature: `class RefactoringSuggestionsTool(BaseMCPTool):`
- members:
  - `_build_suggestions_for_source(self, resolved: str, source: str, include_extractions: bool)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L238) — Run tree-sitter analysis + python bonus + J9 cross-tool surfacing.
  - `_check_language_mismatch(self, resolved: str, file_path: str, explicit_language: str | None, output_format: str)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L202) — O8 gate: reject ``--language java`` on a ``.py`` file.
  - `_echo_detected_language(self, resolved: str, result: dict[str, Any])` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L269) — M14 (round-26): echo detected language so callers don't see None.
  - `_read_source_or_error(self, resolved: str, file_path: str)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L225) — Read source text; return an error envelope on failure.
  - `execute(self, arguments: dict[str, Any])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L152) — Execute refactoring analysis on a source file.
  - `get_tool_definition(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L101) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L147) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L287) — Validate file_path argument.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`extract_elements`](utils/element_extractor.md#extract_elements), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`build_success_response`](utils/refactoring_suggestions_helpers.md#build_success_response), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`analyze_treesitter_patterns`](utils/refactoring_suggestions_treesitter.md#analyze_treesitter_patterns), [`build_precise_plans`](_refactoring_plan_builder.md#build_precise_plans), [`python_bonus_analysis`](utils/refactoring_suggestions_python.md#python_bonus_analysis), [`_surface_security_and_anti_patterns`](refactoring_suggestions_tool.md#_surface_security_and_anti_patterns), [`error_response`](utils/refactoring_suggestions_helpers.md#error_response), [`_EXTRACTABLE_PATTERNS`](refactoring_suggestions_tool.md#_EXTRACTABLE_PATTERNS._EXTRACTABLE_PATTERNS), [`_PATTERN_RULES`](refactoring_suggestions_tool.md#_PATTERN_RULES._PATTERN_RULES), [`get_refactoring_tool_schema`](utils/refactoring_suggestions_helpers.md#get_refactoring_tool_schema)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (2 test-only)

## Functions
- `_collect_security_and_anti_pattern_findings(resolved: str, language: str)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L306) — Run both detectors against ``resolved``; never raise.
- `_finding_to_refactor_suggestion(finding: dict[str, Any])` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L327) — Map one ``code_patterns`` finding to the refactor suggestion contract.
- `_surface_security_and_anti_patterns(resolved: str, suggestions: list[dict[str, Any]], *, file_path: str)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L359) — J9: append code_patterns findings as refactor suggestions.

## Module values
- `_EXTRACTABLE_PATTERNS` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L67)
- `_PATTERN_RULES` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L35)
- `_REFACTOR_SEVERITY_MAP` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L299)
- `logger` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/refactoring_suggestions_tool.py#L33)

