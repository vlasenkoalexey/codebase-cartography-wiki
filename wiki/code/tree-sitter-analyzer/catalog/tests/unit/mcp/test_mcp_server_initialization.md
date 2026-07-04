---
title: 'Module: tests/unit/mcp/test_mcp_server_initialization.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_server_initialization.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_server_initialization`/TestMCPServer
symbols:
  TestMCPServerInitialization.test_components_initialized_properly: Initialization#test_components_initialized_properly().
  TestMCPServerErrorHandling.test_initialization_error_handling_in_decorator: ErrorHandling#test_initialization_error_handling_in_decorator().
  TestMCPServerInitialization.test_initialization_with_invalid_project_root: Initialization#test_initialization_with_invalid_project_root().
  TestMCPServerIntegration.test_server_creation_and_basic_functionality: Integration#test_server_creation_and_basic_functionality().
  TestMCPServerInitialization.test_analyze_code_scale_fails_when_not_initialized: Initialization#test_analyze_code_scale_fails_when_not_initialized().
  TestMCPServerInitialization.test_server_metadata_after_initialization: Initialization#test_server_metadata_after_initialization().
  TestMCPServerInitialization.test_initialization_with_none_project_root: Initialization#test_initialization_with_none_project_root().
  TestMCPServerInitialization.test_server_initialization_state: Initialization#test_server_initialization_state().
  TestMCPServerInitialization.test_ensure_initialized_when_not_ready: Initialization#test_ensure_initialized_when_not_ready().
  TestMCPServerInitialization.test_analyze_code_scale_with_initialization_check: Initialization#test_analyze_code_scale_with_initialization_check().
  TestMCPServerIntegration.test_server_handles_concurrent_initialization_checks: Integration#test_server_handles_concurrent_initialization_checks().
  TestMCPServerInitialization.test_ensure_initialized_when_ready: Initialization#test_ensure_initialized_when_ready().
  TestMCPServerInitialization.test_server_run_method_exists: Initialization#test_server_run_method_exists().
  TestMCPServerErrorHandling.test_other_runtime_errors_not_converted: ErrorHandling#test_other_runtime_errors_not_converted().
  TestMCPServerErrorHandling.mock_function: ErrorHandling#mock_function().
  TestMCPServerInitialization.test_server_initialization_logging: Initialization#test_server_initialization_logging().
  TestMCPServerInitialization: Initialization#
  TestMCPServerErrorHandling: ErrorHandling#
  TestMCPServerIntegration: Integration#
---
# Module: [`tests/unit/mcp/test_mcp_server_initialization.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py)

## Classes
### `TestMCPServerErrorHandling`
- def: [`tests/unit/mcp/test_mcp_server_initialization.py:174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L174)
- doc: Test MCP server error handling improvements.
- signature: `class TestMCPServerErrorHandling:`
- members:
  - `mock_function()` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L184)
  - `test_initialization_error_handling_in_decorator(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L178) — Test that the error handling decorator properly handles initialization errors.
  - `test_other_runtime_errors_not_converted(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L198) — Test that other RuntimeErrors are not converted to initialization errors.
- uses (calls/refs, reference-scoped): [`ErrorCategory`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory), [`ErrorSeverity`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity), [`MCPError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`handle_mcp_errors`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#handle_mcp_errors), [`LOW`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorSeverity.LOW), [`CONFIGURATION`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorCategory.CONFIGURATION)

### `TestMCPServerInitialization`
- def: [`tests/unit/mcp/test_mcp_server_initialization.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L26)
- doc: Test MCP server initialization and state management.
- signature: `class TestMCPServerInitialization:`
- members:
  - `test_analyze_code_scale_fails_when_not_initialized(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L91) — Test that analyze_code_scale fails when not initialized.
  - `test_analyze_code_scale_with_initialization_check(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L72) — Test that analyze_code_scale checks initialization.
  - `test_components_initialized_properly(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L113) — Test that all server components are initialized.
  - `test_ensure_initialized_when_not_ready(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L59) — Test _ensure_initialized when server is not ready.
  - `test_ensure_initialized_when_ready(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L51) — Test _ensure_initialized when server is ready.
  - `test_initialization_with_invalid_project_root(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L157) — Test initialization with invalid project root.
  - `test_initialization_with_none_project_root(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L149) — Test initialization with None project root.
  - `test_server_initialization_logging(self, caplog)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L38) — Test that initialization produces proper log messages.
  - `test_server_initialization_state(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L29) — Test that server properly tracks initialization state.
  - `test_server_metadata_after_initialization(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L103) — Test that server metadata is properly set after initialization.
  - `test_server_run_method_exists(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L140) — Test that server has a run method.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`analyze_file`](../../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`MCPError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#MCPError), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`boundary_manager`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.boundary_manager), [`universal_analyze_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`security_validator`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.security_validator), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete), [`_ensure_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._ensure_initialized), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info)

### `TestMCPServerIntegration`
- def: [`tests/unit/mcp/test_mcp_server_initialization.py:212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L212)
- doc: Integration tests for MCP server functionality.
- signature: `class TestMCPServerIntegration:`
- members:
  - `test_server_creation_and_basic_functionality(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L215) — Test basic server creation and functionality.
  - `test_server_handles_concurrent_initialization_checks(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_server_initialization.py#L240) — Test that server handles concurrent initialization checks properly.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`boundary_manager`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.boundary_manager), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`security_validator`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.security_validator), [`project_root`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.project_root), [`_ensure_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._ensure_initialized)

