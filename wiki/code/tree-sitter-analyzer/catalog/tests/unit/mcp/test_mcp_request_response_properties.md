---
title: 'Module: tests/unit/mcp/test_mcp_request_response_properties.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_request_response_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_request_response_properties`/Test
symbols:
  TestMCPRequestResponseConsistency.test_analyze_file_error_response_format: MCPRequestResponseConsistency#test_analyze_file_error_response_format().
  TestMCPRequestResponseConsistency.test_invalid_file_path_handling: MCPRequestResponseConsistency#test_invalid_file_path_handling().
  TestErrorResponseConsistency.test_file_not_found_error_format: ErrorResponseConsistency#test_file_not_found_error_format().
  TestErrorResponseConsistency.test_unsupported_language_handling: ErrorResponseConsistency#test_unsupported_language_handling().
  TestErrorResponseConsistency.test_empty_file_handling: ErrorResponseConsistency#test_empty_file_handling().
  TestMCPRequestResponseConsistency.test_analyze_file_valid_response_structure: MCPRequestResponseConsistency#test_analyze_file_valid_response_structure().
  TestMCPRequestResponseConsistency.test_tool_definition_format: MCPRequestResponseConsistency#test_tool_definition_format().
  TestMCPRequestResponseConsistency.test_concurrent_requests_consistency: MCPRequestResponseConsistency#test_concurrent_requests_consistency().
  TestMCPProtocolCompliance.test_tool_schema_validity: MCPProtocolCompliance#test_tool_schema_validity().
  TestMCPProtocolCompliance.test_mcp_info_has_required_fields: MCPProtocolCompliance#test_mcp_info_has_required_fields().
  TestMCPProtocolCompliance.test_mcp_capabilities_structure: MCPProtocolCompliance#test_mcp_capabilities_structure().
  TestMCPRequestResponseConsistency: MCPRequestResponseConsistency#
  TestMCPRequestResponseConsistency.temp_dir: MCPRequestResponseConsistency#temp_dir().
  TestMCPRequestResponseConsistency.sample_files: MCPRequestResponseConsistency#sample_files().
  TestMCPProtocolCompliance: MCPProtocolCompliance#
  TestErrorResponseConsistency: ErrorResponseConsistency#
---
# Module: [`tests/unit/mcp/test_mcp_request_response_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py)

## Classes
### `TestErrorResponseConsistency`
- def: [`tests/unit/mcp/test_mcp_request_response_properties.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L179)
- doc: Test error response consistency.
- signature: `class TestErrorResponseConsistency:`
- members:
  - `test_empty_file_handling(self, tmp_path)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L215) — Test handling of empty files.
  - `test_file_not_found_error_format(self, tmp_path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L183) — Test error response for file not found.
  - `test_unsupported_language_handling(self, tmp_path)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L197) — Test handling of unsupported file types.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute)

### `TestMCPProtocolCompliance`
- def: [`tests/unit/mcp/test_mcp_request_response_properties.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L141)
- doc: Test MCP protocol compliance.
- signature: `class TestMCPProtocolCompliance:`
- members:
  - `test_mcp_capabilities_structure(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L152) — Test that MCP capabilities are properly structured.
  - `test_mcp_info_has_required_fields(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L144) — Test that MCP_INFO contains all required fields.
  - `test_tool_schema_validity(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L161) — Test that tool schemas are valid.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.get_tool_definition)

### `TestMCPRequestResponseConsistency`
- def: [`tests/unit/mcp/test_mcp_request_response_properties.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L28)
- doc: Property tests for MCP request-response consistency.
- signature: `class TestMCPRequestResponseConsistency:`
- members:
  - `sample_files(self, temp_dir)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L38) — Create sample files for testing.
  - `temp_dir(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L32) — Create a temporary directory for testing.
  - `test_analyze_file_error_response_format(self, temp_dir)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L75) — Test that error responses have proper format.
  - `test_analyze_file_valid_response_structure(self, temp_dir, sample_files)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L60) — Test that execute produces valid response structure.
  - `test_concurrent_requests_consistency(self, temp_dir, sample_files)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L119) — Test that concurrent requests produce consistent responses.
  - `test_invalid_file_path_handling(self, temp_dir)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L105) — Test that invalid file paths are handled gracefully.
  - `test_tool_definition_format(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_request_response_properties.py#L88) — Test that tool definition returns proper format.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.get_tool_definition)

