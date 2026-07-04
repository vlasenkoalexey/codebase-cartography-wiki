---
title: 'Module: tests/unit/mcp/test_utils/test_error_handler.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_error_handler.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_error_handler`/Test
symbols:
  TestMCPError.test_basic_initialization: MCPError#test_basic_initialization().
  TestMCPError.test_initialization_with_all_parameters: MCPError#test_initialization_with_all_parameters().
  TestErrorCategory.test_category_values: ErrorCategory#test_category_values().
  TestHandleMCPErrorsDecorator.test_func: HandleMCPErrorsDecorator#test_func().
  TestMCPError.test_to_dict: MCPError#test_to_dict().
  TestFileAccessError.test_file_access_error_initialization: FileAccessError#test_file_access_error_initialization().
  TestParsingError.test_parsing_error_initialization: ParsingError#test_parsing_error_initialization().
  TestAnalysisError.test_analysis_error_initialization: AnalysisError#test_analysis_error_initialization().
  TestValidationError.test_validation_error_initialization: ValidationError#test_validation_error_initialization().
  TestResourceError.test_resource_error_initialization: ResourceError#test_resource_error_initialization().
  TestErrorHandler.test_handle_mcp_error: ErrorHandler#test_handle_mcp_error().
  TestErrorSeverity.test_severity_values: ErrorSeverity#test_severity_values().
  TestFileAccessError.test_file_access_error_with_custom_severity: FileAccessError#test_file_access_error_with_custom_severity().
  TestErrorHandler.test_handler_initialization: ErrorHandler#test_handler_initialization().
  TestErrorHandler.test_clear_history: ErrorHandler#test_clear_history().
  TestErrorHandler.test_exact_type_match_takes_precedence: ErrorHandler#test_exact_type_match_takes_precedence().
  TestErrorSeverity.test_severity_comparison: ErrorSeverity#test_severity_comparison().
  TestAnalysisError.test_analysis_error_with_custom_severity: AnalysisError#test_analysis_error_with_custom_severity().
  TestErrorHandler.test_register_recovery_strategy: ErrorHandler#test_register_recovery_strategy().
  TestErrorHandler.test_history_size_limit: ErrorHandler#test_history_size_limit().
  TestErrorHandler.test_custom_recovery_strategy_called: ErrorHandler#test_custom_recovery_strategy_called().
  TestErrorHandler.test_recovery_strategy_failure_handling: ErrorHandler#test_recovery_strategy_failure_handling().
  TestErrorHandler.test_parent_class_recovery_strategy: ErrorHandler#test_parent_class_recovery_strategy().
  TestHandleMCPErrorsDecorator.test_decorator_with_runtime_error_not_initialized: HandleMCPErrorsDecorator#test_decorator_with_runtime_error_not_initialized().
  TestHandleMCPErrorsDecorator.test_decorator_updates_error_stats: HandleMCPErrorsDecorator#test_decorator_updates_error_stats().
  TestErrorHandlerRecovery.test_recovery_strategy_returns_none: ErrorHandlerRecovery#test_recovery_strategy_returns_none().
  TestErrorHandlerRecovery.test_recovery_strategy_returns_empty_dict: ErrorHandlerRecovery#test_recovery_strategy_returns_empty_dict().
  TestErrorHandlerEdgeCases.test_clear_history_with_no_history: ErrorHandlerEdgeCases#test_clear_history_with_no_history().
  TestErrorHandler.test_error_statistics_update: ErrorHandler#test_error_statistics_update().
  TestErrorHandler.test_error_history_tracking: ErrorHandler#test_error_history_tracking().
  TestErrorHandler.test_get_error_stats: ErrorHandler#test_get_error_stats().
  TestErrorHandler.test_get_recent_errors: ErrorHandler#test_get_recent_errors().
  TestErrorHandlerRecovery.test_multiple_recovery_strategies: ErrorHandlerRecovery#test_multiple_recovery_strategies().
  TestErrorHandlerEdgeCases.test_error_with_complex_details: ErrorHandlerEdgeCases#test_error_with_complex_details().
  TestParsingError.test_parsing_error_without_language: ParsingError#test_parsing_error_without_language().
  TestValidationError.test_validation_error_without_value: ValidationError#test_validation_error_without_value().
  TestErrorHandler.test_handle_generic_file_not_found_error: ErrorHandler#test_handle_generic_file_not_found_error().
  TestErrorHandler.test_handle_permission_error: ErrorHandler#test_handle_permission_error().
  TestErrorHandler.test_handle_value_error: ErrorHandler#test_handle_value_error().
  TestErrorHandler.test_handle_os_error: ErrorHandler#test_handle_os_error().
  TestErrorHandler.test_handle_runtime_error: ErrorHandler#test_handle_runtime_error().
  TestErrorHandler.test_handle_memory_error: ErrorHandler#test_handle_memory_error().
  TestErrorHandler.test_handle_timeout_error: ErrorHandler#test_handle_timeout_error().
  TestErrorHandler.test_get_recent_errors_empty_history: ErrorHandler#test_get_recent_errors_empty_history().
  TestHandleMCPErrorsDecorator.test_decorator_with_sync_function_exception: HandleMCPErrorsDecorator#test_decorator_with_sync_function_exception().
  TestHandleMCPErrorsDecorator.test_decorator_with_async_function_exception: HandleMCPErrorsDecorator#test_decorator_with_async_function_exception().
  TestHandleMCPErrorsDecorator.test_decorator_with_mcp_error: HandleMCPErrorsDecorator#test_decorator_with_mcp_error().
  TestGetErrorHandler.test_get_error_handler_is_error_handler_instance: GetErrorHandler#test_get_error_handler_is_error_handler_instance().
  TestErrorHandlerLogging.test_critical_error_logging: ErrorHandlerLogging#test_critical_error_logging().
  TestErrorHandlerLogging.test_high_severity_error_logging: ErrorHandlerLogging#test_high_severity_error_logging().
  TestErrorHandlerLogging.test_medium_severity_error_logging: ErrorHandlerLogging#test_medium_severity_error_logging().
  TestErrorHandlerLogging.test_low_severity_error_logging: ErrorHandlerLogging#test_low_severity_error_logging().
  TestErrorHandlerEdgeCases.test_handle_error_with_none_context: ErrorHandlerEdgeCases#test_handle_error_with_none_context().
  TestErrorHandlerEdgeCases.test_handle_error_with_empty_operation: ErrorHandlerEdgeCases#test_handle_error_with_empty_operation().
  TestErrorHandlerEdgeCases.test_get_error_stats_with_no_errors: ErrorHandlerEdgeCases#test_get_error_stats_with_no_errors().
  TestHandleMCPErrorsDecorator.my_function: HandleMCPErrorsDecorator#my_function().
  TestHandleMCPErrorsDecorator.test_decorator_with_sync_function_success: HandleMCPErrorsDecorator#test_decorator_with_sync_function_success().
  TestHandleMCPErrorsDecorator.test_decorator_with_async_function_success: HandleMCPErrorsDecorator#test_decorator_with_async_function_success().
  TestHandleMCPErrorsDecorator.test_decorator_preserves_function_name: HandleMCPErrorsDecorator#test_decorator_preserves_function_name().
  TestGetErrorHandler.test_get_error_handler_returns_singleton: GetErrorHandler#test_get_error_handler_returns_singleton().
  TestErrorHandler.custom_strategy: ErrorHandler#custom_strategy().
  TestErrorHandler.parent_recovery: ErrorHandler#parent_recovery().
  TestErrorHandler.custom_recovery: ErrorHandler#custom_recovery().
  TestErrorHandler.failing_recovery: ErrorHandler#failing_recovery().
  TestErrorHandler.exact_recovery: ErrorHandler#exact_recovery().
  TestErrorHandlerRecovery.none_recovery: ErrorHandlerRecovery#none_recovery().
  TestErrorHandlerRecovery.empty_recovery: ErrorHandlerRecovery#empty_recovery().
  TestErrorSeverity: ErrorSeverity#
  TestErrorCategory: ErrorCategory#
  TestMCPError: MCPError#
  TestFileAccessError: FileAccessError#
  TestParsingError: ParsingError#
  TestAnalysisError: AnalysisError#
  TestValidationError: ValidationError#
  TestResourceError: ResourceError#
  TestErrorHandler: ErrorHandler#
  TestHandleMCPErrorsDecorator: HandleMCPErrorsDecorator#
  TestGetErrorHandler: GetErrorHandler#
  TestErrorHandlerLogging: ErrorHandlerLogging#
  TestErrorHandlerRecovery: ErrorHandlerRecovery#
  TestErrorHandlerEdgeCases: ErrorHandlerEdgeCases#
