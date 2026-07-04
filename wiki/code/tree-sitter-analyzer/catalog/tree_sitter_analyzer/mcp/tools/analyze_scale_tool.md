---
title: 'Module: tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.analyze_scale_tool`/
symbols:
  AnalyzeScaleTool: AnalyzeScaleTool#
  AnalyzeScaleTool.execute: AnalyzeScaleTool#execute().
  AnalyzeScaleTool._run_structural_analysis: AnalyzeScaleTool#_run_structural_analysis().
  AnalyzeScaleTool._execute_single_file: AnalyzeScaleTool#_execute_single_file().
  AnalyzeScaleTool._build_single_file_response: AnalyzeScaleTool#_build_single_file_response().
  AnalyzeScaleTool._scatter_batch_metrics: AnalyzeScaleTool#_scatter_batch_metrics().
  AnalyzeScaleTool._build_enhanced_result: AnalyzeScaleTool#_build_enhanced_result().
  AnalyzeScaleTool._execute_metrics_batch: AnalyzeScaleTool#_execute_metrics_batch().
  AnalyzeScaleTool._calculate_file_metrics: AnalyzeScaleTool#_calculate_file_metrics().
  AnalyzeScaleTool._check_language_mismatch: AnalyzeScaleTool#_check_language_mismatch().
  AnalyzeScaleTool.analysis_engine: AnalyzeScaleTool#analysis_engine.
  logger: logger.
  AnalyzeScaleTool._resolve_language: AnalyzeScaleTool#_resolve_language().
  AnalyzeScaleTool.get_tool_definition: AnalyzeScaleTool#get_tool_definition().
  AnalyzeScaleTool.get_tool_schema: AnalyzeScaleTool#get_tool_schema().
  AnalyzeScaleTool.validate_arguments: AnalyzeScaleTool#validate_arguments().
  analyze_scale_tool: analyze_scale_tool.
  AnalyzeScaleTool._on_project_root_changed: AnalyzeScaleTool#_on_project_root_changed().
  AnalyzeScaleTool._generate_llm_guidance: AnalyzeScaleTool#_generate_llm_guidance().
  AnalyzeScaleTool._extract_structural_overview: AnalyzeScaleTool#_extract_structural_overview().
  AnalyzeScaleTool._extract_structural_overview_universal: AnalyzeScaleTool#_extract_structural_overview_universal().
  AnalyzeScaleTool._count_elements: AnalyzeScaleTool#_count_elements().
  AnalyzeScaleTool._create_json_file_analysis: AnalyzeScaleTool#_create_json_file_analysis().
  _TOOL_DESCRIPTION: _TOOL_DESCRIPTION.
  AnalyzeScaleTool.__init__: AnalyzeScaleTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py)

## Classes
### `AnalyzeScaleTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L64) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Tool for analyzing code scale and complexity metrics.
- signature: `class AnalyzeScaleTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L73) — Initialize the analyze scale tool.
  - `_build_enhanced_result(self, file_path: str, language: str, file_metrics: dict[str, Any], analysis_result: Any, structural_overview: dict[str, Any], include_guidance: bool, include_details: bool)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L293) — Build enhanced result with metrics, structure, and guidance.
  - `_build_single_file_response(self, file_path: str, resolved: str, language: str, include_details: bool, include_guidance: bool, output_format: str)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L189) — Run the actual metrics+structural pipeline inside the perf monitor.
  - `_calculate_file_metrics(self, file_path: str, language: str | None = None)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L82) — Compute file-level metrics (lines, complexity, size).
  - `_check_language_mismatch(self, file_path: str, resolved: str, language: str | None, output_format: str)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L164) — Refuse ``language='java'`` on a ``.py`` file, return envelope.
  - `_count_elements(self, elements: list, element_type_const: str, element_type_str: str)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L98) — Count elements by type from analysis result.
  - `_create_json_file_analysis(self, file_path: str, file_metrics: dict[str, Any], include_guidance: bool, output_format: str = "toon")` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L364) — Create analysis for non-source files (JSON, YAML, etc.).
  - `_execute_metrics_batch(self, arguments: dict[str, Any])` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L327) — Execute batch metrics computation for multiple files.
  - `_execute_single_file(self, arguments: dict[str, Any])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L126) — Single-file analysis path — orchestrates the 4 phases linearly. — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `_extract_structural_overview(self, analysis_result: Any)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L88) — Extract structural overview using Python-specific analysis.
  - `_extract_structural_overview_universal(self, analysis_result: Any)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L92) — Extract structural overview using universal tree-sitter analysis.
  - `_generate_llm_guidance(self, file_metrics: dict[str, Any], structural_overview: dict[str, Any])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L104) — Generate LLM-oriented guidance based on analysis.
  - `_resolve_language(self, resolved: str, language: str | None)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L238) — Detect language from file extension or argument override.
  - `_run_structural_analysis(self, resolved: str, language: str, include_details: bool)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L249) — Run structural analysis using tree-sitter elements.
  - `_scatter_batch_metrics(self, file_paths: list[str])` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L342) — Fan out per-file analysis with a semaphore — order preserved.
  - `execute(self, arguments: dict[str, Any])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L114) — Execute code scale analysis for single or batch files.
  - `get_tool_definition(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L376) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L110) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L360) — Validate file_path and option arguments.
  - `analysis_engine` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L75)
- protocol/private: `_on_project_root_changed`[`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L79)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`generate_llm_guidance`](analyze_scale_helpers.md#generate_llm_guidance), [`extract_structural_overview`](analyze_scale_helpers.md#extract_structural_overview), [`extract_structural_overview_universal`](analyze_scale_helpers.md#extract_structural_overview_universal), [`sanitize_input`](../../security/validator.md#SecurityValidator.sanitize_input), [`security_validator`](base_tool.md#BaseMCPTool.security_validator), [`create_json_file_analysis`](analyze_scale_helpers.md#create_json_file_analysis), [`build_analysis_result`](analyze_scale_helpers.md#build_analysis_result), [`build_detailed_analysis`](analyze_scale_helpers.md#build_detailed_analysis), [`validate_scale_arguments`](analyze_scale_helpers.md#validate_scale_arguments), [`get_performance_monitor`](../utils/__init__.md#get_performance_monitor), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`logger`](analyze_scale_tool.md#logger), [`_do_compute_file_metrics`](analyze_scale_helpers.md#_do_compute_file_metrics), [`assemble_batch_response`](analyze_scale_helpers.md#assemble_batch_response), [`_analyze_batch_item_core`](analyze_scale_helpers.md#_analyze_batch_item_core), [`_count_elements_impl`](analyze_scale_helpers.md#_count_elements_impl), [`validate_batch_arguments`](analyze_scale_helpers.md#validate_batch_arguments), [`BATCH_CONCURRENCY`](analyze_scale_helpers.md#BATCH_CONCURRENCY), [`TOOL_SCHEMA`](analyze_scale_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`validate_mode_argument`](analyze_scale_helpers.md#validate_mode_argument), [`_TOOL_DESCRIPTION`](analyze_scale_tool.md#_TOOL_DESCRIPTION), [`_normalize_file_path`](base_tool.md#BaseMCPTool._normalize_file_path)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_handle_check_scale`](../../cli/special_commands.md#_handle_check_scale), [`_handle_batch_metrics`](../../cli/special_commands.md#_handle_batch_metrics), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class), [`analyze_scale_tool`](analyze_scale_tool.md#analyze_scale_tool)  (92 test-only)

## Module values
- `_TOOL_DESCRIPTION` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L44)
- `analyze_scale_tool` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L392)
- `logger` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool.py#L41)

