---
title: 'Module: tree_sitter_analyzer/mcp/utils/error_handler.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/error_handler.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.error_handler`/
symbols:
  AnalysisError: AnalysisError#
  ErrorHandler.handle_error: ErrorHandler#handle_error().
  ErrorCategory: ErrorCategory#
  ErrorHandler: ErrorHandler#
  ErrorSeverity: ErrorSeverity#
  MCPError: MCPError#
  handle_mcp_errors: handle_mcp_errors().
  ErrorHandler._classify_error: ErrorHandler#_classify_error().
  _handle_runtime_error: _handle_runtime_error().
  ErrorHandler.error_history: ErrorHandler#error_history.
  ErrorHandler.error_counts: ErrorHandler#error_counts.
  get_error_handler: get_error_handler().
  MCPError.to_dict: MCPError#to_dict().
  _handle_and_rethrow_as_analysis_error: _handle_and_rethrow_as_analysis_error().
  MCPError.__init__: MCPError#__init__().
  ErrorHandler.register_recovery_strategy: ErrorHandler#register_recovery_strategy().
  ErrorSeverity.MEDIUM: ErrorSeverity#MEDIUM.
  ErrorHandler.clear_history: ErrorHandler#clear_history().
  ErrorHandler.recovery_strategies: ErrorHandler#recovery_strategies.
  ErrorHandler.get_error_stats: ErrorHandler#get_error_stats().
  ErrorHandler._register_default_strategies: ErrorHandler#_register_default_strategies().
  MCPError.category: MCPError#category.
  MCPError.details: MCPError#details.
  ErrorSeverity.HIGH: ErrorSeverity#HIGH.
  ErrorCategory.VALIDATION: ErrorCategory#VALIDATION.
  logger: logger.
  ErrorSeverity.LOW: ErrorSeverity#LOW.
  MCPError.message: MCPError#message.
  FileAccessError.__init__: FileAccessError#__init__().
  ParsingError.__init__: ParsingError#__init__().
  AnalysisError.__init__: AnalysisError#__init__().
  ValidationError.__init__: ValidationError#__init__().
  ResourceError.__init__: ResourceError#__init__().
  MCPError.severity: MCPError#severity.
  ErrorSeverity.CRITICAL: ErrorSeverity#CRITICAL.
  ErrorCategory.FILE_ACCESS: ErrorCategory#FILE_ACCESS.
  ErrorCategory.ANALYSIS: ErrorCategory#ANALYSIS.
  FileAccessError: FileAccessError#
  ParsingError: ParsingError#
  ValidationError: ValidationError#
  ErrorCategory.PARSING: ErrorCategory#PARSING.
  ErrorCategory.CONFIGURATION: ErrorCategory#CONFIGURATION.
  ErrorCategory.UNKNOWN: ErrorCategory#UNKNOWN.
  ErrorHandler._add_to_history: ErrorHandler#_add_to_history().
  ErrorHandler._attempt_recovery: ErrorHandler#_attempt_recovery().
  _make_async_handler.wrapper: _make_async_handler().wrapper().
  handle_mcp_errors.decorator: handle_mcp_errors().decorator().
  ResourceError: ResourceError#
  ErrorHandler.get_recent_errors: ErrorHandler#get_recent_errors().
  ErrorCategory.RESOURCE: ErrorCategory#RESOURCE.
  MCPError.recoverable: MCPError#recoverable.
  ErrorHandler.max_history_size: ErrorHandler#max_history_size.
  ErrorHandler._log_error: ErrorHandler#_log_error().
  ErrorHandler._update_error_stats: ErrorHandler#_update_error_stats().
  ErrorHandler._try_strategy: ErrorHandler#_try_strategy().
  ErrorHandler._count_recent_errors: ErrorHandler#_count_recent_errors().
  _make_async_handler: _make_async_handler().
  _make_sync_handler: _make_sync_handler().
  _make_sync_handler.wrapper: _make_sync_handler().wrapper().
  _error_handler: _error_handler.
  ErrorCategory.NETWORK: ErrorCategory#NETWORK.
  MCPError.timestamp: MCPError#timestamp.
  _build_error_context: _build_error_context().
  _recovery_file_not_found: _recovery_file_not_found().
  _recovery_permission: _recovery_permission().
  _recovery_value_error: _recovery_value_error().
  ErrorHandler.__init__: ErrorHandler#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/utils/error_handler.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py)

