---
title: 'Module: src/codegraphcontext/tools/indexing/persistence/utils.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/persistence/utils.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.persistence.utils`/
symbols:
  get_backend_type: get_backend_type().
  execute_write_operation: execute_write_operation().
  execute_read_operation: execute_read_operation().
---
# Module: [`src/codegraphcontext/tools/indexing/persistence/utils.py`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/persistence/utils.py)

## Functions
- `execute_read_operation(driver: Any, backend: str, work_fn: callable)` — [`L34`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/persistence/utils.py#L34) — Execute a database read operation utilizing managed read transactions where supported. — documented in [codegraphcontext-tools-indexing-persistence-utils](../../../../../../concepts/codegraphcontext-tools-indexing-persistence-utils.md)
- `execute_write_operation(driver: Any, backend: str, work_fn: callable)` — [`L13`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/persistence/utils.py#L13) — Execute a database write operation with full transaction and retry support. — documented in [codegraphcontext-server](../../../../../../concepts/codegraphcontext-server.md)
- `get_backend_type(driver: Any, db_manager: Any = None)` — [`L6`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/persistence/utils.py#L6) — Determine the database backend type dynamically. — documented in [codegraphcontext-server](../../../../../../concepts/codegraphcontext-server.md)

