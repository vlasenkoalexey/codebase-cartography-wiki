---
title: 'Module: tests/unit/core/test_database.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_database.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_database`/Test
symbols:
  TestDatabaseManager: DatabaseManager#
  TestDatabaseManager.mock_driver: DatabaseManager#mock_driver().
  TestDatabaseManager.test_initialization: DatabaseManager#test_initialization().
  TestDatabaseManager.test_verify_connection_success: DatabaseManager#test_verify_connection_success().
  TestDatabaseManager.test_verify_connection_failure: DatabaseManager#test_verify_connection_failure().
  TestDatabaseManager.test_initialization_with_database: DatabaseManager#test_initialization_with_database().
  TestDatabaseManager.test_initialization_without_database: DatabaseManager#test_initialization_without_database().
  TestDatabaseManager.test_get_driver_returns_wrapper_with_database: DatabaseManager#test_get_driver_returns_wrapper_with_database().
  TestDatabaseManager.test_get_driver_returns_wrapper_without_database: DatabaseManager#test_get_driver_returns_wrapper_without_database().
  TestDatabaseManager.test_is_connected_passes_database_to_session: DatabaseManager#test_is_connected_passes_database_to_session().
  TestDatabaseManager.test_is_connected_no_database_in_session: DatabaseManager#test_is_connected_no_database_in_session().
  TestNeo4jDriverWrapper: Neo4jDriverWrapper#
  TestNeo4jDriverWrapper.test_session_injects_database_when_set: Neo4jDriverWrapper#test_session_injects_database_when_set().
  TestNeo4jDriverWrapper.test_session_no_database_when_none: Neo4jDriverWrapper#test_session_no_database_when_none().
  TestNeo4jDriverWrapper.test_session_does_not_override_existing_database: Neo4jDriverWrapper#test_session_does_not_override_existing_database().
  TestNeo4jDriverWrapper.test_close_delegates_to_driver: Neo4jDriverWrapper#test_close_delegates_to_driver().
  TestTestConnection: TestConnection#
  TestTestConnection.test_test_connection_with_database: TestConnection#test_test_connection_with_database().
  TestTestConnection.test_test_connection_without_database: TestConnection#test_test_connection_without_database().
  TestNeo4jPreflight: Neo4jPreflight#
  TestNeo4jPreflight.test_check_port_reachable_success: Neo4jPreflight#test_check_port_reachable_success().
  TestNeo4jPreflight.test_check_port_reachable_failure: Neo4jPreflight#test_check_port_reachable_failure().
  TestNeo4jPreflight.test_missing_credentials_message_contains_config_commands: Neo4jPreflight#test_missing_credentials_message_contains_config_commands().
  TestNeo4jPreflight.test_get_driver_fails_fast_when_port_unreachable: Neo4jPreflight#test_get_driver_fails_fast_when_port_unreachable().
---
# Module: [`tests/unit/core/test_database.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py)

## Classes
### `TestDatabaseManager`
- def: [`tests/unit/core/test_database.py:7`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L7)
- doc: Unit tests for the DatabaseManager class.
- signature: `class TestDatabaseManager:`
- members:
  - `mock_driver(self)` — [`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L14)
  - `test_get_driver_returns_wrapper_with_database(self, mock_driver)` — [`L82`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L82) — Test get_driver() returns a Neo4jDriverWrapper with the configured database.
  - `test_get_driver_returns_wrapper_without_database(self, mock_driver)` — [`L103`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L103) — Test get_driver() returns a Neo4jDriverWrapper with None database when not configured.
  - `test_initialization(self, mock_driver)` — [`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L20) — Test that DatabaseManager initializes with correct config from env.
  - `test_initialization_with_database(self, mock_driver)` — [`L60`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L60) — Test that DatabaseManager reads NEO4J_DATABASE from env.
  - `test_initialization_without_database(self, mock_driver)` — [`L73`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L73) — Test that neo4j_database is None when NEO4J_DATABASE is not set.
  - `test_is_connected_no_database_in_session(self, mock_driver)` — [`L138`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L138) — Test is_connected() does NOT include database in session kwargs when neo4j_database is None.
  - `test_is_connected_passes_database_to_session(self, mock_driver)` — [`L119`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L119) — Test is_connected() includes database in session kwargs when neo4j_database is set.
  - `test_verify_connection_failure(self, mock_driver)` — [`L50`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L50) — Test verify_connectivity returns False on exception.
  - `test_verify_connection_success(self, mock_driver)` — [`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L31) — Test verify_connectivity returns True on success.

### `TestNeo4jDriverWrapper`
- def: [`tests/unit/core/test_database.py:154`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L154)
- doc: Unit tests for the Neo4jDriverWrapper class.
- signature: `class TestNeo4jDriverWrapper:`
- members:
  - `test_close_delegates_to_driver(self)` — [`L181`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L181) — Test close() calls close() on the underlying driver.
  - `test_session_does_not_override_existing_database(self)` — [`L173`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L173) — Test session() respects caller-provided database kwarg.
  - `test_session_injects_database_when_set(self)` — [`L157`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L157) — Test session() adds database kwarg when wrapper has a database configured.
  - `test_session_no_database_when_none(self)` — [`L165`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L165) — Test session() does NOT add database kwarg when database is None.

### `TestNeo4jPreflight`
- def: [`tests/unit/core/test_database.py:240`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L240)
- signature: `class TestNeo4jPreflight:`
- members:
  - `test_check_port_reachable_failure(self, _mock_create_connection)` — [`L252`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L252)
  - `test_check_port_reachable_success(self, mock_create_connection)` — [`L242`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L242)
  - `test_get_driver_fails_fast_when_port_unreachable(self, _mock_reachable)` — [`L265`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L265)
  - `test_missing_credentials_message_contains_config_commands(self)` — [`L258`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L258)

### `TestTestConnection`
- def: [`tests/unit/core/test_database.py:190`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L190)
- doc: Unit tests for DatabaseManager.test_connection() with database parameter.
- signature: `class TestTestConnection:`
- members:
  - `test_test_connection_with_database(self, mock_socket_cls, mock_gdb)` — [`L195`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L195) — Test test_connection() passes database to session when provided.
  - `test_test_connection_without_database(self, mock_socket_cls, mock_gdb)` — [`L219`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database.py#L219) — Test test_connection() does NOT pass database to session when None.