## Classes
### `AnalysisError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L106) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- doc: Error related to code analysis operations
- signature: `class AnalysisError(MCPError):`
- protocol/private: `__init__`[`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L109)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`MCPError`](error_handler.md#MCPError), [`__init__`](error_handler.md#MCPError.__init__), [`ANALYSIS`](error_handler.md#ErrorCategory.ANALYSIS)
- used by: [`execute`](../tools/query_tool.md#QueryTool.execute), [`MCPError`](error_handler.md#MCPError), [`_handle_and_rethrow_as_analysis_error`](error_handler.md#_handle_and_rethrow_as_analysis_error), [`_analysis_error`](../tools/query_tool.md#_analysis_error)  (47 test-only)

### `ErrorCategory`  ·  implements/extends Enum
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L31) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- doc: Error categories for classification
- signature: `class ErrorCategory(Enum):`
- members:
  - `ANALYSIS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L36)
  - `CONFIGURATION` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L40)
  - `FILE_ACCESS` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L34)
  - `NETWORK` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L37)
  - `PARSING` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L35)
  - `RESOURCE` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L39)
  - `UNKNOWN` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L41)
  - `VALIDATION` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L38)
- used by: [`_classify_error`](error_handler.md#ErrorHandler._classify_error), [`_handle_runtime_error`](error_handler.md#_handle_runtime_error), [`__init__`](error_handler.md#MCPError.__init__), [`__init__`](error_handler.md#AnalysisError.__init__), [`__init__`](error_handler.md#FileAccessError.__init__), [`__init__`](error_handler.md#ParsingError.__init__), [`__init__`](error_handler.md#ResourceError.__init__), [`__init__`](error_handler.md#ValidationError.__init__)  (19 test-only)

### `ErrorHandler`
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L180) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- doc: Centralized error handling and recovery system
- signature: `class ErrorHandler:`
- members:
  - `__init__(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L188) — Initialize error handler
  - `_add_to_history(self, error_info: dict[str, Any], context: dict[str, Any], operation: str)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L332) — Add error to history with size limit.
  - `_attempt_recovery(self, error: Exception, context: dict[str, Any])` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L356) — Attempt recovery using registered strategies.
  - `_classify_error(self, error: Exception, context: dict[str, Any], operation: str)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L250) — Classify a generic exception into MCP error categories. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `_count_recent_errors(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L375) — Count errors from the past hour.
  - `_log_error(self, error: Exception, error_info: dict[str, Any], context: dict[str, Any], operation: str)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L300) — Log error with appropriate level based on severity.
  - `_register_default_strategies(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L200) — Register default error recovery strategies.
  - `_try_strategy(self, strategy: Callable, error: Exception, context: dict[str, Any])` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L342) — Attempt one recovery strategy; return result or None on failure.
  - `_update_error_stats(self, error_info: dict[str, Any])` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L320) — Update error statistics.
  - `clear_history(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L401) — Clear error history and reset statistics
  - `get_error_stats(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L386) — Get error statistics.
  - `get_recent_errors(self, limit: int = 10)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L397) — Get recent errors from history.
  - `handle_error(self, error: Exception, context: dict[str, Any] | None = None, operation: str = "unknown")` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L219) — Handle an error with classification, logging, and recovery. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `register_recovery_strategy(self, exception_type: type[Exception], strategy: Callable)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L210) — Register a custom recovery strategy for an exception type.
  - `error_counts` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L190) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `error_history` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L191) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `max_history_size` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L192)
  - `recovery_strategies` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L193) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`ErrorSeverity`](error_handler.md#ErrorSeverity), [`MCPError`](error_handler.md#MCPError), [`to_dict`](error_handler.md#MCPError.to_dict), [`MEDIUM`](error_handler.md#ErrorSeverity.MEDIUM), [`HIGH`](error_handler.md#ErrorSeverity.HIGH), [`VALIDATION`](error_handler.md#ErrorCategory.VALIDATION), [`LOW`](error_handler.md#ErrorSeverity.LOW), [`logger`](error_handler.md#logger), [`ANALYSIS`](error_handler.md#ErrorCategory.ANALYSIS), [`CRITICAL`](error_handler.md#ErrorSeverity.CRITICAL), [`FILE_ACCESS`](error_handler.md#ErrorCategory.FILE_ACCESS), [`UNKNOWN`](error_handler.md#ErrorCategory.UNKNOWN), [`RESOURCE`](error_handler.md#ErrorCategory.RESOURCE), [`NETWORK`](error_handler.md#ErrorCategory.NETWORK), [`_recovery_file_not_found`](error_handler.md#_recovery_file_not_found), [`_recovery_permission`](error_handler.md#_recovery_permission), [`_recovery_value_error`](error_handler.md#_recovery_value_error)
- used by: [`_handle_runtime_error`](error_handler.md#_handle_runtime_error), [`get_error_handler`](error_handler.md#get_error_handler), [`_handle_and_rethrow_as_analysis_error`](error_handler.md#_handle_and_rethrow_as_analysis_error), [`_error_handler`](error_handler.md#_error_handler)  (44 test-only)

### `ErrorSeverity`  ·  implements/extends Enum
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L22) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- doc: Error severity levels
- signature: `class ErrorSeverity(Enum):`
- members:
  - `CRITICAL` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L28)
  - `HIGH` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L27)
  - `LOW` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L25)
  - `MEDIUM` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L26) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- used by: [`_classify_error`](error_handler.md#ErrorHandler._classify_error), [`_handle_runtime_error`](error_handler.md#_handle_runtime_error), [`_handle_and_rethrow_as_analysis_error`](error_handler.md#_handle_and_rethrow_as_analysis_error), [`__init__`](error_handler.md#MCPError.__init__)  (14 test-only)

### `FileAccessError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L76)
- doc: Error related to file access operations
- signature: `class FileAccessError(MCPError):`
- protocol/private: `__init__`[`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L79)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`MCPError`](error_handler.md#MCPError), [`__init__`](error_handler.md#MCPError.__init__), [`FILE_ACCESS`](error_handler.md#ErrorCategory.FILE_ACCESS)
- used by: [`MCPError`](error_handler.md#MCPError)  (2 test-only)

### `MCPError`  ·  implements/extends Exception
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L44) — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- doc: Base exception class for MCP-specific errors
- signature: `class MCPError(Exception):`
- members:
  - `to_dict(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L63) — Convert error to dictionary representation
  - `category` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L57)
  - `details` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L59)
  - `message` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L56)
  - `recoverable` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L60)
  - `severity` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L58)
  - `timestamp` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L61)
