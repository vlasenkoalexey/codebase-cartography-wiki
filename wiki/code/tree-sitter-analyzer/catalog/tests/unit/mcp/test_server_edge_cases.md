---
title: 'Module: tests/unit/mcp/test_server_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_server_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_server_edge_cases`/TestMCPServer
symbols:
  TestMCPServerInitializationEdgeCases.test_initialization_with_invalid_project_root: InitializationEdgeCases#test_initialization_with_invalid_project_root().
  TestMCPServerInitializationEdgeCases.test_initialization_with_file_as_project_root: InitializationEdgeCases#test_initialization_with_file_as_project_root().
  TestMCPServerToolHandlingEdgeCases.test_tool_call_server_not_initialized: ToolHandlingEdgeCases#test_tool_call_server_not_initialized().
  TestMCPServerToolHandlingEdgeCases.test_tool_call_with_non_existent_project_path: ToolHandlingEdgeCases#test_tool_call_with_non_existent_project_path().
  TestMCPServerResourceHandlingEdgeCases.test_read_resource_with_failing_resource: ResourceHandlingEdgeCases#test_read_resource_with_failing_resource().
  TestMCPServerInitializationEdgeCases.test_initialization_with_unicode_path: InitializationEdgeCases#test_initialization_with_unicode_path().
  TestMCPServerInitializationEdgeCases.test_initialization_with_very_long_path: InitializationEdgeCases#test_initialization_with_very_long_path().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_empty_file: CodeAnalysisEdgeCases#test_analyze_empty_file().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_binary_file: CodeAnalysisEdgeCases#test_analyze_binary_file().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_large_file: CodeAnalysisEdgeCases#test_analyze_large_file().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_with_invalid_language: CodeAnalysisEdgeCases#test_analyze_with_invalid_language().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_with_malformed_code: CodeAnalysisEdgeCases#test_analyze_with_malformed_code().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_with_encoding_issues: CodeAnalysisEdgeCases#test_analyze_with_encoding_issues().
  TestMCPServerCodeAnalysisEdgeCases.test_analyze_with_very_long_lines: CodeAnalysisEdgeCases#test_analyze_with_very_long_lines().
  TestMCPServerFileMetricsEdgeCases.test_calculate_metrics_with_mixed_line_endings: FileMetricsEdgeCases#test_calculate_metrics_with_mixed_line_endings().
  TestMCPServerFileMetricsEdgeCases.test_calculate_metrics_with_only_comments: FileMetricsEdgeCases#test_calculate_metrics_with_only_comments().
  TestMCPServerFileMetricsEdgeCases.test_calculate_metrics_with_only_blank_lines: FileMetricsEdgeCases#test_calculate_metrics_with_only_blank_lines().
  TestMCPServerFileMetricsEdgeCases.test_calculate_metrics_with_complex_comments: FileMetricsEdgeCases#test_calculate_metrics_with_complex_comments().
  TestMCPServerFileMetricsEdgeCases.test_calculate_metrics_with_nested_comments: FileMetricsEdgeCases#test_calculate_metrics_with_nested_comments().
  TestMCPServerToolHandlingEdgeCases.test_tool_call_with_missing_required_params: ToolHandlingEdgeCases#test_tool_call_with_missing_required_params().
  TestMCPServerResourceHandlingEdgeCases.test_read_resource_invalid_uri: ResourceHandlingEdgeCases#test_read_resource_invalid_uri().
  TestMCPServerRuntimeEdgeCases.test_run_with_stdio_failure: RuntimeEdgeCases#test_run_with_stdio_failure().
  TestMCPServerRuntimeEdgeCases.test_run_with_server_creation_failure: RuntimeEdgeCases#test_run_with_server_creation_failure().
  TestMCPServerRuntimeEdgeCases.test_run_with_initialization_options_failure: RuntimeEdgeCases#test_run_with_initialization_options_failure().
  TestMCPServerLoggingEdgeCases.test_server_with_logging_disabled: LoggingEdgeCases#test_server_with_logging_disabled().
  TestMCPServerLoggingEdgeCases.test_tool_call_with_logging_failure: LoggingEdgeCases#test_tool_call_with_logging_failure().
  TestMCPServerToolHandlingEdgeCases.capture_decorator: ToolHandlingEdgeCases#capture_decorator().
  TestMCPServerInitializationEdgeCases.test_initialization_with_permission_denied: InitializationEdgeCases#test_initialization_with_permission_denied().
  TestMCPServerToolHandlingEdgeCases.server_with_failing_tools: ToolHandlingEdgeCases#server_with_failing_tools().
  TestMCPServerToolHandlingEdgeCases.test_tool_call_with_invalid_params: ToolHandlingEdgeCases#test_tool_call_with_invalid_params().
  TestMCPServerUtilityEdgeCases.test_parse_args_with_invalid_arguments: UtilityEdgeCases#test_parse_args_with_invalid_arguments().
  TestMCPServerUtilityEdgeCases.test_main_with_keyboard_interrupt: UtilityEdgeCases#test_main_with_keyboard_interrupt().
  TestMCPServerUtilityEdgeCases.test_main_with_general_exception: UtilityEdgeCases#test_main_with_general_exception().
  TestMCPServerUtilityEdgeCases.test_main_with_project_root_detection_failure: UtilityEdgeCases#test_main_with_project_root_detection_failure().
  TestMCPServerUtilityEdgeCases.test_main_with_environment_variable_issues: UtilityEdgeCases#test_main_with_environment_variable_issues().
  TestMCPServerUtilityEdgeCases.test_main_sync_with_exception: UtilityEdgeCases#test_main_sync_with_exception().
  TestMCPServerToolHandlingEdgeCases.decorator: ToolHandlingEdgeCases#decorator().
  TestMCPServerInitializationEdgeCases: InitializationEdgeCases#
  TestMCPServerCodeAnalysisEdgeCases: CodeAnalysisEdgeCases#
  TestMCPServerCodeAnalysisEdgeCases.empty_file: CodeAnalysisEdgeCases#empty_file().
  TestMCPServerCodeAnalysisEdgeCases.binary_file: CodeAnalysisEdgeCases#binary_file().
  TestMCPServerCodeAnalysisEdgeCases.large_file: CodeAnalysisEdgeCases#large_file().
  TestMCPServerFileMetricsEdgeCases: FileMetricsEdgeCases#
  TestMCPServerToolHandlingEdgeCases: ToolHandlingEdgeCases#
  TestMCPServerToolHandlingEdgeCases.test_tool_call_with_failing_tool: ToolHandlingEdgeCases#test_tool_call_with_failing_tool().
  TestMCPServerResourceHandlingEdgeCases: ResourceHandlingEdgeCases#
  TestMCPServerRuntimeEdgeCases: RuntimeEdgeCases#
  TestMCPServerUtilityEdgeCases: UtilityEdgeCases#
  TestMCPServerLoggingEdgeCases: LoggingEdgeCases#
