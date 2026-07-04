---
title: 'Module: src/codegraphcontext/core/database.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/database.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.database`/
symbols:
  DatabaseManager.get_driver: DatabaseManager#get_driver().
  DatabaseManager: DatabaseManager#
  DatabaseManager._driver: DatabaseManager#_driver.
  DatabaseManager.test_connection: DatabaseManager#test_connection().
  DatabaseManager.check_port_reachable: DatabaseManager#check_port_reachable().
  Neo4jConnectionError.__str__: Neo4jConnectionError#__str__().
  DatabaseManager.__new__: DatabaseManager#__new__().
  DatabaseManager.close_driver: DatabaseManager#close_driver().
  DatabaseManager.neo4j_uri: DatabaseManager#neo4j_uri.
  Neo4jDriverWrapper.session: Neo4jDriverWrapper#session().
  DatabaseManager.is_connected: DatabaseManager#is_connected().
  Neo4jConnectionError: Neo4jConnectionError#
  DatabaseManager._instance: DatabaseManager#_instance.
  DatabaseManager.neo4j_username: DatabaseManager#neo4j_username.
  DatabaseManager.neo4j_password: DatabaseManager#neo4j_password.
  DatabaseManager.validate_config: DatabaseManager#validate_config().
  DatabaseManager._lock: DatabaseManager#_lock.
  DatabaseManager.neo4j_database: DatabaseManager#neo4j_database.
  DatabaseManager.extract_host_port: DatabaseManager#extract_host_port().
  Neo4jDriverWrapper.close: Neo4jDriverWrapper#close().
  Neo4jConnectionError.suggestions: Neo4jConnectionError#suggestions.
  Neo4jDriverWrapper._driver: Neo4jDriverWrapper#_driver.
  Neo4jDriverWrapper._database: Neo4jDriverWrapper#_database.
  DatabaseManager.get_db_selection_source: DatabaseManager#get_db_selection_source().
  DatabaseManager.get_missing_credentials: DatabaseManager#get_missing_credentials().
  DatabaseManager.get_neo4j_suggestions: DatabaseManager#get_neo4j_suggestions().
  Neo4jConnectionError.reason: Neo4jConnectionError#reason.
  Neo4jConnectionError.source: Neo4jConnectionError#source.
  Neo4jDriverWrapper: Neo4jDriverWrapper#
  DatabaseManager.build_missing_credentials_message: DatabaseManager#build_missing_credentials_message().
  Neo4jConnectionError.__init__: Neo4jConnectionError#__init__().
  Neo4jDriverWrapper.__init__: Neo4jDriverWrapper#__init__().
  DatabaseManager.__init__: DatabaseManager#__init__().
  DatabaseManager._initialized: DatabaseManager#_initialized.
  DatabaseManager.get_backend_type: DatabaseManager#get_backend_type().
---
# Module: [`src/codegraphcontext/core/database.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py)

## Classes
### `DatabaseManager`
- def: [`src/codegraphcontext/core/database.py:50`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L50) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- doc: Manages the Neo4j database driver as a singleton to ensure only one
- signature: `class DatabaseManager:`
- members:
  - `__init__(self)` — [`L71`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L71) — Initializes the manager by reading credentials from environment variables.
  - `__new__(cls)` — [`L62`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L62) — Standard singleton pattern implementation.
  - `build_missing_credentials_message(missing_keys: list)` — [`L205`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L205)
  - `check_port_reachable(uri: str, timeout_seconds: float = 2)` — [`L232`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L232) — Lightweight TCP preflight check for Neo4j endpoint reachability. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `close_driver(self)` — [`L161`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L161) — Closes the Neo4j driver connection if it exists.
  - `extract_host_port(uri: str)` — [`L224`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L224) — Extract host and port from Neo4j URI, defaulting port to 7687.
  - `get_backend_type(self)` — [`L184`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L184) — Returns the database backend type.
  - `get_db_selection_source()` — [`L189`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L189) — Best-effort source for why neo4j is selected (environment, .env, mcp.json, etc.).
  - `get_driver(self)` — [`L85`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L85) — Gets the Neo4j driver instance, creating it if it doesn't exist. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `get_missing_credentials(uri: Optional[str], username: Optional[str], password: Optional[str])` — [`L194`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L194)
  - `get_neo4j_suggestions()` — [`L216`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L216)
  - `is_connected(self)` — [`L170`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L170) — Checks if the database connection is currently active.
  - `test_connection(uri: str, username: str, password: str, database: str = None)` — [`L288`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L288) — Tests the Neo4j database connection.
  - `validate_config(uri: str, username: str, password: str)` — [`L253`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L253) — Validates Neo4j configuration parameters.
  - `neo4j_database` — [`L82`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L82)
  - `neo4j_password` — [`L81`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L81)
  - `neo4j_uri` — [`L79`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L79) — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `neo4j_username` — [`L80`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L80)
