---
title: 'Module: tests/unit/core/test_exception_context_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_exception_context_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_exception_context_properties`/
symbols:
  safe_text: safe_text.
  TestExceptionContextPreservationProperty.test_base_exception_preserves_context: TestExceptionContextPreservationProperty#test_base_exception_preserves_context().
  TestExceptionContextPreservationProperty.test_mcp_resource_error_preserves_resource_context: TestExceptionContextPreservationProperty#test_mcp_resource_error_preserves_resource_context().
  TestExceptionContextPreservationProperty.test_mcp_timeout_error_preserves_timeout_context: TestExceptionContextPreservationProperty#test_mcp_timeout_error_preserves_timeout_context().
  TestExceptionContextPreservationProperty.test_to_dict_preserves_all_information: TestExceptionContextPreservationProperty#test_to_dict_preserves_all_information().
  TestExceptionContextPreservationProperty.test_create_error_response_preserves_context: TestExceptionContextPreservationProperty#test_create_error_response_preserves_context().
  TestExceptionContextPreservationProperty.test_nested_exception_chain_preserves_all_causes: TestExceptionContextPreservationProperty#test_nested_exception_chain_preserves_all_causes().
  TestExceptionContextPreservationProperty.test_language_not_supported_error_preserves_language_info: TestExceptionContextPreservationProperty#test_language_not_supported_error_preserves_language_info().
  TestExceptionContextPreservationProperty.test_analysis_error_preserves_file_and_language_context: TestExceptionContextPreservationProperty#test_analysis_error_preserves_file_and_language_context().
  TestExceptionContextPreservationProperty.test_exception_chain_preserves_cause: TestExceptionContextPreservationProperty#test_exception_chain_preserves_cause().
  TestExceptionContextPreservationProperty.test_mcp_error_response_preserves_tool_context: TestExceptionContextPreservationProperty#test_mcp_error_response_preserves_tool_context().
  TestExceptionContextPreservationProperty.test_query_error_preserves_all_query_context: TestExceptionContextPreservationProperty#test_query_error_preserves_all_query_context().
  TestExceptionContextPreservationProperty.test_validation_error_preserves_validation_context: TestExceptionContextPreservationProperty#test_validation_error_preserves_validation_context().
  TestExceptionChainWithDecorator.test_handle_exceptions_decorator_preserves_cause_chain: TestExceptionChainWithDecorator#test_handle_exceptions_decorator_preserves_cause_chain().
  context_dict: context_dict.
  TestExceptionChainWithDecorator.failing_function: TestExceptionChainWithDecorator#failing_function().
  context_value: context_value.
  safe_key: safe_key.
  TestExceptionContextPreservationProperty: TestExceptionContextPreservationProperty#
  TestExceptionChainWithDecorator: TestExceptionChainWithDecorator#
---
# Module: [`tests/unit/core/test_exception_context_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py)

## Classes
### `TestExceptionChainWithDecorator`
- def: [`tests/unit/core/test_exception_context_properties.py:455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L455)
- doc: Test exception chain preservation with handle_exceptions decorator.
- signature: `class TestExceptionChainWithDecorator:`
- members:
  - `failing_function()` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L472)
  - `test_handle_exceptions_decorator_preserves_cause_chain(self, original_message: str)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L460) — Property: When handle_exceptions decorator re-raises as a different
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`handle_exceptions`](../../../tree_sitter_analyzer/_exceptions_execution.md#handle_exceptions)  (1 test-only)

### `TestExceptionContextPreservationProperty`
- def: [`tests/unit/core/test_exception_context_properties.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L68)
- doc: Property-based tests for exception context preservation.
- signature: `class TestExceptionContextPreservationProperty:`
- members:
  - `test_analysis_error_preserves_file_and_language_context(self, message: str, file_path: str | None, language: str | None)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L114) — Property: For any AnalysisError, file_path and language SHALL be
  - `test_base_exception_preserves_context(self, message: str, error_code: str | None, context: dict[str, Any])` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L84) — Property: For any TreeSitterAnalyzerError, the context dictionary
  - `test_create_error_response_preserves_context(self, message: str, context: dict[str, Any])` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L200) — Property: For any exception with context, create_error_response()
  - `test_exception_chain_preserves_cause(self, original_message: str, wrapper_message: str)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L141) — Property: For any chained exception, the __cause__ attribute SHALL
  - `test_language_not_supported_error_preserves_language_info(self, message: str, language: str, supported: list[str])` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L400) — Property: For any LanguageNotSupportedError, the unsupported language
  - `test_mcp_error_response_preserves_tool_context(self, message: str, tool_name: str | None)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L230) — Property: For any MCP error, create_mcp_error_response() SHALL
  - `test_mcp_resource_error_preserves_resource_context(self, message: str, resource_uri: str | None, resource_type: str | None, access_mode: str | None)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L330) — Property: For any MCPResourceError, all resource-related context
  - `test_mcp_timeout_error_preserves_timeout_context(self, message: str, timeout_seconds: float, operation_type: str | None)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L298) — Property: For any MCPTimeoutError, timeout_seconds and operation_type
  - `test_nested_exception_chain_preserves_all_causes(self, inner_message: str, outer_message: str, inner_context: dict[str, Any])` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L368) — Property: For any nested exception chain (A -> B -> C), all causes
  - `test_query_error_preserves_all_query_context(self, message: str, query_name: str | None, query_string: str | None, language: str | None)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L262) — Property: For any QueryError, all query-related context (name, string,
  - `test_to_dict_preserves_all_information(self, message: str, context: dict[str, Any])` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L171) — Property: For any exception, to_dict() SHALL produce a dictionary
  - `test_validation_error_preserves_validation_context(self, message: str, validation_type: str | None, invalid_value: Any)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L435) — Property: For any ValidationError, validation_type and invalid_value
- uses (calls/refs, reference-scoped): [`context`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`MCPError`](../../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`AnalysisError`](../../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`ValidationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`MCPResourceError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError), [`QueryError`](../../../tree_sitter_analyzer/_exceptions_core.md#QueryError), [`MCPTimeoutError`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError), [`create_mcp_error_response`](../../../tree_sitter_analyzer/_exceptions_mcp_response.md#create_mcp_error_response), [`message`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`LanguageNotSupportedError`](../../../tree_sitter_analyzer/_exceptions_core.md#LanguageNotSupportedError), [`to_dict`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`create_error_response`](../../../tree_sitter_analyzer/_exceptions_execution.md#create_error_response), [`error_code`](../../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.error_code), [`access_mode`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.access_mode), [`resource_type`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_type), [`resource_uri`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_uri), [`timeout_seconds`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.timeout_seconds), [`operation_type`](../../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.operation_type)  (2 test-only)

## Module values
- `context_dict` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L56)
- `context_value` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L48)
- `safe_key` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L41)
- `safe_text` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_exception_context_properties.py#L32)

