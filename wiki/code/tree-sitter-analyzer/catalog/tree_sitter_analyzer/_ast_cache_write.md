---
title: 'Module: tree_sitter_analyzer/_ast_cache_write.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_write.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_write`/
symbols:
  write_graph_edges_for_file: write_graph_edges_for_file().
  write_activation_for_file: write_activation_for_file().
  write_imports_for_file: write_imports_for_file().
  logger: logger.
  _insert_import_entry: _insert_import_entry().
  write_fts5_symbols: write_fts5_symbols().
  write_fts5_symbols_from_tuples: write_fts5_symbols_from_tuples().
  _parse_import_raw: _parse_import_raw().
---
# Module: [`tree_sitter_analyzer/_ast_cache_write.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py)

## Functions
- `_insert_import_entry(conn: sqlite3.Connection, rel_path: str, language: str, entry: Any)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L120) — Insert one parsed import entry into ast_imports.
- `_parse_import_raw(raw: Any)` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L109) — Extract (text, line) from a raw import entry (str or dict).
- `write_activation_for_file(conn: sqlite3.Connection, rel_path: str, inserted_symbol_rows: list[dict[str, Any]], project_root: str)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L152) — Refresh ast_symbol_activation rows for a single file.
- `write_fts5_symbols(conn: sqlite3.Connection, rel_path: str, language: str, symbols: dict[str, Any])` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L19) — Replace FTS5 symbol rows for ``rel_path``. Returns inserted row list.
- `write_fts5_symbols_from_tuples(conn: sqlite3.Connection, rel_path: str, language: str, symbol_rows: list[tuple[str, str, int, int]])` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L66) — Insert FTS5 symbols from worker-serialised tuples (name, kind, line, end_line).
- `write_graph_edges_for_file(conn: sqlite3.Connection, rel_path: str, language: str, symbols: dict[str, Any], imports: list[str] | list[dict[str, Any]], call_edges: list[dict[str, Any]], *, preserve_calls: bool = False)` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L238) — Refresh unified EdgeStore rows derived from one indexed file. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
- `write_imports_for_file(conn: sqlite3.Connection, rel_path: str, language: str, imports: list[str] | list[dict[str, Any]])` — [`L213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L213) — Refresh ast_imports rows for rel_path.

## Module values
- `logger` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_write.py#L16)

