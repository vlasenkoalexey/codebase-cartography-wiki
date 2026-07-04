---
title: 'Module: tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.server_utils.code_scale_handler`/
symbols:
  _count_elements: _count_elements().
  analyze_code_scale: analyze_code_scale().
  _run_scale_analysis: _run_scale_analysis().
  _build_code_scale_result: _build_code_scale_result().
  _validate_and_resolve_path: _validate_and_resolve_path().
  _validate_security: _validate_security().
  _detect_language_for_scale: _detect_language_for_scale().
  logger: logger.
  _get_base_root: _get_base_root().
  _resolve_path: _resolve_path().
---
# Module: [`tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py)

## Functions
- `_build_code_scale_result(*, file_path: str, language: str | None, analysis_result: Any, base_root: str | None, resolved_path: str, include_complexity: bool, include_details: bool)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L132) — Assemble metrics envelope + optional complexity + optional detailed elements.
- `_count_elements(elements: list[Any])` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L214)
- `_detect_language_for_scale(explicit: str | None, resolved_path: str, base_root: str | None)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L100) — Detect language when caller didn't pass one explicitly.
- `_get_base_root(security_validator: Any)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L185)
- `_resolve_path(file_path: str, base_root: str | None)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L193)
- `_run_scale_analysis(analysis_engine: Any, resolved_path: str, language: str | None, include_complexity: bool, include_details: bool)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L113) — Construct AnalysisRequest and run the engine.
- `_validate_and_resolve_path(file_path: str, security_validator: Any, path_class: Any)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L86) — Resolve + security-validate the file path, returning (base_root, resolved).
- `_validate_security(resolved_path: str, base_root: str | None, security_validator: Any)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L199)
- `analyze_code_scale(arguments: dict[str, Any], *, analysis_engine: Any, security_validator: Any, universal_analyze_tool: Any | None = None, initialization_complete: bool = True, path_class: Any = PathClass)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L21) — Handle check_code_scale tool execution with full validation.

## Module values
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/code_scale_handler.py#L18)

