---
title: 'Module: tests/unit/core/test_error_handling_improvements.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_error_handling_improvements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_error_handling_improvements`/Test
symbols:
  TestMCPErrorTypes.test_error_category_enum: MCPErrorTypes#test_error_category_enum().
  TestMCPErrorTypes.test_mcp_error_creation: MCPErrorTypes#test_mcp_error_creation().
  TestMCPErrorTypes.test_mcp_error_defaults: MCPErrorTypes#test_mcp_error_defaults().
  TestErrorHandlerImprovements.test_handle_mcp_errors_decorator_with_initialization_error: ErrorHandlerImprovements#test_handle_mcp_errors_decorator_with_initialization_error().
  TestErrorHandlerImprovements.test_handle_mcp_errors_decorator_with_sync_initialization_error: ErrorHandlerImprovements#test_handle_mcp_errors_decorator_with_sync_initialization_error().
  TestErrorHandlerImprovements.test_error_severity_classification: ErrorHandlerImprovements#test_error_severity_classification().
  TestMCPErrorTypes.test_error_severity_enum: MCPErrorTypes#test_error_severity_enum().
  TestErrorHandlerImprovements.test_initialization_error_detection: ErrorHandlerImprovements#test_initialization_error_detection().
  TestErrorHandlerStatistics.test_error_counting: ErrorHandlerStatistics#test_error_counting().
  TestErrorHandlerStatistics.test_error_history: ErrorHandlerStatistics#test_error_history().
  TestErrorHandlerStatistics.test_statistics_clearing: ErrorHandlerStatistics#test_statistics_clearing().
  TestErrorHandlerImprovements.test_non_initialization_runtime_error: ErrorHandlerImprovements#test_non_initialization_runtime_error().
  TestErrorHandlerImprovements.test_error_handler_context_preservation: ErrorHandlerImprovements#test_error_handler_context_preservation().
  TestErrorHandlerImprovements.test_error_logging: ErrorHandlerImprovements#test_error_logging().
  TestErrorHandlerImprovements.test_concurrent_error_handling: ErrorHandlerImprovements#test_concurrent_error_handling().
  TestErrorHandlerImprovements.failing_function: ErrorHandlerImprovements#failing_function().
  TestErrorHandlerImprovements.successful_function: ErrorHandlerImprovements#successful_function().
  TestErrorHandlerImprovements.sync_function: ErrorHandlerImprovements#sync_function().
  TestErrorHandlerImprovements.failing_sync_function: ErrorHandlerImprovements#failing_sync_function().
  TestErrorHandlerImprovements.concurrent_function: ErrorHandlerImprovements#concurrent_function().
  TestErrorHandlerImprovements.test_handle_mcp_errors_decorator_with_other_runtime_error: ErrorHandlerImprovements#test_handle_mcp_errors_decorator_with_other_runtime_error().
  TestErrorHandlerImprovements.test_handle_mcp_errors_decorator_with_successful_function: ErrorHandlerImprovements#test_handle_mcp_errors_decorator_with_successful_function().
  TestErrorHandlerImprovements.test_handle_mcp_errors_decorator_with_sync_function: ErrorHandlerImprovements#test_handle_mcp_errors_decorator_with_sync_function().
  TestErrorHandlerImprovements.test_error_handler_singleton: ErrorHandlerImprovements#test_error_handler_singleton().
  TestMCPErrorTypes.test_error_inheritance: MCPErrorTypes#test_error_inheritance().
  TestErrorHandlerImprovements: ErrorHandlerImprovements#
  TestMCPErrorTypes: MCPErrorTypes#
  TestErrorHandlerStatistics: ErrorHandlerStatistics#
---
# Module: [`tests/unit/core/test_error_handling_improvements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py)

