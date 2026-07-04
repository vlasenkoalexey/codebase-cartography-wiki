---
title: 'Module: tree_sitter_analyzer/_ast_cache_build_state.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_build_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_build_state`/
symbols:
  build_in_progress: build_in_progress().
  mark_build_in_progress: mark_build_in_progress().
  clear_build_in_progress: clear_build_in_progress().
  _pid_alive: _pid_alive().
  logger: logger.
  _DEFAULT_TTL_SECONDS: _DEFAULT_TTL_SECONDS.
  _CLOCK_SKEW_GRACE_SECONDS: _CLOCK_SKEW_GRACE_SECONDS.
  _CREATE_DDL: _CREATE_DDL.
---
# Module: [`tree_sitter_analyzer/_ast_cache_build_state.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py)

## Functions
- `_pid_alive(pid: int)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L55) — Best-effort: is a process with this pid running on THIS machine?
- `build_in_progress(conn: sqlite3.Connection, *, ttl_seconds: float = _DEFAULT_TTL_SECONDS)` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L111) — True iff a full rebuild is actively in progress.
- `clear_build_in_progress(conn: sqlite3.Connection)` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L102) — Clear the marker after a rebuild finishes (or aborts cleanly).
- `mark_build_in_progress(conn: sqlite3.Connection)` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L76) — Stamp the single-row marker that a full rebuild has started.

## Module values
- `_CLOCK_SKEW_GRACE_SECONDS` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L44)
- `_CREATE_DDL` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L46)
- `_DEFAULT_TTL_SECONDS` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L40)
- `logger` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_build_state.py#L32)

