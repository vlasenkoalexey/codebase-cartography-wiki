---
title: 'Module: src/codegraphcontext/core/database_nornic.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_nornic.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_nornic`/NornicD
symbols:
  NornicDBManager.get_driver: BManager#get_driver().
  NornicDBManager._driver: BManager#_driver.
  NornicDBManager: BManager#
  NornicDBManager.__new__: BManager#__new__().
  NornicDBManager.close_driver: BManager#close_driver().
  NornicDriverWrapper.session: riverWrapper#session().
  NornicDBManager.nornic_uri: BManager#nornic_uri.
  NornicDBManager.is_connected: BManager#is_connected().
  NornicDBManager._instance: BManager#_instance.
  NornicDBManager.nornic_username: BManager#nornic_username.
  NornicDBManager.nornic_password: BManager#nornic_password.
  NornicDBManager._lock: BManager#_lock.
  NornicDBManager.nornic_database: BManager#nornic_database.
  NornicDriverWrapper.close: riverWrapper#close().
  NornicDriverWrapper._driver: riverWrapper#_driver.
  NornicDriverWrapper._database: riverWrapper#_database.
  NornicDriverWrapper: riverWrapper#
  NornicDBManager.validate_config: BManager#validate_config().
  NornicDBManager.test_connection: BManager#test_connection().
  NornicDriverWrapper.__init__: riverWrapper#__init__().
  NornicDBManager.__init__: BManager#__init__().
  NornicDBManager._initialized: BManager#_initialized.
  NornicDBManager.get_backend_type: BManager#get_backend_type().
---
# Module: [`src/codegraphcontext/core/database_nornic.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py)

## Classes
### `NornicDBManager`
- def: [`src/codegraphcontext/core/database_nornic.py:32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L32)
- doc: Manages the Nornic database driver as a singleton to ensure only one
- signature: `class NornicDBManager:`
- members:
  - `__init__(self)` — [`L49`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L49) — Initializes the manager by reading credentials from environment variables.
  - `__new__(cls)` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L41) — Standard singleton pattern implementation.
  - `close_driver(self)` — [`L118`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L118) — Closes the Nornic driver connection if it exists.
  - `get_backend_type(self)` — [`L141`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L141) — Returns the database backend type.
  - `get_driver(self)` — [`L63`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L63) — Gets the Nornic driver instance, creating it if it doesn't exist.
  - `is_connected(self)` — [`L127`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L127) — Checks if the database connection is currently active.
  - `test_connection(uri: str, username: str, password: str, database: str = None)` — [`L168`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L168) — Tests the Nornic database connection.
  - `validate_config(uri: str, username: str, password: str)` — [`L146`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L146) — Validates Nornic configuration parameters.
  - `nornic_database` — [`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L60)
  - `nornic_password` — [`L59`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L59)
  - `nornic_uri` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L57)
  - `nornic_username` — [`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L58)
- protocol/private: `_driver`[`L38`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L38), `_initialized`[`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L61), `_instance`[`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L37), `_lock`[`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L39)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`error_logger`](../utils/debug_log.md#error_logger), [`NornicDriverWrapper`](database_nornic.md#NornicDriverWrapper)
- used by: [`get_database_manager`](__init__.md#get_database_manager)

### `NornicDriverWrapper`
- def: [`src/codegraphcontext/core/database_nornic.py:14`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L14)
- doc: A simple wrapper around the Nornic (Neo4j) Driver to inject a database name into session() calls.
- signature: `class NornicDriverWrapper:`
- members:
  - `close(self)` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L28) — Proxy method to close the underlying driver.
  - `session(self, **kwargs)` — [`L22`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L22) — Proxy method to get a session from the underlying driver.
- protocol/private: `__init__`[`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L18), `_database`[`L20`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L20), `_driver`[`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_nornic.py#L19)
- used by: [`get_driver`](database_nornic.md#NornicDBManager.get_driver)

