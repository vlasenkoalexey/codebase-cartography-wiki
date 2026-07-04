---
title: 'Module: tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.analyze_code_structure_tool`/
symbols:
  AnalyzeCodeStructureTool: AnalyzeCodeStructureTool#
  AnalyzeCodeStructureTool.execute: AnalyzeCodeStructureTool#execute().
  AnalyzeCodeStructureTool._format_response: AnalyzeCodeStructureTool#_format_response().
  AnalyzeCodeStructureTool._prepare_execution_options: AnalyzeCodeStructureTool#_prepare_execution_options().
  AnalyzeCodeStructureTool._analyze_structure: AnalyzeCodeStructureTool#_analyze_structure().
  _build_next_steps: _build_next_steps().
  AnalyzeCodeStructureTool._save_output: AnalyzeCodeStructureTool#_save_output().
  AnalyzeCodeStructureTool.validate_arguments: AnalyzeCodeStructureTool#validate_arguments().
  _format_table: _format_table().
  _get_method_parameters: _get_method_parameters().
  _build_success_response: _build_success_response().
  AnalyzeCodeStructureTool._pre_validate_language_mismatch: AnalyzeCodeStructureTool#_pre_validate_language_mismatch().
  _attach_agent_summary: _attach_agent_summary().
  _convert_parameters: _convert_parameters().
  _base_success_response: _base_success_response().
  AnalyzeCodeStructureTool._on_project_root_changed: AnalyzeCodeStructureTool#_on_project_root_changed().
  _get_method_modifiers: _get_method_modifiers().
  _ExecutionOptions: _ExecutionOptions#
  _attach_parse_validity: _attach_parse_validity().
  AnalyzeCodeStructureTool.get_tool_definition: AnalyzeCodeStructureTool#get_tool_definition().
  _get_field_modifiers: _get_field_modifiers().
  AnalyzeCodeStructureTool._resolve_language: AnalyzeCodeStructureTool#_resolve_language().
  AnalyzeCodeStructureTool.file_output_manager: AnalyzeCodeStructureTool#file_output_manager.
  _validate_format_type: _validate_format_type().
  _complex_method_step: _complex_method_step().
  _suppress_table_output_if_requested: _suppress_table_output_if_requested().
  _output_base_name: _output_base_name().
  AnalyzeCodeStructureTool.analysis_engine: AnalyzeCodeStructureTool#analysis_engine.
  AnalyzeCodeStructureTool._sanitize_optional_arg: AnalyzeCodeStructureTool#_sanitize_optional_arg().
  _convert_analysis_result: _convert_analysis_result().
  _ExecutionOptions.file_path: _ExecutionOptions#file_path.
  _ExecutionOptions.language: _ExecutionOptions#language.
  _ExecutionOptions.output_file: _ExecutionOptions#output_file.
  _large_file_first_method_step: _large_file_first_method_step().
  _MethodData: _MethodData.
  _ExecutionOptions.format_type: _ExecutionOptions#format_type.
  _safe_int: _safe_int().
  logger: logger.
  _parse_string_param: _parse_string_param().
  _query_navigation_steps: _query_navigation_steps().
  _hoist_structure_keys: _hoist_structure_keys().
  AnalyzeCodeStructureTool.logger: AnalyzeCodeStructureTool#logger.
  AnalyzeCodeStructureTool.get_tool_schema: AnalyzeCodeStructureTool#get_tool_schema().
  _ExecutionOptions.resolved_path: _ExecutionOptions#resolved_path.
  _ExecutionOptions.output_format: _ExecutionOptions#output_format.
  analyze_code_structure_tool: analyze_code_structure_tool.
  _STATS_KEY: _STATS_KEY.
  _ANALYZE_ERR_PREFIX: _ANALYZE_ERR_PREFIX.
  _ExecutionOptions.suppress_output: _ExecutionOptions#suppress_output.
  _structure_items: _structure_items().
  _method_complexity: _method_complexity().
  _line_range: _line_range().
  _VALID_FORMAT_TYPES: _VALID_FORMAT_TYPES.
  _validate_optional_string: _validate_optional_string().
  _TOOL_NAME: _TOOL_NAME.
  _SAVE_ERR_MSG: _SAVE_ERR_MSG.
  _param_from_dict: _param_from_dict().
  _param_from_obj: _param_from_obj().
  _total_lines: _total_lines().
  _attach_next_steps: _attach_next_steps().
  _validate_required_file_path: _validate_required_file_path().
  _validate_suppress_output: _validate_suppress_output().
  _ensure_input_file_exists: _ensure_input_file_exists().
  _mark_file_saved: _mark_file_saved().
  _mark_file_save_error: _mark_file_save_error().
  _try_save_file: _try_save_file().
  _safe_resolve: _safe_resolve().
  _HOIST_KEYS: _HOIST_KEYS.
  _TOOL_DESCRIPTION: _TOOL_DESCRIPTION.
  _TOOL_ANNOTATIONS._TOOL_ANNOTATIONS: _TOOL_ANNOTATIONS._TOOL_ANNOTATIONS.
  AnalyzeCodeStructureTool.__init__: AnalyzeCodeStructureTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py)

