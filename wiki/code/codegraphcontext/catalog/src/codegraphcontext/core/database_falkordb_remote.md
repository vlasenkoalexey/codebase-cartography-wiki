---
title: 'Module: src/codegraphcontext/core/database_falkordb_remote.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_falkordb_remote.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_falkordb_remote`/FalkorDBRemoteManager#
symbols:
  FalkorDBRemoteManager.get_driver: get_driver().
  FalkorDBRemoteManager.close_driver: close_driver().
  FalkorDBRemoteManager: ''
  FalkorDBRemoteManager.__new__: __new__().
  FalkorDBRemoteManager._driver: _driver.
  FalkorDBRemoteManager._graph: _graph.
  FalkorDBRemoteManager._instance: _instance.
  FalkorDBRemoteManager.shutdown: shutdown().
  FalkorDBRemoteManager._initialized: _initialized.
  FalkorDBRemoteManager.is_connected: is_connected().
  FalkorDBRemoteManager._lock: _lock.
  FalkorDBRemoteManager.host: host.
  FalkorDBRemoteManager.port: port.
  FalkorDBRemoteManager.password: password.
  FalkorDBRemoteManager.username: username.
  FalkorDBRemoteManager.ssl: ssl.
  FalkorDBRemoteManager.graph_name: graph_name.
  FalkorDBRemoteManager.validate_config: validate_config().
  FalkorDBRemoteManager.test_connection: test_connection().
  FalkorDBRemoteManager.__init__: __init__().
  FalkorDBRemoteManager.get_backend_type: get_backend_type().
---
# Module: [`src/codegraphcontext/core/database_falkordb_remote.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py)

## Classes
### `FalkorDBRemoteManager`
- def: [`src/codegraphcontext/core/database_falkordb_remote.py:34`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L34)
- doc: Manages a remote FalkorDB database connection as a singleton.
- signature: `class FalkorDBRemoteManager:`
- members:
  - `close_driver(self)` — [`L115`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L115) — Closes the connection.
  - `get_backend_type(self)` — [`L136`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L136) — Returns the database backend type.
  - `get_driver(self)` — [`L65`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L65) — Gets the remote FalkorDB connection, creating it if necessary.
  - `is_connected(self)` — [`L126`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L126) — Checks if the database connection is currently active.
  - `shutdown(self)` — [`L122`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L122) — Clean up on exit. No subprocess to kill for remote connections.
  - `test_connection()` — [`L163`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L163) — Tests the remote FalkorDB connection.
  - `validate_config()` — [`L141`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L141) — Validates remote FalkorDB configuration.
  - `graph_name` — [`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L60)
  - `host` — [`L55`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L55)
  - `password` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L57)
  - `port` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L56)
  - `ssl` — [`L59`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L59)
  - `username` — [`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L58)
- protocol/private: `__init__`[`L51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L51), `__new__`[`L44`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L44), `_driver`[`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L40), `_graph`[`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L41), `_initialized`[`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L61), `_instance`[`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L39), `_lock`[`L42`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb_remote.py#L42)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`error_logger`](../utils/debug_log.md#error_logger), [`FalkorDBDriverWrapper`](database_falkordb.md#FalkorDBDriverWrapper)
- used by: [`get_database_manager`](__init__.md#get_database_manager), [`doctor`](../cli/main.md#doctor)

