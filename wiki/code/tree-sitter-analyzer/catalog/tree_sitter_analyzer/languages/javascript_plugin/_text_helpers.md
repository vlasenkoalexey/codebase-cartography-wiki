---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._text_helpers`/
symbols:
  get_node_text_optimized: get_node_text_optimized().
  _extract_from_encoded_content: _extract_from_encoded_content().
  _fallback_node_text: _fallback_node_text().
  _fallback_multiline_text: _fallback_multiline_text().
  TextSliceExtractor.TextSliceExtractor: TextSliceExtractor.TextSliceExtractor.
  SafeEncoder.SafeEncoder: SafeEncoder.SafeEncoder.
  _slice_fallback_line: _slice_fallback_line().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py)

## Functions
- `_extract_from_encoded_content(node: tree_sitter.Node, content_lines: list[str], file_encoding: str | None, extract_text_slice_func: TextSliceExtractor, safe_encode_func: SafeEncoder)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L46)
- `_fallback_multiline_text(start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L78)
- `_fallback_node_text(node: tree_sitter.Node, content_lines: list[str])` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L63)
- `_slice_fallback_line(line_index: int, start_point: tuple[int, int], end_point: tuple[int, int], content_lines: list[str])` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L92)
- `get_node_text_optimized(node: tree_sitter.Node, content_lines: list[str], file_encoding: str | None, node_text_cache: dict[tuple[int, int], str], extract_text_slice_func: TextSliceExtractor, safe_encode_func: SafeEncoder)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L18) — Get node text with optimized caching using position-based keys.

## Module values
- `SafeEncoder` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L15)
- `TextSliceExtractor` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.py#L14)

