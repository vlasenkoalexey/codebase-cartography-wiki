---
title: 'Module: tree_sitter_analyzer/_exceptions_execution.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_execution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_execution`/
symbols:
  handle_exception: handle_exception().
  handle_exceptions: handle_exceptions().
  safe_execute: safe_execute().
  safe_execute_async: safe_execute_async().
  create_error_response: create_error_response().
  _handle_decorated_exception: _handle_decorated_exception().
  handle_exceptions.decorator: handle_exceptions().decorator().
  handle_exceptions.decorator.wrapper: handle_exceptions().decorator().wrapper().
  _log_decorated_exception: _log_decorated_exception().
  _raise_as: _raise_as().
---
# Module: [`tree_sitter_analyzer/_exceptions_execution.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py)

## Functions
- `_handle_decorated_exception(exception: Exception, func_name: str, default_return: Any, reraise_as: type[Exception] | None, log_errors: bool)` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L131)
- `_log_decorated_exception(func_name: str, exception: Exception)` — [`L145`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L145)
- `_raise_as(reraise_as: type[Exception], exception: Exception)` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L151)
- `create_error_response(exception: Exception, include_traceback: bool = False)` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L69) — Create standardized error response dictionary.
- `decorator(func: Any)` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L117)
- `handle_exception(exception: Exception, context: dict[str, Any] | None = None, reraise_as: type[Exception] | None = None)` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L8) — Handle exceptions with optional context and re-raising.
- `handle_exceptions(default_return: Any = None, exception_types: tuple[type[Exception], ...] = (Exception,), reraise_as: type[Exception] | None = None, log_errors: bool = True)` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L101) — Decorator for automatic exception handling.
- `safe_execute(func: Any, *args: Any, default_return: Any = None, exception_types: tuple[type[Exception], ...] = (Exception,), log_errors: bool = True, **kwargs: Any)` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L37) — Safely execute a function with exception handling.
- `safe_execute_async(coro: Any, default_return: Any = None, exception_types: tuple[type[Exception], ...] = (Exception,), log_errors: bool = True, tool_name: str | None = None)` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L155) — Safely execute an async function with exception handling.
- `wrapper(*args: Any, **kwargs: Any)` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_execution.py#L118)

