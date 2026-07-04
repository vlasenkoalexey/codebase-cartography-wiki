---
title: 'Module: tests/integration/cli/test_read_partial_tool_extended.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_read_partial_tool_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_read_partial_tool_extended`/TestReadPartialTool
symbols:
  TestReadPartialToolEdgeCases.test_execute_with_nonexistent_file: EdgeCases#test_execute_with_nonexistent_file().
  TestReadPartialToolEdgeCases.test_execute_with_path_traversal_attempt: EdgeCases#test_execute_with_path_traversal_attempt().
  TestReadPartialToolConfiguration.test_tool_initialization_with_invalid_project_root: Configuration#test_tool_initialization_with_invalid_project_root().
  TestReadPartialToolConfiguration.test_tool_components_initialization: Configuration#test_tool_components_initialization().
  TestReadPartialToolEdgeCases.tool: EdgeCases#tool().
  TestReadPartialToolEdgeCases.test_execute_with_negative_line_numbers: EdgeCases#test_execute_with_negative_line_numbers().
  TestReadPartialToolEdgeCases.test_execute_with_reversed_line_range: EdgeCases#test_execute_with_reversed_line_range().
  TestReadPartialToolEdgeCases.test_execute_with_binary_file: EdgeCases#test_execute_with_binary_file().
  TestReadPartialToolEdgeCases.test_execute_with_invalid_arguments: EdgeCases#test_execute_with_invalid_arguments().
  TestReadPartialToolConfiguration.test_tool_initialization_with_valid_project_root: Configuration#test_tool_initialization_with_valid_project_root().
  TestReadPartialToolConfiguration.test_tool_initialization_with_none_project_root: Configuration#test_tool_initialization_with_none_project_root().
  TestReadPartialToolPerformance.tool: Performance#tool().
  TestReadPartialToolIntegration.tool: Integration#tool().
  TestReadPartialToolEdgeCases: EdgeCases#
  TestReadPartialToolEdgeCases.temp_dir: EdgeCases#temp_dir().
  TestReadPartialToolEdgeCases.test_execute_with_empty_file: EdgeCases#test_execute_with_empty_file().
  TestReadPartialToolEdgeCases.test_execute_with_single_line_file: EdgeCases#test_execute_with_single_line_file().
  TestReadPartialToolEdgeCases.test_execute_with_large_line_range: EdgeCases#test_execute_with_large_line_range().
  TestReadPartialToolEdgeCases.test_execute_with_unicode_content: EdgeCases#test_execute_with_unicode_content().
  TestReadPartialToolConfiguration: Configuration#
  TestReadPartialToolPerformance: Performance#
  TestReadPartialToolPerformance.temp_dir: Performance#temp_dir().
  TestReadPartialToolPerformance.test_concurrent_reading: Performance#test_concurrent_reading().
  TestReadPartialToolPerformance.test_reading_large_file_portions: Performance#test_reading_large_file_portions().
  TestReadPartialToolPerformance.test_memory_usage_with_repeated_reading: Performance#test_memory_usage_with_repeated_reading().
  TestReadPartialToolIntegration: Integration#
  TestReadPartialToolIntegration.temp_dir: Integration#temp_dir().
  TestReadPartialToolIntegration.test_tool_with_realistic_source_file: Integration#test_tool_with_realistic_source_file().
  TestReadPartialToolIntegration.test_tool_with_different_file_types: Integration#test_tool_with_different_file_types().
---
# Module: [`tests/integration/cli/test_read_partial_tool_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py)

## Classes
### `TestReadPartialToolConfiguration`
- def: [`tests/integration/cli/test_read_partial_tool_extended.py:264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L264)
- doc: Test ReadPartialTool configuration and initialization.
- signature: `class TestReadPartialToolConfiguration:`
- members:
  - `test_tool_components_initialization(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L298) — Test that tool components are properly initialized.
  - `test_tool_initialization_with_invalid_project_root(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L281) — Test tool initialization with invalid project root.
  - `test_tool_initialization_with_none_project_root(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L275) — Test tool initialization with None project root.
  - `test_tool_initialization_with_valid_project_root(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L267) — Test tool initialization with valid project root.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`security_validator`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.security_validator)

### `TestReadPartialToolEdgeCases`
- def: [`tests/integration/cli/test_read_partial_tool_extended.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L19)
- doc: Test edge cases and error conditions in ReadPartialTool.
- signature: `class TestReadPartialToolEdgeCases:`
- members:
  - `temp_dir(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L23) — Create a temporary directory for testing.
  - `test_execute_with_binary_file(self, tool, temp_dir)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L160) — Test reading from a binary file.
  - `test_execute_with_empty_file(self, tool, temp_dir)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L34) — Test reading from an empty file.
  - `test_execute_with_invalid_arguments(self, tool)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L202) — Test executing with invalid arguments.
  - `test_execute_with_large_line_range(self, tool, temp_dir)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L74) — Test reading with a very large line range.
  - `test_execute_with_negative_line_numbers(self, tool, temp_dir)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L95) — Test reading with negative line numbers.
  - `test_execute_with_nonexistent_file(self, tool)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L183) — Test reading from a non-existent file.
  - `test_execute_with_path_traversal_attempt(self, tool)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L240) — Test executing with path traversal attempts.
  - `test_execute_with_reversed_line_range(self, tool, temp_dir)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L113) — Test reading with start_line > end_line.
  - `test_execute_with_single_line_file(self, tool, temp_dir)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L55) — Test reading from a single line file.
  - `test_execute_with_unicode_content(self, tool, temp_dir)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L135) — Test reading files with Unicode content.
  - `tool(self, temp_dir)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L29) — Create a ReadPartialTool instance for testing.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`FileHandlingError`](../../../tree_sitter_analyzer/_exceptions_core.md#FileHandlingError)

### `TestReadPartialToolIntegration`
- def: [`tests/integration/cli/test_read_partial_tool_extended.py:420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L420)
- doc: Integration tests for ReadPartialTool.
- signature: `class TestReadPartialToolIntegration:`
- members:
  - `temp_dir(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L424) — Create a temporary directory for testing.
  - `test_tool_with_different_file_types(self, tool, temp_dir)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L498) — Test tool with different file types.
  - `test_tool_with_realistic_source_file(self, tool, temp_dir)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L435) — Test tool with realistic source code file.
  - `tool(self, temp_dir)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L430) — Create a ReadPartialTool instance for testing.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool)

### `TestReadPartialToolPerformance`
- def: [`tests/integration/cli/test_read_partial_tool_extended.py:308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L308)
- doc: Test ReadPartialTool performance characteristics.
- signature: `class TestReadPartialToolPerformance:`
- members:
  - `temp_dir(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L312) — Create a temporary directory for testing.
  - `test_concurrent_reading(self, tool, temp_dir)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L323) — Test concurrent file reading.
  - `test_memory_usage_with_repeated_reading(self, tool, temp_dir)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L383) — Test memory usage with repeated reading operations.
  - `test_reading_large_file_portions(self, tool, temp_dir)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L351) — Test reading large portions of files.
  - `tool(self, temp_dir)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_read_partial_tool_extended.py#L318) — Create a ReadPartialTool instance for testing.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool)

