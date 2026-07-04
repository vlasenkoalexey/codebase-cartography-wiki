---
title: 'Module: tests/test_falkordb_integration.py'
type: catalog
provenance: extracted
module: tests/test_falkordb_integration.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_falkordb_integration`/
symbols:
  test_push_to_falkordb_creates_expected_graph: test_push_to_falkordb_creates_expected_graph().
  test_push_to_falkordb_is_idempotent: test_push_to_falkordb_is_idempotent().
  _connect: _connect().
  GRAPH_NAME: GRAPH_NAME.
  HOST: HOST.
  PORT: PORT.
  db: db().
  FIXTURES: FIXTURES.
  falkordb: falkordb.
---
# Module: [`tests/test_falkordb_integration.py`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py)

## Functions
- `_connect()` — [`L28`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L28) — Return a connected FalkorDB client, or skip if none is reachable.
- `db()` — [`L39`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L39)
- `test_push_to_falkordb_creates_expected_graph(db)` — [`L53`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L53)
- `test_push_to_falkordb_is_idempotent(db)` — [`L75`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L75) — MERGE-based push is safe to re-run - counts must not grow.

## Module values
- `FIXTURES` — [`L22`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L22)
- `GRAPH_NAME` — [`L25`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L25)
- `HOST` — [`L23`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L23)
- `PORT` — [`L24`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L24)
- `falkordb` — [`L20`](../../../../../raw/code/graphify/tests/test_falkordb_integration.py#L20)