## Classes
### `TestErrorHandlerImprovements`
- def: [`tests/unit/core/test_error_handling_improvements.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L24)
- doc: Test improvements to the error handling system.
- signature: `class TestErrorHandlerImprovements:`
- members:
  - `concurrent_function(should_fail=False)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L184)
  - `failing_function()` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L59)
  - `failing_sync_function()` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L110)
  - `successful_function()` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L90)
  - `sync_function()` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L100)
  - `test_concurrent_error_handling(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L180) — Test that error handling works correctly under concurrent access.
  - `test_error_handler_context_preservation(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L123) — Test that error context is preserved in error handling.
  - `test_error_handler_singleton(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L161) — Test that get_error_handler returns a singleton.
  - `test_error_logging(self, caplog)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L168) — Test that errors are properly logged.
  - `test_error_severity_classification(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L141) — Test that errors are classified with appropriate severity.
  - `test_handle_mcp_errors_decorator_with_initialization_error(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L55) — Test the handle_mcp_errors decorator with initialization errors.
  - `test_handle_mcp_errors_decorator_with_other_runtime_error(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L74) — Test the handle_mcp_errors decorator with other runtime errors.
  - `test_handle_mcp_errors_decorator_with_successful_function(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L86) — Test the handle_mcp_errors decorator with successful function.
  - `test_handle_mcp_errors_decorator_with_sync_function(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L96) — Test the handle_mcp_errors decorator with synchronous functions.
  - `test_handle_mcp_errors_decorator_with_sync_initialization_error(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L106) — Test the handle_mcp_errors decorator with sync initialization error.
  - `test_initialization_error_detection(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L27) — Test that initialization errors are properly detected.
  - `test_non_initialization_runtime_error(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L42) — Test that other RuntimeErrors are handled normally.
- uses (calls/refs, reference-scoped): [`handle_error`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorCategory`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorHandler`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`ErrorSeverity`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`MCPError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`handle_mcp_errors`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#handle_mcp_errors), [`get_error_handler`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#get_error_handler), [`MEDIUM`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.MEDIUM), [`HIGH`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.HIGH), [`LOW`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.LOW), [`ANALYSIS`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.ANALYSIS), [`CONFIGURATION`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.CONFIGURATION)

### `TestErrorHandlerStatistics`
- def: [`tests/unit/core/test_error_handling_improvements.py:269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L269)
- doc: Test error handler statistics and monitoring.
- signature: `class TestErrorHandlerStatistics:`
- members:
  - `test_error_counting(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L272) — Test that error handler counts errors properly.
  - `test_error_history(self)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L288) — Test that error handler maintains error history.
  - `test_statistics_clearing(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L304) — Test that statistics can be cleared.
- uses (calls/refs, reference-scoped): [`handle_error`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorHandler`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`clear_history`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.clear_history), [`get_error_stats`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.get_error_stats), [`get_recent_errors`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.get_recent_errors)

### `TestMCPErrorTypes`
- def: [`tests/unit/core/test_error_handling_improvements.py:207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L207)
- doc: Test MCP error type definitions and behavior.
- signature: `class TestMCPErrorTypes:`
- members:
  - `test_error_category_enum(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L229) — Test ErrorCategory enum values.
  - `test_error_inheritance(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L261) — Test that MCPError properly inherits from Exception.
  - `test_error_severity_enum(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L247) — Test ErrorSeverity enum values.
  - `test_mcp_error_creation(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L210) — Test creating MCPError instances.
  - `test_mcp_error_defaults(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_error_handling_improvements.py#L222) — Test MCPError default values.
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorSeverity`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`MCPError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`MEDIUM`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.MEDIUM), [`HIGH`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.HIGH), [`VALIDATION`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`category`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`LOW`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.LOW), [`ANALYSIS`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.ANALYSIS), [`CRITICAL`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.CRITICAL), [`FILE_ACCESS`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.FILE_ACCESS), [`severity`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.severity), [`CONFIGURATION`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.CONFIGURATION), [`PARSING`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.PARSING), [`UNKNOWN`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.UNKNOWN), [`RESOURCE`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.RESOURCE), [`NETWORK`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.NETWORK)

