---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/node_text.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/node_text.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.node_text`/_
symbols:
  _extract_node_text_by_points: extract_node_text_by_points().
  _extract_node_text_by_bytes: extract_node_text_by_bytes().
  _line_in_bounds: line_in_bounds().
  _slice_single_line: slice_single_line().
  _slice_multiline_node_text: slice_multiline_node_text().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/node_text.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py)

## Functions
- `_extract_node_text_by_bytes(node: tree_sitter.Node, content_lines: list[str], encoding: str)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py#L11) — Extract node text from byte offsets using the file encoding.
- `_extract_node_text_by_points(node: tree_sitter.Node, content_lines: list[str])` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py#L26) — Fallback node text extraction using tree-sitter point coordinates.
- `_line_in_bounds(line_number: int, content_lines: list[str])` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py#L48) — Return whether a line index can be read from content_lines.
- `_slice_multiline_node_text(start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py#L60) — Return bounded line slices for a multi-line node.
- `_slice_single_line(line: str, start_col: int, end_col: int)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/node_text.py#L53) — Return a bounded slice from one line.

