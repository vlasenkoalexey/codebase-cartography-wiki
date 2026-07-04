---
title: 'Module: tests/unit/mcp/test_server.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_server.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_server`/Test
symbols:
  TestServerInit.test_initialization_creates_resources: ServerInit#test_initialization_creates_resources().
  TestServerInit.test_initialization_with_project_root: ServerInit#test_initialization_with_project_root().
  TestServerInit.test_initialization_without_project_root: ServerInit#test_initialization_without_project_root().
  TestIsInitialized.test_uninitialized_server: IsInitialized#test_uninitialized_server().
  TestEnsureInitialized.test_ensure_initialized_raises_when_not_initialized: EnsureInitialized#test_ensure_initialized_raises_when_not_initialized().
  TestReadResource.test_read_code_file_resource: ReadResource#test_read_code_file_resource().
  TestReadResource.test_read_project_stats_resource: ReadResource#test_read_project_stats_resource().
  TestServerInit.test_initialization_creates_tools: ServerInit#test_initialization_creates_tools().
  TestIsInitialized.server: IsInitialized#server().
  TestEnsureInitialized.server: EnsureInitialized#server().
  TestSetProjectPath.server: SetProjectPath#server().
  TestReadResource.server: ReadResource#server().
  TestParseMCPArgs.test_parse_args_with_project_root: ParseMCPArgs#test_parse_args_with_project_root().
  TestParseMCPArgs.test_parse_args_without_project_root: ParseMCPArgs#test_parse_args_without_project_root().
  TestServerCreation.server: ServerCreation#server().
  TestRegistryDeferral.server: RegistryDeferral#server().
  TestProjectStatsResource.server: ProjectStatsResource#server().
  TestCodeFileResource.server: CodeFileResource#server().
  TestVersionInfo.server: VersionInfo#server().
  TestVersionInfo.test_server_version: VersionInfo#test_server_version().
  TestAnalysisEngine.server: AnalysisEngine#server().
  TestSecurityValidator.server: SecurityValidator#server().
  TestToolDefinitions.server: ToolDefinitions#server().
  TestUniversalTool.server: UniversalTool#server().
  TestTableFormatTool.server: TableFormatTool#server().
  TestResourceInfo.server: ResourceInfo#server().
  TestServerInit: ServerInit#
  TestServerInit.tmp_path: ServerInit#tmp_path().
  TestIsInitialized: IsInitialized#
  TestIsInitialized.test_initialized_server: IsInitialized#test_initialized_server().
  TestEnsureInitialized: EnsureInitialized#
  TestEnsureInitialized.test_ensure_initialized_passes: EnsureInitialized#test_ensure_initialized_passes().
  TestSetProjectPath: SetProjectPath#
  TestSetProjectPath.tmp_path: SetProjectPath#tmp_path().
  TestSetProjectPath.test_set_project_path_valid: SetProjectPath#test_set_project_path_valid().
  TestSetProjectPath.test_set_project_path_updates_resources: SetProjectPath#test_set_project_path_updates_resources().
  TestSetProjectPath.test_set_project_path_invalid_directory: SetProjectPath#test_set_project_path_invalid_directory().
  TestReadResource: ReadResource#
  TestReadResource.test_read_unknown_resource_raises_error: ReadResource#test_read_unknown_resource_raises_error().
  TestParseMCPArgs: ParseMCPArgs#
  TestServerCreation: ServerCreation#
  TestServerCreation.test_create_server_without_mcp_library: ServerCreation#test_create_server_without_mcp_library().
  TestRegistryDeferral: RegistryDeferral#
  TestRegistryDeferral.test_registry_not_built_at_init: RegistryDeferral#test_registry_not_built_at_init().
  TestRegistryDeferral.test_create_server_does_not_build_registry: RegistryDeferral#test_create_server_does_not_build_registry().
  TestRegistryDeferral.test_accessing_tools_builds_registry_once: RegistryDeferral#test_accessing_tools_builds_registry_once().
  TestRegistryDeferral.test_eager_components_available_before_registry: RegistryDeferral#test_eager_components_available_before_registry().
  TestProjectStatsResource: ProjectStatsResource#
  TestProjectStatsResource.test_project_stats_resource_initialized: ProjectStatsResource#test_project_stats_resource_initialized().
  TestProjectStatsResource.test_project_stats_resource_supported_types: ProjectStatsResource#test_project_stats_resource_supported_types().
  TestCodeFileResource: CodeFileResource#
  TestCodeFileResource.test_code_file_resource_initialized: CodeFileResource#test_code_file_resource_initialized().
  TestCodeFileResource.test_code_file_resource_matches_uri: CodeFileResource#test_code_file_resource_matches_uri().
  TestVersionInfo: VersionInfo#
  TestVersionInfo.test_server_name: VersionInfo#test_server_name().
  TestAnalysisEngine: AnalysisEngine#
  TestAnalysisEngine.test_analysis_engine_initialized: AnalysisEngine#test_analysis_engine_initialized().
  TestSecurityValidator: SecurityValidator#
  TestSecurityValidator.test_security_validator_initialized: SecurityValidator#test_security_validator_initialized().
  TestToolDefinitions: ToolDefinitions#
  TestToolDefinitions.test_query_tool_definition: ToolDefinitions#test_query_tool_definition().
  TestToolDefinitions.test_read_partial_tool_definition: ToolDefinitions#test_read_partial_tool_definition().
  TestToolDefinitions.test_analyze_code_structure_tool_definition: ToolDefinitions#test_analyze_code_structure_tool_definition().
  TestToolDefinitions.test_analyze_scale_tool_definition: ToolDefinitions#test_analyze_scale_tool_definition().
  TestToolDefinitions.test_list_files_tool_definition: ToolDefinitions#test_list_files_tool_definition().
  TestToolDefinitions.test_search_content_tool_definition: ToolDefinitions#test_search_content_tool_definition().
  TestToolDefinitions.test_find_and_grep_tool_definition: ToolDefinitions#test_find_and_grep_tool_definition().
  TestToolDefinitions.test_agent_skills_tool_definition: ToolDefinitions#test_agent_skills_tool_definition().
  TestToolDefinitions.test_agent_workflow_tool_definition: ToolDefinitions#test_agent_workflow_tool_definition().
  TestToolDefinitions.test_parser_readiness_tool_definition: ToolDefinitions#test_parser_readiness_tool_definition().
  TestUniversalTool: UniversalTool#
  TestUniversalTool.test_universal_tool_available: UniversalTool#test_universal_tool_available().
  TestTableFormatTool: TableFormatTool#
  TestTableFormatTool.test_table_format_tool_is_alias: TableFormatTool#test_table_format_tool_is_alias().
  TestResourceInfo: ResourceInfo#
  TestResourceInfo.test_code_file_resource_info: ResourceInfo#test_code_file_resource_info().
  TestResourceInfo.test_project_stats_resource_info: ResourceInfo#test_project_stats_resource_info().
