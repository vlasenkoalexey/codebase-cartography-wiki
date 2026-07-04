---
title: 'Module: src/codegraphcontext/core/database_falkordb.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_falkordb.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_falkordb`/
symbols:
  FalkorDBManager._drain_threads: FalkorDBManager#_drain_threads.
  FalkorDBManager.get_driver: FalkorDBManager#get_driver().
  FalkorDBManager.socket_path: FalkorDBManager#socket_path.
  FalkorDBManager._ensure_server_running: FalkorDBManager#_ensure_server_running().
  FalkorDBSessionWrapper.run: FalkorDBSessionWrapper#run().
  FalkorDBUnavailableError: FalkorDBUnavailableError#
  FalkorDBManager._process: FalkorDBManager#_process.
  FalkorDBManager.__init__: FalkorDBManager#__init__().
  FalkorDBManager.close_driver: FalkorDBManager#close_driver().
  FalkorDBManager.shutdown: FalkorDBManager#shutdown().
  FalkorDBManager.__new__: FalkorDBManager#__new__().
  FalkorDBResultWrapper.result: FalkorDBResultWrapper#result.
  FalkorDBResultWrapper.data: FalkorDBResultWrapper#data().
  FalkorDBManager: FalkorDBManager#
  FalkorDBManager._graph: FalkorDBManager#_graph.
  FalkorDBManager.graph_name: FalkorDBManager#graph_name.
  FalkorDBDriverWrapper.session: FalkorDBDriverWrapper#session().
  FalkorDBResultWrapper: FalkorDBResultWrapper#
  _probe: _probe.
  FalkorDBManager._instance: FalkorDBManager#_instance.
  FalkorDBManager._driver: FalkorDBManager#_driver.
  FalkorDBSessionWrapper._translate_constraint_command: FalkorDBSessionWrapper#_translate_constraint_command().
  FalkorDBSessionWrapper.graph: FalkorDBSessionWrapper#graph.
  FalkorDBRecord: FalkorDBRecord#
  FalkorDBDriverWrapper: FalkorDBDriverWrapper#
  FalkorDBManager.is_connected: FalkorDBManager#is_connected().
  FalkorDBResultWrapper.consume: FalkorDBResultWrapper#consume().
  FalkorDBResultWrapper.single: FalkorDBResultWrapper#single().
  FalkorDBResultWrapper.__iter__: FalkorDBResultWrapper#__iter__().
  FalkorDBManager._stdout_lines: FalkorDBManager#_stdout_lines.
  FalkorDBManager._stderr_lines: FalkorDBManager#_stderr_lines.
  FalkorDBManager._drain: FalkorDBManager#_drain().
  FalkorDBSessionWrapper: FalkorDBSessionWrapper#
  FalkorDBManager._lock: FalkorDBManager#_lock.
  FalkorDBManager._startup_failed: FalkorDBManager#_startup_failed.
  FalkorDBManager._STARTUP_TIMEOUT_SEC: FalkorDBManager#_STARTUP_TIMEOUT_SEC.
  FalkorDBManager._initialized: FalkorDBManager#_initialized.
  FalkorDBManager.db_path: FalkorDBManager#db_path.
  FalkorDBDriverWrapper.graph: FalkorDBDriverWrapper#graph.
  FalkorDBSessionWrapper._translate_schema_query: FalkorDBSessionWrapper#_translate_schema_query().
  FalkorDBResultWrapper._consumed: FalkorDBResultWrapper#_consumed.
  FalkorDBManager._atexit_registered: FalkorDBManager#_atexit_registered.
  FalkorDBManager.get_backend_type: FalkorDBManager#get_backend_type().
  FalkorDBManager.validate_config: FalkorDBManager#validate_config().
  FalkorDBManager.test_connection: FalkorDBManager#test_connection().
  FalkorDBDriverWrapper.__init__: FalkorDBDriverWrapper#__init__().
  FalkorDBDriverWrapper.close: FalkorDBDriverWrapper#close().
  FalkorDBSessionWrapper.__init__: FalkorDBSessionWrapper#__init__().
  FalkorDBSessionWrapper.__enter__: FalkorDBSessionWrapper#__enter__().
  FalkorDBSessionWrapper.__exit__: FalkorDBSessionWrapper#__exit__().
  FalkorDBRecord.data: FalkorDBRecord#data().
  FalkorDBRecord.__getitem__: FalkorDBRecord#__getitem__().
  FalkorDBResultWrapper.__init__: FalkorDBResultWrapper#__init__().
---
# Module: [`src/codegraphcontext/core/database_falkordb.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py)

## Classes
### `FalkorDBDriverWrapper`
- def: [`src/codegraphcontext/core/database_falkordb.py:468`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L468)
- members:
  - `close(self)` — [`L481`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L481) — FalkorDB Lite doesn't need explicit close for sessions.
  - `session(self, **kwargs)` — [`L477`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L477) — Returns a session-like object for FalkorDB.
  - `graph` — [`L475`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L475)
