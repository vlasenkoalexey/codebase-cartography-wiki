---
title: 'Module: src/codegraphcontext/core/database_embedded_kuzu.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database_embedded_kuzu.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database_embedded_kuzu`/Embedded
symbols:
  EmbeddedGraphManager._conn: GraphManager#_conn.
  EmbeddedSessionWrapper.run: SessionWrapper#run().
  EmbeddedGraphManager.get_driver: GraphManager#get_driver().
  EmbeddedGraphManager.close_driver: GraphManager#close_driver().
  EmbeddedSessionWrapper._translate_query: SessionWrapper#_translate_query().
  EmbeddedGraphManager.__init__: GraphManager#__init__().
  EmbeddedBackendSpec.display_name: BackendSpec#display_name.
  EmbeddedGraphManager: GraphManager#
  EmbeddedGraphManager._db: GraphManager#_db.
  EmbeddedGraphManager._pool: GraphManager#_pool.
  EmbeddedGraphManager._initialize_schema: GraphManager#_initialize_schema().
  EmbeddedSessionWrapper._log_query_type_skip_once: SessionWrapper#_log_query_type_skip_once().
  EmbeddedSessionWrapper._disable_query_type: SessionWrapper#_disable_query_type().
  EmbeddedGraphManager.test_connection: GraphManager#test_connection().
  EmbeddedSessionWrapper._sanitize_value: SessionWrapper#_sanitize_value().
  EmbeddedSessionWrapper: SessionWrapper#
  EmbeddedGraphManager.BACKEND_SPEC: GraphManager#BACKEND_SPEC.
  EmbeddedSessionWrapper.conn: SessionWrapper#conn.
  EmbeddedResultWrapper: ResultWrapper#
  EmbeddedGraphManager._run_schema_migrations: GraphManager#_run_schema_migrations().
  EmbeddedDriverWrapper._query_lock: DriverWrapper#_query_lock.
  EmbeddedCompatState: CompatState#
  EmbeddedGraphManager.db_path: GraphManager#db_path.
  EmbeddedGraphManager.__new__: GraphManager#__new__().
  EmbeddedRecord._data: Record#_data.
  EmbeddedSessionWrapper._logged_disabled_query_types: SessionWrapper#_logged_disabled_query_types.
  EmbeddedGraphManager._initialized: GraphManager#_initialized.
  EmbeddedSessionWrapper._is_query_type_disabled: SessionWrapper#_is_query_type_disabled().
  EmbeddedRecord: Record#
  EmbeddedSessionWrapper._state_lock: SessionWrapper#_state_lock.
  EmbeddedResultWrapper.data_raw: ResultWrapper#data_raw().
  EmbeddedBackendSpec: BackendSpec#
  EmbeddedBackendSpec.backend_id: BackendSpec#backend_id.
  EmbeddedGraphManager.is_connected: GraphManager#is_connected().
  EmbeddedGraphManager.get_backend_type: GraphManager#get_backend_type().
  EmbeddedSessionWrapper.__exit__: SessionWrapper#__exit__().
  EmbeddedRecord.__getitem__: Record#__getitem__().
  EmbeddedResultWrapper.single: ResultWrapper#single().
  EmbeddedResultWrapper.__iter__: ResultWrapper#__iter__().
  EmbeddedDriverWrapper: DriverWrapper#
  EmbeddedSessionWrapper._disabled_query_types: SessionWrapper#_disabled_query_types.
  EmbeddedBackendSpec.python_module: BackendSpec#python_module.
  EmbeddedBackendSpec.install_hint: BackendSpec#install_hint.
  EmbeddedGraphManager._instance: GraphManager#_instance.
  EmbeddedSessionWrapper._pool: SessionWrapper#_pool.
  EmbeddedSessionWrapper.uid_map: SessionWrapper#uid_map.
  EmbeddedResultWrapper.result: ResultWrapper#result.
  EmbeddedGraphManager._compat_state: GraphManager#_compat_state.
  EmbeddedSessionWrapper._display_name: SessionWrapper#_display_name.
  EmbeddedBackendSpec.path_env_var: BackendSpec#path_env_var.
  EmbeddedBackendSpec.config_key: BackendSpec#config_key.
  EmbeddedBackendSpec.default_dir: BackendSpec#default_dir.
  EmbeddedGraphManager._lock: GraphManager#_lock.
  EmbeddedRecord._keys: Record#_keys.
  EmbeddedDriverWrapper.session: DriverWrapper#session().
  EmbeddedSessionWrapper._query_lock: SessionWrapper#_query_lock.
  EmbeddedRecord.data: Record#data().
  EmbeddedRecord.keys: Record#keys().
  EmbeddedRecord.items: Record#items().
  EmbeddedRecord.values: Record#values().
  EmbeddedRecord.__len__: Record#__len__().
  EmbeddedRecord.get: Record#get().
  EmbeddedResultWrapper.consume: ResultWrapper#consume().
  EmbeddedResultWrapper.data: ResultWrapper#data().
  EmbeddedDriverWrapper._write_lock: DriverWrapper#_write_lock.
  EmbeddedSessionWrapper._write_lock: SessionWrapper#_write_lock.
  EmbeddedCompatState.lock: CompatState#lock.
  EmbeddedCompatState.disabled_query_types: CompatState#disabled_query_types.
  EmbeddedCompatState.logged_disabled_query_types: CompatState#logged_disabled_query_types.
  EmbeddedGraphManager._write_lock: GraphManager#_write_lock.
  EmbeddedDriverWrapper._pool: DriverWrapper#_pool.
  EmbeddedSessionWrapper._classify_query_type: SessionWrapper#_classify_query_type().
  EmbeddedSessionWrapper._should_fail_fast: SessionWrapper#_should_fail_fast().
  EmbeddedSessionWrapper._filter_set_clause: SessionWrapper#_filter_set_clause().
  EmbeddedSessionWrapper.poly_replacer: SessionWrapper#poly_replacer().
  EmbeddedSessionWrapper.single_label_replacer: SessionWrapper#single_label_replacer().
  EmbeddedSessionWrapper.not_label_replacer: SessionWrapper#not_label_replacer().
  EmbeddedSessionWrapper._rewrite_kuzu_compat_patterns: SessionWrapper#_rewrite_kuzu_compat_patterns().
  EmbeddedResultWrapper._consumed: ResultWrapper#_consumed.
  EmbeddedCompatState.__init__: CompatState#__init__().
  EmbeddedGraphManager._query_lock: GraphManager#_query_lock.
  EmbeddedGraphManager.validate_config: GraphManager#validate_config().
  EmbeddedDriverWrapper.__init__: DriverWrapper#__init__().
  EmbeddedDriverWrapper.db: DriverWrapper#db.
  EmbeddedDriverWrapper._compat_state: DriverWrapper#_compat_state.
  EmbeddedDriverWrapper._display_name: DriverWrapper#_display_name.
  EmbeddedDriverWrapper._backend_id: DriverWrapper#_backend_id.
  EmbeddedDriverWrapper.close: DriverWrapper#close().
  EmbeddedDriverWrapper.get_backend_type: DriverWrapper#get_backend_type().
  EmbeddedSessionWrapper.__init__: SessionWrapper#__init__().
  EmbeddedSessionWrapper._compat_state: SessionWrapper#_compat_state.
  EmbeddedSessionWrapper.__enter__: SessionWrapper#__enter__().
  EmbeddedRecord.__init__: Record#__init__().
  EmbeddedResultWrapper.__init__: ResultWrapper#__init__().
