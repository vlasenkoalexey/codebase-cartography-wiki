---
title: 'Module: tests/unit/utils/test_utils.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_utils`/
symbols:
  get_log_output: get_log_output().
  test_logging_context_enable_disable: test_logging_context_enable_disable().
  test_logging_context_level_change: test_logging_context_level_change().
  test_logging_context_nesting: test_logging_context_nesting().
  test_logging_context_with_safe_print: test_logging_context_with_safe_print().
  LOGGING_CONTEXT_AVAILABLE: LOGGING_CONTEXT_AVAILABLE.
  test_log_info: test_log_info().
  test_log_warning: test_log_warning().
  test_log_error: test_log_error().
  test_log_debug: test_log_debug().
  test_logging_with_arguments: test_logging_with_arguments().
  test_logging_with_kwargs: test_logging_with_kwargs().
  test_log_performance: test_log_performance().
  test_log_performance_without_details: test_log_performance_without_details().
  test_safe_print_info: test_safe_print_info().
  test_safe_print_debug: test_safe_print_debug().
  test_safe_print_error: test_safe_print_error().
  test_safe_print_warning: test_safe_print_warning().
  test_safe_print_quiet_mode: test_safe_print_quiet_mode().
  test_safe_print_invalid_level: test_safe_print_invalid_level().
  test_performance_logger_setup: test_performance_logger_setup().
  test_logging_with_exception: test_logging_with_exception().
  test_logging_with_unicode: test_logging_with_unicode().
  test_safe_print_with_none: test_safe_print_with_none().
  test_all_logging_functions_work_together: test_all_logging_functions_work_together().
  test_performance_logging_integration: test_performance_logging_integration().
  test_logger: test_logger().
  perf_logger: perf_logger().
  test_testing_mode_detection: test_testing_mode_detection().
---
# Module: [`tests/unit/utils/test_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py)

## Functions
- `get_log_output(log_capture)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L111) — Get captured log output
- `perf_logger()` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L72) — Set up performance logger fixture
- `test_all_logging_functions_work_together(test_logger)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L375) — Test that all logging functions work together
- `test_log_debug(test_logger)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L142) — Test debug logging
- `test_log_error(test_logger)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L134) — Test error logging
- `test_log_info(test_logger)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L117) — Test info logging
- `test_log_performance(perf_logger)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L167) — Test performance logging
- `test_log_performance_without_details(perf_logger)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L178) — Test performance logging without details
- `test_log_warning(test_logger)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L126) — Test warning logging
- `test_logger()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L33) — Set up test logger fixture
- `test_logging_context_enable_disable()` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L247) — Test LoggingContext enable/disable functionality
- `test_logging_context_level_change()` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L261) — Test LoggingContext level change
- `test_logging_context_nesting()` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L286) — Test nested LoggingContext
- `test_logging_context_with_safe_print(test_logger)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L390) — Test LoggingContext works with safe_print
- `test_logging_with_arguments(test_logger)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L150) — Test logging with format arguments
- `test_logging_with_exception(test_logger)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L346) — Test logging with exception objects
- `test_logging_with_kwargs(test_logger)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L158) — Test logging with keyword arguments
- `test_logging_with_unicode(test_logger)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L358) — Test logging with unicode characters
- `test_performance_logger_setup()` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L325) — Test performance logger setup
- `test_performance_logging_integration()` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L402) — Test performance logging integration
- `test_safe_print_debug(test_logger)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L198) — Test safe_print with debug level
- `test_safe_print_error(test_logger)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L207) — Test safe_print with error level
- `test_safe_print_info(test_logger)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L189) — Test safe_print with info level
- `test_safe_print_invalid_level(test_logger)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L237) — Test safe_print with invalid level defaults to info
- `test_safe_print_quiet_mode(test_logger)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L225) — Test safe_print in quiet mode
- `test_safe_print_warning(test_logger)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L216) — Test safe_print with warning level
- `test_safe_print_with_none(test_logger)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L366) — Test safe_print with None message
- `test_testing_mode_detection()` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L319) — Test detection of testing mode

## Module values
- `LOGGING_CONTEXT_AVAILABLE` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils.py#L29)

