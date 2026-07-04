---
title: 'Module: tree_sitter_analyzer/utils/logging.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/logging.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils.logging`/
symbols:
  log_debug: log_debug().
  log_error: log_error().
  setup_logger: setup_logger().
  log_warning: log_warning().
  logger: logger.
  log_info: log_info().
  safe_print: safe_print().
  LoggingContext: LoggingContext#
  log_performance: log_performance().
  SafeStreamHandler: SafeStreamHandler#
  perf_logger: perf_logger.
  SafeStreamHandler.emit: SafeStreamHandler#emit().
  QuietMode: QuietMode#
  create_performance_logger: create_performance_logger().
  setup_performance_logger: setup_performance_logger().
  suppress_output: suppress_output().
  LoggingContext.__enter__: LoggingContext#__enter__().
  LoggingContext.target_logger: LoggingContext#target_logger.
  QuietMode.__enter__: QuietMode#__enter__().
  setup_safe_logging_shutdown: setup_safe_logging_shutdown().
  LoggingContext.enabled: LoggingContext#enabled.
  QuietMode.__exit__: QuietMode#__exit__().
  LoggingContext.__exit__: LoggingContext#__exit__().
  LoggingContext.old_level: LoggingContext#old_level.
  QuietMode.enabled: QuietMode#enabled.
  LoggingContext.level: LoggingContext#level.
  suppress_output.wrapper: suppress_output().wrapper().
  QuietMode.old_level: QuietMode#old_level.
  SafeStreamHandler.__init__: SafeStreamHandler#__init__().
  QuietMode.__init__: QuietMode#__init__().
  LoggingContext.__init__: LoggingContext#__init__().
---
# Module: [`tree_sitter_analyzer/utils/logging.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py)

## Classes
### `LoggingContext`
- def: [`tree_sitter_analyzer/utils/logging.py:276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L276)
- doc: Context manager for controlling logging behavior
- signature: `class LoggingContext:`
- members:
  - `enabled` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L280)
  - `level` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L281)
  - `old_level` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L282)
  - `target_logger` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L284)
- protocol/private: `__enter__`[`L286`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L286), `__exit__`[`L296`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L296), `__init__`[`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L279)
- used by: (22 test-only callers)

### `QuietMode`
- def: [`tree_sitter_analyzer/utils/logging.py:159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L159)
- doc: Context manager for quiet execution
- signature: `class QuietMode:`
- members:
  - `enabled` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L163)
  - `old_level` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L164)
- protocol/private: `__enter__`[`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L166), `__exit__`[`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L172), `__init__`[`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L162)
- uses (calls/refs, reference-scoped): [`logger`](logging.md#logger)
- used by: (12 test-only callers)

### `SafeStreamHandler`
- def: [`tree_sitter_analyzer/utils/logging.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L57)
- members:
  - `emit(self, record: Any)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L66) — Emit a record, safely handling closed streams and pytest capture
- protocol/private: `__init__`[`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L62)
- uses (calls/refs, reference-scoped): [`should_skip_stream_emit`](_logging_helpers.md#should_skip_stream_emit), [`STREAM_EMIT_ERRORS`](_logging_helpers.md#STREAM_EMIT_ERRORS)
- used by: [`setup_logger`](logging.md#setup_logger), [`create_performance_logger`](logging.md#create_performance_logger), [`setup_performance_logger`](logging.md#setup_performance_logger)  (21 test-only)

## Functions
- `create_performance_logger(name: str)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L199) — Create performance-focused logger.
- `log_debug(message: str, *args: Any, **kwargs: Any)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L123) — Log debug message — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `log_error(message: str, *args: Any, **kwargs: Any)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L115) — Log error message — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `log_info(message: str, *args: Any, **kwargs: Any)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L99) — Log info message
- `log_performance(operation: str, execution_time: float | None = None, details: dict[Any, Any] | str | None = None)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L240) — Log performance metrics
- `log_warning(message: str, *args: Any, **kwargs: Any)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L107) — Log warning message — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `safe_print(message: str | None, level: str = "info", quiet: bool = False)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L177) — Safe print function that can be controlled
- `setup_logger(name: str = "tree_sitter_analyzer", level: int | str = logging.WARNING)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L29) — Setup unified logger for the project — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `setup_performance_logger()` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L261) — Set up performance logging
- `setup_safe_logging_shutdown()` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L83) — Setup safe logging shutdown to prevent I/O errors
- `suppress_output(func: Any)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L131) — Decorator to suppress print statements in production
- `wrapper(*args: Any, **kwargs: Any)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L135)

## Module values
- `logger` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L96) — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `perf_logger` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/logging.py#L237)

