---
title: 'Module: tests/unit/mcp/test_mcp_server.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_server.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_server`/Test
symbols:
  TestMCPServerBasic.test_server_initialization: MCPServerBasic#test_server_initialization().
  TestToolsAndResources.test_resources_initialization: ToolsAndResources#test_resources_initialization().
  TestAnalyzeCodeScale.test_analyze_code_scale_method: AnalyzeCodeScale#test_analyze_code_scale_method().
  TestMCPServerWithMCP.test_create_server_success: MCPServerWithMCP#test_create_server_success().
  TestMCPServerWithMCP.test_run_server_basic: MCPServerWithMCP#test_run_server_basic().
  TestToolsAndResources.test_tools_initialization: ToolsAndResources#test_tools_initialization().
  TestMCPServerBasic.test_set_project_path: MCPServerBasic#test_set_project_path().
  TestMCPServerBasic.test_create_server_mcp_unavailable: MCPServerBasic#test_create_server_mcp_unavailable().
  TestMCPServerBasic.test_run_mcp_unavailable: MCPServerBasic#test_run_mcp_unavailable().
  TestMainFunction.test_main_keyboard_interrupt: MainFunction#test_main_keyboard_interrupt().
  TestMainFunction.test_main_exception_handling: MainFunction#test_main_exception_handling().
  TestMCPAvailability.test_mcp_available_constant: MCPAvailability#test_mcp_available_constant().
  TestFallbackClasses.test_mcp_availability_handling: FallbackClasses#test_mcp_availability_handling().
  TestMCPServerWithMCP.quick_run: MCPServerWithMCP#quick_run().
  TestMCPServerBasic: MCPServerBasic#
  TestMCPServerWithMCP: MCPServerWithMCP#
  TestAnalyzeCodeScale: AnalyzeCodeScale#
  TestMainFunction: MainFunction#
  TestToolsAndResources: ToolsAndResources#
  TestMCPAvailability: MCPAvailability#
  TestFallbackClasses: FallbackClasses#
---
# Module: [`tests/unit/mcp/test_mcp_server.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py)

## Classes
### `TestAnalyzeCodeScale`
- def: [`tests/unit/mcp/test_mcp_server.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L154)
- doc: Test analyze code scale functionality.
- signature: `class TestAnalyzeCodeScale:`
- members:
  - `test_analyze_code_scale_method(self, mock_logger, mock_engine)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L160) — Test _analyze_code_scale method.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`analyze`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine)

### `TestFallbackClasses`
- def: [`tests/unit/mcp/test_mcp_server.py:312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L312)
- doc: Test fallback classes when MCP is not available.
- signature: `class TestFallbackClasses:`
- members:
  - `test_mcp_availability_handling(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L315) — Test that MCP availability is properly handled.
- uses (calls/refs, reference-scoped): [`MCP_AVAILABLE`](../../../tree_sitter_analyzer/mcp/server.md#MCP_AVAILABLE)

### `TestMCPAvailability`
- def: [`tests/unit/mcp/test_mcp_server.py:304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L304)
- doc: Test MCP availability detection.
- signature: `class TestMCPAvailability:`
- members:
  - `test_mcp_available_constant(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L307) — Test MCP_AVAILABLE constant is properly set.
- uses (calls/refs, reference-scoped): [`MCP_AVAILABLE`](../../../tree_sitter_analyzer/mcp/server.md#MCP_AVAILABLE)

### `TestMCPServerBasic`
- def: [`tests/unit/mcp/test_mcp_server.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L19)
- doc: Basic tests for MCP server.
- signature: `class TestMCPServerBasic:`
- members:
  - `test_create_server_mcp_unavailable(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L55) — Test server creation when MCP is unavailable.
  - `test_run_mcp_unavailable(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L67) — Test run when MCP is unavailable.
  - `test_server_initialization(self, mock_logger, mock_engine)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L25) — Test server initialization.
  - `test_set_project_path(self, mock_logger, mock_engine)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L43) — Test setting project path.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.server)

### `TestMCPServerWithMCP`
- def: [`tests/unit/mcp/test_mcp_server.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L86)
- doc: Tests for MCP server when MCP is available.
- signature: `class TestMCPServerWithMCP:`
- members:
  - `quick_run(*args, **kwargs)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L134)
  - `test_create_server_success(self, mock_logger, mock_engine, mock_server_class)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L93) — Test successful server creation.
  - `test_run_server_basic(self, mock_logger, mock_engine, mock_server_class, mock_init_options, mock_stdio_server)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L113) — Test basic server running.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server), [`server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.server)

### `TestMainFunction`
- def: [`tests/unit/mcp/test_mcp_server.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L220)
- doc: Test main function.
- signature: `class TestMainFunction:`
- members:
  - `test_main_exception_handling(self, mock_logger, mock_server_class)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L249) — Test main function handles exceptions.
  - `test_main_keyboard_interrupt(self, mock_logger, mock_server_class)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L225) — Test main function handles KeyboardInterrupt.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/mcp/server.md#main)

### `TestToolsAndResources`
- def: [`tests/unit/mcp/test_mcp_server.py:266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L266)
- doc: Test tools and resources functionality.
- signature: `class TestToolsAndResources:`
- members:
  - `test_resources_initialization(self, mock_logger, mock_engine)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L293) — Test that resources are properly initialized.
  - `test_tools_initialization(self, mock_logger, mock_engine)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server.py#L272) — Test that tools are properly initialized.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`analyze_file`](../../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info)

