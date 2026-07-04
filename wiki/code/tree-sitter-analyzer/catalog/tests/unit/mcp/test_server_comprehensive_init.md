---
title: 'Module: tests/unit/mcp/test_server_comprehensive_init.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_server_comprehensive_init.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_server_comprehensive_init`/TestTreeSitterAnalyzerMCPServer
symbols:
  TestTreeSitterAnalyzerMCPServerInitialization.test_server_initialization_success: Initialization#test_server_initialization_success().
  TestTreeSitterAnalyzerMCPServerInitialization.test_ensure_initialized_failure: Initialization#test_ensure_initialized_failure().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_missing_file_path: CodeAnalysis#test_analyze_code_scale_missing_file_path().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_not_initialized: CodeAnalysis#test_analyze_code_scale_not_initialized().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_with_universal_tool: CodeAnalysis#test_analyze_code_scale_with_universal_tool().
  TestTreeSitterAnalyzerMCPServerCreation.test_create_server_success: Creation#test_create_server_success().
  TestTreeSitterAnalyzerMCPServerCreation.test_handle_list_tools: Creation#test_handle_list_tools().
  TestTreeSitterAnalyzerMCPServerCreation.test_handle_list_resources: Creation#test_handle_list_resources().
  TestTreeSitterAnalyzerMCPServerInitialization.test_server_initialization_with_universal_tool: Initialization#test_server_initialization_with_universal_tool().
  TestTreeSitterAnalyzerMCPServerInitialization.test_server_initialization_without_universal_tool: Initialization#test_server_initialization_without_universal_tool().
  TestTreeSitterAnalyzerMCPServerInitialization.test_ensure_initialized_success: Initialization#test_ensure_initialized_success().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_success: CodeAnalysis#test_analyze_code_scale_success().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_with_details: CodeAnalysis#test_analyze_code_scale_with_details().
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.test_analyze_code_scale_file_not_found: CodeAnalysis#test_analyze_code_scale_file_not_found().
  TestTreeSitterAnalyzerMCPServerFileMetrics.test_calculate_file_metrics_python: FileMetrics#test_calculate_file_metrics_python().
  TestTreeSitterAnalyzerMCPServerFileMetrics.test_calculate_file_metrics_javascript: FileMetrics#test_calculate_file_metrics_javascript().
  TestTreeSitterAnalyzerMCPServerFileMetrics.test_calculate_file_metrics_java: FileMetrics#test_calculate_file_metrics_java().
  TestTreeSitterAnalyzerMCPServerFileMetrics.test_calculate_file_metrics_multiline_comments: FileMetrics#test_calculate_file_metrics_multiline_comments().
  TestTreeSitterAnalyzerMCPServerFileMetrics.test_calculate_file_metrics_error_handling: FileMetrics#test_calculate_file_metrics_error_handling().
  TestTreeSitterAnalyzerMCPServerCreation.test_create_server_mcp_unavailable: Creation#test_create_server_mcp_unavailable().
  TestTreeSitterAnalyzerMCPServerCreation.test_create_server_tool_registration: Creation#test_create_server_tool_registration().
  TestTreeSitterAnalyzerMCPServerCreation.capture_decorator: Creation#capture_decorator().
  TestTreeSitterAnalyzerMCPServerInitialization.test_server_initialization_with_tools: Initialization#test_server_initialization_with_tools().
  TestTreeSitterAnalyzerMCPServerInitialization.test_server_initialization_with_resources: Initialization#test_server_initialization_with_resources().
  TestTreeSitterAnalyzerMCPServerCreation.decorator: Creation#decorator().
  TestTreeSitterAnalyzerMCPServerInitialization: Initialization#
  TestTreeSitterAnalyzerMCPServerCodeAnalysis: CodeAnalysis#
  TestTreeSitterAnalyzerMCPServerFileMetrics: FileMetrics#
  TestTreeSitterAnalyzerMCPServerCreation: Creation#
  TestTreeSitterAnalyzerMCPServerCodeAnalysis.sample_python_file: CodeAnalysis#sample_python_file().
---
# Module: [`tests/unit/mcp/test_server_comprehensive_init.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py)

