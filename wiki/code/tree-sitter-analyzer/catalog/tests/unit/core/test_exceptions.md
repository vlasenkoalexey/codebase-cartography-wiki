---
title: 'Module: tests/unit/core/test_exceptions.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_exceptions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_exceptions`/Test
symbols:
  TestExceptionInheritance.test_all_exceptions_inherit_from_base: ExceptionInheritance#test_all_exceptions_inherit_from_base().
  TestExceptionInheritance.test_mcp_exceptions_inheritance: ExceptionInheritance#test_mcp_exceptions_inheritance().
  TestBaseException.test_base_exception_initialization: BaseException#test_base_exception_initialization().
  TestSecurityExceptions.test_path_traversal_error: SecurityExceptions#test_path_traversal_error().
  TestSecurityExceptions.test_regex_security_error: SecurityExceptions#test_regex_security_error().
  TestSecurityExceptions.test_file_restriction_error: SecurityExceptions#test_file_restriction_error().
  TestMCPExceptions.test_mcp_tool_error: MCPExceptions#test_mcp_tool_error().
  TestMCPExceptions.test_mcp_resource_error: MCPExceptions#test_mcp_resource_error().
  TestMCPExceptions.test_mcp_validation_error: MCPExceptions#test_mcp_validation_error().
  TestMCPErrorResponse.test_create_mcp_error_response_specific_types: MCPErrorResponse#test_create_mcp_error_response_specific_types().
  TestExceptionInheritance.test_security_exceptions_inheritance: ExceptionInheritance#test_security_exceptions_inheritance().
  TestAnalysisError.test_analysis_error_basic: AnalysisError#test_analysis_error_basic().
  TestLanguageNotSupportedError.test_language_not_supported_basic: LanguageNotSupportedError#test_language_not_supported_basic().
  TestLanguageNotSupportedError.test_language_not_supported_with_list: LanguageNotSupportedError#test_language_not_supported_with_list().
  TestSecurityExceptions.test_security_error_with_type: SecurityExceptions#test_security_error_with_type().
  TestMCPExceptions.test_mcp_timeout_error: MCPExceptions#test_mcp_timeout_error().
  TestExceptionHandlingUtilities.failing_function: ExceptionHandlingUtilities#failing_function().
  TestBaseException.test_base_exception_with_error_code: BaseException#test_base_exception_with_error_code().
  TestBaseException.test_base_exception_with_context: BaseException#test_base_exception_with_context().
  TestBaseException.test_base_exception_to_dict: BaseException#test_base_exception_to_dict().
  TestAnalysisError.test_analysis_error_with_file_path: AnalysisError#test_analysis_error_with_file_path().
  TestAnalysisError.test_analysis_error_with_path_object: AnalysisError#test_analysis_error_with_path_object().
  TestAnalysisError.test_analysis_error_with_language: AnalysisError#test_analysis_error_with_language().
  TestAnalysisError.test_analysis_error_with_all_params: AnalysisError#test_analysis_error_with_all_params().
  TestParseError.test_parse_error_basic: ParseError#test_parse_error_basic().
  TestParseError.test_parse_error_with_language: ParseError#test_parse_error_with_language().
  TestParseError.test_parse_error_with_source_info: ParseError#test_parse_error_with_source_info().
  TestPluginError.test_plugin_error_basic: PluginError#test_plugin_error_basic().
  TestPluginError.test_plugin_error_with_plugin_name: PluginError#test_plugin_error_with_plugin_name().
  TestPluginError.test_plugin_error_with_operation: PluginError#test_plugin_error_with_operation().
  TestQueryError.test_query_error_basic: QueryError#test_query_error_basic().
  TestQueryError.test_query_error_with_all_params: QueryError#test_query_error_with_all_params().
  TestFileHandlingError.test_file_handling_error_basic: FileHandlingError#test_file_handling_error_basic().
  TestFileHandlingError.test_file_handling_error_with_path: FileHandlingError#test_file_handling_error_with_path().
  TestFileHandlingError.test_file_handling_error_with_operation: FileHandlingError#test_file_handling_error_with_operation().
  TestConfigurationError.test_configuration_error_basic: ConfigurationError#test_configuration_error_basic().
  TestConfigurationError.test_configuration_error_with_key_value: ConfigurationError#test_configuration_error_with_key_value().
  TestValidationError.test_validation_error_basic: ValidationError#test_validation_error_basic().
  TestValidationError.test_validation_error_with_type_and_value: ValidationError#test_validation_error_with_type_and_value().
  TestSecurityExceptions.test_security_error_basic: SecurityExceptions#test_security_error_basic().
  TestMCPExceptions.test_mcp_error_basic: MCPExceptions#test_mcp_error_basic().
  TestMCPExceptions.test_mcp_error_with_tool_name: MCPExceptions#test_mcp_error_with_tool_name().
  TestMCPExceptions.test_mcp_tool_error_sanitizes_sensitive_params: MCPExceptions#test_mcp_tool_error_sanitizes_sensitive_params().
  TestMCPExceptions.test_mcp_tool_error_truncates_long_values: MCPExceptions#test_mcp_tool_error_truncates_long_values().
  TestMCPExceptions.test_mcp_validation_error_truncates_long_values: MCPExceptions#test_mcp_validation_error_truncates_long_values().
  TestExceptionHandlingUtilities.test_create_error_response_basic: ExceptionHandlingUtilities#test_create_error_response_basic().
  TestExceptionHandlingUtilities.test_create_error_response_with_context: ExceptionHandlingUtilities#test_create_error_response_with_context().
  TestExceptionHandlingUtilities.test_create_error_response_with_traceback: ExceptionHandlingUtilities#test_create_error_response_with_traceback().
  TestExceptionHandlingUtilities.test_safe_execute_success: ExceptionHandlingUtilities#test_safe_execute_success().
  TestExceptionHandlingUtilities.test_safe_execute_with_exception: ExceptionHandlingUtilities#test_safe_execute_with_exception().
  TestExceptionHandlingUtilities.test_safe_execute_with_specific_exception_types: ExceptionHandlingUtilities#test_safe_execute_with_specific_exception_types().
  TestExceptionHandlingUtilities.test_handle_exceptions_decorator_reraise: ExceptionHandlingUtilities#test_handle_exceptions_decorator_reraise().
  TestMCPErrorResponse.test_create_mcp_error_response_basic: MCPErrorResponse#test_create_mcp_error_response_basic().
  TestMCPErrorResponse.test_create_mcp_error_response_with_tool_name: MCPErrorResponse#test_create_mcp_error_response_with_tool_name().
  TestMCPErrorResponse.test_create_mcp_error_response_sanitizes_sensitive_data: MCPErrorResponse#test_create_mcp_error_response_sanitizes_sensitive_data().
  TestMCPErrorResponse.test_create_mcp_error_response_with_debug_info: MCPErrorResponse#test_create_mcp_error_response_with_debug_info().
  TestAsyncExceptionHandling.test_safe_execute_async_success: AsyncExceptionHandling#test_safe_execute_async_success().
  TestAsyncExceptionHandling.test_safe_execute_async_with_exception: AsyncExceptionHandling#test_safe_execute_async_with_exception().
  TestHandleException.test_handle_exception_logs_and_reraises: HandleException#test_handle_exception_logs_and_reraises().
  TestHandleException.test_handle_exception_with_context: HandleException#test_handle_exception_with_context().
  TestHandleException.test_handle_exception_reraise_as_different_type: HandleException#test_handle_exception_reraise_as_different_type().
  TestHandleException.test_handle_exception_with_exception_context: HandleException#test_handle_exception_with_exception_context().
  TestHandleException.test_safe_execute_async_with_logging: HandleException#test_safe_execute_async_with_logging().
  TestHandleException.failing_func: HandleException#failing_func().
  TestAsyncExceptionHandling.failing_async_tool: AsyncExceptionHandling#failing_async_tool().
  TestAsyncExceptionHandling.failing_sync_tool: AsyncExceptionHandling#failing_sync_tool().
  TestExceptionHandlingUtilities.failing_func: ExceptionHandlingUtilities#failing_func().
  TestBaseException.test_base_exception_str_representation: BaseException#test_base_exception_str_representation().
  TestExceptionHandlingUtilities.test_handle_exceptions_decorator: ExceptionHandlingUtilities#test_handle_exceptions_decorator().
  TestAsyncExceptionHandling.test_mcp_exception_handler_decorator_async: AsyncExceptionHandling#test_mcp_exception_handler_decorator_async().
  TestAsyncExceptionHandling.test_mcp_exception_handler_decorator_sync: AsyncExceptionHandling#test_mcp_exception_handler_decorator_sync().
  TestSanitizeErrorContext.test_sanitize_long_string_value: SanitizeErrorContext#test_sanitize_long_string_value().
  TestSanitizeErrorContext.test_sanitize_long_list_value: SanitizeErrorContext#test_sanitize_long_list_value().
  TestSanitizeErrorContext.test_sanitize_long_tuple_value: SanitizeErrorContext#test_sanitize_long_tuple_value().
  TestSanitizeErrorContext.test_sanitize_large_nested_dict: SanitizeErrorContext#test_sanitize_large_nested_dict().
  TestSanitizeErrorContext.test_sanitize_sensitive_keys: SanitizeErrorContext#test_sanitize_sensitive_keys().
  TestSanitizeErrorContext.test_sanitize_normal_values_unchanged: SanitizeErrorContext#test_sanitize_normal_values_unchanged().
  TestSanitizeErrorContext.test_sanitize_empty_context: SanitizeErrorContext#test_sanitize_empty_context().
  TestSanitizeErrorContext.test_sanitize_mixed_context: SanitizeErrorContext#test_sanitize_mixed_context().
  TestHandleException.test_handle_exception_reraise_non_tree_sitter_error: HandleException#test_handle_exception_reraise_non_tree_sitter_error().
  TestHandleException.test_handle_exceptions_decorator_with_logging: HandleException#test_handle_exceptions_decorator_with_logging().
  TestHandleException.test_handle_exceptions_reraise_with_logging: HandleException#test_handle_exceptions_reraise_with_logging().
  TestExceptionHandlingUtilities.success_func: ExceptionHandlingUtilities#success_func().
  TestAsyncExceptionHandling.success_coro: AsyncExceptionHandling#success_coro().
  TestAsyncExceptionHandling.failing_coro: AsyncExceptionHandling#failing_coro().
  TestHandleException.failing_async: HandleException#failing_async().
  TestBaseException: BaseException#
  TestAnalysisError: AnalysisError#
  TestParseError: ParseError#
  TestLanguageNotSupportedError: LanguageNotSupportedError#
  TestPluginError: PluginError#
  TestQueryError: QueryError#
  TestFileHandlingError: FileHandlingError#
  TestConfigurationError: ConfigurationError#
  TestValidationError: ValidationError#
  TestSecurityExceptions: SecurityExceptions#
  TestMCPExceptions: MCPExceptions#
  TestExceptionHandlingUtilities: ExceptionHandlingUtilities#
  TestMCPErrorResponse: MCPErrorResponse#
  TestAsyncExceptionHandling: AsyncExceptionHandling#
  TestExceptionInheritance: ExceptionInheritance#
  TestSanitizeErrorContext: SanitizeErrorContext#
  TestHandleException: HandleException#
