---
title: 'Module: src/codegraphcontext/core/database_ladybug.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_ladybug.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_ladybug`/
symbols:
  LADYBUG_SPEC: LADYBUG_SPEC.
  LadybugDBManager: LadybugDBManager#
  LadybugDBManager.BACKEND_SPEC: LadybugDBManager#BACKEND_SPEC.
  LadybugDBManager._compat_state: LadybugDBManager#_compat_state.
  LadybugDriverWrapper: LadybugDriverWrapper.
  LadybugSessionWrapper: LadybugSessionWrapper.
  LadybugRecord: LadybugRecord.
  LadybugResultWrapper: LadybugResultWrapper.
  _LadybugCompatState: _LadybugCompatState.
---
# Module: [`src/codegraphcontext/core/database_ladybug.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py)

## Classes
### `LadybugDBManager`  ·  implements/extends EmbeddedGraphManager
- def: [`src/codegraphcontext/core/database_ladybug.py:29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L29)
- doc: Manages the LadybugDB database connection as a singleton.
- signature: `class LadybugDBManager(EmbeddedGraphManager):`
- members:
  - `BACKEND_SPEC` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L32)
- protocol/private: `_compat_state`[`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L33)
- uses (calls/refs, reference-scoped): [`LADYBUG_SPEC`](database_ladybug.md#LADYBUG_SPEC), [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager), [`EmbeddedCompatState`](database_embedded_kuzu.md#EmbeddedCompatState)
- used by: [`get_database_manager`](__init__.md#get_database_manager), [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager)

## Module values
- `LADYBUG_SPEC` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L18)
- `LadybugDriverWrapper` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L37)
- `LadybugRecord` — [`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L39)
- `LadybugResultWrapper` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L40)
- `LadybugSessionWrapper` — [`L38`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L38)
- `_LadybugCompatState` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_ladybug.py#L41)