## Classes
### `TestTreeSitterAnalyzerMCPServerCodeAnalysis`
- def: [`tests/unit/mcp/test_server_comprehensive_init.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L93)
- doc: Test MCP server code analysis functionality.
- signature: `class TestTreeSitterAnalyzerMCPServerCodeAnalysis:`
- members:
  - `sample_python_file(self, temp_project_dir)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L97) — Create a sample Python file for testing.
  - `test_analyze_code_scale_file_not_found(self, temp_project_dir)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L182) — Test code scale analysis with non-existent file.
  - `test_analyze_code_scale_missing_file_path(self, temp_project_dir)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L169) — Test code scale analysis with missing file_path.
  - `test_analyze_code_scale_not_initialized(self, temp_project_dir)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L192) — Test code scale analysis when server is not initialized.
  - `test_analyze_code_scale_success(self, temp_project_dir, sample_python_file)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L123) — Test successful code scale analysis.
  - `test_analyze_code_scale_with_details(self, temp_project_dir, sample_python_file)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L151) — Test code scale analysis with detailed elements.
  - `test_analyze_code_scale_with_universal_tool(self, temp_project_dir)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L211) — Test code scale analysis delegation to universal tool.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`universal_analyze_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete)

### `TestTreeSitterAnalyzerMCPServerCreation`
- def: [`tests/unit/mcp/test_server_comprehensive_init.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L330)
- doc: Test MCP server creation and configuration.
- signature: `class TestTreeSitterAnalyzerMCPServerCreation:`
- members:
  - `capture_decorator(name)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L378)
  - `decorator(func)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L379)
  - `test_create_server_mcp_unavailable(self, temp_project_dir)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L347) — Test server creation when MCP is unavailable.
  - `test_create_server_success(self, temp_project_dir)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L334) — Test successful server creation.
  - `test_create_server_tool_registration(self, temp_project_dir)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L355) — Test that tools are properly registered.
  - `test_handle_list_resources(self, temp_project_dir)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L415) — Test resource listing functionality.
  - `test_handle_list_tools(self, temp_project_dir)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L372) — Test tool listing functionality.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name)

### `TestTreeSitterAnalyzerMCPServerFileMetrics`
- def: [`tests/unit/mcp/test_server_comprehensive_init.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L227)
- doc: Test MCP server file metrics calculation.
- signature: `class TestTreeSitterAnalyzerMCPServerFileMetrics:`
- members:
  - `test_calculate_file_metrics_error_handling(self, temp_project_dir)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L318) — Test file metrics calculation error handling.
  - `test_calculate_file_metrics_java(self, temp_project_dir)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L276) — Test file metrics calculation for Java file.
  - `test_calculate_file_metrics_javascript(self, temp_project_dir)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L253) — Test file metrics calculation for JavaScript file.
  - `test_calculate_file_metrics_multiline_comments(self, temp_project_dir)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L299) — Test file metrics with complex multiline comments.
  - `test_calculate_file_metrics_python(self, temp_project_dir)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L230) — Test file metrics calculation for Python file.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_calculate_file_metrics`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._calculate_file_metrics)

### `TestTreeSitterAnalyzerMCPServerInitialization`
- def: [`tests/unit/mcp/test_server_comprehensive_init.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L16)
- doc: Test MCP server initialization and setup.
- signature: `class TestTreeSitterAnalyzerMCPServerInitialization:`
- members:
  - `test_ensure_initialized_failure(self, temp_project_dir)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L84) — Test _ensure_initialized when server is not initialized.
  - `test_ensure_initialized_success(self, temp_project_dir)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L77) — Test _ensure_initialized when server is initialized.
  - `test_server_initialization_success(self, temp_project_dir)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L19) — Test successful server initialization.
  - `test_server_initialization_with_resources(self, temp_project_dir)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L49) — Test server initialization includes required resources.
  - `test_server_initialization_with_tools(self, temp_project_dir)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L36) — Test server initialization includes all required tools.
  - `test_server_initialization_with_universal_tool(self, temp_project_dir)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L56) — Test server initialization with optional universal tool.
  - `test_server_initialization_without_universal_tool(self, temp_project_dir)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_init.py#L67) — Test server initialization when universal tool is not available.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`universal_analyze_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`security_validator`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.security_validator), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete), [`_ensure_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._ensure_initialized)

