---
title: 'Module: tests/integration/mcp/test_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_integration`/
symbols:
  TestMCPServerIntegration.test_server_initialization: TestMCPServerIntegration#test_server_initialization().
  TestMCPServerIntegration.server: TestMCPServerIntegration#server.
  TestMCPServerIntegration.test_files: TestMCPServerIntegration#test_files.
  TestMCPServerIntegration.test_resource_functionality: TestMCPServerIntegration#test_resource_functionality().
  cleanup_event_loop: cleanup_event_loop().
  TestMCPServerIntegration.teardown_method: TestMCPServerIntegration#teardown_method().
  TestMCPServerIntegration.test_multi_language_support: TestMCPServerIntegration#test_multi_language_support().
  TestMCPServerIntegration.test_complete_analysis_workflow: TestMCPServerIntegration#test_complete_analysis_workflow().
  TestMCPServerIntegration.temp_dir: TestMCPServerIntegration#temp_dir.
  _is_language_support_error: _is_language_support_error().
  TestMCPServerIntegration._create_test_files: TestMCPServerIntegration#_create_test_files().
  _UNSUPPORTED_LANG_KEYWORDS: _UNSUPPORTED_LANG_KEYWORDS.
  _cancel_pending_tasks: _cancel_pending_tasks().
  _cleanup_loop_internals: _cleanup_loop_internals().
  _cleanup_server_instance: _cleanup_server_instance().
  TestMCPServerIntegration: TestMCPServerIntegration#
  TestMCPServerIntegration.setup_method: TestMCPServerIntegration#setup_method().
---
# Module: [`tests/integration/mcp/test_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py)

## Classes
### `TestMCPServerIntegration`
- def: [`tests/integration/mcp/test_integration.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L131)
- doc: Integration tests for the complete MCP server
- signature: `class TestMCPServerIntegration:`
- members:
  - `_create_test_files(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L168) — Create test files for integration testing
  - `setup_method(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L134) — Set up test fixtures
  - `teardown_method(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L150) — Clean up test fixtures
  - `test_complete_analysis_workflow(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L307) — Test complete analysis workflow with multiple tools
  - `test_multi_language_support(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L357) — Test multi-language analysis support
  - `test_resource_functionality(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L390) — Test MCP resource functionality
  - `test_server_initialization(self)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L414) — Test server initialization and configuration — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `server` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L136)
  - `temp_dir` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L139)
  - `test_files` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L140)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`ProjectStatsResource`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`read_resource`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`CodeFileResource`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`read_resource`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`get_error_handler`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#get_error_handler), [`get_performance_monitor`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#get_performance_monitor), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`clear_history`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler.clear_history), [`project_root`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.project_root), [`get_cache_manager`](../../../tree_sitter_analyzer/mcp/utils/__init__.md#get_cache_manager), [`matches_uri`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri), [`matches_uri`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info)  (2 test-only)

## Functions
- `_cancel_pending_tasks(pending: set)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L53) — Cancel pending tasks and wait briefly for them to finish.
- `_cleanup_loop_internals(loop: asyncio.AbstractEventLoop)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L71) — Clear internal loop queues and deregister selector file descriptors.
- `_cleanup_server_instance(server)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L89) — Clear server references to release resources.
- `_is_language_support_error(exc: Exception)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L47) — Return True if exc indicates a missing/unsupported language.
- `cleanup_event_loop()` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L101) — Event loop cleanup fixture (root fix version)

## Module values
- `_UNSUPPORTED_LANG_KEYWORDS` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_integration.py#L35)

