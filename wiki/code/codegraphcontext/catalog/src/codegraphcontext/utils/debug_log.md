---
title: 'Module: src/codegraphcontext/utils/debug_log.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/utils/debug_log.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.utils.debug_log`/
symbols:
  info_logger: info_logger().
  warning_logger: warning_logger().
  debug_log: debug_log().
  error_logger: error_logger().
  debug_logger: debug_logger().
  _should_log: _should_log().
  _get_config_value: _get_config_value().
  logger: logger.
  LOG_LEVELS: LOG_LEVELS.
---
# Module: [`src/codegraphcontext/utils/debug_log.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py)

## Functions
- `_get_config_value(key, default)` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L18) — Helper to get config value with fallback — documented in [codegraphcontext-tools-indexing-persistence-writer](../../../../concepts/codegraphcontext-tools-indexing-persistence-writer.md)
- `_should_log(level_name)` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L33) — Check if a message at the given level should be logged — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- `debug_log(message)` — [`L55`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L55) — Write debug message to a file if DEBUG_LOGS is enabled — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- `debug_logger(msg)` — [`L88`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L88) — Log debug message if log level allows
- `error_logger(msg)` — [`L78`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L78) — Log error message if log level allows — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- `info_logger(msg)` — [`L73`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L73) — Log info message if log level allows — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `warning_logger(msg)` — [`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L83) — Log warning message if log level allows — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)

## Module values
- `LOG_LEVELS` — [`L9`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L9) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
- `logger` — [`L6`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/debug_log.py#L6) — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)

