---
title: 'Module: tests/integration/mcp/test_tools/test_read_partial_tool.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_read_partial_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_read_partial_tool`/TestReadPartialTool
symbols:
  TestReadPartialToolSchema.tool: Schema#tool.
  TestReadPartialToolSchema.test_tool_schema_structure: Schema#test_tool_schema_structure().
  TestReadPartialToolSchema.test_input_parameters_validation: Schema#test_input_parameters_validation().
  TestReadPartialToolSchema.test_required_parameters: Schema#test_required_parameters().
  TestReadPartialToolErrorHandling.test_invalid_arguments: ErrorHandling#test_invalid_arguments().
  TestReadPartialToolErrorHandling.tool: ErrorHandling#tool.
  TestReadPartialToolFunctionality.tool: Functionality#tool.
  TestReadPartialToolIntegration.tool: Integration#tool.
  TestReadPartialToolIntegration.test_integration_with_file_handler: Integration#test_integration_with_file_handler().
  TestReadPartialToolSchema: Schema#
  TestReadPartialToolSchema.setup_method: Schema#setup_method().
  TestReadPartialToolFunctionality: Functionality#
  TestReadPartialToolFunctionality.setup_method: Functionality#setup_method().
  TestReadPartialToolFunctionality.sample_content: Functionality#sample_content.
  TestReadPartialToolFunctionality.test_read_line_range_placeholder: Functionality#test_read_line_range_placeholder().
  TestReadPartialToolFunctionality.test_read_single_line_placeholder: Functionality#test_read_single_line_placeholder().
  TestReadPartialToolFunctionality.test_read_with_column_range_placeholder: Functionality#test_read_with_column_range_placeholder().
  TestReadPartialToolFunctionality.test_json_format_output_placeholder: Functionality#test_json_format_output_placeholder().
  TestReadPartialToolFunctionality.test_read_beyond_file_end_placeholder: Functionality#test_read_beyond_file_end_placeholder().
  TestReadPartialToolErrorHandling: ErrorHandling#
  TestReadPartialToolErrorHandling.setup_method: ErrorHandling#setup_method().
  TestReadPartialToolErrorHandling.test_invalid_line_range_placeholder: ErrorHandling#test_invalid_line_range_placeholder().
  TestReadPartialToolErrorHandling.test_nonexistent_file_placeholder: ErrorHandling#test_nonexistent_file_placeholder().
  TestReadPartialToolIntegration: Integration#
  TestReadPartialToolIntegration.setup_method: Integration#setup_method().
---
# Module: [`tests/integration/mcp/test_tools/test_read_partial_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py)

## Classes
### `TestReadPartialToolErrorHandling`
- def: [`tests/integration/mcp/test_tools/test_read_partial_tool.py:116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L116)
- doc: Test error handling in read_partial_file tool
- signature: `class TestReadPartialToolErrorHandling:`
- members:
  - `setup_method(self)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L119) — Set up test fixtures
  - `test_invalid_arguments(self)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L123) — Test validation of invalid arguments
  - `test_invalid_line_range_placeholder(self)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L135) — Test invalid line range handling - placeholder
  - `test_nonexistent_file_placeholder(self)` — [`L140`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L140) — Test error handling for nonexistent file - placeholder
  - `tool` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L121)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments)

### `TestReadPartialToolFunctionality`
- def: [`tests/integration/mcp/test_tools/test_read_partial_tool.py:68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L68)
- doc: Test read_partial_file tool core functionality
- signature: `class TestReadPartialToolFunctionality:`
- members:
  - `setup_method(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L71) — Set up test fixtures
  - `test_json_format_output_placeholder(self)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L105) — Test JSON format output - placeholder
  - `test_read_beyond_file_end_placeholder(self)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L110) — Test reading beyond file end - placeholder
  - `test_read_line_range_placeholder(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L90) — Test reading a specific line range - placeholder
  - `test_read_single_line_placeholder(self)` — [`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L95) — Test reading a single line - placeholder
  - `test_read_with_column_range_placeholder(self)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L100) — Test reading with column range - placeholder
  - `sample_content` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L74)
  - `tool` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L73)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool)

### `TestReadPartialToolIntegration`
- def: [`tests/integration/mcp/test_tools/test_read_partial_tool.py:146`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L146)
- doc: Test integration with existing file handling components
- signature: `class TestReadPartialToolIntegration:`
- members:
  - `setup_method(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L149) — Set up test fixtures
  - `test_integration_with_file_handler(self)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L153) — Test integration with file handling utilities
  - `tool` — [`L151`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L151)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`read_file_partial`](../../../../tree_sitter_analyzer/file_handler.md#read_file_partial)

### `TestReadPartialToolSchema`
- def: [`tests/integration/mcp/test_tools/test_read_partial_tool.py:17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L17)
- doc: Test read_partial_file tool schema and validation
- signature: `class TestReadPartialToolSchema:`
- members:
  - `setup_method(self)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L20) — Set up test fixtures
  - `test_input_parameters_validation(self)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L44) — Test input parameter validation
  - `test_required_parameters(self)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L58) — Test required parameter validation
  - `test_tool_schema_structure(self)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L24) — Test that tool schema has required structure
  - `tool` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_read_partial_tool.py#L22)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.get_tool_schema)

