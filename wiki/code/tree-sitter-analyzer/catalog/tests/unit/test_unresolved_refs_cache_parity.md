---
title: 'Module: tests/unit/test_unresolved_refs_cache_parity.py'
type: catalog
provenance: extracted
module: tests/unit/test_unresolved_refs_cache_parity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_unresolved_refs_cache_parity`/
symbols:
  test_candidate_cache_collapses_duplicate_selects: test_candidate_cache_collapses_duplicate_selects().
  test_cached_candidate_lookup_matches_uncached_byte_for_byte: test_cached_candidate_lookup_matches_uncached_byte_for_byte().
  _CountingConn.execute: _CountingConn#execute().
  _CountingConn.candidate_selects: _CountingConn#candidate_selects.
  _reset_resolution: _reset_resolution().
  _write_repeated_name_project: _write_repeated_name_project().
  _CountingConn._conn: _CountingConn#_conn.
  _CountingConn.commit: _CountingConn#commit().
  _CountingConn.__getattr__: _CountingConn#__getattr__().
  test_candidate_cache_returns_empty_on_broken_connection: test_candidate_cache_returns_empty_on_broken_connection().
  _snapshot_edges: _snapshot_edges().
  _CountingConn: _CountingConn#
  test_cached_candidate_lookup_matches_uncached_byte_for_byte.uncached: test_cached_candidate_lookup_matches_uncached_byte_for_byte().uncached().
  test_candidate_cache_collapses_duplicate_selects.uncached: test_candidate_cache_collapses_duplicate_selects().uncached().
  _CountingConn.__init__: _CountingConn#__init__().
---
# Module: [`tests/unit/test_unresolved_refs_cache_parity.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py)

## Classes
### `_CountingConn`
- def: [`tests/unit/test_unresolved_refs_cache_parity.py:67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L67)
- doc: Wrap a sqlite3 connection and count candidate-table SELECTs.
- signature: `class _CountingConn:`
- members:
  - `commit(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L79)
  - `execute(self, sql: str, *args: Any, **kwargs: Any)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L74)
  - `candidate_selects` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L72)
- protocol/private: `__getattr__`[`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L82), `__init__`[`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L70), `_conn`[`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L71)
- used by: (1 test-only callers)

## Functions
- `_reset_resolution(conn: sqlite3.Connection)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L86) — Reset CALLS resolution + drop second-pass EXTENDS edges so the pass re-runs.
- `_snapshot_edges(conn: sqlite3.Connection)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L56) — Full, deterministic snapshot of every edge row (resolution columns incl.).
- `_write_repeated_name_project(root: Path)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L24) — A project where one callee/base name recurs across many files.
- `test_cached_candidate_lookup_matches_uncached_byte_for_byte(tmp_path: Path)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L96) — Cached pass == uncached pass: identical edge snapshot + identical stats. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- `test_candidate_cache_collapses_duplicate_selects(tmp_path: Path)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L145) — The cache must issue far fewer candidate SELECTs than the uncached path. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- `test_candidate_cache_returns_empty_on_broken_connection()` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L178) — A failing candidate SELECT still yields [] and is cached as the abort.
- `uncached(c: Any, sf: str, rn: str, rk: str, _cache: Any = None)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L120)
- `uncached(c: Any, sf: str, rn: str, rk: str, _cache: Any = None)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unresolved_refs_cache_parity.py#L157)

