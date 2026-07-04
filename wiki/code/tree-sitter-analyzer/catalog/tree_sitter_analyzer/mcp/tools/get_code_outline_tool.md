---
title: 'Module: tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.get_code_outline_tool`/
symbols:
  GetCodeOutlineTool: GetCodeOutlineTool#
  GetCodeOutlineTool.execute: GetCodeOutlineTool#execute().
  GetCodeOutlineTool._build_outline: GetCodeOutlineTool#_build_outline().
  GetCodeOutlineTool._run_outline_analysis: GetCodeOutlineTool#_run_outline_analysis().
  GetCodeOutlineTool.analysis_engine: GetCodeOutlineTool#analysis_engine.
  GetCodeOutlineTool.validate_arguments: GetCodeOutlineTool#validate_arguments().
  GetCodeOutlineTool._resolve_outline_request: GetCodeOutlineTool#_resolve_outline_request().
  _build_class_outlines: _build_class_outlines().
  _method_owned_by_class: _method_owned_by_class().
  _in_class_ranges: _in_class_ranges().
  _normalize_receiver_type: _normalize_receiver_type().
  GetCodeOutlineTool._assemble_outline_response: GetCodeOutlineTool#_assemble_outline_response().
  DEFAULT_OUTLINE_CLASSES_CAP.DEFAULT_OUTLINE_CLASSES_CAP: DEFAULT_OUTLINE_CLASSES_CAP.DEFAULT_OUTLINE_CLASSES_CAP.
  GetCodeOutlineTool.get_tool_schema: GetCodeOutlineTool#get_tool_schema().
  GetCodeOutlineTool._on_project_root_changed: GetCodeOutlineTool#_on_project_root_changed().
  GetCodeOutlineTool._attach_input_diagnostics: GetCodeOutlineTool#_attach_input_diagnostics().
  _method_entry: _method_entry().
  _enrich_markdown_outline: _enrich_markdown_outline().
  GetCodeOutlineTool.get_tool_definition: GetCodeOutlineTool#get_tool_definition().
  logger: logger.
  GetCodeOutlineTool.logger: GetCodeOutlineTool#logger.
  GetCodeOutlineTool._attach_outline_summary: GetCodeOutlineTool#_attach_outline_summary().
  _enrich_sql_outline: _enrich_sql_outline().
  _resolve_extends: _resolve_extends().
  _resolve_implements: _resolve_implements().
  GetCodeOutlineTool.__init__: GetCodeOutlineTool#__init__().
  get_code_outline_tool: get_code_outline_tool.
  _field_entry: _field_entry().
  DEFAULT_OUTLINE_FUNCTIONS_CAP.DEFAULT_OUTLINE_FUNCTIONS_CAP: DEFAULT_OUTLINE_FUNCTIONS_CAP.DEFAULT_OUTLINE_FUNCTIONS_CAP.
  _outline_diagnostics_next_step: _outline_diagnostics_next_step().
  _cap_class_members: _cap_class_members().
  _in_function_spans: _in_function_spans().
  _enrich_markup_outline: _enrich_markup_outline().
  _enrich_yaml_outline: _enrich_yaml_outline().
  _enrich_json_outline: _enrich_json_outline().
  _SQL_OBJECT_TYPES._SQL_OBJECT_TYPES: _SQL_OBJECT_TYPES._SQL_OBJECT_TYPES.
  _MD_HEADING_TYPES._MD_HEADING_TYPES: _MD_HEADING_TYPES._MD_HEADING_TYPES.
  _MD_BLOCK_TYPES._MD_BLOCK_TYPES: _MD_BLOCK_TYPES._MD_BLOCK_TYPES.
---
# Module: [`tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py)

