---
title: 'Module: tests/unit/utils/test_logging_configuration.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_logging_configuration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_logging_configuration`/Test
symbols:
  TestLoggingConfiguration.teardown_method: LoggingConfiguration#teardown_method().
  TestLoggingConfiguration.test_custom_log_directory: LoggingConfiguration#test_custom_log_directory().
  TestSafeStreamHandler.test_safe_stream_handler_closed_stream: SafeStreamHandler#test_safe_stream_handler_closed_stream().
  TestSafeStreamHandler.test_safe_stream_handler_invalid_stream: SafeStreamHandler#test_safe_stream_handler_invalid_stream().
  TestSafeStreamHandler.test_safe_stream_handler_pytest_stream: SafeStreamHandler#test_safe_stream_handler_pytest_stream().
  TestLoggingConfiguration.original_env: LoggingConfiguration#original_env.
  TestLoggingConfiguration.test_default_behavior_no_file_logging: LoggingConfiguration#test_default_behavior_no_file_logging().
  TestLoggingConfiguration.test_enable_file_logging_true: LoggingConfiguration#test_enable_file_logging_true().
  TestLoggingConfiguration.test_custom_file_log_level: LoggingConfiguration#test_custom_file_log_level().
  TestLoggingConfiguration.test_system_temp_directory_fallback: LoggingConfiguration#test_system_temp_directory_fallback().
  TestLoggingConfiguration.test_file_logging_error_handling: LoggingConfiguration#test_file_logging_error_handling().
  TestLoggingConfiguration.test_log_level_environment_variable: LoggingConfiguration#test_log_level_environment_variable().
  TestLoggingConfiguration.test_log_level_string_conversion: LoggingConfiguration#test_log_level_string_conversion().
  TestLoggingConfiguration.test_file_log_level_string_conversion: LoggingConfiguration#test_file_log_level_string_conversion().
  TestLoggingConfiguration.test_logger_level_minimum_calculation: LoggingConfiguration#test_logger_level_minimum_calculation().
  TestLoggingConfiguration.test_test_logger_special_handling: LoggingConfiguration#test_test_logger_special_handling().
  TestLoggingConfiguration.test_file_logging_utf8_encoding: LoggingConfiguration#test_file_logging_utf8_encoding().
  TestLoggingConfiguration.test_concurrent_logger_setup: LoggingConfiguration#test_concurrent_logger_setup().
  TestLoggingConfiguration.test_stderr_error_handling: LoggingConfiguration#test_stderr_error_handling().
  TestSafeStreamHandler.test_safe_stream_handler_default_stream: SafeStreamHandler#test_safe_stream_handler_default_stream().
  TestSafeStreamHandler.test_safe_stream_handler_custom_stream: SafeStreamHandler#test_safe_stream_handler_custom_stream().
  TestLoggingConfiguration.temp_dir: LoggingConfiguration#temp_dir.
  TestLoggingConfiguration: LoggingConfiguration#
  TestLoggingConfiguration.setup_method: LoggingConfiguration#setup_method().
  TestSafeStreamHandler: SafeStreamHandler#
---
# Module: [`tests/unit/utils/test_logging_configuration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py)

## Classes
### `TestLoggingConfiguration`
- def: [`tests/unit/utils/test_logging_configuration.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L19)
- doc: Test logging configuration with environment variables.
- signature: `class TestLoggingConfiguration:`
- members:
  - `setup_method(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L22) — Set up test fixtures.
  - `teardown_method(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L39) — Clean up test fixtures.
  - `test_concurrent_logger_setup(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L290) — Test that concurrent logger setup doesn't create duplicate handlers.
  - `test_custom_file_log_level(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L129) — Test custom file log level with TREE_SITTER_ANALYZER_FILE_LOG_LEVEL.
  - `test_custom_log_directory(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L106) — Test custom log directory with TREE_SITTER_ANALYZER_LOG_DIR.
  - `test_default_behavior_no_file_logging(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L64) — Test default behavior with file logging disabled.
  - `test_enable_file_logging_true(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L80) — Test file logging when TREE_SITTER_ANALYZER_ENABLE_FILE_LOG=true.
  - `test_file_log_level_string_conversion(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L220) — Test file log level string conversion.
  - `test_file_logging_error_handling(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L168) — Test error handling when file logging setup fails.
  - `test_file_logging_utf8_encoding(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L275) — Test that file logging uses UTF-8 encoding.
  - `test_log_level_environment_variable(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L195) — Test LOG_LEVEL environment variable.
  - `test_log_level_string_conversion(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L204) — Test string to log level conversion.
  - `test_logger_level_minimum_calculation(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L250) — Test that logger level is set to minimum of main and file levels.
  - `test_stderr_error_handling(self, mock_stderr)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L308) — Test error handling when stderr operations fail.
  - `test_system_temp_directory_fallback(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L149) — Test fallback to system temporary directory.
  - `test_test_logger_special_handling(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L261) — Test special handling for test loggers.
  - `original_env` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L25)
  - `temp_dir` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L24)
- uses (calls/refs, reference-scoped): [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger)

### `TestSafeStreamHandler`
- def: [`tests/unit/utils/test_logging_configuration.py:326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L326)
- doc: Test SafeStreamHandler functionality.
- signature: `class TestSafeStreamHandler:`
- members:
  - `test_safe_stream_handler_closed_stream(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L344) — Test SafeStreamHandler handles closed streams safely.
  - `test_safe_stream_handler_custom_stream(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L336) — Test SafeStreamHandler with custom stream.
  - `test_safe_stream_handler_default_stream(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L329) — Test SafeStreamHandler uses stderr by default.
  - `test_safe_stream_handler_invalid_stream(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L368) — Test SafeStreamHandler handles invalid streams safely.
  - `test_safe_stream_handler_pytest_stream(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging_configuration.py#L391) — Test SafeStreamHandler handles pytest capture streams.
- uses (calls/refs, reference-scoped): [`SafeStreamHandler`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler), [`emit`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler.emit)

