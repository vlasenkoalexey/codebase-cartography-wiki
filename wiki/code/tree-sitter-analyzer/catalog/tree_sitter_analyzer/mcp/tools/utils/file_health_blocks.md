---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.file_health_blocks`/
symbols:
  find_long_blocks_heuristic: find_long_blocks_heuristic().
  _BlockTracker.start: _BlockTracker#start().
  _BlockTracker.snapshot: _BlockTracker#snapshot().
  _BlockTracker.ended_at: _BlockTracker#ended_at().
  _BlockTracker: _BlockTracker#
  _BlockTracker.active: _BlockTracker#active.
  _BlockTracker.block_lines: _BlockTracker#block_lines.
  _TripleQuoteTracker.update: _TripleQuoteTracker#update().
  _BlockTracker.process_line: _BlockTracker#process_line().
  _TripleQuoteTracker.inside: _TripleQuoteTracker#inside.
  _BlockTracker.def_name: _BlockTracker#def_name.
  _BlockTracker.def_indent: _BlockTracker#def_indent.
  _TripleQuoteTracker.delimiter: _TripleQuoteTracker#delimiter.
  _BlockTracker.def_start: _BlockTracker#def_start.
  _TripleQuoteTracker: _TripleQuoteTracker#
  _BlockTracker.__init__: _BlockTracker#__init__().
  _TripleQuoteTracker.__init__: _TripleQuoteTracker#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py)

## Classes
### `_BlockTracker`
- def: [`tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py:65`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L65)
- members:
  - `__init__(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L68) — Initialize block tracker state.
  - `ended_at(self, stripped: str, line: str)` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L92) — Check if the current block has ended at this line.
  - `process_line(self)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L88) — Process a line within a tracked block.
  - `snapshot(self)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L84) — Return a snapshot of the current block.
  - `start(self, name: str, start: int, indent: int)` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L76) — Start tracking a new function block.
  - `active` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L70)
  - `block_lines` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L74)
  - `def_indent` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L73)
  - `def_name` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L71)
  - `def_start` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L72)
- used by: [`find_long_blocks_heuristic`](file_health_blocks.md#find_long_blocks_heuristic)  (9 test-only)

### `_TripleQuoteTracker`
- def: [`tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py:117`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L117)
- members:
  - `update(self, line: str)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L133) — Advance the tracker for ``line`` and return the resulting state.
  - `delimiter` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L131)
  - `inside` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L130)
- protocol/private: `__init__`[`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L129)
- used by: [`find_long_blocks_heuristic`](file_health_blocks.md#find_long_blocks_heuristic)

## Functions
- `find_long_blocks_heuristic(lines: list[str], threshold: int = 50)` — [`L6`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_blocks.py#L6) — Fallback long block detection using indentation heuristics.