---
# Module: [`tests/unit/mcp/test_server_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py)

## Classes
### `TestMCPServerCodeAnalysisEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L91)
- doc: Test MCP server code analysis edge cases.
- signature: `class TestMCPServerCodeAnalysisEdgeCases:`
- members:
  - `binary_file(self, temp_project_dir)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L102) — Create a binary file for testing.
  - `empty_file(self, temp_project_dir)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L95) — Create an empty file for testing.
  - `large_file(self, temp_project_dir)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L109) — Create a large file for testing.
  - `test_analyze_binary_file(self, temp_project_dir, binary_file)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L128) — Test analyzing a binary file.
  - `test_analyze_empty_file(self, temp_project_dir, empty_file)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L117) — Test analyzing an empty file.
  - `test_analyze_large_file(self, temp_project_dir, large_file)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L140) — Test analyzing a large file.
  - `test_analyze_with_encoding_issues(self, temp_project_dir)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L196) — Test analyzing file with encoding issues.
  - `test_analyze_with_invalid_language(self, temp_project_dir)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L151) — Test analyzing with invalid language specification.
  - `test_analyze_with_malformed_code(self, temp_project_dir)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L167) — Test analyzing file with malformed code.
  - `test_analyze_with_very_long_lines(self, temp_project_dir)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L221) — Test analyzing file with very long lines.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale)

### `TestMCPServerFileMetricsEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L238)
- doc: Test file metrics calculation edge cases.
- signature: `class TestMCPServerFileMetricsEdgeCases:`
- members:
  - `test_calculate_metrics_with_complex_comments(self, temp_project_dir)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L285) — Test file metrics with complex comment patterns.
  - `test_calculate_metrics_with_mixed_line_endings(self, temp_project_dir)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L241) — Test file metrics with mixed line endings.
  - `test_calculate_metrics_with_nested_comments(self, temp_project_dir)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L308) — Test file metrics with nested comment patterns.
  - `test_calculate_metrics_with_only_blank_lines(self, temp_project_dir)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L271) — Test file metrics with only blank lines.
  - `test_calculate_metrics_with_only_comments(self, temp_project_dir)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L255) — Test file metrics with only comments.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_calculate_file_metrics`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._calculate_file_metrics)

