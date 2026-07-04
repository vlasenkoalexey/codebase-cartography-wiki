---
title: 'Module: tests/unit/test_exceptions_mcp_types.py'
type: catalog
provenance: extracted
module: tests/unit/test_exceptions_mcp_types.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_exceptions_mcp_types`/Test
symbols:
  TestMCPResourceError.test_all_fields_populated: MCPResourceError#test_all_fields_populated().
  TestMCPToolError.test_without_optional_fields: MCPToolError#test_without_optional_fields().
  TestMCPResourceError.test_without_optional_fields: MCPResourceError#test_without_optional_fields().
  TestMCPValidationError.test_without_optional_fields: MCPValidationError#test_without_optional_fields().
  TestMCPToolError.test_tool_name_stored: MCPToolError#test_tool_name_stored().
  TestMCPToolError.test_execution_stage_stored: MCPToolError#test_execution_stage_stored().
  TestMCPToolError.test_input_params_stored_and_sanitized: MCPToolError#test_input_params_stored_and_sanitized().
  TestMCPResourceError.test_resource_type_in_context: MCPResourceError#test_resource_type_in_context().
  TestMCPResourceError.test_access_mode_in_context: MCPResourceError#test_access_mode_in_context().
  TestMCPTimeoutError.test_timeout_seconds_stored: MCPTimeoutError#test_timeout_seconds_stored().
  TestMCPTimeoutError.test_operation_type_stored: MCPTimeoutError#test_operation_type_stored().
  TestMCPTimeoutError.test_without_optional_fields: MCPTimeoutError#test_without_optional_fields().
  TestMCPValidationError.test_tool_name_in_context: MCPValidationError#test_tool_name_in_context().
  TestMCPValidationError.test_parameter_name_in_context: MCPValidationError#test_parameter_name_in_context().
  TestMCPValidationError.test_validation_rule_in_context: MCPValidationError#test_validation_rule_in_context().
  TestMCPToolError.test_sensitive_keys_redacted: MCPToolError#test_sensitive_keys_redacted().
  TestMCPToolError.test_long_param_value_truncated: MCPToolError#test_long_param_value_truncated().
  TestMCPToolError.test_inherits_from_mcp_error: MCPToolError#test_inherits_from_mcp_error().
  TestMCPToolError.test_inherits_from_tree_sitter_error: MCPToolError#test_inherits_from_tree_sitter_error().
  TestMCPToolError.test_to_dict_includes_context: MCPToolError#test_to_dict_includes_context().
  TestMCPToolError.test_empty_input_params_not_added_to_context: MCPToolError#test_empty_input_params_not_added_to_context().
  TestMCPToolError.test_extra_kwargs_forwarded: MCPToolError#test_extra_kwargs_forwarded().
  TestMCPResourceError.test_resource_uri_stored: MCPResourceError#test_resource_uri_stored().
  TestMCPResourceError.test_inherits_from_mcp_error: MCPResourceError#test_inherits_from_mcp_error().
  TestMCPResourceError.test_inherits_from_tree_sitter_error: MCPResourceError#test_inherits_from_tree_sitter_error().
  TestMCPResourceError.test_resource_type_none_not_in_context: MCPResourceError#test_resource_type_none_not_in_context().
  TestMCPTimeoutError.test_inherits_from_mcp_error: MCPTimeoutError#test_inherits_from_mcp_error().
  TestMCPValidationError.test_parameter_value_in_context: MCPValidationError#test_parameter_value_in_context().
  TestMCPValidationError.test_long_parameter_value_truncated: MCPValidationError#test_long_parameter_value_truncated().
  TestMCPValidationError.test_none_parameter_value_not_in_context: MCPValidationError#test_none_parameter_value_not_in_context().
  TestMCPValidationError.test_inherits_from_validation_error: MCPValidationError#test_inherits_from_validation_error().
  TestMCPValidationError.test_inherits_from_tree_sitter_error: MCPValidationError#test_inherits_from_tree_sitter_error().
  TestMCPValidationError.test_validation_type_is_mcp_parameter: MCPValidationError#test_validation_type_is_mcp_parameter().
  TestExceptionHierarchy.test_mcp_tool_error_can_be_caught_as_mcp_error: ExceptionHierarchy#test_mcp_tool_error_can_be_caught_as_mcp_error().
  TestExceptionHierarchy.test_mcp_resource_error_can_be_caught_as_mcp_error: ExceptionHierarchy#test_mcp_resource_error_can_be_caught_as_mcp_error().
  TestExceptionHierarchy.test_mcp_validation_error_can_be_caught_as_validation_error: ExceptionHierarchy#test_mcp_validation_error_can_be_caught_as_validation_error().
  TestMCPToolError.test_basic_message: MCPToolError#test_basic_message().
  TestMCPResourceError.test_basic_message: MCPResourceError#test_basic_message().
  TestMCPTimeoutError.test_basic_message: MCPTimeoutError#test_basic_message().
  TestMCPValidationError.test_basic_message: MCPValidationError#test_basic_message().
  TestExceptionHierarchy.test_mcp_tool_error_is_exception: ExceptionHierarchy#test_mcp_tool_error_is_exception().
  TestExceptionHierarchy.test_mcp_resource_error_is_exception: ExceptionHierarchy#test_mcp_resource_error_is_exception().
  TestExceptionHierarchy.test_mcp_timeout_error_is_exception: ExceptionHierarchy#test_mcp_timeout_error_is_exception().
  TestExceptionHierarchy.test_mcp_validation_error_is_exception: ExceptionHierarchy#test_mcp_validation_error_is_exception().
  TestMCPToolError: MCPToolError#
  TestMCPResourceError: MCPResourceError#
  TestMCPTimeoutError: MCPTimeoutError#
  TestMCPValidationError: MCPValidationError#
  TestExceptionHierarchy: ExceptionHierarchy#
---
# Module: [`tests/unit/test_exceptions_mcp_types.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py)