---
# Module: [`tests/unit/core/test_exceptions.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py)

## Classes
### `TestAnalysisError`
- def: [`tests/unit/core/test_exceptions.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L79)
- doc: Test AnalysisError exception.
- signature: `class TestAnalysisError:`
- members:
  - `test_analysis_error_basic(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L82) — Test AnalysisError with basic message.
  - `test_analysis_error_with_all_params(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L104) — Test AnalysisError with all parameters.
  - `test_analysis_error_with_file_path(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L88) — Test AnalysisError with file path.
  - `test_analysis_error_with_language(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L99) — Test AnalysisError with language parameter.
  - `test_analysis_error_with_path_object(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L93) — Test AnalysisError with Path object.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message)

### `TestAsyncExceptionHandling`
- def: [`tests/unit/core/test_exceptions.py:528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L528)
- doc: Test async exception handling utilities.
- signature: `class TestAsyncExceptionHandling:`
- members:
  - `failing_async_tool()` — [`L558`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L558)
  - `failing_coro()` — [`L545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L545)
  - `failing_sync_tool()` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L571)
  - `success_coro()` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L535)
  - `test_mcp_exception_handler_decorator_async(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L554) — Test mcp_exception_handler decorator with async function.
  - `test_mcp_exception_handler_decorator_sync(self)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L567) — Test mcp_exception_handler decorator with sync function.
  - `test_safe_execute_async_success(self)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L532) — Test safe_execute_async with successful execution.
  - `test_safe_execute_async_with_exception(self)` — [`L542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L542) — Test safe_execute_async returns default on exception.
