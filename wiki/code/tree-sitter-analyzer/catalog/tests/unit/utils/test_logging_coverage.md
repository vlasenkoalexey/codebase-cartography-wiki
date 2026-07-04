---
title: 'Module: tests/unit/utils/test_logging_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_logging_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_logging_coverage`/Test
symbols:
  TestSafeStreamHandler.test_handler_emit_with_closed_stream: SafeStreamHandler#test_handler_emit_with_closed_stream().
  TestSafeStreamHandler.test_handler_emit_with_non_writable_stream: SafeStreamHandler#test_handler_emit_with_non_writable_stream().
  TestSafeStreamHandler.test_handler_emit_success: SafeStreamHandler#test_handler_emit_success().
  TestLogFunctions.test_log_info_with_closed_handler: LogFunctions#test_log_info_with_closed_handler().
  TestLogFunctions.test_log_warning_with_closed_handler: LogFunctions#test_log_warning_with_closed_handler().
  TestLogFunctions.test_log_error_with_closed_handler: LogFunctions#test_log_error_with_closed_handler().
  TestLogFunctions.test_log_debug_with_closed_handler: LogFunctions#test_log_debug_with_closed_handler().
  TestQuietMode.test_quiet_mode_enabled: QuietMode#test_quiet_mode_enabled().
  TestQuietMode.test_quiet_mode_disabled: QuietMode#test_quiet_mode_disabled().
  TestSuppressOutput.func_with_print: SuppressOutput#func_with_print().
  TestSetupLogger.test_setup_logger_default: SetupLogger#test_setup_logger_default().
  TestSetupLogger.test_setup_logger_with_string_level_debug: SetupLogger#test_setup_logger_with_string_level_debug().
  TestSetupLogger.test_setup_logger_with_string_level_info: SetupLogger#test_setup_logger_with_string_level_info().
  TestSetupLogger.test_setup_logger_with_string_level_warning: SetupLogger#test_setup_logger_with_string_level_warning().
  TestSetupLogger.test_setup_logger_with_string_level_error: SetupLogger#test_setup_logger_with_string_level_error().
  TestSetupLogger.test_setup_logger_with_invalid_string_level: SetupLogger#test_setup_logger_with_invalid_string_level().
  TestSetupLogger.test_setup_logger_respects_env_debug: SetupLogger#test_setup_logger_respects_env_debug().
  TestSetupLogger.test_setup_logger_respects_env_info: SetupLogger#test_setup_logger_respects_env_info().
  TestSetupLogger.test_setup_logger_empty_env_uses_default: SetupLogger#test_setup_logger_empty_env_uses_default().
  TestSafeStreamHandler.test_handler_default_stream: SafeStreamHandler#test_handler_default_stream().
  TestSafeStreamHandler.test_handler_with_custom_stream: SafeStreamHandler#test_handler_with_custom_stream().
  TestLogFunctions.test_log_info: LogFunctions#test_log_info().
  TestLogFunctions.test_log_warning: LogFunctions#test_log_warning().
  TestLogFunctions.test_log_error: LogFunctions#test_log_error().
  TestLogFunctions.test_log_debug: LogFunctions#test_log_debug().
  TestSafePrint.test_safe_print_info: SafePrint#test_safe_print_info().
  TestSafePrint.test_safe_print_warning: SafePrint#test_safe_print_warning().
  TestSafePrint.test_safe_print_error: SafePrint#test_safe_print_error().
  TestSafePrint.test_safe_print_debug: SafePrint#test_safe_print_debug().
  TestSafePrint.test_safe_print_unknown_level: SafePrint#test_safe_print_unknown_level().
  TestSafePrint.test_safe_print_quiet: SafePrint#test_safe_print_quiet().
  TestSafePrint.test_safe_print_none_message: SafePrint#test_safe_print_none_message().
  TestPerformanceLogging.test_create_performance_logger: PerformanceLogging#test_create_performance_logger().
  TestPerformanceLogging.test_log_performance_basic: PerformanceLogging#test_log_performance_basic().
  TestPerformanceLogging.test_log_performance_with_time: PerformanceLogging#test_log_performance_with_time().
  TestPerformanceLogging.test_log_performance_with_dict_details: PerformanceLogging#test_log_performance_with_dict_details().
  TestPerformanceLogging.test_log_performance_with_string_details: PerformanceLogging#test_log_performance_with_string_details().
  TestPerformanceLogging.test_log_performance_full: PerformanceLogging#test_log_performance_full().
  TestPerformanceLogging.test_setup_performance_logger: PerformanceLogging#test_setup_performance_logger().
  TestLoggingContext.test_logging_context_enabled_with_level: LoggingContext#test_logging_context_enabled_with_level().
  TestLoggingContext.test_logging_context_disabled: LoggingContext#test_logging_context_disabled().
  TestLoggingContext.test_logging_context_without_level: LoggingContext#test_logging_context_without_level().
  TestSuppressOutput.test_suppress_output_decorator: SuppressOutput#test_suppress_output_decorator().
  TestSuppressOutput.test_suppress_output_in_test_mode: SuppressOutput#test_suppress_output_in_test_mode().
  TestSetupSafeLoggingShutdown.test_setup_safe_logging_shutdown: SetupSafeLoggingShutdown#test_setup_safe_logging_shutdown().
  TestGlobalLoggers.test_logger_exists: GlobalLoggers#test_logger_exists().
  TestGlobalLoggers.test_perf_logger_exists: GlobalLoggers#test_perf_logger_exists().
  TestSetupLogger: SetupLogger#
  TestSafeStreamHandler: SafeStreamHandler#
  TestLogFunctions: LogFunctions#
  TestQuietMode: QuietMode#
  TestSafePrint: SafePrint#
  TestPerformanceLogging: PerformanceLogging#
  TestLoggingContext: LoggingContext#
  TestSuppressOutput: SuppressOutput#
  TestSetupSafeLoggingShutdown: SetupSafeLoggingShutdown#
  TestGlobalLoggers: GlobalLoggers#
