---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_text_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_text_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._text_helpers`/_
symbols:
  _extract_node_text_by_points: extract_node_text_by_points().
  _extract_node_text_by_bytes: extract_node_text_by_bytes().
  _extract_single_line_text: extract_single_line_text().
  _point_range_within_lines: point_range_within_lines().
  _clamped_line_slice: clamped_line_slice().
  _extract_multiline_text: extract_multiline_text().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_text_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py)

## Functions
- `_clamped_line_slice(line: str, start_col: int, end_col: int)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L47)
- `_extract_multiline_text(content_lines: list[str], start_point: tuple[int, int], end_point: tuple[int, int])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L53)
- `_extract_node_text_by_bytes(content_lines: list[str], encoding: str, start_byte: int, end_byte: int, safe_encode_fn: Callable[[str, str], bytes] = safe_encode, extract_text_slice_fn: Callable[[bytes, int, int, str], str] = extract_text_slice)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L10)
- `_extract_node_text_by_points(content_lines: list[str], start_point: tuple[int, int], end_point: tuple[int, int])` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L22)
- `_extract_single_line_text(content_lines: list[str], start_point: tuple[int, int], end_point: tuple[int, int])` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L40)
- `_point_range_within_lines(start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_text_helpers.py#L32)

