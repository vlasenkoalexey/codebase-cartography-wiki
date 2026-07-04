---
title: 'Module: tree_sitter_analyzer/utils/_logging_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/_logging_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils._logging_helpers`/
symbols:
  write_stderr_safely: write_stderr_safely().
  cleanup_all_logging_handlers: cleanup_all_logging_handlers().
  add_file_handler: add_file_handler().
  resolve_configured_log_level: resolve_configured_log_level().
  should_skip_stream_emit: should_skip_stream_emit().
  configure_default_handlers: configure_default_handlers().
  coerce_log_level: coerce_log_level().
  is_stream_writable: is_stream_writable().
  resolve_file_log_level: resolve_file_log_level().
  close_handlers_for_shutdown: close_handlers_for_shutdown().
  _LOG_LEVELS: _LOG_LEVELS.
  STREAM_EMIT_ERRORS: STREAM_EMIT_ERRORS.
  file_logging_enabled: file_logging_enabled().
  clear_logger_handlers: clear_logger_handlers().
  resolve_final_logger_level: resolve_final_logger_level().
  apply_test_logger_settings: apply_test_logger_settings().
  create_log_formatter: create_log_formatter().
  is_pytest_capture_stream: is_pytest_capture_stream().
  resolve_log_path: resolve_log_path().
  iter_known_loggers: iter_known_loggers().
---
# Module: [`tree_sitter_analyzer/utils/_logging_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py)

## Functions
- `add_file_handler(logger: logging.Logger, formatter: logging.Formatter, level: int)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L104) — Attach optional file logging and return the configured file level.
- `apply_test_logger_settings(logger: logging.Logger, level: int)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L147) — Keep test loggers isolated from parent logger configuration.
- `cleanup_all_logging_handlers()` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L156) — Close and remove handlers from all known loggers during shutdown.
- `clear_logger_handlers(logger: logging.Logger)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L79) — Close and remove all handlers from a logger.
- `close_handlers_for_shutdown(logger: logging.Logger)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L172) — Close and remove each handler while reporting best-effort failures.
- `coerce_log_level(level: int | str)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L21) — Convert a user-facing log level into a logging module level.
- `configure_default_handlers(logger: logging.Logger, handler_factory: Callable[[], logging.Handler], level: int, enable_file_log: bool)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L87) — Attach default stream and optional file handlers, returning file level.
- `create_log_formatter()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L40) — Create the standard runtime log formatter.
- `file_logging_enabled()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L35) — Return whether optional file logging is enabled.
- `is_pytest_capture_stream(stream: object)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L65) — Detect pytest capture streams that should avoid pre-flush checks.
- `is_stream_writable(stream: object)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L71) — Best-effort writable check that treats stream errors as not writable.
- `iter_known_loggers()` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L165) — Return the root logger plus all named loggers.
- `resolve_configured_log_level(level: int | str)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L28) — Resolve the requested level, including LOG_LEVEL override.
- `resolve_file_log_level(level: int)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L132) — Resolve optional file handler level, falling back to main logger level.
- `resolve_final_logger_level(level: int, file_log_level: int, enable_file_log: bool)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L138) — Return the lowest level required by any configured handler.
- `resolve_log_path()` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L122) — Resolve the file logging destination path.
- `should_skip_stream_emit(stream: object)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L54) — Return whether a stream handler should skip emitting to this stream.
- `write_stderr_safely(message: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L45) — Best-effort write to stderr without disrupting runtime behavior.

## Module values
- `STREAM_EMIT_ERRORS` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L18)
- `_LOG_LEVELS` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_logging_helpers.py#L11)

