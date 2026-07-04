---
title: 'Module: tests/unit/mcp/test_server_comprehensive_tools.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_server_comprehensive_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_server_comprehensive_tools`/
symbols:
  TestTreeSitterAnalyzerMCPServerProjectPath.test_set_project_path_success: TestTreeSitterAnalyzerMCPServerProjectPath#test_set_project_path_success().
  TestTreeSitterAnalyzerMCPServerToolHandling.capture_decorator: TestTreeSitterAnalyzerMCPServerToolHandling#capture_decorator().
  TestTreeSitterAnalyzerMCPServerProjectPath.test_set_project_path_with_universal_tool: TestTreeSitterAnalyzerMCPServerProjectPath#test_set_project_path_with_universal_tool().
  TestTreeSitterAnalyzerMCPServerProjectPath.test_set_project_path_without_universal_tool: TestTreeSitterAnalyzerMCPServerProjectPath#test_set_project_path_without_universal_tool().
  TestTreeSitterAnalyzerMCPServerToolHandling.decorator: TestTreeSitterAnalyzerMCPServerToolHandling#decorator().
  TestTreeSitterAnalyzerMCPServerRuntime.test_run_success: TestTreeSitterAnalyzerMCPServerRuntime#test_run_success().
  TestTreeSitterAnalyzerMCPServerRuntime.test_run_mcp_unavailable: TestTreeSitterAnalyzerMCPServerRuntime#test_run_mcp_unavailable().
  TestTreeSitterAnalyzerMCPServerRuntime.test_run_with_exception: TestTreeSitterAnalyzerMCPServerRuntime#test_run_with_exception().
  _capture_call_tool_handler.capture_decorator: _capture_call_tool_handler().capture_decorator().
  _capture_call_tool_handler: _capture_call_tool_handler().
  TestTreeSitterAnalyzerMCPServerToolHandling.mock_server_with_tools: TestTreeSitterAnalyzerMCPServerToolHandling#mock_server_with_tools().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_check_code_scale: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_check_code_scale().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_analyze_code_structure: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_analyze_code_structure().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_extract_code_section: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_extract_code_section().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_extract_code_section_batch_requests: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_extract_code_section_batch_requests().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_set_project_path: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_set_project_path().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_unknown_tool: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_unknown_tool().
  TestTreeSitterAnalyzerMCPServerToolHandling.test_handle_call_tool_security_validation: TestTreeSitterAnalyzerMCPServerToolHandling#test_handle_call_tool_security_validation().
  TestMCPServerUtilities.test_parse_mcp_args_default: TestMCPServerUtilities#test_parse_mcp_args_default().
  TestMCPServerUtilities.test_parse_mcp_args_with_project_root: TestMCPServerUtilities#test_parse_mcp_args_with_project_root().
  TestMCPServerUtilities.test_main_with_args: TestMCPServerUtilities#test_main_with_args().
  TestMCPServerUtilities.test_main_with_env_var: TestMCPServerUtilities#test_main_with_env_var().
  TestMCPServerUtilities.test_main_with_auto_detection: TestMCPServerUtilities#test_main_with_auto_detection().
  TestMCPServerUtilities.test_main_with_invalid_placeholder: TestMCPServerUtilities#test_main_with_invalid_placeholder().
  TestMCPServerUtilities.test_main_sync: TestMCPServerUtilities#test_main_sync().
  TestMCPServerUtilities.test_main_exception_handling: TestMCPServerUtilities#test_main_exception_handling().
  _capture_call_tool_handler.capture_decorator.decorator: _capture_call_tool_handler().capture_decorator().decorator().
  TestTreeSitterAnalyzerMCPServerToolHandling: TestTreeSitterAnalyzerMCPServerToolHandling#
  TestTreeSitterAnalyzerMCPServerProjectPath: TestTreeSitterAnalyzerMCPServerProjectPath#
  TestTreeSitterAnalyzerMCPServerRuntime: TestTreeSitterAnalyzerMCPServerRuntime#
  TestMCPServerUtilities: TestMCPServerUtilities#
---
# Module: [`tests/unit/mcp/test_server_comprehensive_tools.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py)

