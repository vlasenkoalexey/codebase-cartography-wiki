---
title: 'Module: tests/unit/test_ast_cache_maintenance.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_maintenance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_maintenance`/
symbols:
  _FakeConn.execute: _FakeConn#execute().
  test_index_project_force_includes_db_maintenance: test_index_project_force_includes_db_maintenance().
  test_reclaim_storage_skips_when_free_pages_are_below_threshold: test_reclaim_storage_skips_when_free_pages_are_below_threshold().
  test_reclaim_storage_vacuums_legacy_auto_vacuum_none_db: test_reclaim_storage_vacuums_legacy_auto_vacuum_none_db().
  test_reclaim_storage_uses_incremental_vacuum_when_enabled: test_reclaim_storage_uses_incremental_vacuum_when_enabled().
  _Cursor: _Cursor#
  _FakeConn: _FakeConn#
  _Cursor.fetchone: _Cursor#fetchone().
  _FakeConn.commands: _FakeConn#commands.
  test_get_db_storage_stats_reports_exact_page_counters: test_get_db_storage_stats_reports_exact_page_counters().
  _BrokenConn.execute: _BrokenConn#execute().
  test_reclaim_storage_reports_errors_without_raising: test_reclaim_storage_reports_errors_without_raising().
  _FakeConn.commits: _FakeConn#commits.
  _BrokenConn: _BrokenConn#
  _FakeConn.free_pages: _FakeConn#free_pages.
  _Row.__getitem__: _Row#__getitem__().
  _FakeConn.commit: _FakeConn#commit().
  _Row: _Row#
  _FakeConn.auto_vacuum: _FakeConn#auto_vacuum.
  _Row._value: _Row#_value.
  _Cursor._value: _Cursor#_value.
  test_index_project_force_includes_db_maintenance._fake_reclaim: test_index_project_force_includes_db_maintenance()._fake_reclaim().
  _Row.__init__: _Row#__init__().
  _Cursor.__init__: _Cursor#__init__().
  _FakeConn.__init__: _FakeConn#__init__().
---
# Module: [`tests/unit/test_ast_cache_maintenance.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py)

## Classes
### `_BrokenConn`  ·  implements/extends _FakeConn
- def: [`tests/unit/test_ast_cache_maintenance.py:131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L131)
- signature: `class _BrokenConn(_FakeConn):`
- members:
  - `execute(self, sql: str)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L132)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `_Cursor`
- def: [`tests/unit/test_ast_cache_maintenance.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L24)
- signature: `class _Cursor:`
- members:
  - `fetchone(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L28)
- protocol/private: `__init__`[`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L25), `_value`[`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L26)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `_FakeConn`
- def: [`tests/unit/test_ast_cache_maintenance.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L32)
- signature: `class _FakeConn:`
- members:
  - `commit(self)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L60)
  - `execute(self, sql: str)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L39)
  - `auto_vacuum` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L37)
  - `commands` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L34)
  - `commits` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L35)
  - `free_pages` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L36)
- protocol/private: `__init__`[`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L33)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (6 test-only callers)

### `_Row`
- def: [`tests/unit/test_ast_cache_maintenance.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L15)
- signature: `class _Row:`
- protocol/private: `__getitem__`[`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L19), `__init__`[`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L16), `_value`[`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L17)
- used by: (1 test-only callers)

## Functions
- `_fake_reclaim(conn, db_path)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L162)
- `test_get_db_storage_stats_reports_exact_page_counters()` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L64)
- `test_index_project_force_includes_db_maintenance(tmp_path, monkeypatch)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L151)
- `test_reclaim_storage_reports_errors_without_raising()` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L138)
- `test_reclaim_storage_skips_when_free_pages_are_below_threshold()` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L80)
- `test_reclaim_storage_uses_incremental_vacuum_when_enabled()` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L117)
- `test_reclaim_storage_vacuums_legacy_auto_vacuum_none_db()` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_maintenance.py#L100)