- protocol/private: `__init__`[`L474`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L474)
- uses (calls/refs, reference-scoped): [`FalkorDBSessionWrapper`](database_falkordb.md#FalkorDBSessionWrapper)
- used by: [`get_driver`](database_falkordb_remote.md#FalkorDBRemoteManager.get_driver), [`get_driver`](database_falkordb.md#FalkorDBManager.get_driver)

### `FalkorDBManager`
- def: [`src/codegraphcontext/core/database_falkordb.py:74`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L74)
- doc: Manages the FalkorDB Lite database connection as a singleton.
- signature: `class FalkorDBManager:`
- members:
  - `__init__(self, db_path: Optional[str] = None, socket_path: Optional[str] = None)` — [`L95`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L95) — Initializes the manager with default database path or explicit overrides. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `__new__(cls, *args, **kwargs)` — [`L87`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L87) — Standard singleton pattern implementation.
  - `_ensure_server_running(self)` — [`L244`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L244) — Starts the FalkorDB worker subprocess if not reachable.
  - `close_driver(self, *, teardown: bool = False)` — [`L398`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L398) — Closes the connection. Pass teardown=True to stop the worker subprocess.
  - `get_backend_type(self)` — [`L428`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L428) — Returns the database backend type.
  - `get_driver(self)` — [`L155`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L155) — Gets the FalkorDB connection, starting the subprocess if necessary. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
  - `is_connected(self)` — [`L418`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L418) — Checks if the database connection is currently active.
  - `shutdown(self)` — [`L407`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L407) — Kills the subprocess on exit.
  - `test_connection(db_path: str = None)` — [`L451`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L451) — Tests the FalkorDB Lite connection availability.
  - `validate_config(db_path: str = None)` — [`L434`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L434) — Validates FalkorDB configuration parameters.
  - `db_path` — [`L131`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L131)
  - `graph_name` — [`L148`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L148)
  - `socket_path` — [`L135`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L135)
- protocol/private: `_STARTUP_TIMEOUT_SEC`[`L85`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L85), `_atexit_registered`[`L153`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L153), `_drain`[`L315`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L315), `_drain_threads`[`L329`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L329), `_driver`[`L81`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L81), `_graph`[`L82`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L82), `_initialized`[`L130`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L130), `_instance`[`L79`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L79), `_lock`[`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L83), `_process`[`L80`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L80), `_startup_failed`[`L84`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L84), `_stderr_lines`[`L313`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L313), `_stdout_lines`[`L312`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L312)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`get_config_value`](../cli/config_manager.md#get_config_value), [`FalkorDBUnavailableError`](database_falkordb.md#FalkorDBUnavailableError), [`FalkorDBDriverWrapper`](database_falkordb.md#FalkorDBDriverWrapper)
- used by: [`get_database_manager`](__init__.md#get_database_manager)

### `FalkorDBRecord`  ·  implements/extends dict
- def: [`src/codegraphcontext/core/database_falkordb.py:603`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L603)
- doc: Dict wrapper that provides a .data() method and integer/key index access
- signature: `class FalkorDBRecord(dict):`
- members:
  - `data(self)` — [`L608`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L608)
- protocol/private: `__getitem__`[`L611`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L611)
- used by: [`data`](database_falkordb.md#FalkorDBResultWrapper.data)

### `FalkorDBResultWrapper`
- def: [`src/codegraphcontext/core/database_falkordb.py:619`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L619)
- members:
  - `__iter__(self)` — [`L671`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L671) — Iterate over results as FalkorDBRecord objects.
  - `consume(self)` — [`L628`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L628) — Mark result as consumed (for compatibility).
  - `data(self)` — [`L638`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L638) — Return all results as list of FalkorDBRecord objects.
  - `single(self)` — [`L633`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L633) — Return single result record as a FalkorDBRecord.
  - `result` — [`L625`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L625)
- protocol/private: `__init__`[`L624`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L624), `_consumed`[`L626`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L626)
- uses (calls/refs, reference-scoped): [`FalkorDBRecord`](database_falkordb.md#FalkorDBRecord)
- used by: [`run`](database_falkordb.md#FalkorDBSessionWrapper.run)

### `FalkorDBSessionWrapper`
- def: [`src/codegraphcontext/core/database_falkordb.py:486`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L486)
- members:
  - `_translate_constraint_command(self, query: str)` — [`L525`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L525) — Translate Neo4j-style CREATE CONSTRAINT queries to GRAPH.CONSTRAINT CREATE.
  - `_translate_schema_query(self, query: str)` — [`L575`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L575) — Translate Neo4j schema queries to FalkorDB/RedisGraph syntax.
  - `run(self, query, **parameters)` — [`L494`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L494) — Execute a Cypher query on FalkorDB.
  - `graph` — [`L492`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L492)
- protocol/private: `__enter__`[`L596`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L596), `__exit__`[`L599`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L599), `__init__`[`L491`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L491)
- uses (calls/refs, reference-scoped): [`error_logger`](../utils/debug_log.md#error_logger), [`FalkorDBResultWrapper`](database_falkordb.md#FalkorDBResultWrapper)
- used by: [`session`](database_falkordb.md#FalkorDBDriverWrapper.session)

### `FalkorDBUnavailableError`  ·  implements/extends RuntimeError
- def: [`src/codegraphcontext/core/database_falkordb.py:7`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L7)
- doc: Raised when FalkorDB Lite is installed but cannot actually run in this
- signature: `class FalkorDBUnavailableError(RuntimeError):`
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`get_database_manager`](__init__.md#get_database_manager), [`_drain_threads`](database_falkordb.md#FalkorDBManager._drain_threads), [`get_driver`](database_falkordb.md#FalkorDBManager.get_driver), [`_ensure_server_running`](database_falkordb.md#FalkorDBManager._ensure_server_running)

## Module values
- `_probe` — [`L62`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_falkordb.py#L62)

