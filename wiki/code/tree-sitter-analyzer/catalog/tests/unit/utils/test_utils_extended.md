---
title: 'Module: tests/unit/utils/test_utils_extended.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_utils_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_utils_extended`/TestUtilsExtended#
symbols:
  TestUtilsExtended.test_logging_functions_with_kwargs: test_logging_functions_with_kwargs().
  TestUtilsExtended.test_logging_context_manager: test_logging_context_manager().
  TestUtilsExtended.test_logging_context_enable_disable: test_logging_context_enable_disable().
  TestUtilsExtended.test_all_logging_functions_work_together: test_all_logging_functions_work_together().
  TestUtilsExtended.test_logging_context_nesting: test_logging_context_nesting().
  TestUtilsExtended.test_logging_context_level_change: test_logging_context_level_change().
  TestUtilsExtended.test_logging_context_with_safe_print: test_logging_context_with_safe_print().
  TestUtilsExtended.test_logging_with_safe_print_integration: test_logging_with_safe_print_integration().
  TestUtilsExtended.log_file: log_file.
  TestUtilsExtended.teardown_method: teardown_method().
  TestUtilsExtended.test_setup_logger_with_custom_level: test_setup_logger_with_custom_level().
  TestUtilsExtended.test_setup_logger_with_custom_format: test_setup_logger_with_custom_format().
  TestUtilsExtended.test_setup_logger_with_file_handler: test_setup_logger_with_file_handler().
  TestUtilsExtended.test_log_performance_with_details: test_log_performance_with_details().
  TestUtilsExtended.test_log_performance_without_details: test_log_performance_without_details().
  TestUtilsExtended.test_safe_print_functions: test_safe_print_functions().
  TestUtilsExtended.test_safe_print_with_none_message: test_safe_print_with_none_message().
  TestUtilsExtended.test_safe_print_with_invalid_level: test_safe_print_with_invalid_level().
  TestUtilsExtended.test_safe_print_quiet_mode: test_safe_print_quiet_mode().
  TestUtilsExtended.test_get_performance_monitor: test_get_performance_monitor().
  TestUtilsExtended.test_logging_with_exception: test_logging_with_exception().
  TestUtilsExtended.test_logging_with_unicode: test_logging_with_unicode().
  TestUtilsExtended.test_performance_logger_setup: test_performance_logger_setup().
  TestUtilsExtended.test_performance_logging_integration: test_performance_logging_integration().
  TestUtilsExtended.test_edge_cases: test_edge_cases().
  TestUtilsExtended.test_error_handling: test_error_handling().
  TestUtilsExtended.temp_dir: temp_dir.
  TestUtilsExtended: ''
  TestUtilsExtended.setup_method: setup_method().
  TestUtilsExtended.test_is_testing_mode: test_is_testing_mode().
---
# Module: [`tests/unit/utils/test_utils_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py)

## Classes
### `TestUtilsExtended`
- def: [`tests/unit/utils/test_utils_extended.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L25)
- doc: Extended tests for utils module.
- signature: `class TestUtilsExtended:`
- members:
  - `setup_method(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L28) — Set up test fixtures.
  - `teardown_method(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L33) — Clean up test fixtures.
  - `test_all_logging_functions_work_together(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L270) — Test that all logging functions work together.
  - `test_edge_cases(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L296) — Test various edge cases.
  - `test_error_handling(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L311) — Test error handling in various scenarios.
  - `test_get_performance_monitor(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L153) — Test get_performance_monitor function.
  - `test_is_testing_mode(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L163) — Test is_testing_mode function.
  - `test_log_performance_with_details(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L84) — Test log_performance with details.
  - `test_log_performance_without_details(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L93) — Test log_performance without details.
  - `test_logging_context_enable_disable(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L235) — Test logging context enable/disable.
  - `test_logging_context_level_change(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L222) — Test logging context level change.
  - `test_logging_context_manager(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L190) — Test logging context manager.
  - `test_logging_context_nesting(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L204) — Test nested logging contexts.
  - `test_logging_context_with_safe_print(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L283) — Test logging context with safe print.
  - `test_logging_functions_with_kwargs(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L67) — Test logging functions with keyword arguments.
  - `test_logging_with_exception(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L172) — Test logging with exception.
  - `test_logging_with_safe_print_integration(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L259) — Test integration between logging and safe print.
  - `test_logging_with_unicode(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L182) — Test logging with unicode characters.
  - `test_performance_logger_setup(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L248) — Test performance logger setup.
  - `test_performance_logging_integration(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L254) — Test performance logging integration.
  - `test_safe_print_functions(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L100) — Test safe print functions.
  - `test_safe_print_quiet_mode(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L147) — Test safe print in quiet mode.
  - `test_safe_print_with_invalid_level(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L140) — Test safe print with invalid level.
  - `test_safe_print_with_none_message(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L118) — Test safe print functions with None message.
  - `test_setup_logger_with_custom_format(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L48) — Test setup_logger with custom format.
  - `test_setup_logger_with_custom_level(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L39) — Test setup_logger with custom log level.
  - `test_setup_logger_with_file_handler(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L57) — Test setup_logger with file handler.
  - `log_file` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L31)
  - `temp_dir` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_extended.py#L30)
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info), [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`create_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#create_performance_logger), [`target_logger`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.target_logger), [`enabled`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.enabled), [`old_level`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.old_level), [`level`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.level)

