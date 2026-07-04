---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.file_health_locations`/
symbols:
  deepest_nesting_location: deepest_nesting_location().
  largest_function: largest_function().
  first_control_flow_line: first_control_flow_line().
  first_import_line: first_import_line().
  counts_for_nesting: counts_for_nesting().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py)

## Functions
- `counts_for_nesting(stripped_line: str)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py#L40) — Return whether an indented line is likely executable nesting signal.
- `deepest_nesting_location(lines: list[str])` — [`L11`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py#L11) — Return the deepest indentation-derived nesting depth and its line.
- `first_control_flow_line(lines: list[str])` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py#L60) — Return the first likely decision branch line.
- `first_import_line(lines: list[str])` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py#L84) — Return the first likely import/dependency declaration line.
- `largest_function(analysis: Any)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_locations.py#L50) — Return the largest function-like element from analysis, if available.

