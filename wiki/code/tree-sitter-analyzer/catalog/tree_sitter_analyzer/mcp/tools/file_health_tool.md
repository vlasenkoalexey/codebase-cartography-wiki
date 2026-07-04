---
title: 'Module: tree_sitter_analyzer/mcp/tools/file_health_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/file_health_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.file_health_tool`/
symbols:
  FileHealthTool.execute: FileHealthTool#execute().
  FileHealthTool: FileHealthTool#
  FileHealthTool._score_and_echo_metrics: FileHealthTool#_score_and_echo_metrics().
  FileHealthTool._check_early_exit_paths: FileHealthTool#_check_early_exit_paths().
  FileHealthTool._scorer: FileHealthTool#_scorer.
  _file_metrics: _file_metrics().
  FileHealthTool._get_scorer: FileHealthTool#_get_scorer().
  FileHealthTool._resolve_language_for_health: FileHealthTool#_resolve_language_for_health().
  _non_code_file_response: _non_code_file_response().
  _syntax_error_response: _syntax_error_response().
  FileHealthTool.get_tool_definition: FileHealthTool#get_tool_definition().
  FileHealthTool.get_tool_schema: FileHealthTool#get_tool_schema().
  _empty_file_response: _empty_file_response().
  _looks_binary: _looks_binary().
  _binary_file_response: _binary_file_response().
  FileHealthTool.validate_arguments: FileHealthTool#validate_arguments().
  logger: logger.
  FileHealthTool._on_project_root_changed: FileHealthTool#_on_project_root_changed().
  _NON_CODE_EXTENSIONS._NON_CODE_EXTENSIONS: _NON_CODE_EXTENSIONS._NON_CODE_EXTENSIONS.
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  FileHealthTool.__init__: FileHealthTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/file_health_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py)

## Classes
### `FileHealthTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/file_health_tool.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L87)
- doc: MCP Tool for file-level code health scoring with code smell detection.
- signature: `class FileHealthTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L90) — Initialize with optional project root for path resolution.
  - `_check_early_exit_paths(self, resolved: str, file_path: str, language: str | None, output_format: str)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L218) — Run O3 / H7 / M7+H9 guards. Return first matching envelope or ``None``.
  - `_get_scorer(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L99) — Get or create the HealthScorer instance.
  - `_resolve_language_for_health(self, resolved: str, language: str | None)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L253) — Best-effort language detection when caller didn't pass ``language``.
  - `_score_and_echo_metrics(self, resolved: str, file_path: str, language: str | None, analysis: Any)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L264) — Run HealthScorer + detect_code_smells, then attach M14/N9 echoes.
  - `execute(self, arguments: dict[str, Any])` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L166) — Execute health scoring and code smell detection.
  - `get_tool_definition(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L106) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema()` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L151) — Return the JSON schema for tool input validation.
  - `validate_arguments(arguments: dict[str, Any])` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L157) — Validate file_path argument.
- protocol/private: `_on_project_root_changed`[`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L95), `_scorer`[`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L92)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`HealthScorer`](../../health_scorer.md#HealthScorer), [`extract_elements`](utils/element_extractor.md#extract_elements), [`score_file`](../../health_scorer.md#HealthScorer.score_file), [`detect_code_smells`](utils/file_health_smells.md#detect_code_smells), [`build_file_health_result`](utils/file_health_response.md#build_file_health_result), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`dimensions`](../../health_scorer.md#HealthScore.dimensions), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`_file_metrics`](file_health_tool.md#_file_metrics), [`_non_code_file_response`](file_health_tool.md#_non_code_file_response), [`_syntax_error_response`](file_health_tool.md#_syntax_error_response), [`_binary_file_response`](file_health_tool.md#_binary_file_response), [`_empty_file_response`](file_health_tool.md#_empty_file_response), [`_looks_binary`](file_health_tool.md#_looks_binary), [`TOOL_SCHEMA`](file_health_tool.md#TOOL_SCHEMA.TOOL_SCHEMA)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases)  (12 test-only)

## Functions
- `_binary_file_response(file_path: str, resolved: str)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L518) — Return an error envelope refusing to analyze a binary file.
- `_empty_file_response(resolved: str, file_path: str)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L338) — Return an n/a envelope when ``resolved`` is empty or whitespace-only.
- `_file_metrics(resolved: str)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L295) — N9 (round-28): compute ``line_count`` + ``binary`` for the envelope.
- `_looks_binary(resolved: str, language: str | None, analysis: Any)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L455) — Heuristic: is ``resolved`` a non-source / binary file?
- `_non_code_file_response(resolved: str, file_path: str)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L406) — Return an n/a envelope when ``resolved`` is a non-code file.
- `_syntax_error_response(resolved: str, file_path: str, language: str | None)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L541) — M3 (round-26): short-circuit when tree-sitter detected syntax errors.

## Module values
- `TOOL_SCHEMA` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L55)
- `_NON_CODE_EXTENSIONS` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L39)
- `logger` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/file_health_tool.py#L31)

