---
title: 'Module: tree_sitter_analyzer/mcp/tools/_fts_fast_path.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_fts_fast_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._fts_fast_path`/
symbols:
  try_fts5_fast_path: try_fts5_fast_path().
  _is_fts_eligible: _is_fts_eligible().
  _extensions_to_language: _extensions_to_language().
  _SIMPLE_IDENTIFIER_RE: _SIMPLE_IDENTIFIER_RE.
  _aggregate_by_file: _aggregate_by_file().
  _build_symbol_groups: _build_symbol_groups().
  _match_line_from_fts: _match_line_from_fts().
  _EXTS_TO_LANG_SUFFIX._EXTS_TO_LANG_SUFFIX: _EXTS_TO_LANG_SUFFIX._EXTS_TO_LANG_SUFFIX.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_fts_fast_path.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py)

## Functions
- `_aggregate_by_file(fts_results: list)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L82) — Count FTS results per file path.
- `_build_symbol_groups(fts_results: list)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L91) — Group FTS results into per-file symbol lists, preserving sorted order.
- `_extensions_to_language(arguments: dict[str, Any])` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L74) — Map extensions argument to a language filter for FTS5 search.
- `_is_fts_eligible(arguments: dict[str, Any])` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L45) — Return True if the query can be served from the FTS5 index.
- `_match_line_from_fts(file_path: str, line: int, source_root: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L112) — Best-effort extraction of the matching line text from the source file.
- `try_fts5_fast_path(arguments: dict[str, Any], project_root: str | None, requested_format: str)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L126) — Try to answer the search query from the FTS5 AST index.

## Module values
- `_EXTS_TO_LANG_SUFFIX` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L22)
- `_SIMPLE_IDENTIFIER_RE` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_fts_fast_path.py#L20)

