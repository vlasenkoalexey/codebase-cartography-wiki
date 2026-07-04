---
title: 'Module: tests/test_pg_introspect.py'
type: catalog
provenance: extracted
module: tests/test_pg_introspect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_pg_introspect`/
symbols:
  _q: _q().
  test_pg_introspect_success: test_pg_introspect_success().
  test_pg_introspect_quoted_identifiers: test_pg_introspect_quoted_identifiers().
  test_pg_introspect_composite_fk: test_pg_introspect_composite_fk().
  test_pg_introspect_connection_error: test_pg_introspect_connection_error().
  _make_mock_psycopg: _make_mock_psycopg().
  _make_mock_psycopg.MockCursor.fetchall: _make_mock_psycopg().MockCursor#fetchall().
  _make_mock_psycopg.MockConnection.cursor: _make_mock_psycopg().MockConnection#cursor().
  test_pg_introspect_import_error: test_pg_introspect_import_error().
  _make_mock_psycopg.MockCursor: _make_mock_psycopg().MockCursor#
  MockCursor.query: MockCursor#query.
  _make_mock_psycopg.MockConnection: _make_mock_psycopg().MockConnection#
  test_pg_introspect_connection_error.FakeOperationalError: test_pg_introspect_connection_error().FakeOperationalError#
  _make_mock_psycopg.MockCursor.__enter__: _make_mock_psycopg().MockCursor#__enter__().
  _make_mock_psycopg.MockCursor.__exit__: _make_mock_psycopg().MockCursor#__exit__().
  _make_mock_psycopg.MockCursor.execute: _make_mock_psycopg().MockCursor#execute().
  _make_mock_psycopg.MockConnection.execute: _make_mock_psycopg().MockConnection#execute().
  _make_mock_psycopg.MockConnection.close: _make_mock_psycopg().MockConnection#close().
  _make_mock_psycopg.MockConnection.info: _make_mock_psycopg().MockConnection#info().
---
# Module: [`tests/test_pg_introspect.py`](../../../../../raw/code/graphify/tests/test_pg_introspect.py)

## Classes
### `FakeOperationalError`  ·  implements/extends Exception
- def: [`tests/test_pg_introspect.py:251`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L251)
- signature: `class FakeOperationalError(Exception):`
- used by: (1 test-only callers)

### `MockConnection`
- def: [`tests/test_pg_introspect.py:49`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L49)
- signature: `class MockConnection:`
- members:
  - `close(self)` — [`L56`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L56)
  - `cursor(self)` — [`L53`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L53)
  - `execute(self, query)` — [`L50`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L50)
  - `info(self)` — [`L60`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L60)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `MockCursor`
- def: [`tests/test_pg_introspect.py:27`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L27)
- signature: `class MockCursor:`
- members:
  - `execute(self, query, params=None)` — [`L34`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L34)
  - `fetchall(self)` — [`L37`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L37)
  - `query` — [`L35`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L35)
- protocol/private: `__enter__`[`L28`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L28), `__exit__`[`L31`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L31)
- used by: (1 test-only callers)

## Functions
- `_make_mock_psycopg(tables, views, routines, fks, host="myhost", dbname="mydb", connect_raises=None)` — [`L16`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L16) — Return a mock psycopg module wired to the provided catalog data.
- `_q(schema: str, name: str)` — [`L85`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L85) — Return the label form that tree-sitter produces for a quoted identifier.
- `test_pg_introspect_composite_fk()` — [`L198`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L198) — A 2-column composite FK must produce exactly ONE references edge, not two.
- `test_pg_introspect_connection_error()` — [`L247`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L247) — A psycopg.OperationalError must be re-raised as ConnectionError with a
- `test_pg_introspect_import_error()` — [`L274`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L274) — If psycopg is missing, introspect_postgres raises ImportError.
- `test_pg_introspect_quoted_identifiers()` — [`L159`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L159) — Reserved-word and special-character table names must survive DDL round-trip.
- `test_pg_introspect_success()` — [`L99`](../../../../../raw/code/graphify/tests/test_pg_introspect.py#L99) — Baseline: tables, views, routines, and a single-column FK all survive.

