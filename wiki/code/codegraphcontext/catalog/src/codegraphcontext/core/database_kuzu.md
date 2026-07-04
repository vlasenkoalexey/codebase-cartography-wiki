---
title: 'Module: src/codegraphcontext/core/database_kuzu.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_kuzu.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_kuzu`/
symbols:
  KUZU_SPEC: KUZU_SPEC.
  KuzuDBManager: KuzuDBManager#
  KuzuDBManager.BACKEND_SPEC: KuzuDBManager#BACKEND_SPEC.
  KuzuDBManager._compat_state: KuzuDBManager#_compat_state.
  KuzuDriverWrapper: KuzuDriverWrapper.
  KuzuSessionWrapper: KuzuSessionWrapper.
  KuzuRecord: KuzuRecord.
  KuzuResultWrapper: KuzuResultWrapper.
  _KuzuCompatState: _KuzuCompatState.
---
# Module: [`src/codegraphcontext/core/database_kuzu.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py)

## Classes
### `KuzuDBManager`  ·  implements/extends EmbeddedGraphManager
- def: [`src/codegraphcontext/core/database_kuzu.py:29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L29)
- doc: Manages the KùzuDB database connection as a singleton.
- signature: `class KuzuDBManager(EmbeddedGraphManager):`
- members:
  - `BACKEND_SPEC` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L32)
- protocol/private: `_compat_state`[`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L33)
- uses (calls/refs, reference-scoped): [`KUZU_SPEC`](database_kuzu.md#KUZU_SPEC), [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager), [`EmbeddedCompatState`](database_embedded_kuzu.md#EmbeddedCompatState)
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`get_database_manager`](__init__.md#get_database_manager), [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager)

## Module values
- `KUZU_SPEC` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L18)
- `KuzuDriverWrapper` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L37)
- `KuzuRecord` — [`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L39)
- `KuzuResultWrapper` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L40)
- `KuzuSessionWrapper` — [`L38`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L38)
- `_KuzuCompatState` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_kuzu.py#L41)

