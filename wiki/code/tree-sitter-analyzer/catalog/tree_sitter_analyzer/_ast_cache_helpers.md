---
title: 'Module: tree_sitter_analyzer/_ast_cache_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_helpers`/_
symbols:
  _commit_index_results: commit_index_results().
  _build_function_entry: build_function_entry().
  _project_index_activation_enabled: project_index_activation_enabled().
  _make_error_entry: make_error_entry().
  _process_one_index_result: process_one_index_result().
  _COMMIT_BATCH_SIZE: COMMIT_BATCH_SIZE.
---
# Module: [`tree_sitter_analyzer/_ast_cache_helpers.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py)

## Functions
- `_build_function_entry(sym: dict[str, Any], file_path: str, language: str)` — [`L13`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L13) — Build one function-entry dict from a symbol row.
- `_commit_index_results(conn: Any, results: list[dict[str, Any]], stats: dict[str, Any], insert_fn: Any, indexed_at: str, activation_enabled: bool, batch_size: int = _COMMIT_BATCH_SIZE)` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L75) — Commit worker results to the DB in bounded-size transactions.
- `_make_error_entry(rel_path: str, reason: str)` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L64)
- `_process_one_index_result(r: dict[str, Any], stats: dict[str, Any], insert_fn: Any, indexed_at: str, activation_enabled: bool)` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L38) — Apply one worker result dict to stats and DB (in-place).
- `_project_index_activation_enabled(include_activation: bool | None)` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L30) — Return whether project-wide indexing should compute git activation.

## Module values
- `_COMMIT_BATCH_SIZE` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_helpers.py#L72)

