---
title: 'Module: tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.analyze_scale_helpers`/
symbols:
  generate_llm_guidance: generate_llm_guidance().
  extract_structural_overview: extract_structural_overview().
  extract_structural_overview_universal: extract_structural_overview_universal().
  create_json_file_analysis: create_json_file_analysis().
  build_analysis_result: build_analysis_result().
  build_detailed_analysis: build_detailed_analysis().
  validate_scale_arguments: validate_scale_arguments().
  _extract_method_infos: _extract_method_infos().
  _attach_available_queries: _attach_available_queries().
  _do_compute_file_metrics: _do_compute_file_metrics().
  assemble_batch_response: assemble_batch_response().
  _extract_class_infos: _extract_class_infos().
  _extract_field_infos: _extract_field_infos().
  _extract_import_infos: _extract_import_infos().
  _build_workflow_steps: _build_workflow_steps().
  METHODS_OUTPUT_CAP: METHODS_OUTPUT_CAP.
  validate_batch_arguments: validate_batch_arguments().
  _count_elements_impl: _count_elements_impl().
  _analyze_batch_item_core: _analyze_batch_item_core().
  logger: logger.
  _ensure_required_overview_fields: _ensure_required_overview_fields().
  _small_or_medium_steps: _small_or_medium_steps().
  _resolve_batch_path: _resolve_batch_path().
  _COMPLEXITY_HOTSPOT_THRESHOLD: _COMPLEXITY_HOTSPOT_THRESHOLD.
  BATCH_MAX_FILES: BATCH_MAX_FILES.
  BATCH_CONCURRENCY: BATCH_CONCURRENCY.
  HOTSPOTS_OUTPUT_CAP: HOTSPOTS_OUTPUT_CAP.
  _apply_hotspot_cap: _apply_hotspot_cap().
  validate_mode_argument: validate_mode_argument().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  _make_hotspot_entry: _make_hotspot_entry().
  _PRIORITY_QUERIES: _PRIORITY_QUERIES.
  _REQUIRED_OVERVIEW_FIELDS: _REQUIRED_OVERVIEW_FIELDS.
  _empty_guidance: _empty_guidance().
  _classify_size: _classify_size().
  _recommend_tools: _recommend_tools().
  _assess_complexity: _assess_complexity().
  _identify_key_areas: _identify_key_areas().
  _large_file_steps: _large_file_steps().
  _LANG_QUERIES._LANG_QUERIES: _LANG_QUERIES._LANG_QUERIES.
---
# Module: [`tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py)

