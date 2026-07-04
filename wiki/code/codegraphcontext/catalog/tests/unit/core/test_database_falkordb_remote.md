---
title: 'Module: tests/unit/core/test_database_falkordb_remote.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_database_falkordb_remote.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_database_falkordb_remote`/TestFa
symbols:
  TestFalkorDBRemoteManager._reset_singleton: lkorDBRemoteManager#_reset_singleton().
  TestFalkorDBRemoteManager.setup_method: lkorDBRemoteManager#setup_method().
  TestFalkorDBRemoteManager.teardown_method: lkorDBRemoteManager#teardown_method().
  TestFalkorDBRemoteManager.test_initialization_defaults: lkorDBRemoteManager#test_initialization_defaults().
  TestFalkorDBRemoteManager.test_initialization_custom_values: lkorDBRemoteManager#test_initialization_custom_values().
  TestFalkorDBRemoteManager.test_ssl_variations: lkorDBRemoteManager#test_ssl_variations().
  TestFalkorDBRemoteManager.test_get_driver_connects_with_correct_params: lkorDBRemoteManager#test_get_driver_connects_with_correct_params().
  TestFalkorDBRemoteManager.test_get_driver_minimal_params: lkorDBRemoteManager#test_get_driver_minimal_params().
  TestFalkorDBRemoteManager.test_get_driver_singleton_reuses_connection: lkorDBRemoteManager#test_get_driver_singleton_reuses_connection().
  TestFalkorDBRemoteManager.test_is_connected_true: lkorDBRemoteManager#test_is_connected_true().
  TestFalkorDBRemoteManager.test_is_connected_false_no_graph: lkorDBRemoteManager#test_is_connected_false_no_graph().
  TestFalkorDBRemoteManager.test_is_connected_false_on_exception: lkorDBRemoteManager#test_is_connected_false_on_exception().
  TestFalkorDBRemoteManager.test_get_backend_type: lkorDBRemoteManager#test_get_backend_type().
  TestFalkorDBRemoteManager.test_close_driver: lkorDBRemoteManager#test_close_driver().
  TestFalkorDBRemoteManager.test_get_driver_import_error: lkorDBRemoteManager#test_get_driver_import_error().
  TestFalkorDBRemoteManager: lkorDBRemoteManager#
  TestFalkorDBRemoteManager.test_validate_config_no_host: lkorDBRemoteManager#test_validate_config_no_host().
  TestFalkorDBRemoteManager.test_validate_config_valid: lkorDBRemoteManager#test_validate_config_valid().
  TestFalkorDBRemoteManager.test_validate_config_bad_port: lkorDBRemoteManager#test_validate_config_bad_port().
  TestFactoryFalkorDBRemote: ctoryFalkorDBRemote#
  TestFactoryFalkorDBRemote.setup_method: ctoryFalkorDBRemote#setup_method().
  TestFactoryFalkorDBRemote.teardown_method: ctoryFalkorDBRemote#teardown_method().
  TestFactoryFalkorDBRemote.test_explicit_falkordb_remote: ctoryFalkorDBRemote#test_explicit_falkordb_remote().
  TestFactoryFalkorDBRemote.test_explicit_falkordb_remote_missing_host: ctoryFalkorDBRemote#test_explicit_falkordb_remote_missing_host().
  TestFactoryFalkorDBRemote.test_auto_detect_remote_via_host: ctoryFalkorDBRemote#test_auto_detect_remote_via_host().
  TestFactoryFalkorDBRemote.test_unknown_db_type_includes_falkordb_remote: ctoryFalkorDBRemote#test_unknown_db_type_includes_falkordb_remote().
  TestFactoryFalkorDBRemote.test_runtime_db_type_overrides_default_database: ctoryFalkorDBRemote#test_runtime_db_type_overrides_default_database().
---
# Module: [`tests/unit/core/test_database_falkordb_remote.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py)

## Classes
### `TestFactoryFalkorDBRemote`
- def: [`tests/unit/core/test_database_falkordb_remote.py:314`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L314)
- doc: Test that get_database_manager() correctly routes to FalkorDBRemoteManager.
- signature: `class TestFactoryFalkorDBRemote:`
- members:
  - `setup_method(self)` — [`L317`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L317)
  - `teardown_method(self)` — [`L323`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L323)
  - `test_auto_detect_remote_via_host(self)` — [`L359`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L359) — Test that setting FALKORDB_HOST (without DEFAULT_DATABASE) auto-detects remote.
  - `test_explicit_falkordb_remote(self)` — [`L329`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L329) — Test DEFAULT_DATABASE=falkordb-remote returns FalkorDBRemoteManager.
  - `test_explicit_falkordb_remote_missing_host(self)` — [`L347`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L347) — Test DEFAULT_DATABASE=falkordb-remote without FALKORDB_HOST raises.
  - `test_runtime_db_type_overrides_default_database(self)` — [`L385`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L385) — CGC_RUNTIME_DB_TYPE wins over DEFAULT_DATABASE.
  - `test_unknown_db_type_includes_falkordb_remote(self)` — [`L374`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L374) — Test that unknown DEFAULT_DATABASE error message mentions falkordb-remote.

### `TestFalkorDBRemoteManager`
- def: [`tests/unit/core/test_database_falkordb_remote.py:9`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L9)
- doc: Unit tests for the FalkorDBRemoteManager class.
- signature: `class TestFalkorDBRemoteManager:`
- members:
  - `_reset_singleton(self)` — [`L15`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L15) — Reset the singleton so each test starts fresh.
  - `setup_method(self)` — [`L25`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L25)
  - `teardown_method(self)` — [`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L28)
  - `test_close_driver(self)` — [`L248`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L248) — Test close_driver clears internal state.
  - `test_get_backend_type(self)` — [`L236`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L236) — Test backend type string.
  - `test_get_driver_connects_with_correct_params(self)` — [`L97`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L97) — Test that get_driver() calls FalkorDB with the right kwargs.
  - `test_get_driver_import_error(self)` — [`L297`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L297) — Test that missing falkordb package raises ValueError.
  - `test_get_driver_minimal_params(self)` — [`L140`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L140) — Test get_driver with only host set (no password/username/ssl).
  - `test_get_driver_singleton_reuses_connection(self)` — [`L167`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L167) — Test that calling get_driver() twice doesn't create a second connection.
  - `test_initialization_custom_values(self)` — [`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L52) — Test that all env vars are correctly read.
  - `test_initialization_defaults(self)` — [`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L31) — Test default config values when no env vars are set.
  - `test_is_connected_false_no_graph(self)` — [`L208`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L208) — Test is_connected returns False when graph is None.
  - `test_is_connected_false_on_exception(self)` — [`L220`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L220) — Test is_connected returns False when query raises.
  - `test_is_connected_true(self)` — [`L192`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L192) — Test is_connected returns True when graph query succeeds.
  - `test_ssl_variations(self)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L77) — Test various truthy values for FALKORDB_SSL.
  - `test_validate_config_bad_port(self)` — [`L286`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L286) — Test validate_config fails with non-numeric port.
  - `test_validate_config_no_host(self)` — [`L265`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L265) — Test validate_config fails when FALKORDB_HOST not set.
  - `test_validate_config_valid(self)` — [`L275`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_falkordb_remote.py#L275) — Test validate_config succeeds with host set.

