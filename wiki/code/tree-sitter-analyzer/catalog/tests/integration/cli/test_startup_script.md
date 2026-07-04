---
title: 'Module: tests/integration/cli/test_startup_script.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_startup_script.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_startup_script`/
symbols:
  TestStartupScriptErrorRecovery.failing_startup: TestStartupScriptErrorRecovery#failing_startup().
  TestStartupScriptErrorRecovery.test_resource_cleanup_on_failure.MockResource.cleanup: TestStartupScriptErrorRecovery#test_resource_cleanup_on_failure().MockResource#cleanup().
  TestStartupScriptFunctions.test_server_initialization_waiting_logic: TestStartupScriptFunctions#test_server_initialization_waiting_logic().
  TestStartupScriptFunctions.test_retry_logic_with_exponential_backoff: TestStartupScriptFunctions#test_retry_logic_with_exponential_backoff().
  TestStartupScriptFunctions.test_concurrent_initialization_checks: TestStartupScriptFunctions#test_concurrent_initialization_checks().
  TestStartupScriptIntegration.test_project_root_detection: TestStartupScriptIntegration#test_project_root_detection().
  TestStartupScriptIntegration.test_logging_configuration: TestStartupScriptIntegration#test_logging_configuration().
  TestStartupScriptIntegration.test_graceful_shutdown_handling: TestStartupScriptIntegration#test_graceful_shutdown_handling().
  TestStartupScriptErrorRecovery.test_recovery_from_temporary_failures: TestStartupScriptErrorRecovery#test_recovery_from_temporary_failures().
  TestStartupScriptErrorRecovery.test_resource_cleanup_on_failure: TestStartupScriptErrorRecovery#test_resource_cleanup_on_failure().
  TestStartupScriptErrorRecovery.test_resource_cleanup_on_failure.MockResource: TestStartupScriptErrorRecovery#test_resource_cleanup_on_failure().MockResource#
  TestStartupScriptFunctions.mock_is_initialized: TestStartupScriptFunctions#mock_is_initialized().
  TestStartupScriptFunctions.mock_operation: TestStartupScriptFunctions#mock_operation().
  TestStartupScriptFunctions.check_initialization: TestStartupScriptFunctions#check_initialization().
  TestStartupScriptIntegration.mock_server_run: TestStartupScriptIntegration#mock_server_run().
  TestStartupScriptErrorRecovery.flaky_operation: TestStartupScriptErrorRecovery#flaky_operation().
  MockResource.name: MockResource#name.
  TestStartupScriptFunctions: TestStartupScriptFunctions#
  TestStartupScriptFunctions.test_main_execution_with_dependencies_ok: TestStartupScriptFunctions#test_main_execution_with_dependencies_ok().
  TestStartupScriptFunctions.test_dependency_checking_logic: TestStartupScriptFunctions#test_dependency_checking_logic().
  TestStartupScriptFunctions.test_server_initialization_timeout: TestStartupScriptFunctions#test_server_initialization_timeout().
  TestStartupScriptIntegration: TestStartupScriptIntegration#
  TestStartupScriptIntegration.test_server_creation_in_startup: TestStartupScriptIntegration#test_server_creation_in_startup().
  TestStartupScriptIntegration.test_startup_error_handling: TestStartupScriptIntegration#test_startup_error_handling().
  TestStartupScriptIntegration.test_environment_variable_handling: TestStartupScriptIntegration#test_environment_variable_handling().
  TestStartupScriptErrorRecovery: TestStartupScriptErrorRecovery#
  TestStartupScriptErrorRecovery.test_dependency_fallback_mechanisms: TestStartupScriptErrorRecovery#test_dependency_fallback_mechanisms().
  TestStartupScriptErrorRecovery.test_resource_cleanup_on_failure.MockResource.__init__: TestStartupScriptErrorRecovery#test_resource_cleanup_on_failure().MockResource#__init__().
---
# Module: [`tests/integration/cli/test_startup_script.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py)

## Classes
### `MockResource`
- def: [`tests/integration/cli/test_startup_script.py:317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L317)
- signature: `class MockResource:`
- members:
  - `cleanup(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L322)
  - `name` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L319)
- protocol/private: `__init__`[`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L318)
- used by: (1 test-only callers)

### `TestStartupScriptErrorRecovery`
- def: [`tests/integration/cli/test_startup_script.py:265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L265)
- doc: Test error recovery mechanisms in startup script.
- signature: `class TestStartupScriptErrorRecovery:`
- members:
  - `failing_startup()` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L325)
  - `flaky_operation()` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L273)
  - `test_dependency_fallback_mechanisms(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L294) — Test fallback mechanisms for missing dependencies.
  - `test_recovery_from_temporary_failures(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L269) — Test recovery from temporary failures.
  - `test_resource_cleanup_on_failure(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L312) — Test that resources are cleaned up on startup failure.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestStartupScriptFunctions`
- def: [`tests/integration/cli/test_startup_script.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L24)
- doc: Test startup script functionality.
- signature: `class TestStartupScriptFunctions:`
- members:
  - `check_initialization()` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L140)
  - `mock_is_initialized()` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L63)
  - `mock_operation()` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L110)
  - `test_concurrent_initialization_checks(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L133) — Test concurrent initialization checks don't interfere.
  - `test_dependency_checking_logic(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L39) — Test the dependency checking logic.
  - `test_main_execution_with_dependencies_ok(self, mock_asyncio_run, mock_check_deps)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L29) — Test main execution when dependencies are available.
  - `test_retry_logic_with_exponential_backoff(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L104) — Test retry logic with exponential backoff.
  - `test_server_initialization_timeout(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L84) — Test server initialization timeout handling.
  - `test_server_initialization_waiting_logic(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L57) — Test the server initialization waiting logic.

### `TestStartupScriptIntegration`
- def: [`tests/integration/cli/test_startup_script.py:151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L151)
- doc: Integration tests for startup script functionality.
- signature: `class TestStartupScriptIntegration:`
- members:
  - `mock_server_run()` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L228)
  - `test_environment_variable_handling(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L250) — Test handling of environment variables.
  - `test_graceful_shutdown_handling(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L224) — Test graceful shutdown handling.
  - `test_logging_configuration(self, caplog)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L197) — Test that startup script configures logging properly.
  - `test_project_root_detection(self, mock_detect)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L155) — Test project root detection in startup.
  - `test_server_creation_in_startup(self, mock_server_class)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L167) — Test server creation during startup.
  - `test_startup_error_handling(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_startup_script.py#L182) — Test error handling during startup.
- uses (calls/refs, reference-scoped): [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger), [`detect_project_root`](../../../tree_sitter_analyzer/project_detector.md#detect_project_root)