## Functions
- `_analyze_batch_item_core(fp: str, sem: Any, resolve_fn: Any, project_root: str | None, calc_fn: Any, detect_fn: Any)` — [`L955`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L955) — One file slot of the batch scatter: validate → resolve → metrics.
- `_apply_hotspot_cap(overview: dict[str, Any], hotspots: list[dict[str, Any]], hotspot_cap: int)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L120) — Cap hotspot payloads and expose metadata only when truncation occurs.
- `_assess_complexity(guidance: dict[str, Any], structural_overview: dict[str, Any])` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L434) — Set complexity_assessment based on hotspot count.
- `_attach_available_queries(guidance: dict[str, Any], language: str)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L520) — Look up tree-sitter queries for ``language`` and cap to 15 entries.
- `_build_workflow_steps(guidance: dict[str, Any], structural_overview: dict[str, Any])` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L463) — Compose the ordered workflow_steps list — size-dependent middle, fixed tail.
- `_classify_size(guidance: dict[str, Any], total_lines: int)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L396) — Pick a size_category + matching analysis_strategy from total_lines.
- `_count_elements_impl(elements: list, element_type_const: str, element_type_str: str)` — [`L923`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L923) — Count elements matching either a typed constant or a string attribute.
- `_do_compute_file_metrics(file_path: str, language: str | None, project_root: str | None)` — [`L892`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L892) — Compute file-level metrics; returns a dict with file_size_kb added.
- `_empty_guidance()` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L376) — The skeleton guidance dict — 7 named fields, all empty/zero.
- `_ensure_required_overview_fields(structural_overview: dict[str, Any])` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L389) — Fill in missing keys so downstream lookups never KeyError.
- `_extract_class_infos(elements: list[Any])` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L66) — Class element → dict with position + inheritance + annotations.
- `_extract_field_infos(elements: list[Any])` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L133) — Field element → dict with type + modifiers + position.
- `_extract_import_infos(elements: list[Any])` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L151) — Import element → dict with statement + static/wildcard flags.
- `_extract_method_infos(elements: list[Any])` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L85) — Method element → (method_infos, complexity_hotspots) with threshold ≥8.
- `_identify_key_areas(guidance: dict[str, Any], structural_overview: dict[str, Any])` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L447) — Note structural characteristics worth surfacing to the agent.
- `_large_file_steps(structural_overview: dict[str, Any])` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L479) — Targeted-analysis steps for files ≥500 lines.
- `_make_hotspot_entry(name: str, complexity: Any, start_line: int, end_line: int)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L171) — Build a complexity hotspot dict for a method element.
- `_recommend_tools(guidance: dict[str, Any], total_lines: int, structural_overview: dict[str, Any])` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L421) — Append tool recommendations based on size + presence of hotspots.
- `_resolve_batch_path(fp: str, resolve_fn: Any, project_root: str | None)` — [`L943`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L943) — Try to resolve *fp* via *resolve_fn*; return (resolved, error_msg).
- `_small_or_medium_steps(structural_overview: dict[str, Any])` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L499) — Full-analysis steps for files <500 lines.
- `assemble_batch_response(per_file: list[dict[str, Any]], file_paths: list[str], output_format: str, metrics_only: bool)` — [`L993`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L993) — Compose the canonical batch envelope (raw — caller applies TOON format).
- `build_analysis_result(file_path: str, language: str, file_metrics: dict[str, Any], analysis_result: Any, structural_overview: dict[str, Any], count_elements_fn: Any)` — [`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L671) — Build the main analysis result dict.
- `build_detailed_analysis(analysis_result: Any, file_path: str)` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L758) — Build the detailed_analysis dict for include_details=True.
- `create_json_file_analysis(file_path: str, file_metrics: dict[str, Any], include_guidance: bool, output_format: str = "toon")` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L593) — Create analysis for non-source files (JSON, YAML, etc.).
- `extract_structural_overview(analysis_result: Any, *, method_cap: int = METHODS_OUTPUT_CAP, hotspot_cap: int = HOTSPOTS_OUTPUT_CAP)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L33) — Extract structural overview with position information for LLM guidance.
- `extract_structural_overview_universal(analysis_result: Any, *, method_cap: int = METHODS_OUTPUT_CAP, hotspot_cap: int = HOTSPOTS_OUTPUT_CAP)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L185) — Extract structural overview from universal analysis result (non-Java languages).
- `generate_llm_guidance(file_metrics: dict[str, Any], structural_overview: dict[str, Any])` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L350) — Generate guidance for LLM on how to efficiently analyze this file.
- `validate_batch_arguments(metrics_only: bool, file_paths: object)` — [`L875`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L875) — Reject malformed batch inputs early with a precise message.
- `validate_mode_argument(arguments: dict[str, Any])` — [`L861`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L861) — Reject unknown ``mode`` values early instead of silent no-op.
- `validate_scale_arguments(arguments: dict[str, Any])` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L535) — Validate file_path and option arguments for analyze scale tool.

## Module values
- `BATCH_CONCURRENCY` — [`L827`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L827)
- `BATCH_MAX_FILES` — [`L826`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L826)
- `HOTSPOTS_OUTPUT_CAP` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L28)
- `METHODS_OUTPUT_CAP` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L27)
- `TOOL_SCHEMA` — [`L832`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L832)
- `_COMPLEXITY_HOTSPOT_THRESHOLD` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L168)
- `_LANG_QUERIES` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L276)
- `_PRIORITY_QUERIES` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L327)
- `_REQUIRED_OVERVIEW_FIELDS` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L341)
- `logger` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.py#L19)

