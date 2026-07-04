---
title: 'Module: tests/unit/mcp/test_mcp_query_tool_definition.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_query_tool_definition.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_query_tool_definition`/TestMCPQueryTool
symbols:
  TestMCPQueryToolDefinition.test_initialization: Definition#test_initialization().
  TestMCPQueryToolDefinition.query_tool: Definition#query_tool.
  TestMCPQueryToolDefinition.test_get_available_queries: Definition#test_get_available_queries().
  TestMCPQueryToolHelpers.query_tool: Helpers#query_tool.
  TestMCPQueryToolDefinition.test_tool_definition_structure: Definition#test_tool_definition_structure().
  TestMCPQueryToolDefinition.test_tool_definition_filter_parameter: Definition#test_tool_definition_filter_parameter().
  TestMCPQueryToolDefinition.test_tool_definition_required_fields: Definition#test_tool_definition_required_fields().
  TestMCPQueryToolDefinition.test_tool_definition_properties_types: Definition#test_tool_definition_properties_types().
  TestMCPQueryToolHelpers.test_extract_name_from_content_java: Helpers#test_extract_name_from_content_java().
  TestMCPQueryToolHelpers.test_extract_name_from_content_unknown: Helpers#test_extract_name_from_content_unknown().
  TestMCPQueryToolHelpers.test_format_summary: Helpers#test_format_summary().
  TestMCPQueryToolDefinition: Definition#
  TestMCPQueryToolDefinition.setup_method: Definition#setup_method().
  TestMCPQueryToolHelpers: Helpers#
  TestMCPQueryToolHelpers.setup_method: Helpers#setup_method().
---
# Module: [`tests/unit/mcp/test_mcp_query_tool_definition.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py)

## Classes
### `TestMCPQueryToolDefinition`
- def: [`tests/unit/mcp/test_mcp_query_tool_definition.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L15)
- doc: Tests for MCP query tool definition and metadata
- signature: `class TestMCPQueryToolDefinition:`
- members:
  - `setup_method(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L18) — Set up test fixtures
  - `test_get_available_queries(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L77) — Test getting available queries
  - `test_initialization(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L89) — Test tool initialization
  - `test_tool_definition_filter_parameter(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L41) — Test that filter parameter is correctly defined
  - `test_tool_definition_properties_types(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L60) — Test that all properties have correct types
  - `test_tool_definition_required_fields(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L51) — Test that key fields are defined (file_path or symbol required at runtime)
  - `test_tool_definition_structure(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L22) — Test that tool definition has correct structure
  - `query_tool` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L20)
- uses (calls/refs, reference-scoped): [`project_root`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`security_validator`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.security_validator), [`query_service`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.query_service), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.get_tool_definition), [`get_available_queries`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.get_available_queries)

### `TestMCPQueryToolHelpers`
- def: [`tests/unit/mcp/test_mcp_query_tool_definition.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L105)
- doc: Tests for MCP query tool helper methods
- signature: `class TestMCPQueryToolHelpers:`
- members:
  - `setup_method(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L108) — Set up test fixtures
  - `test_extract_name_from_content_java(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L112) — Test extracting names from Java method content
  - `test_extract_name_from_content_unknown(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L126) — Test extracting name from unrecognized content
  - `test_format_summary(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L131) — Test formatting summary output
  - `query_tool` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_query_tool_definition.py#L110)
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`_extract_name_from_content`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool._extract_name_from_content), [`_format_summary`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool._format_summary)

