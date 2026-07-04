---
title: 'Module: tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.analyze_code_structure_helpers`/
symbols:
  convert_analysis_result_to_dict: convert_analysis_result_to_dict().
  _parse_string_parameter: _parse_string_parameter().
  _convert_class: _convert_class().
  convert_analysis_result_to_structure_dict: convert_analysis_result_to_structure_dict().
  extract_metadata: extract_metadata().
  get_method_parameters: get_method_parameters().
  extract_metadata.safe_int: extract_metadata().safe_int().
  _resolve_class_extends: _resolve_class_extends().
  _resolve_class_implements: _resolve_class_implements().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  get_method_modifiers: get_method_modifiers().
  get_field_modifiers: get_field_modifiers().
  convert_parameters: convert_parameters().
  _convert_method: _convert_method().
  _convert_field: _convert_field().
  _convert_import: _convert_import().
---
# Module: [`tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py)

## Functions
- `_convert_class(cls: Any)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L303)
- `_convert_field(field: Any, get_mods: Any)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L338)
- `_convert_import(imp: Any)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L353)
- `_convert_method(method: Any, get_params: Any, get_mods: Any)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L319)
- `_parse_string_parameter(param_str: str)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L85) — Parse one string-form parameter into ``{name, type[, default]}``.
- `_resolve_class_extends(cls: Any)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L276) — Return the superclass name, checking both plugin spelling conventions.
- `_resolve_class_implements(cls: Any)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L290) — Return implemented interfaces, checking both plugin spelling conventions.
- `convert_analysis_result_to_dict(result: Any, get_method_parameters: Any, get_method_modifiers: Any, get_field_modifiers: Any)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L217) — Convert AnalysisResult to dictionary format expected by TableFormatter.
- `convert_analysis_result_to_structure_dict(result: Any)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L200) — Convert an :class:`AnalysisResult` to the rich structure dict.
- `convert_parameters(parameters: Any)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L51) — Convert method parameters to dict format.
- `extract_metadata(structure_dict: dict[str, Any])` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L260) — Extract response metadata from the structure statistics block.
- `get_field_modifiers(field: Any)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L38) — Extract field modifiers (visibility, static, final).
- `get_method_modifiers(method: Any)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L26) — Extract method modifiers (static, final, abstract).
- `get_method_parameters(method: Any)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L72) — Extract method parameters with types.
- `safe_int(value: Any)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L264)

## Module values
- `TOOL_SCHEMA` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.py#L159)