---
# Module: [`tests/unit/mcp/test_server.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py)

## Classes
### `TestAnalysisEngine`
- def: [`tests/unit/mcp/test_server.py:337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L337)
- doc: Test analysis engine initialization
- signature: `class TestAnalysisEngine:`
- members:
  - `server(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L341) — Create server instance
  - `test_analysis_engine_initialized(self, server)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L346) — Test analysis engine is initialized
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestCodeFileResource`
- def: [`tests/unit/mcp/test_server.py:299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L299)
- doc: Test code_file_resource initialization
- signature: `class TestCodeFileResource:`
- members:
  - `server(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L303) — Create server instance
  - `test_code_file_resource_initialized(self, server)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L308) — Test code file resource is initialized
  - `test_code_file_resource_matches_uri(self, server)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L312) — Test code file resource URI matching
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestEnsureInitialized`
- def: [`tests/unit/mcp/test_server.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L93)
- doc: Test _ensure_initialized method
- signature: `class TestEnsureInitialized:`
- members:
  - `server(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L97) — Create server instance
  - `test_ensure_initialized_passes(self, server)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L102) — Test ensure_initialized passes when initialized
  - `test_ensure_initialized_raises_when_not_initialized(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L107) — Test ensure_initialized raises when not initialized
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete), [`_ensure_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._ensure_initialized)

