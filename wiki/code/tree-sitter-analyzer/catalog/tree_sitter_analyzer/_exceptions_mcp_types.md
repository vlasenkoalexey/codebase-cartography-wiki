---
title: 'Module: tree_sitter_analyzer/_exceptions_mcp_types.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_mcp_types.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_mcp_types`/MCP
symbols:
  MCPToolError: ToolError#
  MCPValidationError: ValidationError#
  MCPResourceError: ResourceError#
  MCPTimeoutError: TimeoutError#
  MCPResourceError.resource_uri: ResourceError#resource_uri.
  MCPResourceError.resource_type: ResourceError#resource_type.
  MCPResourceError.access_mode: ResourceError#access_mode.
  MCPTimeoutError.timeout_seconds: TimeoutError#timeout_seconds.
  MCPToolError.__init__: ToolError#__init__().
  MCPValidationError.__init__: ValidationError#__init__().
  MCPToolError.execution_stage: ToolError#execution_stage.
  MCPTimeoutError.operation_type: TimeoutError#operation_type.
  MCPToolError.tool_name: ToolError#tool_name.
  MCPValidationError.tool_name: ValidationError#tool_name.
  MCPValidationError.parameter_name: ValidationError#parameter_name.
  MCPValidationError.validation_rule: ValidationError#validation_rule.
  MCPResourceError.__init__: ResourceError#__init__().
  MCPTimeoutError.__init__: TimeoutError#__init__().
  MCPToolError.input_params: ToolError#input_params.
---
# Module: [`tree_sitter_analyzer/_exceptions_mcp_types.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py)

## Classes
### `MCPResourceError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/_exceptions_mcp_types.py:32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L32)
- doc: Raised when MCP resource access fails.
- signature: `class MCPResourceError(MCPError):`
- members:
  - `access_mode` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L52)
  - `resource_type` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L51)
  - `resource_uri` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L50)
- protocol/private: `__init__`[`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L35)
- uses (calls/refs, reference-scoped): [`MCPError`](_exceptions_core.md#MCPError), [`__init__`](_exceptions_core.md#MCPError.__init__)
- used by: [`MCPError`](_exceptions_core.md#MCPError)  (15 test-only)

### `MCPTimeoutError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/_exceptions_mcp_types.py:55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L55)
- doc: Raised when MCP operation times out.
- signature: `class MCPTimeoutError(MCPError):`
- members:
  - `operation_type` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L73)
  - `timeout_seconds` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L72)
- protocol/private: `__init__`[`L58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L58)
- uses (calls/refs, reference-scoped): [`MCPError`](_exceptions_core.md#MCPError), [`__init__`](_exceptions_core.md#MCPError.__init__)
- used by: [`MCPError`](_exceptions_core.md#MCPError), [`_attach_exception_details`](_exceptions_mcp_response.md#_attach_exception_details)  (11 test-only)

### `MCPToolError`  ·  implements/extends MCPError
- def: [`tree_sitter_analyzer/_exceptions_mcp_types.py:9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L9) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when MCP tool execution fails.
- signature: `class MCPToolError(MCPError):`
- members:
  - `execution_stage` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L29)
  - `input_params` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L28)
  - `tool_name` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L27)
- protocol/private: `__init__`[`L12`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L12)
- uses (calls/refs, reference-scoped): [`MCPError`](_exceptions_core.md#MCPError), [`__init__`](_exceptions_core.md#MCPError.__init__), [`_sanitize_params`](_exceptions_sanitization.md#_sanitize_params)
- used by: [`MCPError`](_exceptions_core.md#MCPError), [`_attach_exception_details`](_exceptions_mcp_response.md#_attach_exception_details)  (20 test-only)

### `MCPValidationError`  ·  implements/extends ValidationError
- def: [`tree_sitter_analyzer/_exceptions_mcp_types.py:76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L76) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when MCP input validation fails.
- signature: `class MCPValidationError(ValidationError):`
- members:
  - `parameter_name` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L102)
  - `tool_name` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L101)
  - `validation_rule` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L103)
- protocol/private: `__init__`[`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_mcp_types.py#L79)
- uses (calls/refs, reference-scoped): [`ValidationError`](_exceptions_core.md#ValidationError), [`__init__`](_exceptions_core.md#ValidationError.__init__), [`_sanitize_parameter_value`](_exceptions_sanitization.md#_sanitize_parameter_value)
- used by: [`ValidationError`](_exceptions_core.md#ValidationError)  (17 test-only)

