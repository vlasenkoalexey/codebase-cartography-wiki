---
title: 'Module: tree_sitter_analyzer/_ast_cache_synapse.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_synapse.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_synapse`/
symbols:
  resolve_call_edges_for_file: resolve_call_edges_for_file().
  run_synapse_backfill: run_synapse_backfill().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/_ast_cache_synapse.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_synapse.py)

## Functions
- `resolve_call_edges_for_file(cache: Any, conn: sqlite3.Connection, rel_path: str)` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_synapse.py#L19) — Resolve Synapse call-edge columns for ``rel_path`` (skipped when disabled).
- `run_synapse_backfill(cache: Any, conn: sqlite3.Connection)` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_synapse.py#L75) — Re-resolve every unresolved call edge. Returns stats dict or None.

## Module values
- `logger` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_synapse.py#L16)