- uses (calls/refs, reference-scoped): [`mcp_exception_handler`](../../../tree_sitter_analyzer/_exceptions_mcp_response.md#mcp_exception_handler), [`safe_execute_async`](../../../tree_sitter_analyzer/_exceptions_execution.md#safe_execute_async)

### `TestBaseException`
- def: [`tests/unit/core/test_exceptions.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L40)
- doc: Test TreeSitterAnalyzerError base exception.
- signature: `class TestBaseException:`
- members:
  - `test_base_exception_initialization(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L43) — Test base exception can be initialized with message only.
  - `test_base_exception_str_representation(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L73) — Test exception string representation.
  - `test_base_exception_to_dict(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L61) — Test exception conversion to dictionary.
  - `test_base_exception_with_context(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L55) — Test base exception with context dictionary.
  - `test_base_exception_with_error_code(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L50) — Test base exception with custom error code.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`to_dict`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`error_code`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.error_code)

### `TestConfigurationError`
- def: [`tests/unit/core/test_exceptions.py:210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L210)
- doc: Test ConfigurationError exception.
- signature: `class TestConfigurationError:`
- members:
  - `test_configuration_error_basic(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L213) — Test ConfigurationError with basic message.
  - `test_configuration_error_with_key_value(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L218) — Test ConfigurationError with config key and value.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`ConfigurationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ConfigurationError)

### `TestExceptionHandlingUtilities`
- def: [`tests/unit/core/test_exceptions.py:383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L383)
- doc: Test exception handling utility functions.
- signature: `class TestExceptionHandlingUtilities:`
- members:
  - `failing_func()` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L421)
  - `failing_function()` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L449)
  - `success_func()` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L412)
  - `test_create_error_response_basic(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L386) — Test create_error_response with basic exception.
  - `test_create_error_response_with_context(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L395) — Test create_error_response includes context.
  - `test_create_error_response_with_traceback(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L402) — Test create_error_response with traceback.
  - `test_handle_exceptions_decorator(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L445) — Test handle_exceptions decorator.
  - `test_handle_exceptions_decorator_reraise(self)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L455) — Test handle_exceptions decorator with reraise_as.
  - `test_safe_execute_success(self)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L409) — Test safe_execute with successful execution.
  - `test_safe_execute_with_exception(self)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L418) — Test safe_execute returns default on exception.
  - `test_safe_execute_with_specific_exception_types(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L427) — Test safe_execute catches specific exception types.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`handle_exceptions`](../../../tree_sitter_analyzer/_exceptions_execution.md#handle_exceptions), [`safe_execute`](../../../tree_sitter_analyzer/_exceptions_execution.md#safe_execute), [`create_error_response`](../../../tree_sitter_analyzer/_exceptions_execution.md#create_error_response)

### `TestExceptionInheritance`
- def: [`tests/unit/core/test_exceptions.py:581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L581)
- doc: Test exception inheritance chain.
- signature: `class TestExceptionInheritance:`
- members:
  - `test_all_exceptions_inherit_from_base(self)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L584) — Test that all custom exceptions inherit from TreeSitterAnalyzerError.
  - `test_mcp_exceptions_inheritance(self)` — [`L615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L615) — Test MCP exception inheritance chain.
  - `test_security_exceptions_inheritance(self)` — [`L609`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L609) — Test security exception inheritance chain.
