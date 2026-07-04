---
title: 'Module: graphify/pg_introspect.py'
type: catalog
provenance: extracted
module: graphify/pg_introspect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.pg_introspect`/
symbols:
  _quote_ident: _quote_ident().
  introspect_postgres: introspect_postgres().
---
# Module: [`graphify/pg_introspect.py`](../../../../../raw/code/graphify/graphify/pg_introspect.py)

## Functions
- `_quote_ident(name: str)` — [`L6`](../../../../../raw/code/graphify/graphify/pg_introspect.py#L6) — Double-quote a PostgreSQL identifier, escaping embedded double-quotes.
- `introspect_postgres(dsn: str | None = None)` — [`L11`](../../../../../raw/code/graphify/graphify/pg_introspect.py#L11) — Connect to PostgreSQL, reconstruct DDL, and extract via extract_sql().

