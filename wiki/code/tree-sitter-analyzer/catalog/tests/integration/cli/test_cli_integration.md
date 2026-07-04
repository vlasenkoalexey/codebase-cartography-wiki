---
title: 'Module: tests/integration/cli/test_cli_integration.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_integration`/TestCLI
symbols:
  TestCLIWithMCPServerIntegration.test_mcp_server_initializes: WithMCPServerIntegration#test_mcp_server_initializes().
  TestCLIWithMCPServerIntegration.test_mcp_server_has_required_tools: WithMCPServerIntegration#test_mcp_server_has_required_tools().
  TestCLIWithMCPServerIntegration.test_mcp_server_has_required_resources: WithMCPServerIntegration#test_mcp_server_has_required_resources().
  TestCLICommandFactoryIntegration.test_factory_creates_table_command: CommandFactoryIntegration#test_factory_creates_table_command().
  TestCLICommandFactoryIntegration.test_factory_creates_structure_command: CommandFactoryIntegration#test_factory_creates_structure_command().
  TestCLICommandFactoryIntegration.test_factory_creates_summary_command: CommandFactoryIntegration#test_factory_creates_summary_command().
  TestCLICommandFactoryIntegration.test_factory_creates_advanced_command: CommandFactoryIntegration#test_factory_creates_advanced_command().
  TestCLICommandFactoryIntegration.test_factory_creates_query_command: CommandFactoryIntegration#test_factory_creates_query_command().
  TestCLICommandFactoryIntegration.test_factory_creates_default_command: CommandFactoryIntegration#test_factory_creates_default_command().
  TestCLICommandFactoryIntegration.test_factory_returns_none_without_file: CommandFactoryIntegration#test_factory_returns_none_without_file().
  TestCLIWithMCPServerIntegration.test_mcp_server_set_project_path: WithMCPServerIntegration#test_mcp_server_set_project_path().
  TestCLIArgumentParserIntegration.test_parser_creates_valid_namespace: ArgumentParserIntegration#test_parser_creates_valid_namespace().
  TestCLIArgumentParserIntegration.test_parser_with_all_options: ArgumentParserIntegration#test_parser_with_all_options().
  TestCLIArgumentParserIntegration.test_parser_mutually_exclusive_options: ArgumentParserIntegration#test_parser_mutually_exclusive_options().
  TestCLIFileHandlingIntegration.test_cli_handles_python_file: FileHandlingIntegration#test_cli_handles_python_file().
  TestCLIFileHandlingIntegration.test_cli_handles_javascript_file: FileHandlingIntegration#test_cli_handles_javascript_file().
  TestCLIFileHandlingIntegration.test_cli_handles_java_file: FileHandlingIntegration#test_cli_handles_java_file().
  TestCLIOutputFormatIntegration.test_cli_supports_json_output: OutputFormatIntegration#test_cli_supports_json_output().
  TestCLIOutputFormatIntegration.test_cli_supports_text_output: OutputFormatIntegration#test_cli_supports_text_output().
  TestCLIOutputFormatIntegration.test_cli_supports_toon_output: OutputFormatIntegration#test_cli_supports_toon_output().
  TestCLIOutputFormatIntegration.test_cli_format_alias: OutputFormatIntegration#test_cli_format_alias().
  TestCLIArgumentParserIntegration: ArgumentParserIntegration#
  TestCLICommandFactoryIntegration: CommandFactoryIntegration#
  TestCLIWithMCPServerIntegration: WithMCPServerIntegration#
  TestCLIFileHandlingIntegration: FileHandlingIntegration#
  TestCLIOutputFormatIntegration: OutputFormatIntegration#
---
# Module: [`tests/integration/cli/test_cli_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py)

## Classes
### `TestCLIArgumentParserIntegration`
- def: [`tests/integration/cli/test_cli_integration.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L27)
- doc: Tests for CLI argument parser integration.
- signature: `class TestCLIArgumentParserIntegration:`
- members:
  - `test_parser_creates_valid_namespace(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L30) — Test that parser creates valid namespace.
  - `test_parser_mutually_exclusive_options(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L58) — Test mutually exclusive options.
  - `test_parser_with_all_options(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L37) — Test parser with all options.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

### `TestCLICommandFactoryIntegration`
- def: [`tests/integration/cli/test_cli_integration.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L67)
- doc: Tests for CLI command factory integration.
- signature: `class TestCLICommandFactoryIntegration:`
- members:
  - `test_factory_creates_advanced_command(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L94) — Test factory creates advanced command.
  - `test_factory_creates_default_command(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L108) — Test factory creates default command.
  - `test_factory_creates_query_command(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L101) — Test factory creates query command.
  - `test_factory_creates_structure_command(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L77) — Test factory creates structure command.
  - `test_factory_creates_summary_command(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L84) — Test factory creates summary command.
  - `test_factory_creates_table_command(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L70) — Test factory creates table command.
  - `test_factory_returns_none_without_file(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L115) — Test factory returns ListQueriesCommand for --list-queries.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser), [`create_command`](../../../tree_sitter_analyzer/cli_main.md#CLICommandFactory.create_command), [`CLICommandFactory`](../../../tree_sitter_analyzer/cli_main.md#CLICommandFactory)

### `TestCLIFileHandlingIntegration`
- def: [`tests/integration/cli/test_cli_integration.py:158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L158)
- doc: Tests for CLI file handling integration.
- signature: `class TestCLIFileHandlingIntegration:`
- members:
  - `test_cli_handles_java_file(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L179) — Test CLI handles Java file.
  - `test_cli_handles_javascript_file(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L170) — Test CLI handles JavaScript file.
  - `test_cli_handles_python_file(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L161) — Test CLI handles Python file.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

### `TestCLIOutputFormatIntegration`
- def: [`tests/integration/cli/test_cli_integration.py:189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L189)
- doc: Tests for CLI output format integration.
- signature: `class TestCLIOutputFormatIntegration:`
- members:
  - `test_cli_format_alias(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L213) — Test CLI format alias.
  - `test_cli_supports_json_output(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L192) — Test CLI supports JSON output.
  - `test_cli_supports_text_output(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L199) — Test CLI supports text output.
  - `test_cli_supports_toon_output(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L206) — Test CLI supports TOON output.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

### `TestCLIWithMCPServerIntegration`
- def: [`tests/integration/cli/test_cli_integration.py:124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L124)
- doc: Tests for CLI integration with MCP server.
- signature: `class TestCLIWithMCPServerIntegration:`
- members:
  - `test_mcp_server_has_required_resources(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L143) — Test MCP server has required resources.
  - `test_mcp_server_has_required_tools(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L135) — Test MCP server has required tools.
  - `test_mcp_server_initializes(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L127) — Test MCP server initializes successfully.
  - `test_mcp_server_set_project_path(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_integration.py#L149) — Test MCP server sets project path.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`ProjectStatsResource`](../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`CodeFileResource`](../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`version`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`is_initialized`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.is_initialized), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`name`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.name)