- uses (calls/refs, reference-scoped): [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`TreeSitterAnalyzerError`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`MCPError`](../../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`ValidationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`MCPToolError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError), [`MCPValidationError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError), [`MCPResourceError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError), [`QueryError`](../../../tree_sitter_analyzer/_exceptions_core.md#QueryError), [`MCPTimeoutError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError), [`FileHandlingError`](../../../tree_sitter_analyzer/_exceptions_core.md#FileHandlingError), [`ParseError`](../../../tree_sitter_analyzer/_exceptions_core.md#ParseError), [`FileRestrictionError`](../../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError), [`LanguageNotSupportedError`](../../../tree_sitter_analyzer/_exceptions_core.md#LanguageNotSupportedError), [`PathTraversalError`](../../../tree_sitter_analyzer/_exceptions_security.md#PathTraversalError), [`ConfigurationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ConfigurationError), [`PluginError`](../../../tree_sitter_analyzer/_exceptions_core.md#PluginError), [`RegexSecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError)

### `TestFileHandlingError`
- def: [`tests/unit/core/test_exceptions.py:191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L191)
- doc: Test FileHandlingError exception.
- signature: `class TestFileHandlingError:`
- members:
  - `test_file_handling_error_basic(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L194) — Test FileHandlingError with basic message.
  - `test_file_handling_error_with_operation(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L204) — Test FileHandlingError with operation type.
  - `test_file_handling_error_with_path(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L199) — Test FileHandlingError with file path.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`FileHandlingError`](../../../tree_sitter_analyzer/_exceptions_core.md#FileHandlingError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message)

### `TestHandleException`
- def: [`tests/unit/core/test_exceptions.py:724`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L724)
- doc: Tests for handle_exception utility function (not decorator).
- signature: `class TestHandleException:`
- members:
  - `failing_async()` — [`L792`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L792)
  - `failing_func()` — [`L772`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L772)
  - `test_handle_exception_logs_and_reraises(self)` — [`L727`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L727) — Test that handle_exception logs and re-raises the original exception.
  - `test_handle_exception_reraise_as_different_type(self)` — [`L744`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L744) — Test re-raising as different exception type.
  - `test_handle_exception_reraise_non_tree_sitter_error(self)` — [`L752`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L752) — Test re-raising as non-TreeSitterAnalyzerError type.
  - `test_handle_exception_with_context(self)` — [`L735`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L735) — Test handle_exception with additional context.
  - `test_handle_exception_with_exception_context(self)` — [`L760`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L760) — Test handle_exception when exception has context attribute.
  - `test_handle_exceptions_decorator_with_logging(self)` — [`L768`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L768) — Test decorator with logging enabled (covers logging path).
  - `test_handle_exceptions_reraise_with_logging(self)` — [`L778`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L778) — Test decorator reraise with logging enabled.
  - `test_safe_execute_async_with_logging(self)` — [`L789`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L789) — Test async execution with logging enabled.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`handle_exception`](../../../tree_sitter_analyzer/_exceptions_execution.md#handle_exception), [`handle_exceptions`](../../../tree_sitter_analyzer/_exceptions_execution.md#handle_exceptions), [`safe_execute_async`](../../../tree_sitter_analyzer/_exceptions_execution.md#safe_execute_async)

### `TestLanguageNotSupportedError`
- def: [`tests/unit/core/test_exceptions.py:133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L133)
- doc: Test LanguageNotSupportedError exception.
- signature: `class TestLanguageNotSupportedError:`
- members:
  - `test_language_not_supported_basic(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L136) — Test LanguageNotSupportedError with language name.
  - `test_language_not_supported_with_list(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L142) — Test LanguageNotSupportedError with supported languages list.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`LanguageNotSupportedError`](../../../tree_sitter_analyzer/_exceptions_core.md#LanguageNotSupportedError)

### `TestMCPErrorResponse`
- def: [`tests/unit/core/test_exceptions.py:466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L466)
- doc: Test MCP-specific error response utilities.
- signature: `class TestMCPErrorResponse:`
- members:
  - `test_create_mcp_error_response_basic(self)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L469) — Test create_mcp_error_response with basic exception.
  - `test_create_mcp_error_response_sanitizes_sensitive_data(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L486) — Test create_mcp_error_response sanitizes sensitive information.
  - `test_create_mcp_error_response_specific_types(self)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L510) — Test create_mcp_error_response with specific exception types.
  - `test_create_mcp_error_response_with_debug_info(self)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L502) — Test create_mcp_error_response includes debug information.
  - `test_create_mcp_error_response_with_tool_name(self)` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L479) — Test create_mcp_error_response includes tool name.