---
# Module: [`tests/unit/utils/test_logging_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py)

## Classes
### `TestGlobalLoggers`
- def: [`tests/unit/utils/test_logging_coverage.py:408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L408)
- doc: Tests for global logger instances
- signature: `class TestGlobalLoggers:`
- members:
  - `test_logger_exists(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L411) — Test global logger exists
  - `test_perf_logger_exists(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L416) — Test global perf_logger exists
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`perf_logger`](../../../tree_sitter_analyzer/utils/logging.md#perf_logger)

### `TestLogFunctions`
- def: [`tests/unit/utils/test_logging_coverage.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L168)
- doc: Tests for logging functions
- signature: `class TestLogFunctions:`
- members:
  - `test_log_debug(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L189) — Test log_debug function
  - `test_log_debug_with_closed_handler(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L217) — Test log_debug handles closed handlers gracefully
  - `test_log_error(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L183) — Test log_error function
  - `test_log_error_with_closed_handler(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L210) — Test log_error handles closed handlers gracefully
  - `test_log_info(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L171) — Test log_info function
  - `test_log_info_with_closed_handler(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L195) — Test log_info handles closed handlers gracefully
  - `test_log_warning(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L177) — Test log_warning function
  - `test_log_warning_with_closed_handler(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L203) — Test log_warning handles closed handlers gracefully
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info)

