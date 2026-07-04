---
title: 'Module: tree_sitter_analyzer/_exceptions_mcp_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_mcp_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_mcp_response`/
symbols:
  _attach_exception_details: _attach_exception_details().
  create_mcp_error_response: create_mcp_error_response().
  mcp_exception_handler: mcp_exception_handler().
  mcp_exception_handler.decorator._handle_error: mcp_exception_handler().decorator()._handle_error().
  mcp_exception_handler.decorator: mcp_exception_handler().decorator().
  mcp_exception_handler.decorator.async_wrapper: mcp_exception_handler().decorator().async_wrapper().
  mcp_exception_handler.decorator.sync_wrapper: mcp_exception_handler().decorator().sync_wrapper().
  _attach_context: _attach_context().
---
# Module: [`tree_sitter_analyzer/_exceptions_mcp_response.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py)

## Functions
- `_attach_context(error: dict[str, Any], exception: Exception, sanitize_sensitive: bool)` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L92)
- `_attach_exception_details(error: dict[str, Any], exception: Exception)` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L101) — Attach type-specific details from known exception types to error dict.
- `_handle_error(e: Exception)` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L59)
- `async_wrapper(*args: Any, **kwargs: Any)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L73)
- `create_mcp_error_response(exception: Exception, tool_name: str | None = None, include_debug_info: bool = False, sanitize_sensitive: bool = True)` — [`L10`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L10) — Create standardized MCP error response dictionary.
- `decorator(func: Any)` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L58)
- `mcp_exception_handler(tool_name: str, include_debug: bool = False, sanitize_sensitive: bool = True)` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L44) — Decorator for MCP tool exception handling.
- `sync_wrapper(*args: Any, **kwargs: Any)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_response.py#L79)

