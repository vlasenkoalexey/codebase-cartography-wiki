---
title: 'Module: tree_sitter_analyzer/models/_result_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/_result_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models._result_helpers`/_
symbols:
  _group_elements_by_type: group_elements_by_type().
  _mcp_metadata_block: mcp_metadata_block().
  _safe_get_attr: safe_get_attr().
  _mcp_import_entries: mcp_import_entries().
  _mcp_class_entries: mcp_class_entries().
  _mcp_method_entries: mcp_method_entries().
  _mcp_field_entries: mcp_field_entries().
  _mcp_annotation_entries: mcp_annotation_entries().
  _mcp_line_range: mcp_line_range().
  _mcp_package_info: mcp_package_info().
  _to_dict_import_row: to_dict_import_row().
  _to_dict_class_row: to_dict_class_row().
  _to_dict_method_row: to_dict_method_row().
  _to_dict_field_row: to_dict_field_row().
  _to_dict_annotation_row: to_dict_annotation_row().
  __all__: _all__.
---
# Module: [`tree_sitter_analyzer/models/_result_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py)

## Functions
- `_group_elements_by_type(elements: Any)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L150) — Single-pass partition of ``elements`` by their ``element_type``.
- `_mcp_annotation_entries(elements: Sequence[Any])` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L107)
- `_mcp_class_entries(elements: Sequence[Any])` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L69)
- `_mcp_field_entries(elements: Sequence[Any])` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L95)
- `_mcp_import_entries(elements: Sequence[Any])` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L56)
- `_mcp_line_range(obj: Any)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L48) — Canonical ``{start, end}`` from any element-like object.
- `_mcp_metadata_block(elements: Sequence[Any], *, line_count: int, analysis_time: float, success: bool, error_message: str | None)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L118) — Element-type counts + analysis flags — paired with ``to_mcp_format``.
- `_mcp_method_entries(elements: Sequence[Any])` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L82)
- `_mcp_package_info(package: Any)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L37) — Normalise the package field for MCP output.
- `_safe_get_attr(obj: Any, attr: str, default: Any = "")` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L24) — Read ``attr`` from an object or dict, falling back to ``default``.
- `_to_dict_annotation_row(ann: Any)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L218) — Build the legacy annotation dict row (name only; falls back to str).
- `_to_dict_class_row(cls: Any)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L195) — Build the legacy class dict row (name + type + package).
- `_to_dict_field_row(field: Any)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L213) — Build the legacy field dict row (name + type).
- `_to_dict_import_row(imp: Any)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L186) — Build the legacy import dict row used by ``AnalysisResult.to_dict``.
- `_to_dict_method_row(method: Any)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L204) — Build the legacy method dict row (name + return_type + parameters).

## Module values
- `__all__` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/_result_helpers.py#L223)