### `TestLoggingContext`
- def: [`tests/unit/utils/test_logging_coverage.py:332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L332)
- doc: Tests for LoggingContext context manager
- signature: `class TestLoggingContext:`
- members:
  - `test_logging_context_disabled(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L346) — Test LoggingContext when disabled
  - `test_logging_context_enabled_with_level(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L335) — Test LoggingContext when enabled with level
  - `test_logging_context_without_level(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L357) — Test LoggingContext without specifying level
- uses (calls/refs, reference-scoped): [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext)

### `TestPerformanceLogging`
- def: [`tests/unit/utils/test_logging_coverage.py:289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L289)
- doc: Tests for performance logging functions
- signature: `class TestPerformanceLogging:`
- members:
  - `test_create_performance_logger(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L292) — Test create_performance_logger
  - `test_log_performance_basic(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L298) — Test log_performance with just operation
  - `test_log_performance_full(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L318) — Test log_performance with all parameters
  - `test_log_performance_with_dict_details(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L308) — Test log_performance with dict details
  - `test_log_performance_with_string_details(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L313) — Test log_performance with string details
  - `test_log_performance_with_time(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L303) — Test log_performance with execution time
  - `test_setup_performance_logger(self)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L325) — Test setup_performance_logger function
- uses (calls/refs, reference-scoped): [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`create_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#create_performance_logger), [`setup_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_performance_logger)

### `TestQuietMode`
- def: [`tests/unit/utils/test_logging_coverage.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L225)
- doc: Tests for QuietMode context manager
- signature: `class TestQuietMode:`
- members:
  - `test_quiet_mode_disabled(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L238) — Test QuietMode when disabled
  - `test_quiet_mode_enabled(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L228) — Test QuietMode when enabled
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode)

### `TestSafePrint`
- def: [`tests/unit/utils/test_logging_coverage.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L249)
- doc: Tests for safe_print function
- signature: `class TestSafePrint:`
- members:
  - `test_safe_print_debug(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L268) — Test safe_print with debug level
  - `test_safe_print_error(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L263) — Test safe_print with error level
  - `test_safe_print_info(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L252) — Test safe_print with info level
  - `test_safe_print_none_message(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L283) — Test safe_print with None message
  - `test_safe_print_quiet(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L278) — Test safe_print with quiet=True does nothing
  - `test_safe_print_unknown_level(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L273) — Test safe_print with unknown level defaults to info
  - `test_safe_print_warning(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L258) — Test safe_print with warning level
- uses (calls/refs, reference-scoped): [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print)

### `TestSafeStreamHandler`
- def: [`tests/unit/utils/test_logging_coverage.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L94)
- doc: Tests for SafeStreamHandler class
- signature: `class TestSafeStreamHandler:`
- members:
  - `test_handler_default_stream(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L97) — Test handler defaults to stderr
  - `test_handler_emit_success(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L147) — Test handler emits to valid stream
  - `test_handler_emit_with_closed_stream(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L108) — Test handler handles closed stream
  - `test_handler_emit_with_non_writable_stream(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L127) — Test handler handles non-writable stream
  - `test_handler_with_custom_stream(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L102) — Test handler with custom stream
- uses (calls/refs, reference-scoped): [`SafeStreamHandler`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler), [`emit`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler.emit)

### `TestSetupLogger`
- def: [`tests/unit/utils/test_logging_coverage.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L34)
- doc: Tests for setup_logger function
- signature: `class TestSetupLogger:`
- members:
  - `test_setup_logger_default(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L37) — Test default logger setup
  - `test_setup_logger_empty_env_uses_default(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L86) — Test logger uses default when LOG_LEVEL is empty
  - `test_setup_logger_respects_env_debug(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L73) — Test logger respects LOG_LEVEL env var
  - `test_setup_logger_respects_env_info(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L80) — Test logger respects LOG_LEVEL=INFO
  - `test_setup_logger_with_invalid_string_level(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L67) — Test logger setup with invalid string level defaults to WARNING
  - `test_setup_logger_with_string_level_debug(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L44) — Test logger setup with string DEBUG level
  - `test_setup_logger_with_string_level_error(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L61) — Test logger setup with string ERROR level
  - `test_setup_logger_with_string_level_info(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L50) — Test logger setup with string INFO level
  - `test_setup_logger_with_string_level_warning(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L56) — Test logger setup with string WARNING level
- uses (calls/refs, reference-scoped): [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger)

### `TestSetupSafeLoggingShutdown`
- def: [`tests/unit/utils/test_logging_coverage.py:399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L399)
- doc: Tests for setup_safe_logging_shutdown function
- signature: `class TestSetupSafeLoggingShutdown:`
- members:
  - `test_setup_safe_logging_shutdown(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L402) — Test setup_safe_logging_shutdown registers cleanup
- uses (calls/refs, reference-scoped): [`setup_safe_logging_shutdown`](../../../tree_sitter_analyzer/utils/logging.md#setup_safe_logging_shutdown)

### `TestSuppressOutput`
- def: [`tests/unit/utils/test_logging_coverage.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L369)
- doc: Tests for suppress_output decorator
- signature: `class TestSuppressOutput:`
- members:
  - `func_with_print()` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L376)
  - `test_suppress_output_decorator(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L372) — Test suppress_output decorator
  - `test_suppress_output_in_test_mode(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_coverage.py#L383) — Test suppress_output doesn't suppress in test mode
- uses (calls/refs, reference-scoped): [`suppress_output`](../../../tree_sitter_analyzer/utils/logging.md#suppress_output)