### `TestIsInitialized`
- def: [`tests/unit/mcp/test_server.py:72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L72)
- doc: Test is_initialized method
- signature: `class TestIsInitialized:`
- members:
  - `server(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L76) — Create server instance
  - `test_initialized_server(self, server)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L81) — Test initialized server returns True
  - `test_uninitialized_server(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L85) — Test uninitialized server returns False
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`_initialization_complete`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._initialization_complete)

### `TestParseMCPArgs`
- def: [`tests/unit/mcp/test_server.py:190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L190)
- doc: Test parse_mcp_args function
- signature: `class TestParseMCPArgs:`
- members:
  - `test_parse_args_with_project_root(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L193) — Test parsing with project root argument
  - `test_parse_args_without_project_root(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L198) — Test parsing without project root argument
- uses (calls/refs, reference-scoped): [`parse_mcp_args`](../../../tree_sitter_analyzer/mcp/server.md#parse_mcp_args)

### `TestProjectStatsResource`
- def: [`tests/unit/mcp/test_server.py:276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L276)
- doc: Test project_stats_resource initialization
- signature: `class TestProjectStatsResource:`
- members:
  - `server(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L280) — Create server instance
  - `test_project_stats_resource_initialized(self, server)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L285) — Test project stats resource is initialized
  - `test_project_stats_resource_supported_types(self, server)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L290) — Test project stats resource has supported types
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestReadResource`
- def: [`tests/unit/mcp/test_server.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L154)
- doc: Test _read_resource method
- signature: `class TestReadResource:`
- members:
  - `server(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L158) — Create server instance
  - `test_read_code_file_resource(self, server, tmp_path)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L164) — Test reading code file resource
  - `test_read_project_stats_resource(self, server, tmp_path)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L176) — Test reading project stats resource
  - `test_read_unknown_resource_raises_error(self, server)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L184) — Test reading unknown resource raises error
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_read_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._read_resource)

### `TestRegistryDeferral`
- def: [`tests/unit/mcp/test_server.py:221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L221)
- doc: Startup fix: the \~54ms facade tool registry is built lazily.
- signature: `class TestRegistryDeferral:`
- members:
  - `server(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L232)
  - `test_accessing_tools_builds_registry_once(self, server)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L253) — First ``.tools`` access builds the 8 facades; second is a no-op.
  - `test_create_server_does_not_build_registry(self, server)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L242) — create_server registers handlers but must not touch the registry.
  - `test_eager_components_available_before_registry(self, server)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L263) — Cheap eager components must exist without triggering the build.
  - `test_registry_not_built_at_init(self, server)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L236) — Construction must not build the facade registry.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestResourceInfo`