- protocol/private: `__init__`[`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L47)
- uses (calls/refs, reference-scoped): [`AnalysisError`](error_handler.md#AnalysisError), [`ErrorCategory`](error_handler.md#ErrorCategory), [`ErrorSeverity`](error_handler.md#ErrorSeverity), [`MEDIUM`](error_handler.md#ErrorSeverity.MEDIUM), [`FileAccessError`](error_handler.md#FileAccessError), [`ParsingError`](error_handler.md#ParsingError), [`ValidationError`](error_handler.md#ValidationError), [`UNKNOWN`](error_handler.md#ErrorCategory.UNKNOWN), [`ResourceError`](error_handler.md#ResourceError)
- used by: [`AnalysisError`](error_handler.md#AnalysisError), [`handle_error`](error_handler.md#ErrorHandler.handle_error), [`_handle_runtime_error`](error_handler.md#_handle_runtime_error), [`_handle_and_rethrow_as_analysis_error`](error_handler.md#_handle_and_rethrow_as_analysis_error), [`analyze_code_scale`](../server_utils/code_scale_handler.md#analyze_code_scale), [`__init__`](error_handler.md#AnalysisError.__init__), [`__init__`](error_handler.md#FileAccessError.__init__), [`__init__`](error_handler.md#ParsingError.__init__), [`__init__`](error_handler.md#ResourceError.__init__), [`__init__`](error_handler.md#ValidationError.__init__), [`FileAccessError`](error_handler.md#FileAccessError), [`ParsingError`](error_handler.md#ParsingError), [`ValidationError`](error_handler.md#ValidationError), [`ResourceError`](error_handler.md#ResourceError)  (25 test-only)

### `ParsingError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L88)
- doc: Error related to code parsing operations
- signature: `class ParsingError(MCPError):`
- protocol/private: `__init__`[`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L91)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`MCPError`](error_handler.md#MCPError), [`__init__`](error_handler.md#MCPError.__init__), [`PARSING`](error_handler.md#ErrorCategory.PARSING)
- used by: [`MCPError`](error_handler.md#MCPError)  (2 test-only)

### `ResourceError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L131)
- doc: Error related to resource operations
- signature: `class ResourceError(MCPError):`
- protocol/private: `__init__`[`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L134)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`MCPError`](error_handler.md#MCPError), [`__init__`](error_handler.md#MCPError.__init__), [`RESOURCE`](error_handler.md#ErrorCategory.RESOURCE)
- used by: [`MCPError`](error_handler.md#MCPError)  (1 test-only)

### `ValidationError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/mcp/utils/error_handler.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L118)
- doc: Error related to input validation
- signature: `class ValidationError(MCPError):`
- protocol/private: `__init__`[`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L121)
- uses (calls/refs, reference-scoped): [`ErrorCategory`](error_handler.md#ErrorCategory), [`MCPError`](error_handler.md#MCPError), [`__init__`](error_handler.md#MCPError.__init__), [`VALIDATION`](error_handler.md#ErrorCategory.VALIDATION)
- used by: [`MCPError`](error_handler.md#MCPError)  (2 test-only)

## Functions
- `_build_error_context(func: Callable[..., Any], args: tuple, kwargs: dict)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L408) — Build the standard error-context dict used by both wrappers.
- `_handle_and_rethrow_as_analysis_error(e: Exception, func: Callable[..., Any], args: tuple, kwargs: dict, operation: str)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L447) — Log the error then wrap non-MCPError exceptions as ``AnalysisError``. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- `_handle_runtime_error(e: RuntimeError, func: Callable[..., Any], args: tuple, kwargs: dict, operation: str)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L419) — Handle ``RuntimeError`` in async wrapper. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- `_make_async_handler(func: Callable, operation: str)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L467) — Build an async error-catching wrapper around func.
- `_make_sync_handler(func: Callable, operation: str)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L483) — Build a sync error-catching wrapper around func.
- `_recovery_file_not_found(error: FileNotFoundError, context: dict[str, Any])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L147) — Recovery for file-not-found errors.
- `_recovery_permission(error: PermissionError, context: dict[str, Any])` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L159) — Recovery for permission errors.
- `_recovery_value_error(error: ValueError, context: dict[str, Any])` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L171) — Recovery for value errors.
- `decorator(func: Callable[..., Any])` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L501)
- `get_error_handler()` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L513) — Get the global error handler instance. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
- `handle_mcp_errors(operation: str = "unknown")` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L496) — Decorator for automatic error handling in MCP operations.
- `wrapper(*args: Any, **kwargs: Any)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L470)
- `wrapper(*args: Any, **kwargs: Any)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L486)

## Module values
- `_error_handler` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L510)
- `logger` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_handler.py#L19)