## Classes
### `TestExceptionHierarchy`
- def: [`tests/unit/test_exceptions_mcp_types.py:257`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L257)
- doc: All MCP exception types live in the correct hierarchy.
- signature: `class TestExceptionHierarchy:`
- members:
  - `test_mcp_resource_error_can_be_caught_as_mcp_error(self)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L280)
  - `test_mcp_resource_error_is_exception(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L264)
  - `test_mcp_timeout_error_is_exception(self)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L268)
  - `test_mcp_tool_error_can_be_caught_as_mcp_error(self)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L276)
  - `test_mcp_tool_error_is_exception(self)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L260)
  - `test_mcp_validation_error_can_be_caught_as_validation_error(self)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L284)
  - `test_mcp_validation_error_is_exception(self)` — [`L272`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L272)
- uses (calls/refs, reference-scoped): [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`ValidationError`](../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`MCPToolError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError), [`MCPValidationError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError), [`MCPResourceError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError), [`MCPTimeoutError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError)

### `TestMCPResourceError`
- def: [`tests/unit/test_exceptions_mcp_types.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L107)
- doc: Tests for MCPResourceError construction and attribute storage.
- signature: `class TestMCPResourceError:`
- members:
  - `test_access_mode_in_context(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L123)
  - `test_all_fields_populated(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L146)
  - `test_basic_message(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L110)
  - `test_inherits_from_mcp_error(self)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L134)
  - `test_inherits_from_tree_sitter_error(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L138)
  - `test_resource_type_in_context(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L118)
  - `test_resource_type_none_not_in_context(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L142)
  - `test_resource_uri_stored(self)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L114)
  - `test_without_optional_fields(self)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L128)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`MCPResourceError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError), [`access_mode`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.access_mode), [`resource_type`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_type), [`resource_uri`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPResourceError.resource_uri)

### `TestMCPTimeoutError`
- def: [`tests/unit/test_exceptions_mcp_types.py:165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L165)
- doc: Tests for MCPTimeoutError construction.
- signature: `class TestMCPTimeoutError:`
- members:
  - `test_basic_message(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L168)
  - `test_inherits_from_mcp_error(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L187)
  - `test_operation_type_stored(self)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L177)
  - `test_timeout_seconds_stored(self)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L172)
  - `test_without_optional_fields(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L182)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`MCPTimeoutError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError), [`timeout_seconds`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.timeout_seconds), [`operation_type`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPTimeoutError.operation_type)

### `TestMCPToolError`
- def: [`tests/unit/test_exceptions_mcp_types.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L22)
- doc: Tests for MCPToolError construction and attribute storage.
- signature: `class TestMCPToolError:`
- members:
  - `test_basic_message(self)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L25)
  - `test_empty_input_params_not_added_to_context(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L91)
  - `test_execution_stage_stored(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L34)
  - `test_extra_kwargs_forwarded(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L96)
  - `test_inherits_from_mcp_error(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L77)
  - `test_inherits_from_tree_sitter_error(self)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L81)
  - `test_input_params_stored_and_sanitized(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L39)
  - `test_long_param_value_truncated(self)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L64)
  - `test_sensitive_keys_redacted(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L49)
  - `test_to_dict_includes_context(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L85)
  - `test_tool_name_stored(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L29)
  - `test_without_optional_fields(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L71)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`MCPToolError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError), [`to_dict`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`execution_stage`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError.execution_stage), [`tool_name`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError.tool_name), [`input_params`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPToolError.input_params)

### `TestMCPValidationError`
- def: [`tests/unit/test_exceptions_mcp_types.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L197)
- doc: Tests for MCPValidationError construction.
- signature: `class TestMCPValidationError:`
- members:
  - `test_basic_message(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L200)
  - `test_inherits_from_tree_sitter_error(self)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L237)
  - `test_inherits_from_validation_error(self)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L233)
  - `test_long_parameter_value_truncated(self)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L223)
  - `test_none_parameter_value_not_in_context(self)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L229)
  - `test_parameter_name_in_context(self)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L209)
  - `test_parameter_value_in_context(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L219)
  - `test_tool_name_in_context(self)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L204)
  - `test_validation_rule_in_context(self)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L214)
  - `test_validation_type_is_mcp_parameter(self)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L241)
  - `test_without_optional_fields(self)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_mcp_types.py#L245)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`ValidationError`](../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`MCPValidationError`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError), [`parameter_name`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.parameter_name), [`tool_name`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.tool_name), [`validation_rule`](../../tree_sitter_analyzer/_exceptions_mcp_types.md#MCPValidationError.validation_rule)