---
# Module: [`tests/unit/mcp/test_utils/test_error_handler.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py)

## Classes
### `TestAnalysisError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L150)
- doc: Test AnalysisError subclass
- signature: `class TestAnalysisError:`
- members:
  - `test_analysis_error_initialization(self)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L153) — Test analysis error initialization
  - `test_analysis_error_with_custom_severity(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L160) — Test analysis error with custom severity
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorSeverity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`ANALYSIS`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.ANALYSIS), [`CRITICAL`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.CRITICAL), [`severity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.severity)

### `TestErrorCategory`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L46)
- doc: Test ErrorCategory enum
- signature: `class TestErrorCategory:`
- members:
  - `test_category_values(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L49) — Test all categories are defined
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`VALIDATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`ANALYSIS`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.ANALYSIS), [`FILE_ACCESS`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.FILE_ACCESS), [`CONFIGURATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.CONFIGURATION), [`PARSING`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.PARSING), [`UNKNOWN`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.UNKNOWN), [`RESOURCE`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.RESOURCE), [`NETWORK`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.NETWORK)

### `TestErrorHandler`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L197)
- doc: Test ErrorHandler class
- signature: `class TestErrorHandler:`
- members:
  - `custom_recovery(error, context)` — [`L402`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L402)
  - `custom_strategy(error, context)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L212)
  - `exact_recovery(error, context)` — [`L445`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L445)
  - `failing_recovery(error, context)` — [`L415`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L415)
  - `parent_recovery(error, context)` — [`L429`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L429)
  - `test_clear_history(self)` — [`L385`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L385) — Test clearing error history
  - `test_custom_recovery_strategy_called(self)` — [`L398`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L398) — Test custom recovery strategy is called
  - `test_error_history_tracking(self)` — [`L332`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L332) — Test error history is tracked
  - `test_error_statistics_update(self)` — [`L319`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L319) — Test error statistics are updated
  - `test_exact_type_match_takes_precedence(self)` — [`L438`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L438) — Test exact type match takes precedence over parent class — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `test_get_error_stats(self)` — [`L355`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L355) — Test getting error statistics
  - `test_get_recent_errors(self)` — [`L367`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L367) — Test getting recent errors
  - `test_get_recent_errors_empty_history(self)` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L379) — Test getting recent errors when history is empty
  - `test_handle_generic_file_not_found_error(self)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L234) — Test handling generic FileNotFoundError
  - `test_handle_mcp_error(self)` — [`L219`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L219) — Test handling MCP error
  - `test_handle_memory_error(self)` — [`L290`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L290) — Test handling MemoryError
  - `test_handle_os_error(self)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L268) — Test handling OSError
  - `test_handle_permission_error(self)` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L245) — Test handling PermissionError
  - `test_handle_runtime_error(self)` — [`L279`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L279) — Test handling RuntimeError
  - `test_handle_timeout_error(self)` — [`L302`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L302) — Test handling asyncio.TimeoutError
  - `test_handle_value_error(self)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L257) — Test handling ValueError
  - `test_handler_initialization(self)` — [`L200`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L200) — Test handler initialization
  - `test_history_size_limit(self)` — [`L344`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L344) — Test history size limit is enforced — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `test_parent_class_recovery_strategy(self)` — [`L424`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L424) — Test parent class recovery strategy is used
  - `test_recovery_strategy_failure_handling(self)` — [`L411`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L411) — Test recovery strategy failure is handled gracefully — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `test_register_recovery_strategy(self)` — [`L208`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L208) — Test registering custom recovery strategy