## Classes
### `TestMCPServerUtilities`
- def: [`tests/unit/mcp/test_server_comprehensive_tools.py:485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L485)
- doc: Test MCP server utility functions.
- signature: `class TestMCPServerUtilities:`
- members:
  - `test_main_exception_handling(self)` — [`L607`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L607) — Test main function exception handling.
  - `test_main_sync(self)` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L588) — Test synchronous main function.
  - `test_main_with_args(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L501) — Test main function with command line arguments.
  - `test_main_with_auto_detection(self)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L543) — Test main function with auto-detected project root.
  - `test_main_with_env_var(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L519) — Test main function with environment variable.
  - `test_main_with_invalid_placeholder(self)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L566) — Test main function with invalid placeholder in project root.
  - `test_parse_mcp_args_default(self)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L488) — Test parsing MCP arguments with defaults.
  - `test_parse_mcp_args_with_project_root(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L494) — Test parsing MCP arguments with project root.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/mcp/server.md#main), [`parse_mcp_args`](../../../tree_sitter_analyzer/mcp/server.md#parse_mcp_args), [`main_sync`](../../../tree_sitter_analyzer/mcp/server.md#main_sync)

### `TestTreeSitterAnalyzerMCPServerProjectPath`
- def: [`tests/unit/mcp/test_server_comprehensive_tools.py:390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L390)
- doc: Test MCP server project path management.
- signature: `class TestTreeSitterAnalyzerMCPServerProjectPath:`
- members:
  - `test_set_project_path_success(self, temp_project_dir)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L393) — Test successful project path setting.
  - `test_set_project_path_with_universal_tool(self, temp_project_dir)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L406) — Test project path setting with universal tool.
  - `test_set_project_path_without_universal_tool(self, temp_project_dir)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L422) — Test project path setting without universal tool.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`universal_analyze_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`project_root`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.project_root)

### `TestTreeSitterAnalyzerMCPServerRuntime`
- def: [`tests/unit/mcp/test_server_comprehensive_tools.py:434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L434)
- doc: Test MCP server runtime functionality.
- signature: `class TestTreeSitterAnalyzerMCPServerRuntime:`
- members:
  - `test_run_mcp_unavailable(self, temp_project_dir)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L465) — Test server run when MCP is unavailable.
  - `test_run_success(self, temp_project_dir)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L439) — Test successful server run.
  - `test_run_with_exception(self, temp_project_dir)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L474) — Test server run with exception handling.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run)

### `TestTreeSitterAnalyzerMCPServerToolHandling`
- def: [`tests/unit/mcp/test_server_comprehensive_tools.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L45)
- doc: Test MCP server tool call handling.
- signature: `class TestTreeSitterAnalyzerMCPServerToolHandling:`
- members:
  - `capture_decorator(name)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L87)
  - `decorator(func)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L88)
  - `mock_server_with_tools(self, temp_project_dir)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L49) — Create a server with mocked tools.
  - `test_handle_call_tool_analyze_code_structure(self, mock_server_with_tools)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L121) — Wave C2: ``analyze_code_structure`` is a deprecated legacy name now
  - `test_handle_call_tool_check_code_scale(self, mock_server_with_tools, temp_project_dir)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L73) — Test check_code_scale tool call.
  - `test_handle_call_tool_extract_code_section(self, mock_server_with_tools)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L162) — Wave C2: ``extract_code_section`` is a deprecated legacy name routed
  - `test_handle_call_tool_extract_code_section_batch_requests(self, mock_server_with_tools)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L202) — Wave C2: batch-mode ``extract_code_section`` (``requests`` present)
  - `test_handle_call_tool_security_validation(self, mock_server_with_tools)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L350) — Test security validation in tool calls.
  - `test_handle_call_tool_set_project_path(self, mock_server_with_tools, temp_project_dir)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L261) — Test set_project_path tool call.
  - `test_handle_call_tool_unknown_tool(self, mock_server_with_tools)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L315) — Test handling of unknown tool calls.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

## Functions
- `_capture_call_tool_handler(server)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L20) — Helper: patch Server, call create_server(), return captured call_tool handler.
- `capture_decorator(name)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L27)
- `decorator(func)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_comprehensive_tools.py#L28)