## Classes
### `GetCodeOutlineTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L76) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Tool: get_code_outline
- signature: `class GetCodeOutlineTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L89) — 初始化 get_code_outline 工具。
  - `_assemble_outline_response(file_path: str, language: str | None, outline: Any, listed_cap: int = DEFAULT_OUTLINE_CLASSES_CAP)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L438) — Build the canonical response dict + hoist outline-level fields.
  - `_attach_input_diagnostics(result: dict[str, Any], resolved_path: str)` — [`L605`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L605) — Attach parse/encoding warnings to a successful outline response.
  - `_attach_outline_summary(result: dict[str, Any], file_path: str)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L539) — Add ``summary_line`` + ``verdict`` + ``agent_summary`` to ``result``.
  - `_build_outline(self, analysis_result: Any, include_fields: bool, include_imports: bool)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L208) — 从分析结果构建层次化大纲。
  - `_on_project_root_changed(self, project_root: str | None)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L95) — Hook fired by ``BaseMCPTool.set_project_path`` (ARCH-A4).
  - `_resolve_outline_request(self, file_path: str, language: str | None, output_format: str)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L362) — Resolve + validate the file path, then run the language-mismatch gate.
  - `_run_outline_analysis(self, resolved_path: str, language: str, original_path: str)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L395) — Run the analysis engine inside the perf monitor span.
  - `execute(self, arguments: dict[str, Any])` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L316) — 执行 get_code_outline 工具。 — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `get_tool_definition(self)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L619) — 返回 MCP tool 定义。
  - `get_tool_schema(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L105) — 返回 MCP tool JSON Schema。
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L166) — 校验工具参数。
  - `analysis_engine` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L92)
  - `logger` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L93)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`ELEMENT_TYPE_CLASS`](../../constants.md#ELEMENT_TYPE_CLASS), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`ELEMENT_TYPE_FUNCTION`](../../constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../constants.md#is_element_of_type), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`ELEMENT_TYPE_VARIABLE`](../../constants.md#ELEMENT_TYPE_VARIABLE), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`ELEMENT_TYPE_IMPORT`](../../constants.md#ELEMENT_TYPE_IMPORT), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`analyze`](../../core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`ELEMENT_TYPE_PACKAGE`](../../constants.md#ELEMENT_TYPE_PACKAGE), [`get_performance_monitor`](../utils/__init__.md#get_performance_monitor), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`_build_class_outlines`](get_code_outline_tool.md#_build_class_outlines), [`_in_class_ranges`](get_code_outline_tool.md#_in_class_ranges), [`DEFAULT_OUTLINE_CLASSES_CAP`](get_code_outline_tool.md#DEFAULT_OUTLINE_CLASSES_CAP.DEFAULT_OUTLINE_CLASSES_CAP), [`file_input_diagnostics`](utils/parse_validity.md#file_input_diagnostics), [`_enrich_markdown_outline`](get_code_outline_tool.md#_enrich_markdown_outline), [`_method_entry`](get_code_outline_tool.md#_method_entry), [`logger`](get_code_outline_tool.md#logger), [`_enrich_sql_outline`](get_code_outline_tool.md#_enrich_sql_outline), [`_field_entry`](get_code_outline_tool.md#_field_entry), [`_cap_class_members`](get_code_outline_tool.md#_cap_class_members), [`_enrich_json_outline`](get_code_outline_tool.md#_enrich_json_outline), [`_enrich_markup_outline`](get_code_outline_tool.md#_enrich_markup_outline), [`_enrich_yaml_outline`](get_code_outline_tool.md#_enrich_yaml_outline), [`_in_function_spans`](get_code_outline_tool.md#_in_function_spans), [`_outline_diagnostics_next_step`](get_code_outline_tool.md#_outline_diagnostics_next_step)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade), [`_handle_outline`](../../cli/special_commands.md#_handle_outline), [`get_code_outline_tool`](get_code_outline_tool.md#get_code_outline_tool)  (113 test-only)

## Functions
- `_build_class_outlines(classes: list[Any], all_methods: list[Any], all_fields: list[Any], include_fields: bool)` — [`L848`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L848) — Build the ``classes`` outline section, sorted by ``line_start``.
- `_cap_class_members(cls: dict[str, Any], cap: int)` — [`L665`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L665) — Cap a class outline's ``methods``/``fields`` lists to ``cap`` (#571).
- `_enrich_json_outline(outline: dict[str, Any], elements: list[Any], classes: list[Any])` — [`L1081`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L1081) — Attach JSON document root + top-level property summaries.
- `_enrich_markdown_outline(outline: dict[str, Any], elements: list[Any], classes: list[Any])` — [`L998`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L998) — Attach Markdown headings + block summaries (guarded by language).
- `_enrich_markup_outline(outline: dict[str, Any], elements: list[Any], classes: list[Any])` — [`L922`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L922) — Attach HTML / CSS element summaries when no class structure is present.
- `_enrich_sql_outline(outline: dict[str, Any], elements: list[Any], classes: list[Any])` — [`L962`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L962) — Attach SQL object summaries (tables / views / procedures / ...).
- `_enrich_yaml_outline(outline: dict[str, Any], elements: list[Any], classes: list[Any])` — [`L1040`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L1040) — Attach YAML document + top-level mapping summaries (guarded by language).
- `_field_entry(f: Any)` — [`L717`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L717) — Convert a field element to an outline entry.
- `_in_class_ranges(method: Any, class_ranges: list[tuple[int, int]], class_names: list[str] | None = None)` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L758) — Return True iff ``method`` falls inside any class range or owns a receiver_type match.
- `_in_function_spans(fn_idx: int, fn_spans: list[tuple[int, int]])` — [`L780`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L780) — Return True iff function at ``fn_idx`` is strictly nested inside another.
- `_method_entry(m: Any)` — [`L687`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L687) — Convert a method element to an outline entry.
- `_method_owned_by_class(method: Any, cls_name: str, cls_start: int, cls_end: int)` — [`L740`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L740) — Return True when ``method`` belongs to ``cls``.
- `_normalize_receiver_type(receiver_type: str | None)` — [`L729`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L729) — Strip a leading ``*`` from a Go receiver type (``*Counter`` → ``Counter``).
- `_outline_diagnostics_next_step(diagnostics: dict[str, Any])` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L56) — Return the next action for parse/encoding diagnostic warnings.
- `_resolve_extends(cls: Any)` — [`L809`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L809) — Return the superclass name for a Class element.
- `_resolve_implements(cls: Any)` — [`L830`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L830) — Return the list of implemented interface names for a Class element.

## Module values
- `DEFAULT_OUTLINE_CLASSES_CAP` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L52)
- `DEFAULT_OUTLINE_FUNCTIONS_CAP` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L53)
- `_MD_BLOCK_TYPES` — [`L993`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L993)
- `_MD_HEADING_TYPES` — [`L992`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L992)
- `_SQL_OBJECT_TYPES` — [`L957`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L957)
- `get_code_outline_tool` — [`L1131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L1131)
- `logger` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/get_code_outline_tool.py#L39)

