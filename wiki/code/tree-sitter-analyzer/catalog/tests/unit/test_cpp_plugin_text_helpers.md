---
title: 'Module: tests/unit/test_cpp_plugin_text_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_cpp_plugin_text_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_cpp_plugin_text_helpers`/
symbols:
  TestGetNodeTextOptimized.test_extraction_success: TestGetNodeTextOptimized#test_extraction_success().
  TestGetNodeTextOptimized.test_extraction_failure_uses_fallback: TestGetNodeTextOptimized#test_extraction_failure_uses_fallback().
  TestGetNodeTextOptimized.test_cache_hit: TestGetNodeTextOptimized#test_cache_hit().
  _make_node: _make_node().
  TestFallbackNodeTextUncached.test_single_line_extraction: TestFallbackNodeTextUncached#test_single_line_extraction().
  TestFallbackNodeTextUncached.test_multiline_extraction: TestFallbackNodeTextUncached#test_multiline_extraction().
  TestFallbackMultilineText.test_extracts_all_lines_between_points: TestFallbackMultilineText#test_extracts_all_lines_between_points().
  TestFallbackMultilineText.test_handles_end_beyond_content: TestFallbackMultilineText#test_handles_end_beyond_content().
  TestSliceFallbackLine.test_first_line_slices_from_start: TestSliceFallbackLine#test_first_line_slices_from_start().
  TestSliceFallbackLine.test_last_line_slices_to_end: TestSliceFallbackLine#test_last_line_slices_to_end().
  TestSliceFallbackLine.test_middle_line_returns_full: TestSliceFallbackLine#test_middle_line_returns_full().
  TestGetNodeTextOptimized.extract_slice: TestGetNodeTextOptimized#extract_slice().
  TestGetNodeTextOptimized.failing_extract: TestGetNodeTextOptimized#failing_extract().
  TestGetNodeTextOptimized: TestGetNodeTextOptimized#
  TestFallbackNodeTextUncached: TestFallbackNodeTextUncached#
  TestFallbackMultilineText: TestFallbackMultilineText#
  TestSliceFallbackLine: TestSliceFallbackLine#
---
# Module: [`tests/unit/test_cpp_plugin_text_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py)

## Classes
### `TestFallbackMultilineText`
- def: [`tests/unit/test_cpp_plugin_text_helpers.py:84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L84)
- signature: `class TestFallbackMultilineText:`
- members:
  - `test_extracts_all_lines_between_points(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L85)
  - `test_handles_end_beyond_content(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L92)
- uses (calls/refs, reference-scoped): [`_fallback_multiline_text`](../../tree_sitter_analyzer/languages/_cpp_plugin_text_helpers.md#_fallback_multiline_text)

### `TestFallbackNodeTextUncached`
- def: [`tests/unit/test_cpp_plugin_text_helpers.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L72)
- signature: `class TestFallbackNodeTextUncached:`
- members:
  - `test_multiline_extraction(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L78)
  - `test_single_line_extraction(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L73)
- uses (calls/refs, reference-scoped): [`_fallback_node_text_uncached`](../../tree_sitter_analyzer/languages/_cpp_plugin_text_helpers.md#_fallback_node_text_uncached)

### `TestGetNodeTextOptimized`
- def: [`tests/unit/test_cpp_plugin_text_helpers.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L22)
- signature: `class TestGetNodeTextOptimized:`
- members:
  - `extract_slice(data, start, end, enc)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L40)
  - `failing_extract(*_)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L57)
  - `test_cache_hit(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L23)
  - `test_extraction_failure_uses_fallback(self)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L54)
  - `test_extraction_success(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L36)
- uses (calls/refs, reference-scoped): [`get_node_text_optimized`](../../tree_sitter_analyzer/languages/_cpp_plugin_text_helpers.md#get_node_text_optimized)  (1 test-only)

### `TestSliceFallbackLine`
- def: [`tests/unit/test_cpp_plugin_text_helpers.py:98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L98)
- signature: `class TestSliceFallbackLine:`
- members:
  - `test_first_line_slices_from_start(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L99)
  - `test_last_line_slices_to_end(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L104)
  - `test_middle_line_returns_full(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L109)
- uses (calls/refs, reference-scoped): [`_slice_fallback_line`](../../tree_sitter_analyzer/languages/_cpp_plugin_text_helpers.md#_slice_fallback_line)

## Functions
- `_make_node(start_byte, end_byte, start_row, start_col, end_row, end_col)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_plugin_text_helpers.py#L13)

