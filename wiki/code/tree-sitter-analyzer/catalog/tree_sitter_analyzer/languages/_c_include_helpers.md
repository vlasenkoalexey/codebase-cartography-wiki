---
title: 'Module: tree_sitter_analyzer/languages/_c_include_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_c_include_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._c_include_helpers`/
symbols:
  _include_import: _include_import().
  extract_include_info: extract_include_info().
  extract_includes_fallback: extract_includes_fallback().
  _include_from_line: _include_from_line().
  _include_path_match: _include_path_match().
---
# Module: [`tree_sitter_analyzer/languages/_c_include_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py)

## Functions
- `_include_from_line(line: str, line_num: int)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py#L46)
- `_include_import(include_path: str, raw_text: str, line_num: int)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py#L61)
- `_include_path_match(include_text: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py#L40)
- `extract_include_info(node: Any, get_node_text: Callable[..., str])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py#L11) — Extract include directive information.
- `extract_includes_fallback(source_code: str)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_include_helpers.py#L28) — Fallback include extraction using regex.

