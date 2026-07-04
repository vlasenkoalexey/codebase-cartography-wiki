---
title: 'Module: tests/unit/mcp/test_mcp_tools_path_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_tools_path_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_tools_path_resolution`/TestMCPTools
symbols:
  TestMCPToolsPathResolution.test_consistent_path_resolution_across_tools: PathResolution#test_consistent_path_resolution_across_tools().
  TestMCPToolsPathResolution.project_root: PathResolution#project_root.
  TestMCPToolsIntegration.test_all_tools_consistent_initialization: Integration#test_all_tools_consistent_initialization().
  TestMCPToolsIntegration.project_root: Integration#project_root.
  TestMCPToolsPathResolution.test_tools_without_project_root: PathResolution#test_tools_without_project_root().
  TestMCPToolsPathResolution.test_file: PathResolution#test_file.
  TestMCPToolsPathResolution.analyze_scale_tool: PathResolution#analyze_scale_tool.
  TestMCPToolsPathResolution.query_tool: PathResolution#query_tool.
  TestMCPToolsPathResolution.test_analyze_scale_tool_uses_path_resolver: PathResolution#test_analyze_scale_tool_uses_path_resolver().
  TestMCPToolsPathResolution.test_query_tool_uses_path_resolver: PathResolution#test_query_tool_uses_path_resolver().
  TestMCPToolsPathResolution.test_read_partial_tool_uses_path_resolver: PathResolution#test_read_partial_tool_uses_path_resolver().
  TestMCPToolsPathResolution.test_analyze_code_structure_tool_uses_path_resolver: PathResolution#test_analyze_code_structure_tool_uses_path_resolver().
  TestMCPToolsPathResolution.test_universal_analyze_tool_uses_path_resolver: PathResolution#test_universal_analyze_tool_uses_path_resolver().
  TestMCPToolsPathResolution.test_query_tool_execute_with_path_resolution: PathResolution#test_query_tool_execute_with_path_resolution().
  TestMCPToolsIntegration.test_query_tool_execute_with_path_resolution: Integration#test_query_tool_execute_with_path_resolution().
  TestMCPToolsPathResolution.read_partial_tool: PathResolution#read_partial_tool.
  TestMCPToolsPathResolution.analyze_code_structure_tool: PathResolution#analyze_code_structure_tool.
  TestMCPToolsPathResolution.universal_analyze_tool: PathResolution#universal_analyze_tool.
  TestMCPToolsPathResolution.test_cross_platform_path_handling: PathResolution#test_cross_platform_path_handling().
  TestMCPToolsIntegration.java_file: Integration#java_file.
  TestMCPToolsPathResolution.teardown_method: PathResolution#teardown_method().
  TestMCPToolsIntegration.teardown_method: Integration#teardown_method().
  TestMCPToolsPathResolution.temp_dir: PathResolution#temp_dir.
  TestMCPToolsIntegration.temp_dir: Integration#temp_dir.
  TestMCPToolsPathResolution: PathResolution#
  TestMCPToolsPathResolution.setup_method: PathResolution#setup_method().
  TestMCPToolsIntegration: Integration#
  TestMCPToolsIntegration.setup_method: Integration#setup_method().
---
# Module: [`tests/unit/mcp/test_mcp_tools_path_resolution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py)

## Classes
### `TestMCPToolsIntegration`
- def: [`tests/unit/mcp/test_mcp_tools_path_resolution.py:158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L158)
- doc: Integration tests for MCP tools working together.
- signature: `class TestMCPToolsIntegration:`
- members:
  - `setup_method(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L161) — Set up test fixtures.
  - `teardown_method(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L179) — Clean up test fixtures.
  - `test_all_tools_consistent_initialization(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L185) — Test that all tools initialize consistently.
  - `test_query_tool_execute_with_path_resolution(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L202) — Test that QueryTool execute method uses path resolution.
  - `java_file` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L168)
  - `project_root` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L164)
  - `temp_dir` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L163)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`resolve`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve), [`path_resolver`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.path_resolver)

### `TestMCPToolsPathResolution`
- def: [`tests/unit/mcp/test_mcp_tools_path_resolution.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L20)
- doc: Test that all MCP tools use the PathResolver consistently.
- signature: `class TestMCPToolsPathResolution:`
- members:
  - `setup_method(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L23) — Set up test fixtures.
  - `teardown_method(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L41) — Clean up test fixtures.
  - `test_analyze_code_structure_tool_uses_path_resolver(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L75) — Test that AnalyzeCodeStructureTool uses PathResolver.
  - `test_analyze_scale_tool_uses_path_resolver(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L47) — Test that AnalyzeScaleTool uses PathResolver.
  - `test_consistent_path_resolution_across_tools(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L95) — Test that all tools resolve paths consistently.
  - `test_cross_platform_path_handling(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L115) — Test cross-platform path handling in all tools.
  - `test_query_tool_execute_with_path_resolution(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L144) — Test that QueryTool execute method uses path resolution.
  - `test_query_tool_uses_path_resolver(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L57) — Test that QueryTool uses PathResolver.
  - `test_read_partial_tool_uses_path_resolver(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L65) — Test that ReadPartialTool uses PathResolver.
  - `test_tools_without_project_root(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L131) — Test tools initialized without project root.
  - `test_universal_analyze_tool_uses_path_resolver(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L85) — Test that UniversalAnalyzeTool uses PathResolver.
  - `analyze_code_structure_tool` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L38)
  - `analyze_scale_tool` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L35)
  - `project_root` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L26)
  - `query_tool` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L36)
  - `read_partial_tool` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L37)
  - `temp_dir` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L25)
  - `test_file` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L30)
  - `universal_analyze_tool` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_tools_path_resolution.py#L39)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`resolve`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve), [`path_resolver`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.path_resolver), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.project_root)

