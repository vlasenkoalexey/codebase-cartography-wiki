---
title: 'Module: tests/unit/test_file_health_blocks.py'
type: catalog
provenance: extracted
module: tests/unit/test_file_health_blocks.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_file_health_blocks`/Test
symbols:
  TestBlockTracker.test_start_sets_state: BlockTracker#test_start_sets_state().
  TestBlockTracker.test_initial_state: BlockTracker#test_initial_state().
  TestBlockTracker.test_process_line_increments: BlockTracker#test_process_line_increments().
  TestBlockTracker.test_ended_at_unindented_def: BlockTracker#test_ended_at_unindented_def().
  TestBlockTracker.test_snapshot_returns_tuple: BlockTracker#test_snapshot_returns_tuple().
  TestBlockTracker.test_ended_at_same_indent_non_def: BlockTracker#test_ended_at_same_indent_non_def().
  TestBlockTracker.test_ended_at_empty_line: BlockTracker#test_ended_at_empty_line().
  TestBlockTracker.test_ended_at_class_at_same_indent: BlockTracker#test_ended_at_class_at_same_indent().
  TestBlockTracker.test_ended_at_decorator: BlockTracker#test_ended_at_decorator().
  TestFindLongBlocksHeuristic.test_empty_lines_no_blocks: FindLongBlocksHeuristic#test_empty_lines_no_blocks().
  TestFindLongBlocksHeuristic.test_short_function_not_reported: FindLongBlocksHeuristic#test_short_function_not_reported().
  TestFindLongBlocksHeuristic.test_long_function_detected: FindLongBlocksHeuristic#test_long_function_detected().
  TestFindLongBlocksHeuristic.test_multiple_functions_tracks_each: FindLongBlocksHeuristic#test_multiple_functions_tracks_each().
  TestFindLongBlocksHeuristic.test_async_def_detected: FindLongBlocksHeuristic#test_async_def_detected().
  TestFindLongBlocksHeuristic.test_results_sorted_by_length_descending: FindLongBlocksHeuristic#test_results_sorted_by_length_descending().
  TestFindLongBlocksHeuristic.test_nested_def_increments_correctly: FindLongBlocksHeuristic#test_nested_def_increments_correctly().
  TestBlockTracker: BlockTracker#
  TestFindLongBlocksHeuristic: FindLongBlocksHeuristic#
---
# Module: [`tests/unit/test_file_health_blocks.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py)

## Classes
### `TestBlockTracker`
- def: [`tests/unit/test_file_health_blocks.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L15)
- signature: `class TestBlockTracker:`
- members:
  - `test_ended_at_class_at_same_indent(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L62)
  - `test_ended_at_decorator(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L67)
  - `test_ended_at_empty_line(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L57)
  - `test_ended_at_same_indent_non_def(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L52)
  - `test_ended_at_unindented_def(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L46)
  - `test_initial_state(self)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L16)
  - `test_process_line_increments(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L31)
  - `test_snapshot_returns_tuple(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L38)
  - `test_start_sets_state(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L22)
- uses (calls/refs, reference-scoped): [`start`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.start), [`snapshot`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.snapshot), [`_BlockTracker`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker), [`ended_at`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.ended_at), [`active`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.active), [`block_lines`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.block_lines), [`process_line`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.process_line), [`def_indent`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.def_indent), [`def_name`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.def_name), [`def_start`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#_BlockTracker.def_start)

### `TestFindLongBlocksHeuristic`
- def: [`tests/unit/test_file_health_blocks.py:78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L78)
- signature: `class TestFindLongBlocksHeuristic:`
- members:
  - `test_async_def_detected(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L107)
  - `test_empty_lines_no_blocks(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L79)
  - `test_long_function_detected(self)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L88)
  - `test_multiple_functions_tracks_each(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L96)
  - `test_nested_def_increments_correctly(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L124) — Inner def at higher indent should not reset outer tracking.
  - `test_results_sorted_by_length_descending(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L113)
  - `test_short_function_not_reported(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_blocks.py#L83)
- uses (calls/refs, reference-scoped): [`find_long_blocks_heuristic`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.md#find_long_blocks_heuristic)

