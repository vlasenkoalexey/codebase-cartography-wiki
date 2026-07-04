---
title: 'Module: src/codegraphcontext/tools/datasources/redis_ingester.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/datasources/redis_ingester.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.datasources.redis_ingester`/
symbols:
  ingest: ingest().
  _normalize_pattern: _normalize_pattern().
---
# Module: [`src/codegraphcontext/tools/datasources/redis_ingester.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/redis_ingester.py)

## Functions
- `_normalize_pattern(key: str)` — [`L18`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/redis_ingester.py#L18) — Replace numeric / UUID segments with * to group keys into patterns.
- `ingest(host: str, port: int, db: int = 0, password: Optional[str] = None, name: Optional[str] = None, env: str = "production", scan_count: int = 1000, max_keys: int = 10000)` — [`L40`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/datasources/redis_ingester.py#L40) — Discover Redis key patterns and return a datasource graph dict.

