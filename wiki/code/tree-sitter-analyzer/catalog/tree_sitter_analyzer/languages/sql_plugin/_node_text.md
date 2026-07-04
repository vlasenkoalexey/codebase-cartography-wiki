---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/_node_text.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/_node_text.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin._node_text`/
symbols:
  _extract_by_points: _extract_by_points().
  get_node_text: get_node_text().
  _extract_by_bytes: _extract_by_bytes().
  _slice_multiline_node_text: _slice_multiline_node_text().
  NodeTextCache: NodeTextCache.
  _line_in_bounds: _line_in_bounds().
  _slice_single_line: _slice_single_line().
  _slice_line_in_span: _slice_line_in_span().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/_node_text.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py)

## Functions
- `_extract_by_bytes(node: tree_sitter.Node, content_lines: list[str], encoding: str)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L36) — Extract node text with tree-sitter byte offsets.
- `_extract_by_points(node: tree_sitter.Node, content_lines: list[str], node_text_cache: NodeTextCache, cache_key: tuple[int, int])` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L55) — Extract node text with tree-sitter point coordinates.
- `_line_in_bounds(line_number: int, content_lines: list[str])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L89) — Return whether a point line index is readable.
- `_slice_line_in_span(line_number: int, start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L118) — Return one line slice for a multi-line node span.
- `_slice_multiline_node_text(start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L101) — Return bounded line slices for a multi-line node.
- `_slice_single_line(line: str, start_col: int, end_col: int)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L94) — Return a bounded slice from one line.
- `get_node_text(node: tree_sitter.Node, content_lines: list[str], node_text_cache: NodeTextCache, file_encoding: str | None)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L17) — Return cached node text, falling back from byte offsets to point slices.

## Module values
- `NodeTextCache` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_node_text.py#L14)

