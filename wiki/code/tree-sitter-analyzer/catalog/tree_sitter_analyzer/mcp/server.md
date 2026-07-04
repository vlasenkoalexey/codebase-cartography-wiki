---
title: 'Module: tree_sitter_analyzer/mcp/server.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/server.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.server`/
symbols:
  TreeSitterAnalyzerMCPServer: TreeSitterAnalyzerMCPServer#
  TreeSitterAnalyzerMCPServer.set_project_path: TreeSitterAnalyzerMCPServer#set_project_path().
  TreeSitterAnalyzerMCPServer._analyze_code_scale: TreeSitterAnalyzerMCPServer#_analyze_code_scale().
  TreeSitterAnalyzerMCPServer.run: TreeSitterAnalyzerMCPServer#run().
  main: main().
  TreeSitterAnalyzerMCPServer.create_server: TreeSitterAnalyzerMCPServer#create_server().
  TreeSitterAnalyzerMCPServer.version: TreeSitterAnalyzerMCPServer#version.
  TreeSitterAnalyzerMCPServer.project_stats_resource: TreeSitterAnalyzerMCPServer#project_stats_resource.
  TreeSitterAnalyzerMCPServer.universal_analyze_tool: TreeSitterAnalyzerMCPServer#universal_analyze_tool.
  _create_tool_registry: _create_tool_registry().
  TreeSitterAnalyzerMCPServer.is_initialized: TreeSitterAnalyzerMCPServer#is_initialized().
  TreeSitterAnalyzerMCPServer.analysis_engine: TreeSitterAnalyzerMCPServer#analysis_engine.
  TreeSitterAnalyzerMCPServer.code_file_resource: TreeSitterAnalyzerMCPServer#code_file_resource.
  TreeSitterAnalyzerMCPServer._calculate_file_metrics: TreeSitterAnalyzerMCPServer#_calculate_file_metrics().
  TreeSitterAnalyzerMCPServer.security_validator: TreeSitterAnalyzerMCPServer#security_validator.
  TreeSitterAnalyzerMCPServer._read_resource: TreeSitterAnalyzerMCPServer#_read_resource().
  logger: logger.
  TreeSitterAnalyzerMCPServer._validate_file_path_security: TreeSitterAnalyzerMCPServer#_validate_file_path_security().
  TreeSitterAnalyzerMCPServer.name: TreeSitterAnalyzerMCPServer#name.
  TreeSitterAnalyzerMCPServer._ensure_registry: TreeSitterAnalyzerMCPServer#_ensure_registry().
  parse_mcp_args: parse_mcp_args().
  TreeSitterAnalyzerMCPServer.call_tool: TreeSitterAnalyzerMCPServer#call_tool().
  TreeSitterAnalyzerMCPServer._initialization_complete: TreeSitterAnalyzerMCPServer#_initialization_complete.
  _log_safely: _log_safely().
  TreeSitterAnalyzerMCPServer.tools: TreeSitterAnalyzerMCPServer#tools().
  MCP_AVAILABLE: MCP_AVAILABLE.
  TreeSitterAnalyzerMCPServer._ensure_initialized: TreeSitterAnalyzerMCPServer#_ensure_initialized().
  main_sync: main_sync().
  UNIVERSAL_TOOL_AVAILABLE: UNIVERSAL_TOOL_AVAILABLE.
  TreeSitterAnalyzerMCPServer._tools: TreeSitterAnalyzerMCPServer#_tools.
  TreeSitterAnalyzerMCPServer._run_server_loop: TreeSitterAnalyzerMCPServer#_run_server_loop().
  TreeSitterAnalyzerMCPServer.tool_instances: TreeSitterAnalyzerMCPServer#tool_instances().
  TreeSitterAnalyzerMCPServer.server: TreeSitterAnalyzerMCPServer#server.
  TreeSitterAnalyzerMCPServer._handle_set_project_path: TreeSitterAnalyzerMCPServer#_handle_set_project_path().
  TreeSitterAnalyzerMCPServer._project_root: TreeSitterAnalyzerMCPServer#_project_root.
  TreeSitterAnalyzerMCPServer.ensure_initialized: TreeSitterAnalyzerMCPServer#ensure_initialized.
  TreeSitterAnalyzerMCPServer.validate_file_path_security: TreeSitterAnalyzerMCPServer#validate_file_path_security.
  TreeSitterAnalyzerMCPServer.handle_set_project_path: TreeSitterAnalyzerMCPServer#handle_set_project_path.
  TreeSitterAnalyzerMCPServer.handle_extract_code_section: TreeSitterAnalyzerMCPServer#handle_extract_code_section.
  TreeSitterAnalyzerMCPServer._registry_built: TreeSitterAnalyzerMCPServer#_registry_built.
  TreeSitterAnalyzerMCPServer._tool_instances: TreeSitterAnalyzerMCPServer#_tool_instances.
  stdio_server: stdio_server.
  _fallback_stdio_server: _fallback_stdio_server().
  _UNKNOWN_URI_PREFIX: _UNKNOWN_URI_PREFIX.
  _MSG_SERVER_ERROR: _MSG_SERVER_ERROR.
  _MSG_SHUTTING_DOWN: _MSG_SHUTTING_DOWN.
  _resolve_relative_path: _resolve_relative_path().
  TreeSitterAnalyzerMCPServer._handle_extract_code_section: TreeSitterAnalyzerMCPServer#_handle_extract_code_section().
  InitializationOptions.__init__: InitializationOptions#__init__().
  TreeSitterAnalyzerMCPServer.__init__: TreeSitterAnalyzerMCPServer#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/server.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py)