- protocol/private: `_driver`[`L59`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L59), `_initialized`[`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L83), `_instance`[`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L58), `_lock`[`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L60)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`error_logger`](../utils/debug_log.md#error_logger), [`Neo4jConnectionError`](database.md#Neo4jConnectionError), [`Neo4jDriverWrapper`](database.md#Neo4jDriverWrapper)
- used by: [`get_database_manager`](__init__.md#get_database_manager), [`doctor`](../cli/main.md#doctor), [`driver`](../tools/code_finder.md#CodeFinder.driver), [`setup_docker`](../cli/setup_wizard.md#setup_docker), [`get_graph`](../viz/server.md#get_graph), [`setup_existing_db`](../cli/setup_wizard.md#setup_existing_db), [`setup_hosted_db`](../cli/setup_wizard.md#setup_hosted_db), [`advanced_language_query`](../tools/advanced_language_query_tool.md#Advanced_language_query.advanced_language_query), [`driver`](../tools/graph_builder.md#GraphBuilder.driver), [`get_repository_stats`](../tools/handlers/management_handlers.md#get_repository_stats), [`set_db_manager`](../viz/server.md#set_db_manager), [`db_manager`](../viz/server.md#db_manager.db_manager), [`__init__`](../tools/graph_builder.md#GraphBuilder.__init__), [`__init__`](../tools/system.md#SystemTools.__init__), [`execute_cypher_query_tool`](../tools/system.md#SystemTools.execute_cypher_query_tool), [`find_dead_code_tool`](../tools/system.md#SystemTools.find_dead_code_tool), [`__init__`](../tools/advanced_language_query_tool.md#Advanced_language_query.__init__), [`__init__`](../tools/code_finder.md#CodeFinder.__init__)

### `Neo4jConnectionError`  ·  implements/extends Exception
- def: [`src/codegraphcontext/core/database.py:16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L16)
- doc: Raised when Neo4j cannot be reached or authenticated with actionable guidance.
- signature: `class Neo4jConnectionError(Exception):`
- members:
  - `reason` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L21)
  - `source` — [`L22`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L22)
  - `suggestions` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L23)
- protocol/private: `__init__`[`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L19), `__str__`[`L25`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L25)
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`get_driver`](database.md#DatabaseManager.get_driver)

### `Neo4jDriverWrapper`
- def: [`src/codegraphcontext/core/database.py:32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L32)
- doc: A simple wrapper around the Neo4j Driver to inject a database name into session() calls.
- signature: `class Neo4jDriverWrapper:`
- members:
  - `close(self)` — [`L46`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L46) — Proxy method to close the underlying driver.
  - `session(self, **kwargs)` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L40) — Proxy method to get a session from the underlying driver.
- protocol/private: `__init__`[`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L36), `_database`[`L38`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L38), `_driver`[`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/database.py#L37)
- used by: [`get_driver`](database.md#DatabaseManager.get_driver)