- def: [`tests/unit/mcp/test_server.py:455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L455)
- doc: Test resource information
- signature: `class TestResourceInfo:`
- members:
  - `server(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L459) — Create server instance
  - `test_code_file_resource_info(self, server)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L464) — Test code file resource info
  - `test_project_stats_resource_info(self, server)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L470) — Test project stats resource info
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestSecurityValidator`
- def: [`tests/unit/mcp/test_server.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L351)
- doc: Test security validator initialization
- signature: `class TestSecurityValidator:`
- members:
  - `server(self)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L355) — Create server instance
  - `test_security_validator_initialized(self, server)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L360) — Test security validator is initialized
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestServerCreation`
- def: [`tests/unit/mcp/test_server.py:204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L204)
- doc: Test create_server method
- signature: `class TestServerCreation:`
- members:
  - `server(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L208) — Create server instance
  - `test_create_server_without_mcp_library(self, server)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L213) — Test create_server raises when MCP library not available
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestServerInit`
- def: [`tests/unit/mcp/test_server.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L18)
- doc: Test TreeSitterAnalyzerMCPServer initialization
- signature: `class TestServerInit:`
- members:
  - `test_initialization_creates_resources(self, tmp_path)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L64) — Test that initialization creates resources
  - `test_initialization_creates_tools(self, tmp_path)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L44) — Test that initialization creates all tools
  - `test_initialization_with_project_root(self, tmp_path)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L27) — Test server initialization with project root
  - `test_initialization_without_project_root(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L35) — Test server initialization without project root
  - `tmp_path(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L22) — Create temporary directory
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name), [`project_root`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.project_root), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info)

### `TestSetProjectPath`
- def: [`tests/unit/mcp/test_server.py:116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L116)
- doc: Test set_project_path method
- signature: `class TestSetProjectPath:`
- members:
  - `server(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L120) — Create server instance
  - `test_set_project_path_invalid_directory(self, server)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L146) — Test setting invalid directory uses fallback
  - `test_set_project_path_updates_resources(self, server, tmp_path)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L139) — Test that set_project_path updates resources
  - `test_set_project_path_valid(self, server, tmp_path)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L131) — Test setting valid project path
  - `tmp_path(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L126) — Create temporary directory
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestTableFormatTool`
- def: [`tests/unit/mcp/test_server.py:441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L441)
- doc: Test table format tool (alias)
- signature: `class TestTableFormatTool:`
- members:
  - `server(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L445) — Create server instance
  - `test_table_format_tool_is_alias(self, server)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L450) — Test table format tool is alias of analyze code structure
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestToolDefinitions`
- def: [`tests/unit/mcp/test_server.py:365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L365)
- doc: Test tool definitions
- signature: `class TestToolDefinitions:`
- members:
  - `server(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L369) — Create server instance
  - `test_agent_skills_tool_definition(self, server)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L409) — Test agent skills tool has definition
  - `test_agent_workflow_tool_definition(self, server)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L414) — Test agent workflow tool has definition
  - `test_analyze_code_structure_tool_definition(self, server)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L384) — Test analyze code structure tool has definition
  - `test_analyze_scale_tool_definition(self, server)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L389) — Test analyze scale tool has definition
  - `test_find_and_grep_tool_definition(self, server)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L404) — Test find and grep tool has definition
  - `test_list_files_tool_definition(self, server)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L394) — Test list files tool has definition
  - `test_parser_readiness_tool_definition(self, server)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L419) — Test parser readiness tool has definition
  - `test_query_tool_definition(self, server)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L374) — Test query tool has definition
  - `test_read_partial_tool_definition(self, server)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L379) — Test read partial tool has definition
  - `test_search_content_tool_definition(self, server)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L399) — Test search content tool has definition
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestUniversalTool`
- def: [`tests/unit/mcp/test_server.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L425)
- doc: Test universal tool availability
- signature: `class TestUniversalTool:`
- members:
  - `server(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L429) — Create server instance
  - `test_universal_tool_available(self, server)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L434) — Test universal tool is available if imported
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestVersionInfo`
- def: [`tests/unit/mcp/test_server.py:318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L318)
- doc: Test version information
- signature: `class TestVersionInfo:`
- members:
  - `server(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L322) — Create server instance
  - `test_server_name(self, server)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L327) — Test server name
  - `test_server_version(self, server)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server.py#L331) — Test server version
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`MCP_INFO`](../../../tree_sitter_analyzer/mcp/__init__.md#MCP_INFO.MCP_INFO)