---
# Module: [`src/codegraphcontext/core/database_embedded_kuzu.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py)

## Classes
### `EmbeddedBackendSpec`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L27) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- doc: Configuration for a Kùzu-dialect embedded graph backend.
- signature: `class EmbeddedBackendSpec:`
- members:
  - `backend_id` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L30) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `config_key` — [`L34`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L34)
  - `default_dir` — [`L35`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L35)
  - `display_name` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L32) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `install_hint` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L36) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `path_env_var` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L33)
  - `python_module` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L31) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- used by: [`_conn`](database_embedded_kuzu.md#EmbeddedGraphManager._conn), [`get_driver`](database_embedded_kuzu.md#EmbeddedGraphManager.get_driver), [`KUZU_SPEC`](database_kuzu.md#KUZU_SPEC), [`LADYBUG_SPEC`](database_ladybug.md#LADYBUG_SPEC), [`close_driver`](database_embedded_kuzu.md#EmbeddedGraphManager.close_driver), [`__init__`](database_embedded_kuzu.md#EmbeddedGraphManager.__init__), [`test_connection`](database_embedded_kuzu.md#EmbeddedGraphManager.test_connection), [`BACKEND_SPEC`](database_embedded_kuzu.md#EmbeddedGraphManager.BACKEND_SPEC), [`_initialized`](database_embedded_kuzu.md#EmbeddedGraphManager._initialized), [`get_backend_type`](database_embedded_kuzu.md#EmbeddedGraphManager.get_backend_type)

### `EmbeddedCompatState`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L39) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- doc: Shared fail-fast state for unsupported query types (fulltext/module_deps).
- signature: `class EmbeddedCompatState:`
- members:
  - `disabled_query_types` — [`L47`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L47) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `lock` — [`L46`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L46) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `logged_disabled_query_types` — [`L48`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L48) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- protocol/private: `__init__`[`L45`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L45)
- used by: [`_logged_disabled_query_types`](database_embedded_kuzu.md#EmbeddedSessionWrapper._logged_disabled_query_types), [`_state_lock`](database_embedded_kuzu.md#EmbeddedSessionWrapper._state_lock), [`_disabled_query_types`](database_embedded_kuzu.md#EmbeddedSessionWrapper._disabled_query_types), [`_compat_state`](database_embedded_kuzu.md#EmbeddedGraphManager._compat_state), [`_display_name`](database_embedded_kuzu.md#EmbeddedSessionWrapper._display_name), [`_KuzuCompatState`](database_kuzu.md#_KuzuCompatState), [`_LadybugCompatState`](database_ladybug.md#_LadybugCompatState), [`_compat_state`](database_kuzu.md#KuzuDBManager._compat_state), [`_compat_state`](database_ladybug.md#LadybugDBManager._compat_state)

### `EmbeddedDriverWrapper`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:466`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L466) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- members:
  - `close(self)` — [`L504`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L504)
  - `get_backend_type(self)` — [`L507`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L507)
  - `session(self, **kwargs)` — [`L488`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L488) — Accepts and ignores Neo4j-specific kwargs (e.g. default_access_mode).
  - `db` — [`L476`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L476)
- protocol/private: `__init__`[`L467`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L467), `_backend_id`[`L479`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L479), `_compat_state`[`L477`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L477), `_display_name`[`L478`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L478), `_pool`[`L481`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L481), `_query_lock`[`L483`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L483), `_write_lock`[`L482`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L482)
- uses (calls/refs, reference-scoped): [`EmbeddedSessionWrapper`](database_embedded_kuzu.md#EmbeddedSessionWrapper)
- used by: [`_conn`](database_embedded_kuzu.md#EmbeddedGraphManager._conn), [`KuzuDriverWrapper`](database_kuzu.md#KuzuDriverWrapper), [`LadybugDriverWrapper`](database_ladybug.md#LadybugDriverWrapper)

### `EmbeddedGraphManager`  ·  implements/extends GraphQueryInterface
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L51)
- doc: Manages an embedded Kùzu-dialect database connection as a per-subclass singleton.
- signature: `class EmbeddedGraphManager(GraphQueryInterface):`
- members:
  - `__init__(self, db_path: Optional[str] = None)` — [`L74`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L74) — Initializes the manager with default database path or explicit overrides. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `__new__(cls, *args, **kwargs)` — [`L66`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L66) — Standard singleton pattern implementation.
  - `_initialize_schema(self)` — [`L159`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L159) — Creates Node and Rel tables if they don't exist. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `_run_schema_migrations(self)` — [`L291`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L291) — Add columns introduced after older local Kùzu databases were created. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `close_driver(self)` — [`L398`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L398) — Closes the connection pool and releases database resources. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `get_backend_type(self)` — [`L444`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L444) — Returns the database backend type.
  - `get_driver(self)` — [`L102`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L102) — Gets the embedded driver. Initialises the database and connection pool. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `is_connected(self)` — [`L429`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L429) — Checks if the database connection is currently active.
  - `test_connection(cls, db_path: str = None)` — [`L457`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L457)
  - `validate_config(cls, db_path: str = None)` — [`L449`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L449)
  - `BACKEND_SPEC` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L56) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `db_path` — [`L98`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L98) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- protocol/private: `_compat_state`[`L64`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L64), `_conn`[`L126`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L126), `_db`[`L59`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L59), `_initialized`[`L96`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L96), `_instance`[`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L58), `_lock`[`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L61), `_pool`[`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L60), `_query_lock`[`L63`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L63), `_write_lock`[`L62`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L62)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`warning_logger`](../utils/debug_log.md#warning_logger), [`debug_log`](../utils/debug_log.md#debug_log), [`error_logger`](../utils/debug_log.md#error_logger), [`get_config_value`](../cli/config_manager.md#get_config_value), [`KuzuDBManager`](database_kuzu.md#KuzuDBManager), [`display_name`](database_embedded_kuzu.md#EmbeddedBackendSpec.display_name), [`LadybugDBManager`](database_ladybug.md#LadybugDBManager), [`EmbeddedCompatState`](database_embedded_kuzu.md#EmbeddedCompatState), [`EmbeddedBackendSpec`](database_embedded_kuzu.md#EmbeddedBackendSpec), [`EmbeddedDriverWrapper`](database_embedded_kuzu.md#EmbeddedDriverWrapper), [`backend_id`](database_embedded_kuzu.md#EmbeddedBackendSpec.backend_id), [`GraphQueryInterface`](graph_query.md#GraphQueryInterface), [`install_hint`](database_embedded_kuzu.md#EmbeddedBackendSpec.install_hint), [`python_module`](database_embedded_kuzu.md#EmbeddedBackendSpec.python_module), [`config_key`](database_embedded_kuzu.md#EmbeddedBackendSpec.config_key), [`default_dir`](database_embedded_kuzu.md#EmbeddedBackendSpec.default_dir), [`path_env_var`](database_embedded_kuzu.md#EmbeddedBackendSpec.path_env_var), [`name`](graph_query.md#GraphQueryInterface.name)
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`KuzuDBManager`](database_kuzu.md#KuzuDBManager), [`LadybugDBManager`](database_ladybug.md#LadybugDBManager), [`GraphQueryInterface`](graph_query.md#GraphQueryInterface), [`close_driver`](graph_query.md#GraphQueryInterface.close_driver), [`get_backend_type`](graph_query.md#GraphQueryInterface.get_backend_type), [`get_driver`](graph_query.md#GraphQueryInterface.get_driver), [`is_connected`](graph_query.md#GraphQueryInterface.is_connected), [`test_connection`](graph_query.md#GraphQueryInterface.test_connection), [`validate_config`](graph_query.md#GraphQueryInterface.validate_config)

### `EmbeddedRecord`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:1177`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1177)
- signature: `class EmbeddedRecord:`
- members:
  - `data(self)` — [`L1182`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1182)
  - `get(self, key, default=None)` — [`L1208`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1208)
  - `items(self)` — [`L1188`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1188)
  - `keys(self)` — [`L1185`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1185)
  - `values(self)` — [`L1191`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1191)
- protocol/private: `__getitem__`[`L1197`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1197), `__init__`[`L1178`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1178), `__len__`[`L1194`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1194), `_data`[`L1179`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1179), `_keys`[`L1180`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1180)
- used by: [`__iter__`](database_embedded_kuzu.md#EmbeddedResultWrapper.__iter__), [`single`](database_embedded_kuzu.md#EmbeddedResultWrapper.single), [`KuzuRecord`](database_kuzu.md#KuzuRecord), [`LadybugRecord`](database_ladybug.md#LadybugRecord)

### `EmbeddedResultWrapper`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:1211`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1211) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- members:
  - `consume(self)` — [`L1215`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1215)
  - `data(self)` — [`L1260`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1260)
  - `data_raw(self)` — [`L1221`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1221)
  - `single(self)` — [`L1218`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1218)
  - `result` — [`L1213`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1213)
- protocol/private: `__init__`[`L1212`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1212), `__iter__`[`L1264`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1264), `_consumed`[`L1214`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1214)
- uses (calls/refs, reference-scoped): [`EmbeddedRecord`](database_embedded_kuzu.md#EmbeddedRecord)
- used by: [`run`](database_embedded_kuzu.md#EmbeddedSessionWrapper.run), [`KuzuResultWrapper`](database_kuzu.md#KuzuResultWrapper), [`LadybugResultWrapper`](database_ladybug.md#LadybugResultWrapper)

### `EmbeddedSessionWrapper`
- def: [`src/codegraphcontext/core/database_embedded_kuzu.py:511`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L511) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- members:
  - `__enter__(self)` — [`L554`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L554) — Enter context manager - return self for 'with' statement.
  - `__exit__(self, exc_type, exc_val, exc_tb)` — [`L558`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L558) — Exit context manager - Return connection to the pool.
  - `_rewrite_kuzu_compat_patterns(self, query: str, parameters: Dict[str, Any])` — [`L1072`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1072) — Rewrite known Neo4j-only query patterns to Kuzu-compatible variants. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `_sanitize_value(v)` — [`L566`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L566) — Recursively coerce Python types that KuzuDB cannot bind (tuples, sets, etc.). — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `_translate_query(self, query: str, parameters: Dict[str, Any])` — [`L763`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L763) — Translates Neo4j Cypher to Kuzu Cypher. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `not_label_replacer(match)` — [`L1046`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1046) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `poly_replacer(match)` — [`L1022`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1022) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `run(self, query, **parameters)` — [`L685`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L685) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `single_label_replacer(match)` — [`L1037`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L1037) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `conn` — [`L528`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L528) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `uid_map` — [`L534`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L534) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- protocol/private: `__init__`[`L512`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L512), `_classify_query_type`[`L623`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L623), `_compat_state`[`L520`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L520), `_disable_query_type`[`L672`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L672), `_disabled_query_types`[`L521`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L521), `_display_name`[`L515`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L515), `_filter_set_clause`[`L945`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L945), `_is_query_type_disabled`[`L641`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L641), `_log_query_type_skip_once`[`L647`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L647), `_logged_disabled_query_types`[`L522`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L522), `_pool`[`L527`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L527), `_query_lock`[`L514`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L514), `_should_fail_fast`[`L659`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L659), `_state_lock`[`L523`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L523), `_write_lock`[`L513`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database_embedded_kuzu.py#L513)
- uses (calls/refs, reference-scoped): [`warning_logger`](../utils/debug_log.md#warning_logger), [`debug_log`](../utils/debug_log.md#debug_log), [`error_logger`](../utils/debug_log.md#error_logger), [`EmbeddedResultWrapper`](database_embedded_kuzu.md#EmbeddedResultWrapper), [`EmbeddedCompatState`](database_embedded_kuzu.md#EmbeddedCompatState), [`disabled_query_types`](database_embedded_kuzu.md#EmbeddedCompatState.disabled_query_types), [`lock`](database_embedded_kuzu.md#EmbeddedCompatState.lock), [`logged_disabled_query_types`](database_embedded_kuzu.md#EmbeddedCompatState.logged_disabled_query_types)
- used by: [`KuzuSessionWrapper`](database_kuzu.md#KuzuSessionWrapper), [`LadybugSessionWrapper`](database_ladybug.md#LadybugSessionWrapper), [`session`](database_embedded_kuzu.md#EmbeddedDriverWrapper.session)

