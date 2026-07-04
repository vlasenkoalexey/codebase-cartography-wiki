---
title: 'Module: tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.universal_analyze_tool`/
symbols:
  UniversalAnalyzeTool: UniversalAnalyzeTool#
  UniversalAnalyzeTool.execute: UniversalAnalyzeTool#execute().
  UniversalAnalyzeTool._analyze_universal: UniversalAnalyzeTool#_analyze_universal().
  UniversalAnalyzeTool._analyze_advanced: UniversalAnalyzeTool#_analyze_advanced().
  UniversalAnalyzeTool.analysis_engine: UniversalAnalyzeTool#analysis_engine.
  UniversalAnalyzeTool._extract_structure_info: UniversalAnalyzeTool#_extract_structure_info().
  UniversalAnalyzeTool._run_universal_analysis: UniversalAnalyzeTool#_run_universal_analysis().
  UniversalAnalyzeTool._get_available_queries: UniversalAnalyzeTool#_get_available_queries().
  UniversalAnalyzeTool._extract_detailed_metrics: UniversalAnalyzeTool#_extract_detailed_metrics().
  UniversalAnalyzeTool.validate_arguments: UniversalAnalyzeTool#validate_arguments().
  UniversalAnalyzeTool.get_tool_definition: UniversalAnalyzeTool#get_tool_definition().
  logger: logger.
  _attach_structure_detail: _attach_structure_detail().
  UniversalAnalyzeTool._extract_universal_comprehensive_metrics: UniversalAnalyzeTool#_extract_universal_comprehensive_metrics().
  UniversalAnalyzeTool._extract_comprehensive_metrics: UniversalAnalyzeTool#_extract_comprehensive_metrics().
  UniversalAnalyzeTool._extract_universal_basic_metrics: UniversalAnalyzeTool#_extract_universal_basic_metrics().
  UniversalAnalyzeTool._extract_universal_detailed_metrics: UniversalAnalyzeTool#_extract_universal_detailed_metrics().
  UniversalAnalyzeTool._on_project_root_changed: UniversalAnalyzeTool#_on_project_root_changed().
  _attach_canonical_envelope: _attach_canonical_envelope().
  UniversalAnalyzeTool._extract_basic_metrics: UniversalAnalyzeTool#_extract_basic_metrics().
  UniversalAnalyzeTool.get_tool_schema: UniversalAnalyzeTool#get_tool_schema().
  UniversalAnalyzeTool._extract_universal_structure_info: UniversalAnalyzeTool#_extract_universal_structure_info().
  UniversalAnalyzeTool.__init__: UniversalAnalyzeTool#__init__().
  _summarize_annotation: _summarize_annotation().
---
# Module: [`tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py)

## Classes
### `UniversalAnalyzeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py:147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L147) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- doc: Universal MCP Tool for code analysis across multiple languages.
- signature: `class UniversalAnalyzeTool(BaseMCPTool):`
- members:
  - `_analyze_advanced(self, file_path: str, language: str, analysis_type: str, arguments: dict[str, Any])` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L331) — Analyze using the advanced analyzer (Java-specific).
  - `_analyze_universal(self, file_path: str, language: str, analysis_type: str, arguments: dict[str, Any])` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L385) — Analyze using the universal analyzer.
  - `_extract_basic_metrics(self, result: Any)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L455) — Extract basic file metrics (lines, functions, classes).
  - `_extract_comprehensive_metrics(self, result: Any)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L504) — Extract comprehensive metrics combining all dimensions.
  - `_extract_detailed_metrics(self, result: Any)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L469) — Extract detailed metrics with complexity and dependencies.
  - `_extract_structure_info(self, result: Any)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L484) — Extract structure information from analysis result.
  - `_extract_universal_basic_metrics(self, analysis_dict: dict[str, Any])` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L512) — Extract basic metrics using universal tree-sitter path.
  - `_extract_universal_comprehensive_metrics(self, analysis_dict: dict[str, Any])` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L587) — Extract comprehensive metrics using universal tree-sitter path.
  - `_extract_universal_detailed_metrics(self, analysis_dict: dict[str, Any])` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L553) — Extract detailed metrics using universal tree-sitter path.
  - `_extract_universal_structure_info(self, analysis_dict: dict[str, Any])` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L562) — Extract structure info using universal tree-sitter path.
  - `_get_available_queries(self, language: str)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L595) — Return available query keys for a language.
  - `_run_universal_analysis(self, resolved: str, language: str, analysis_type: str, arguments: dict[str, Any], output_format: str)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L296) — Execute the analysis inside the perf monitor span.
  - `execute(self, arguments: dict[str, Any])` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L225) — Execute universal analysis using the analysis engine. — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `get_tool_definition(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L160) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L157)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L197) — Validate file_path, language, and output arguments.
  - `analysis_engine` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L151)
- protocol/private: `__init__`[`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L150), `_on_project_root_changed`[`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L154)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`ELEMENT_TYPE_CLASS`](../../constants.md#ELEMENT_TYPE_CLASS), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`ELEMENT_TYPE_FUNCTION`](../../constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../constants.md#is_element_of_type), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`compute_file_metrics`](../utils/file_metrics.md#compute_file_metrics), [`ELEMENT_TYPE_VARIABLE`](../../constants.md#ELEMENT_TYPE_VARIABLE), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`ELEMENT_TYPE_IMPORT`](../../constants.md#ELEMENT_TYPE_IMPORT), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`sanitize_input`](../../security/validator.md#SecurityValidator.sanitize_input), [`is_language_supported`](../../language_detector.md#is_language_supported), [`security_validator`](base_tool.md#BaseMCPTool.security_validator), [`safe_error_message`](../utils/error_sanitizer.md#safe_error_message), [`get_performance_monitor`](../utils/__init__.md#get_performance_monitor), [`count_elements_by_type`](universal_analyze_helpers.md#count_elements_by_type), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`elements_to_summary`](universal_analyze_helpers.md#elements_to_summary), [`logger`](universal_analyze_tool.md#logger), [`_attach_structure_detail`](universal_analyze_tool.md#_attach_structure_detail), [`_attach_canonical_envelope`](universal_analyze_tool.md#_attach_canonical_envelope), [`TOOL_SCHEMA`](universal_analyze_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`count_dict_elements_by_type`](universal_analyze_helpers.md#count_dict_elements_by_type), [`_summarize_annotation`](universal_analyze_tool.md#_summarize_annotation)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`universal_analyze_tool`](../server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`UNIVERSAL_TOOL_AVAILABLE`](../server.md#UNIVERSAL_TOOL_AVAILABLE)  (68 test-only)

## Functions
- `_attach_canonical_envelope(base: dict[str, Any])` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L46) — Inject ``success``/``summary_line``/``agent_summary`` into the response.
- `_attach_structure_detail(base: dict[str, Any], result: Any)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L98) — Hoist per-element detail onto the response.
- `_summarize_annotation(a: Any)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L131) — Return the summary dict for one annotation element.

## Module values
- `logger` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/universal_analyze_tool.py#L43)