## Classes
### `TreeSitterAnalyzerMCPServer`
- def: [`tree_sitter_analyzer/mcp/server.py:114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L114) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP Server for Tree-sitter Analyzer
- signature: `class TreeSitterAnalyzerMCPServer:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L122) — Initialize the MCP server with analyzer components.
  - `_analyze_code_scale(self, arguments: dict[str, Any])` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L248) — Legacy method for analyzing code scale. Delegates to code_scale_handler. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `_calculate_file_metrics(self, file_path: str, language: str)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L260) — Legacy wrapper for file metrics calculation.
  - `_ensure_initialized(self)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L241) — Ensure the server is initialized before processing requests.
  - `_ensure_registry(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L185) — Build the deferred facade tool registry exactly once (idempotent).
  - `_handle_extract_code_section(self, arguments: dict[str, Any])` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L372) — Handle extract_code_section with batch/single mode support.
  - `_handle_set_project_path(self, arguments: dict[str, Any])` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L361) — Handle the set_project_path tool call.
  - `_read_resource(self, uri: str)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L268) — Read a resource by URI; raises ValueError for unknown URIs.
  - `_run_server_loop(self, server: Server, options: Any)` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L425) — Core stdio server I/O loop.
  - `_validate_file_path_security(self, arguments: dict[str, Any])` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L327) — Pre-check file_path arguments for security violations. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `call_tool(self, name: str, arguments: dict[str, Any])` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L204) — Backwards-compatible dispatch.
  - `create_server(self)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L280) — Create, configure, and return the MCP Server instance. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `is_initialized(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L200) — Check if the server is fully initialized.
  - `run(self)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L431) — Run the MCP server via stdio. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `set_project_path(self, project_path: str)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L300) — Set the project path for all components. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `tool_instances(self)` — [`L414`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L414) — Public accessor for _tool_instances (builds the registry on demand).
  - `tools(self)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L420) — Public accessor for _tools (builds the registry on demand).
  - `analysis_engine` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L156)
  - `code_file_resource` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L166)
  - `ensure_initialized` — [`L408`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L408)
  - `handle_extract_code_section` — [`L411`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L411)
  - `handle_set_project_path` — [`L410`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L410)
  - `name` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L170)
  - `project_stats_resource` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L167) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `security_validator` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L157) — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `server` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L138)
  - `universal_analyze_tool` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L160) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `validate_file_path_security` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L409)
  - `version` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L171) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- protocol/private: `_initialization_complete`[`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L139), `_project_root`[`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L140), `_registry_built`[`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L141), `_tool_instances`[`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L142), `_tools`[`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L143)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../security/validator.md#SecurityValidator), [`UniversalAnalyzeTool`](tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`validate_file_path`](../security/validator.md#SecurityValidator.validate_file_path), [`get_analysis_engine`](../core/analysis_engine.md#get_analysis_engine), [`compute_file_metrics`](utils/file_metrics.md#compute_file_metrics), [`ProjectStatsResource`](resources/project_stats_resource.md#ProjectStatsResource), [`CodeFileResource`](resources/code_file_resource.md#CodeFileResource), [`attach_tool_aliases`](_server_helpers.md#attach_tool_aliases), [`MCP_INFO`](__init__.md#MCP_INFO.MCP_INFO), [`get_shared_cache`](../_shared_cache.md#get_shared_cache), [`read_resource`](resources/code_file_resource.md#CodeFileResource.read_resource), [`_create_tool_registry`](server.md#_create_tool_registry), [`resolve`](intent_aliases.md#IntentAliasResolver.resolve), [`set_project_path`](resources/project_stats_resource.md#ProjectStatsResource.set_project_path), [`IntentAliasResolver`](intent_aliases.md#IntentAliasResolver), [`logger`](server.md#logger), [`get_security_validation`](../_shared_cache.md#SharedCache.get_security_validation), [`PlatformDetector`](../platform_compat/detector.md#PlatformDetector), [`dispatch_legacy`](legacy_shim.md#dispatch_legacy), [`set_security_validation`](../_shared_cache.md#SharedCache.set_security_validation), [`analyze_code_scale`](server_utils/code_scale_handler.md#analyze_code_scale), [`clear`](../_shared_cache.md#SharedCache.clear), [`project_root`](resources/project_stats_resource.md#ProjectStatsResource.project_root), [`register_resources`](server_utils/resource_registration.md#register_resources), [`_log_safely`](server.md#_log_safely), [`register_prompts`](server_utils/prompt_registration.md#register_prompts), [`MCP_AVAILABLE`](server.md#MCP_AVAILABLE), [`is_legacy_name`](legacy_shim.md#is_legacy_name), [`UNIVERSAL_TOOL_AVAILABLE`](server.md#UNIVERSAL_TOOL_AVAILABLE), [`build_initialization_options`](_server_helpers.md#build_initialization_options), [`detect_server_version`](_server_helpers.md#detect_server_version), [`init_universal_tool`](_server_helpers.md#init_universal_tool), [`register_tools`](server_utils/tool_registration.md#register_tools), [`stdio_server`](server.md#stdio_server), [`_MSG_SERVER_ERROR`](server.md#_MSG_SERVER_ERROR), [`_MSG_SHUTTING_DOWN`](server.md#_MSG_SHUTTING_DOWN), [`_UNKNOWN_URI_PREFIX`](server.md#_UNKNOWN_URI_PREFIX), [`_resolve_relative_path`](server.md#_resolve_relative_path)
- used by: [`main`](server.md#main), [`start_server_with_initialization_check`](../../start_mcp_server.md#start_server_with_initialization_check)  (218 test-only)

## Functions
- `_create_tool_registry(project_root: str | None)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L105) — Delegates to the single-source registry in ``_tool_registry.py``.
- `_fallback_stdio_server()` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L43)
- `_log_safely(log_fn: Any, msg: str, *args: Any)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L85) — Invoke log_fn, silencing I/O errors (e.g. during shutdown).
- `_resolve_relative_path(base_root: str, file_path: str)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L99) — Resolve a relative file_path against base_root and return the absolute string.
- `main()` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L467) — Main entry point for the MCP server. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- `main_sync()` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L500) — Synchronous entry point for setuptools scripts.
- `parse_mcp_args(args: list[str] | None = None)` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L453) — Parse command line arguments for MCP server.

## Module values
- `MCP_AVAILABLE` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L23)
- `UNIVERSAL_TOOL_AVAILABLE` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L76)
- `_MSG_SERVER_ERROR` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L95)
- `_MSG_SHUTTING_DOWN` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L96)
- `_UNKNOWN_URI_PREFIX` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L94)
- `logger` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L82)
- `stdio_server` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server.py#L20)