- uses (calls/refs, reference-scoped): [`handle_error`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorHandler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`MCPError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`error_history`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.error_history), [`error_counts`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.error_counts), [`register_recovery_strategy`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.register_recovery_strategy), [`clear_history`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.clear_history), [`recovery_strategies`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.recovery_strategies), [`get_error_stats`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.get_error_stats), [`VALIDATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`get_recent_errors`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.get_recent_errors), [`max_history_size`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.max_history_size)

### `TestErrorHandlerEdgeCases`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:653`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L653)
- doc: Test error handler edge cases
- signature: `class TestErrorHandlerEdgeCases:`
- members:
  - `test_clear_history_with_no_history(self)` — [`L681`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L681) — Test clearing history when already empty
  - `test_error_with_complex_details(self)` — [`L688`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L688) — Test error with complex details dictionary
  - `test_get_error_stats_with_no_errors(self)` — [`L674`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L674) — Test getting stats when no errors occurred
  - `test_handle_error_with_empty_operation(self)` — [`L665`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L665) — Test handling error with empty operation name
  - `test_handle_error_with_none_context(self)` — [`L656`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L656) — Test handling error with None context
- uses (calls/refs, reference-scoped): [`handle_error`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorHandler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`MCPError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`error_history`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.error_history), [`error_counts`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.error_counts), [`clear_history`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.clear_history), [`get_error_stats`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.get_error_stats)

### `TestErrorHandlerLogging`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:565`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L565)
- doc: Test error handler logging behavior
- signature: `class TestErrorHandlerLogging:`
- members:
  - `test_critical_error_logging(self, mock_logger)` — [`L569`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L569) — Test critical errors are logged at critical level
  - `test_high_severity_error_logging(self, mock_logger)` — [`L579`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L579) — Test high severity errors are logged at error level
  - `test_low_severity_error_logging(self, mock_logger)` — [`L599`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L599) — Test low severity errors are logged at info level
  - `test_medium_severity_error_logging(self, mock_logger)` — [`L589`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L589) — Test medium severity errors are logged at warning level
