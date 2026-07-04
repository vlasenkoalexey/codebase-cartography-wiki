---
title: 'Module: src/codegraphcontext/tools/datasources/mysql_ingester.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/datasources/mysql_ingester.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.datasources.mysql_ingester`/
symbols:
  ingest: ingest().
  _connect: _connect().
---
# Module: [`src/codegraphcontext/tools/datasources/mysql_ingester.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/mysql_ingester.py)

## Functions
- `_connect(host: str, port: int, user: str, password: str, database: str)` — [`L16`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/mysql_ingester.py#L16) — Return a DB-API 2.0 connection. Tries PyMySQL then mysql-connector-python.
- `ingest(host: str, port: int, user: str, password: str, database: str, name: Optional[str] = None, env: str = "production")` — [`L38`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/mysql_ingester.py#L38) — Fetch schema from Aurora MySQL and return a datasource graph dict.