### `TestMCPServerInitializationEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L21)
- doc: Test MCP server initialization edge cases.
- signature: `class TestMCPServerInitializationEdgeCases:`
- members:
  - `test_initialization_with_file_as_project_root(self, temp_project_dir)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L33) — Test initialization with file instead of directory as project root.
  - `test_initialization_with_invalid_project_root(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L24) — Test initialization with invalid project root.
  - `test_initialization_with_permission_denied(self, temp_project_dir)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L46) — Test initialization with permission denied scenario.
  - `test_initialization_with_unicode_path(self, temp_project_dir)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L67) — Test initialization with Unicode characters in path.
  - `test_initialization_with_very_long_path(self, temp_project_dir)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L75) — Test initialization with very long path.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`boundary_manager`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.boundary_manager), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`security_validator`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.security_validator)

### `TestMCPServerLoggingEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L632)
- doc: Test MCP server logging edge cases.
- signature: `class TestMCPServerLoggingEdgeCases:`
- members:
  - `test_server_with_logging_disabled(self, temp_project_dir)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L635) — Test server behavior when logging is disabled or fails.
  - `test_tool_call_with_logging_failure(self, temp_project_dir)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L648) — Test tool calls when logging fails.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized)

### `TestMCPServerResourceHandlingEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L442)
- doc: Test MCP server resource handling edge cases.
- signature: `class TestMCPServerResourceHandlingEdgeCases:`
- members:
  - `test_read_resource_invalid_uri(self, temp_project_dir)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L446) — Test reading resource with invalid URI.
  - `test_read_resource_with_failing_resource(self, temp_project_dir)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L461) — Test reading resource when resource fails.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`_read_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._read_resource)

### `TestMCPServerRuntimeEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L481)
- doc: Test MCP server runtime edge cases.
- signature: `class TestMCPServerRuntimeEdgeCases:`
- members:
  - `test_run_with_initialization_options_failure(self, temp_project_dir)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L510) — Test server run when initialization options fail.
  - `test_run_with_server_creation_failure(self, temp_project_dir)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L498) — Test server run when server creation fails.
  - `test_run_with_stdio_failure(self, temp_project_dir)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L486) — Test server run when stdio fails.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run)

### `TestMCPServerToolHandlingEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L330)
- doc: Test MCP server tool handling edge cases.
- signature: `class TestMCPServerToolHandlingEdgeCases:`
- members:
  - `capture_decorator(name)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L416)
  - `decorator(func)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L417)
  - `server_with_failing_tools(self, temp_project_dir)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L334) — Create a server with tools that fail.
  - `test_tool_call_server_not_initialized(self, temp_project_dir)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L406) — Test tool calls when server is not initialized.
  - `test_tool_call_with_failing_tool(self, server_with_failing_tools)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L389) — Test tool calls when underlying tools fail.
  - `test_tool_call_with_invalid_params(self, temp_project_dir)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L366) — Test tool calls with invalid parameters.
  - `test_tool_call_with_missing_required_params(self, temp_project_dir)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L354) — Test tool calls with missing required parameters.
  - `test_tool_call_with_non_existent_project_path(self, temp_project_dir)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L379) — Test set_project_path with non-existent path.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete), [`_project_root`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._project_root)

### `TestMCPServerUtilityEdgeCases`
- def: [`tests/unit/mcp/test_server_edge_cases.py:523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L523)
- doc: Test MCP server utility function edge cases.
- signature: `class TestMCPServerUtilityEdgeCases:`
- members:
  - `test_main_sync_with_exception(self)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L611) — Test synchronous main function with exception.
  - `test_main_with_environment_variable_issues(self)` — [`L581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L581) — Test main function with problematic environment variables.
  - `test_main_with_general_exception(self)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L553) — Test main function handling general exceptions.
  - `test_main_with_keyboard_interrupt(self)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L536) — Test main function handling keyboard interrupt.
  - `test_main_with_project_root_detection_failure(self)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L564) — Test main function when project root detection fails.
  - `test_parse_args_with_invalid_arguments(self)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_edge_cases.py#L526) — Test parsing invalid command line arguments.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/mcp/server.md#main), [`parse_mcp_args`](../../../tree_sitter_analyzer/mcp/server.md#parse_mcp_args), [`main_sync`](../../../tree_sitter_analyzer/mcp/server.md#main_sync)