- uses (calls/refs, reference-scoped): [`MCPError`](../../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`MCPToolError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError), [`MCPTimeoutError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError), [`create_mcp_error_response`](../../../tree_sitter_analyzer/_exceptions_mcp_response.md#create_mcp_error_response), [`FileRestrictionError`](../../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError)

### `TestMCPExceptions`
- def: [`tests/unit/core/test_exceptions.py:291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L291)
- doc: Test MCP-related exceptions.
- signature: `class TestMCPExceptions:`
- members:
  - `test_mcp_error_basic(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L294) — Test MCPError with basic message.
  - `test_mcp_error_with_tool_name(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L299) — Test MCPError with tool name.
  - `test_mcp_resource_error(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L337) — Test MCPResourceError exception.
  - `test_mcp_timeout_error(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L349) — Test MCPTimeoutError exception.
  - `test_mcp_tool_error(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L304) — Test MCPToolError exception.
  - `test_mcp_tool_error_sanitizes_sensitive_params(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L316) — Test MCPToolError sanitizes sensitive parameters.
  - `test_mcp_tool_error_truncates_long_values(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L328) — Test MCPToolError truncates long parameter values.
  - `test_mcp_validation_error(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L359) — Test MCPValidationError exception.
  - `test_mcp_validation_error_truncates_long_values(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L372) — Test MCPValidationError truncates long parameter values.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`MCPError`](../../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`MCPToolError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError), [`MCPValidationError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError), [`MCPResourceError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError), [`MCPTimeoutError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`access_mode`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.access_mode), [`resource_type`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_type), [`resource_uri`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_uri), [`timeout_seconds`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.timeout_seconds), [`execution_stage`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError.execution_stage), [`operation_type`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.operation_type), [`parameter_name`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.parameter_name), [`tool_name`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError.tool_name), [`tool_name`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.tool_name), [`validation_rule`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.validation_rule)

### `TestParseError`
- def: [`tests/unit/core/test_exceptions.py:111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L111)
- doc: Test ParseError exception.
- signature: `class TestParseError:`
- members:
  - `test_parse_error_basic(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L114) — Test ParseError with basic message.
  - `test_parse_error_with_language(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L119) — Test ParseError with language.
  - `test_parse_error_with_source_info(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L124) — Test ParseError with source information.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`ParseError`](../../../tree_sitter_analyzer/_exceptions_core.md#ParseError)

### `TestPluginError`
- def: [`tests/unit/core/test_exceptions.py:151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L151)
- doc: Test PluginError exception.
- signature: `class TestPluginError:`
- members:
  - `test_plugin_error_basic(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L154) — Test PluginError with basic message.
  - `test_plugin_error_with_operation(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L164) — Test PluginError with operation.
  - `test_plugin_error_with_plugin_name(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L159) — Test PluginError with plugin name.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`PluginError`](../../../tree_sitter_analyzer/_exceptions_core.md#PluginError)

### `TestQueryError`
- def: [`tests/unit/core/test_exceptions.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L170)
- doc: Test QueryError exception.
- signature: `class TestQueryError:`
- members:
  - `test_query_error_basic(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L173) — Test QueryError with basic message.
  - `test_query_error_with_all_params(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L178) — Test QueryError with all parameters.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`QueryError`](../../../tree_sitter_analyzer/_exceptions_core.md#QueryError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message)

### `TestSanitizeErrorContext`
- def: [`tests/unit/core/test_exceptions.py:623`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L623)
- doc: Test _sanitize_error_context function for edge cases.
- signature: `class TestSanitizeErrorContext:`
- members:
  - `test_sanitize_empty_context(self)` — [`L703`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L703) — Test sanitization of empty context.
  - `test_sanitize_large_nested_dict(self)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L657) — Test that large nested dictionaries are truncated.
  - `test_sanitize_long_list_value(self)` — [`L637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L637) — Test that long list values are truncated.
  - `test_sanitize_long_string_value(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L626) — Test that long string values are truncated.
  - `test_sanitize_long_tuple_value(self)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L648) — Test that long tuple values are truncated.
  - `test_sanitize_mixed_context(self)` — [`L708`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L708) — Test sanitization with mixed content types.
  - `test_sanitize_normal_values_unchanged(self)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L688) — Test that normal values are not modified.
  - `test_sanitize_sensitive_keys(self)` — [`L669`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L669) — Test that sensitive keys are redacted.
- uses (calls/refs, reference-scoped): [`_sanitize_error_context`](../../../tree_sitter_analyzer/_exceptions_sanitization.md#_sanitize_error_context)

### `TestSecurityExceptions`
- def: [`tests/unit/core/test_exceptions.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L244)
- doc: Test security-related exceptions.
- signature: `class TestSecurityExceptions:`
- members:
  - `test_file_restriction_error(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L278) — Test FileRestrictionError exception.
  - `test_path_traversal_error(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L258) — Test PathTraversalError exception.
  - `test_regex_security_error(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L267) — Test RegexSecurityError exception.
  - `test_security_error_basic(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L247) — Test SecurityError with basic message.
  - `test_security_error_with_type(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L252) — Test SecurityError with security type.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`FileRestrictionError`](../../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError), [`PathTraversalError`](../../../tree_sitter_analyzer/_exceptions_security.md#PathTraversalError), [`RegexSecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError), [`security_type`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.security_type), [`allowed_patterns`](../../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError.allowed_patterns), [`current_mode`](../../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError.current_mode), [`attempted_path`](../../../tree_sitter_analyzer/_exceptions_security.md#PathTraversalError.attempted_path), [`dangerous_construct`](../../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError.dangerous_construct), [`pattern`](../../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError.pattern)

### `TestValidationError`
- def: [`tests/unit/core/test_exceptions.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L227)
- doc: Test ValidationError exception.
- signature: `class TestValidationError:`
- members:
  - `test_validation_error_basic(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L230) — Test ValidationError with basic message.
  - `test_validation_error_with_type_and_value(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exceptions.py#L235) — Test ValidationError with validation type and invalid value.
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`ValidationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message)

