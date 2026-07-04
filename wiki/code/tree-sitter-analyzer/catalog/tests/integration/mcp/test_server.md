---
title: 'Module: tests/integration/mcp/test_server.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_server.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_server`/
symbols:
  cleanup_event_loop: cleanup_event_loop().
  TestMCPServerInitialization.test_mcp_info_structure: TestMCPServerInitialization#test_mcp_info_structure().
  TestMCPServerInitialization.test_mcp_info_values: TestMCPServerInitialization#test_mcp_info_values().
  TestMCPProtocolCompliance.test_protocol_version_format: TestMCPProtocolCompliance#test_protocol_version_format().
  TestMCPProtocolCompliance.test_required_capabilities: TestMCPProtocolCompliance#test_required_capabilities().
  TestMCPServerInitialization: TestMCPServerInitialization#
  TestMCPServerCore: TestMCPServerCore#
  TestMCPServerCore.setup_method: TestMCPServerCore#setup_method().
  TestMCPServerCore.server: TestMCPServerCore#server.
  TestMCPServerCore.test_server_initialization_placeholder: TestMCPServerCore#test_server_initialization_placeholder().
  TestMCPServerCore.test_tool_registration_placeholder: TestMCPServerCore#test_tool_registration_placeholder().
  TestMCPServerCore.test_resource_registration_placeholder: TestMCPServerCore#test_resource_registration_placeholder().
  TestMCPProtocolCompliance: TestMCPProtocolCompliance#
  TestMCPServerErrorHandling: TestMCPServerErrorHandling#
  TestMCPServerErrorHandling.test_error_handling_placeholder: TestMCPServerErrorHandling#test_error_handling_placeholder().
  TestMCPServerIntegration: TestMCPServerIntegration#
  TestMCPServerIntegration.test_analyzer_integration_placeholder: TestMCPServerIntegration#test_analyzer_integration_placeholder().
---
# Module: [`tests/integration/mcp/test_server.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py)

## Classes
### `TestMCPProtocolCompliance`
- def: [`tests/integration/mcp/test_server.py:137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L137)
- doc: Test MCP protocol compliance
- signature: `class TestMCPProtocolCompliance:`
- members:
  - `test_protocol_version_format(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L140) — Test that protocol version follows expected format
  - `test_required_capabilities(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L147) — Test that required capabilities are present
- uses (calls/refs, reference-scoped): [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO)

### `TestMCPServerCore`
- def: [`tests/integration/mcp/test_server.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L114)
- doc: Test core MCP server functionality
- signature: `class TestMCPServerCore:`
- members:
  - `setup_method(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L117) — Set up test fixtures
  - `test_resource_registration_placeholder(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L131) — Placeholder test for resource registration
  - `test_server_initialization_placeholder(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L121) — Placeholder test for server initialization
  - `test_tool_registration_placeholder(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L126) — Placeholder test for tool registration
  - `server` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L119)

### `TestMCPServerErrorHandling`
- def: [`tests/integration/mcp/test_server.py:157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L157)
- doc: Test error handling in MCP server
- signature: `class TestMCPServerErrorHandling:`
- members:
  - `test_error_handling_placeholder(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L160) — Placeholder test for error handling

### `TestMCPServerInitialization`
- def: [`tests/integration/mcp/test_server.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L83)
- doc: Test MCP server initialization and basic functionality
- signature: `class TestMCPServerInitialization:`
- members:
  - `test_mcp_info_structure(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L86) — Test that MCP_INFO contains required fields
  - `test_mcp_info_values(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L106) — Test MCP_INFO contains expected values
- uses (calls/refs, reference-scoped): [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO)

### `TestMCPServerIntegration`
- def: [`tests/integration/mcp/test_server.py:166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L166)
- doc: Test integration with existing analyzer components
- signature: `class TestMCPServerIntegration:`
- members:
  - `test_analyzer_integration_placeholder(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L169) — Placeholder test for analyzer integration

## Functions
- `cleanup_event_loop()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_server.py#L20) — イベントループクリーンアップフィクスチャ（根本修正版）