## Classes
### `AnalyzeCodeStructureTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py:504`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L504) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Tool for code structure analysis and table formatting.
- signature: `class AnalyzeCodeStructureTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L507) — Initialize with optional project root for path resolution.
  - `_analyze_structure(self, options: _ExecutionOptions)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L648) — Run the analysis engine for the resolved input file.
  - `_format_response(self, result: Any, options: _ExecutionOptions)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L583) — Convert analysis output into the final MCP response payload.
  - `_pre_validate_language_mismatch(self, args: dict[str, Any])` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L549) — Return an error response when the explicit ``language`` conflicts
  - `_prepare_execution_options(self, args: dict[str, Any])` — [`L610`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L610) — Validate, sanitize, and resolve execute arguments.
  - `_resolve_language(self, language: Any, resolved_path: str)` — [`L641`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L641) — Sanitize the explicit language or detect it from the resolved path.
  - `_sanitize_optional_arg(self, value: Any, max_length: int)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L635) — Sanitize an optional string-like argument when it is present.
  - `_save_output(self, response: dict[str, Any], table_output: str, options: _ExecutionOptions)` — [`L681`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L681) — Persist table output and annotate the response with save status.
  - `execute(self, args: dict[str, Any])` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L540) — Execute AST structure analysis and return formatted results.
  - `get_tool_definition(self)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L518) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L527) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L531) — Validate file_path and format arguments.
  - `analysis_engine` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L509)
  - `file_output_manager` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L510)
  - `logger` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L512)
- protocol/private: `_on_project_root_changed`[`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L514)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`FileOutputManager`](../utils/file_output_manager.md#FileOutputManager), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`sanitize_input`](../../security/validator.md#SecurityValidator.sanitize_input), [`_build_next_steps`](analyze_code_structure_tool.md#_build_next_steps), [`get_managed_instance`](../utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`security_validator`](base_tool.md#BaseMCPTool.security_validator), [`_format_table`](analyze_code_structure_tool.md#_format_table), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`_build_success_response`](analyze_code_structure_tool.md#_build_success_response), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`_ExecutionOptions`](analyze_code_structure_tool.md#_ExecutionOptions), [`extract_metadata`](analyze_code_structure_helpers.md#extract_metadata), [`_validate_format_type`](analyze_code_structure_tool.md#_validate_format_type), [`_output_base_name`](analyze_code_structure_tool.md#_output_base_name), [`_convert_analysis_result`](analyze_code_structure_tool.md#_convert_analysis_result), [`file_path`](analyze_code_structure_tool.md#_ExecutionOptions.file_path), [`language`](analyze_code_structure_tool.md#_ExecutionOptions.language), [`output_file`](analyze_code_structure_tool.md#_ExecutionOptions.output_file), [`format_type`](analyze_code_structure_tool.md#_ExecutionOptions.format_type), [`_hoist_structure_keys`](analyze_code_structure_tool.md#_hoist_structure_keys), [`logger`](analyze_code_structure_tool.md#logger), [`TOOL_SCHEMA`](analyze_code_structure_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`output_format`](analyze_code_structure_tool.md#_ExecutionOptions.output_format), [`resolved_path`](analyze_code_structure_tool.md#_ExecutionOptions.resolved_path), [`_ANALYZE_ERR_PREFIX`](analyze_code_structure_tool.md#_ANALYZE_ERR_PREFIX), [`_STATS_KEY`](analyze_code_structure_tool.md#_STATS_KEY), [`_validate_optional_string`](analyze_code_structure_tool.md#_validate_optional_string), [`suppress_output`](analyze_code_structure_tool.md#_ExecutionOptions.suppress_output), [`_SAVE_ERR_MSG`](analyze_code_structure_tool.md#_SAVE_ERR_MSG)  (+10 more)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`validate_file`](../../../scripts/pre_commit_format_validation.md#PreCommitFormatValidator.validate_file), [`project_root`](../../../scripts/pre_commit_format_validation.md#project_root), [`_monitor_format_type`](../../../scripts/format_monitoring_tool.md#FormatMonitor._monitor_format_type), [`project_root`](../../../scripts/format_monitoring_tool.md#project_root), [`_signatures_route`](structure_facade.md#build_structure_facade._signatures_route), [`analyze_code_structure_tool`](analyze_code_structure_tool.md#analyze_code_structure_tool)  (108 test-only)

### `_ExecutionOptions`
- def: [`tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L45)
- signature: `class _ExecutionOptions:`
- members:
  - `file_path` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L46)
  - `format_type` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L48)
  - `language` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L49)
  - `output_file` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L50)
  - `output_format` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L52)
  - `resolved_path` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L47)
  - `suppress_output` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L51)
- used by: [`_format_response`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool._format_response), [`_prepare_execution_options`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool._prepare_execution_options), [`_analyze_structure`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool._analyze_structure), [`_save_output`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool._save_output), [`_build_success_response`](analyze_code_structure_tool.md#_build_success_response), [`_attach_agent_summary`](analyze_code_structure_tool.md#_attach_agent_summary), [`_base_success_response`](analyze_code_structure_tool.md#_base_success_response), [`_attach_parse_validity`](analyze_code_structure_tool.md#_attach_parse_validity), [`_output_base_name`](analyze_code_structure_tool.md#_output_base_name), [`_suppress_table_output_if_requested`](analyze_code_structure_tool.md#_suppress_table_output_if_requested)

## Functions
- `_attach_agent_summary(response: dict[str, Any], options: _ExecutionOptions, metadata: dict[str, Any], next_steps: list[str])` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L306) — Inject ``agent_summary`` + ``summary_line`` keys on the success path.
- `_attach_next_steps(response: dict[str, Any], next_steps: list[str])` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L366) — Attach compact agent routing suggestions when present.
- `_attach_parse_validity(response: dict[str, Any], options: _ExecutionOptions)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L267) — #572: surface tree-sitter parse errors so a wrong-language or corrupt
- `_base_success_response(options: _ExecutionOptions, metadata: dict[str, Any], table_output: str)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L344) — Build the common success response payload.
- `_build_next_steps(structure_dict: dict[str, Any], file_path: str)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L226) — Build next_steps suggestions for AI agents.
- `_build_success_response(options: _ExecutionOptions, metadata: dict[str, Any], table_output: str, next_steps: list[str])` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L249) — Build the successful tool response before optional file persistence.
- `_complex_method_step(methods: list[_MethodData])` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L178) — Build the focused extraction step for the most complex method.
- `_convert_analysis_result(result: Any)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L244) — Convert AnalysisResult to a JSON-serializable dict.
- `_convert_parameters(parameters: Any)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L116) — Convert method parameters to dict format.
- `_ensure_input_file_exists(resolved_path: str, file_path: str)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L427) — Raise a user-facing error when the resolved input is missing.
- `_format_table(structure_dict: dict[str, Any], result: Any, language: str, format_type: str)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L55) — Format analysis result as a compact or full table.
- `_get_field_modifiers(field: Any)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L90) — Extract field modifiers (visibility, static, final).
- `_get_method_modifiers(method: Any)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L78) — Extract method modifiers (static, final, abstract).
- `_get_method_parameters(method: Any)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L137) — Extract method parameters with types.
- `_hoist_structure_keys(response: dict, structure_dict: dict)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L474) — Copy per-element lists from structure_dict to the top-level response.
- `_large_file_first_method_step(methods: list[_MethodData], total_lines: int)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L211) — Build a fallback extraction step for large files without complex methods.
- `_line_range(method: dict[str, Any])` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L166) — Return usable start/end line values for a method suggestion.
- `_mark_file_save_error(response: dict[str, Any], error: Exception)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L446) — Annotate a failed file save without failing the whole tool call.
- `_mark_file_saved(response: dict[str, Any], saved_path: str)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L440) — Annotate a successful file save.
- `_method_complexity(method: dict[str, Any])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L160) — Normalize method complexity to an integer routing score.
- `_output_base_name(options: _ExecutionOptions)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L433) — Return the managed file-output base name.
- `_param_from_dict(param: dict)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L103) — Build a parameter dict from a dict-typed parameter.
- `_param_from_obj(param: Any)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L108) — Build a parameter dict from an object-typed parameter.
- `_parse_string_param(param_str: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L124) — Parse a single parameter string into a parameter dict.
- `_query_navigation_steps(methods: list[_MethodData], classes: list[_MethodData])` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L197) — Build query steps for larger method/class collections.
- `_safe_int(value: Any)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L301) — Return value as-is when it is an int, otherwise 0.
- `_safe_resolve(resolver: Any, path: str)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L463) — Call resolver(path); return path unchanged if resolver raises.
- `_structure_items(value: Any)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L145) — Return list-shaped structure items and ignore malformed entries.
- `_suppress_table_output_if_requested(response: dict[str, Any], options: _ExecutionOptions)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L372) — Drop table output only when it was persisted to a file.
- `_total_lines(statistics: Any)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L152) — Extract a valid total line count from analysis statistics.
- `_try_save_file(file_output_manager: Any, content: str, base_name: str)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L452) — Attempt file save; return (saved_path, None) or (None, error).
- `_validate_format_type(arguments: dict[str, Any])` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L394) — Validate the optional structure table format.
- `_validate_optional_string(arguments: dict[str, Any], field_name: str, *, allow_blank: bool = True)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L406) — Validate an optional string argument and optional blank rejection.
- `_validate_required_file_path(arguments: dict[str, Any])` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L380) — Validate the required file_path argument.
- `_validate_suppress_output(arguments: dict[str, Any])` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L419) — Validate the optional suppress_output flag.

## Module values
- `_ANALYZE_ERR_PREFIX` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L35)
- `_HOIST_KEYS` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L471)
- `_MethodData` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L31)
- `_SAVE_ERR_MSG` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L34)
- `_STATS_KEY` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L33)
- `_TOOL_ANNOTATIONS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L36)
- `_TOOL_DESCRIPTION` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L480)
- `_TOOL_NAME` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L32)
- `_VALID_FORMAT_TYPES` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L391)
- `analyze_code_structure_tool` — [`L700`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L700)
- `logger` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.py#L27)

