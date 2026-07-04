---
title: 'Module: tests/integration/mcp/test_mcp_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_mcp_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_mcp_integration`/TestMCP
symbols:
  TestMCPServerLifecycle.test_server_components_initialized: ServerLifecycle#test_server_components_initialized().
  TestMCPServerLifecycle.test_server_initialization: ServerLifecycle#test_server_initialization().
  TestMCPServerLifecycle.test_set_project_path: ServerLifecycle#test_set_project_path().
  TestMCPResourcesIntegration.test_project_stats_resource: ResourcesIntegration#test_project_stats_resource().
  TestMCPResourcesIntegration.test_code_file_resource: ResourcesIntegration#test_code_file_resource().
  TestMCPServerLifecycle.test_server_cleanup: ServerLifecycle#test_server_cleanup().
  TestMCPErrorHandling.test_unsupported_language_error: ErrorHandling#test_unsupported_language_error().
  TestMCPPerformanceIntegration.test_performance_monitoring: PerformanceIntegration#test_performance_monitoring().
  TestMCPToolsIntegration.test_analyze_code_scale_tool: ToolsIntegration#test_analyze_code_scale_tool().
  TestMCPErrorHandling.test_invalid_file_path_error: ErrorHandling#test_invalid_file_path_error().
  TestMCPPerformanceIntegration.test_cache_integration: PerformanceIntegration#test_cache_integration().
  TestMCPMultiLanguageIntegration.test_python_analysis: MultiLanguageIntegration#test_python_analysis().
  TestMCPMultiLanguageIntegration.test_javascript_analysis: MultiLanguageIntegration#test_javascript_analysis().
  TestMCPMultiLanguageIntegration.test_java_analysis: MultiLanguageIntegration#test_java_analysis().
  TestMCPConcurrencyIntegration.test_concurrent_analyses: ConcurrencyIntegration#test_concurrent_analyses().
  TestMCPToolsIntegration.test_analyze_code_structure_tool: ToolsIntegration#test_analyze_code_structure_tool().
  TestMCPToolsIntegration.test_extract_code_section_tool: ToolsIntegration#test_extract_code_section_tool().
  TestMCPToolsIntegration.test_query_code_tool: ToolsIntegration#test_query_code_tool().
  TestMCPToolsIntegration.test_file_output_manager_tool: ToolsIntegration#test_file_output_manager_tool().
  TestMCPErrorHandling.test_invalid_query_error: ErrorHandling#test_invalid_query_error().
  TestMCPConcurrencyIntegration.test_concurrent_queries: ConcurrencyIntegration#test_concurrent_queries().
  TestMCPServerLifecycle: ServerLifecycle#
  TestMCPToolsIntegration: ToolsIntegration#
  TestMCPResourcesIntegration: ResourcesIntegration#
  TestMCPErrorHandling: ErrorHandling#
  TestMCPPerformanceIntegration: PerformanceIntegration#
  TestMCPMultiLanguageIntegration: MultiLanguageIntegration#
  TestMCPConcurrencyIntegration: ConcurrencyIntegration#
---
# Module: [`tests/integration/mcp/test_mcp_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py)

## Classes
### `TestMCPConcurrencyIntegration`
- def: [`tests/integration/mcp/test_mcp_integration.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L360)
- doc: Tests for MCP concurrency integration.
- signature: `class TestMCPConcurrencyIntegration:`
- members:
  - `test_concurrent_analyses(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L364) — Test concurrent file analyses.
  - `test_concurrent_queries(self)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L392) — Test concurrent code queries.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale)

### `TestMCPErrorHandling`
- def: [`tests/integration/mcp/test_mcp_integration.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L220)
- doc: Tests for MCP error handling.
- signature: `class TestMCPErrorHandling:`
- members:
  - `test_invalid_file_path_error(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L224) — Test error handling for invalid file path.
  - `test_invalid_query_error(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L250) — Test error handling for invalid query.
  - `test_unsupported_language_error(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L234) — Test error handling for unsupported language.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`UnsupportedLanguageError`](../../../tree_sitter_analyzer/core/_analysis_engine_errors.md#UnsupportedLanguageError)

### `TestMCPMultiLanguageIntegration`
- def: [`tests/integration/mcp/test_mcp_integration.py:314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L314)
- doc: Tests for multi-language MCP integration.
- signature: `class TestMCPMultiLanguageIntegration:`
- members:
  - `test_java_analysis(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L346) — Test Java file analysis.
  - `test_javascript_analysis(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L332) — Test JavaScript file analysis.
  - `test_python_analysis(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L318) — Test Python file analysis.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale)

### `TestMCPPerformanceIntegration`
- def: [`tests/integration/mcp/test_mcp_integration.py:269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L269)
- doc: Tests for MCP performance integration.
- signature: `class TestMCPPerformanceIntegration:`
- members:
  - `test_cache_integration(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L273) — Test cache integration with MCP server.
  - `test_performance_monitoring(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L293) — Test performance monitoring integration.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`get_performance_monitor`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#get_performance_monitor)

### `TestMCPResourcesIntegration`
- def: [`tests/integration/mcp/test_mcp_integration.py:187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L187)
- doc: Tests for MCP resources integration.
- signature: `class TestMCPResourcesIntegration:`
- members:
  - `test_code_file_resource(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L191) — Test code file resource.
  - `test_project_stats_resource(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L205) — Test project statistics resource.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`read_resource`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`read_resource`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`matches_uri`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri), [`matches_uri`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri)

### `TestMCPServerLifecycle`
- def: [`tests/integration/mcp/test_mcp_integration.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L23)
- doc: Tests for MCP server lifecycle management.
- signature: `class TestMCPServerLifecycle:`
- members:
  - `test_server_cleanup(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L69) — Test server cleanup.
  - `test_server_components_initialized(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L33) — Test that all server components are initialized.
  - `test_server_initialization(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L26) — Test server initialization.
  - `test_set_project_path(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L58) — Test setting project path.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`ProjectStatsResource`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`CodeFileResource`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`project_root`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.project_root), [`tools`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.tools), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info), [`server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.server)

### `TestMCPToolsIntegration`
- def: [`tests/integration/mcp/test_mcp_integration.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L82)
- doc: Tests for MCP tools integration.
- signature: `class TestMCPToolsIntegration:`
- members:
  - `test_analyze_code_scale_tool(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L86) — Test analyze_code_scale tool.
  - `test_analyze_code_structure_tool(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L102) — Test analyze_code_structure tool.
  - `test_extract_code_section_tool(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L122) — Test extract_code_section tool.
  - `test_file_output_manager_tool(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L164) — Test file output via tools with output_file parameter.
  - `test_query_code_tool(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_mcp_integration.py#L142) — Test query_code tool.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale)