- uses (calls/refs, reference-scoped): [`handle_error`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorHandler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler)

### `TestErrorHandlerRecovery`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:612`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L612)
- doc: Test error handler recovery mechanisms
- signature: `class TestErrorHandlerRecovery:`
- members:
  - `empty_recovery(error, context)` — [`L631`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L631)
  - `none_recovery(error, context)` — [`L619`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L619)
  - `test_multiple_recovery_strategies(self)` — [`L639`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L639) — Test multiple recovery strategies can be registered
  - `test_recovery_strategy_returns_empty_dict(self)` — [`L627`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L627) — Test recovery strategy returning empty dict is handled
  - `test_recovery_strategy_returns_none(self)` — [`L615`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L615) — Test recovery strategy returning None is handled
- uses (calls/refs, reference-scoped): [`handle_error`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.handle_error), [`ErrorHandler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`register_recovery_strategy`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.register_recovery_strategy)

### `TestErrorSeverity`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:30`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L30)
- doc: Test ErrorSeverity enum
- signature: `class TestErrorSeverity:`
- members:
  - `test_severity_comparison(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L40) — Test severity can be compared
  - `test_severity_values(self)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L33) — Test all severity levels are defined
- uses (calls/refs, reference-scoped): [`ErrorSeverity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`MEDIUM`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.MEDIUM), [`HIGH`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.HIGH), [`LOW`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.LOW), [`CRITICAL`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.CRITICAL)

### `TestFileAccessError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L109)
- doc: Test FileAccessError subclass
- signature: `class TestFileAccessError:`
- members:
  - `test_file_access_error_initialization(self)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L112) — Test file access error initialization
  - `test_file_access_error_with_custom_severity(self)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L119) — Test file access error with custom severity
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorSeverity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`CRITICAL`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.CRITICAL), [`FILE_ACCESS`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.FILE_ACCESS), [`severity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.severity), [`FileAccessError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#FileAccessError), [`recoverable`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.recoverable)

### `TestGetErrorHandler`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:550`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L550)
- doc: Test get_error_handler function
- signature: `class TestGetErrorHandler:`
- members:
  - `test_get_error_handler_is_error_handler_instance(self)` — [`L559`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L559) — Test get_error_handler returns ErrorHandler instance
  - `test_get_error_handler_returns_singleton(self)` — [`L553`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L553) — Test get_error_handler returns singleton instance
- uses (calls/refs, reference-scoped): [`ErrorHandler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), [`get_error_handler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#get_error_handler)

### `TestHandleMCPErrorsDecorator`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:455`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L455)
- doc: Test handle_mcp_errors decorator
- signature: `class TestHandleMCPErrorsDecorator:`
- members:
  - `my_function()` — [`L502`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L502)
  - `test_decorator_preserves_function_name(self)` — [`L498`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L498) — Test decorator preserves function name
  - `test_decorator_updates_error_stats(self)` — [`L532`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L532) — Test decorator updates error statistics
  - `test_decorator_with_async_function_exception(self)` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L488) — Test decorator with exception in async function
  - `test_decorator_with_async_function_success(self)` — [`L478`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L478) — Test decorator with successful async function
  - `test_decorator_with_mcp_error(self)` — [`L507`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L507) — Test decorator with MCPError (should re-raise as-is)
  - `test_decorator_with_runtime_error_not_initialized(self)` — [`L519`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L519) — Test decorator handles 'not fully initialized' runtime error
  - `test_decorator_with_sync_function_exception(self)` — [`L468`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L468) — Test decorator with exception in sync function
  - `test_decorator_with_sync_function_success(self)` — [`L458`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L458) — Test decorator with successful sync function
  - `test_func()` — [`L462`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L462)
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`MCPError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`handle_mcp_errors`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#handle_mcp_errors), [`error_counts`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.error_counts), [`get_error_handler`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#get_error_handler), [`VALIDATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`CONFIGURATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.CONFIGURATION)

### `TestMCPError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L61)
- doc: Test MCPError base class
- signature: `class TestMCPError:`
- members:
  - `test_basic_initialization(self)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L64) — Test basic error initialization
  - `test_initialization_with_all_parameters(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L74) — Test initialization with all parameters
  - `test_to_dict(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L90) — Test error conversion to dictionary
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorSeverity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`MCPError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`to_dict`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.to_dict), [`MEDIUM`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.MEDIUM), [`HIGH`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.HIGH), [`VALIDATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`LOW`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.LOW), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`severity`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.severity), [`PARSING`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.PARSING), [`UNKNOWN`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.UNKNOWN), [`recoverable`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.recoverable), [`timestamp`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.timestamp)

### `TestParsingError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L131)
- doc: Test ParsingError subclass
- signature: `class TestParsingError:`
- members:
  - `test_parsing_error_initialization(self)` — [`L134`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L134) — Test parsing error initialization
  - `test_parsing_error_without_language(self)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L144) — Test parsing error without language specified
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`ParsingError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ParsingError), [`PARSING`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.PARSING)

### `TestResourceError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L186)
- doc: Test ResourceError subclass
- signature: `class TestResourceError:`
- members:
  - `test_resource_error_initialization(self)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L189) — Test resource error initialization
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`ResourceError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ResourceError), [`RESOURCE`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.RESOURCE)

### `TestValidationError`
- def: [`tests/unit/mcp/test_utils/test_error_handler.py:170`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L170)
- doc: Test ValidationError subclass
- signature: `class TestValidationError:`
- members:
  - `test_validation_error_initialization(self)` — [`L173`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L173) — Test validation error initialization
  - `test_validation_error_without_value(self)` — [`L180`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_error_handler.py#L180) — Test validation error without value
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`VALIDATION`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.VALIDATION), [`category`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.category), [`details`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.details), [`message`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError.message), [`ValidationError`](../../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ValidationError)

