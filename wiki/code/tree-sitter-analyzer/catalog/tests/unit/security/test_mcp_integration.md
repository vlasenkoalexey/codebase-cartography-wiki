---
title: 'Module: tests/unit/security/test_mcp_integration.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_mcp_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_mcp_integration`/TestSecurityMCPIntegration#
symbols:
  TestSecurityMCPIntegration.project_root: project_root.
  TestSecurityMCPIntegration.test_mcp_server_security_workflow: test_mcp_server_security_workflow().
  TestSecurityMCPIntegration.test_security_error_handling_in_mcp_context: test_security_error_handling_in_mcp_context().
  TestSecurityMCPIntegration.test_performance_impact_on_mcp_server: test_performance_impact_on_mcp_server().
  TestSecurityMCPIntegration.mcp_server: mcp_server.
  TestSecurityMCPIntegration.test_mcp_server_project_boundary_enforcement: test_mcp_server_project_boundary_enforcement().
  TestSecurityMCPIntegration.test_security_logging_integration: test_security_logging_integration().
  TestSecurityMCPIntegration.test_security_validator_with_mcp_project_path: test_security_validator_with_mcp_project_path().
  TestSecurityMCPIntegration.test_mcp_server_with_security_validation: test_mcp_server_with_security_validation().
  TestSecurityMCPIntegration.src_dir: src_dir.
  TestSecurityMCPIntegration.test_file: test_file.
  TestSecurityMCPIntegration.test_regex_validation_for_mcp_queries: test_regex_validation_for_mcp_queries().
  TestSecurityMCPIntegration.test_input_sanitization_for_mcp_requests: test_input_sanitization_for_mcp_requests().
  TestSecurityMCPIntegration.temp_dir: temp_dir.
  TestSecurityMCPIntegration.teardown_method: teardown_method().
  TestSecurityMCPIntegration: ''
  TestSecurityMCPIntegration.setup_method: setup_method().
---
# Module: [`tests/unit/security/test_mcp_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py)

## Classes
### `TestSecurityMCPIntegration`
- def: [`tests/unit/security/test_mcp_integration.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L16)
- doc: Integration test suite for security module with MCP server.
- signature: `class TestSecurityMCPIntegration:`
- members:
  - `setup_method(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L19) — Set up test fixtures.
  - `teardown_method(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L37) — Clean up test fixtures.
  - `test_input_sanitization_for_mcp_requests(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L115) — Test input sanitization for MCP request data.
  - `test_mcp_server_project_boundary_enforcement(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L202) — Test MCP server respects project boundaries.
  - `test_mcp_server_security_workflow(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L136) — Test complete security workflow with MCP server.
  - `test_mcp_server_with_security_validation(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L62) — Test MCP server operations with security validation.
  - `test_performance_impact_on_mcp_server(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L265) — Test that security validation doesn't significantly impact MCP server performance.
  - `test_regex_validation_for_mcp_queries(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L88) — Test regex validation for MCP query patterns.
  - `test_security_error_handling_in_mcp_context(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L169) — Test security error handling in MCP context.
  - `test_security_logging_integration(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L230) — Test security logging integration with MCP server.
  - `test_security_validator_with_mcp_project_path(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L44) — Test security validator works with MCP server project path.
  - `mcp_server` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L34)
  - `project_root` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L22)
  - `src_dir` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L26)
  - `temp_dir` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L21)
  - `test_file` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_integration.py#L29)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`sanitize_input`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.sanitize_input), [`validate_regex_pattern`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_regex_pattern)

