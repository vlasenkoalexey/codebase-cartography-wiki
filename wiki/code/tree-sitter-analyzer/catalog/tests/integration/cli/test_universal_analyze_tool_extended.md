---
title: 'Module: tests/integration/cli/test_universal_analyze_tool_extended.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_universal_analyze_tool_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_universal_analyze_tool_extended`/TestUniversalAnalyzeTool
symbols:
  TestUniversalAnalyzeToolConfiguration.test_tool_components_initialization: Configuration#test_tool_components_initialization().
  TestUniversalAnalyzeToolConfiguration.test_tool_initialization_with_invalid_project_root: Configuration#test_tool_initialization_with_invalid_project_root().
  TestUniversalAnalyzeToolEdgeCases.tool: EdgeCases#tool().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_empty_file: EdgeCases#test_execute_with_empty_file().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_binary_file: EdgeCases#test_execute_with_binary_file().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_large_file: EdgeCases#test_execute_with_large_file().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_malformed_syntax: EdgeCases#test_execute_with_malformed_syntax().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_unicode_content: EdgeCases#test_execute_with_unicode_content().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_nonexistent_file: EdgeCases#test_execute_with_nonexistent_file().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_invalid_arguments: EdgeCases#test_execute_with_invalid_arguments().
  TestUniversalAnalyzeToolEdgeCases.test_execute_with_path_traversal_attempt: EdgeCases#test_execute_with_path_traversal_attempt().
  TestUniversalAnalyzeToolConfiguration.test_tool_initialization_with_valid_project_root: Configuration#test_tool_initialization_with_valid_project_root().
  TestUniversalAnalyzeToolConfiguration.test_tool_initialization_with_none_project_root: Configuration#test_tool_initialization_with_none_project_root().
  TestUniversalAnalyzeToolPerformance.tool: Performance#tool().
  TestUniversalAnalyzeToolPerformance.test_analysis_with_timeout_scenarios: Performance#test_analysis_with_timeout_scenarios().
  TestUniversalAnalyzeToolIntegration.tool: Integration#tool().
  TestUniversalAnalyzeToolEdgeCases: EdgeCases#
  TestUniversalAnalyzeToolEdgeCases.temp_dir: EdgeCases#temp_dir().
  TestUniversalAnalyzeToolConfiguration: Configuration#
  TestUniversalAnalyzeToolPerformance: Performance#
  TestUniversalAnalyzeToolPerformance.temp_dir: Performance#temp_dir().
  TestUniversalAnalyzeToolPerformance.test_concurrent_analysis: Performance#test_concurrent_analysis().
  TestUniversalAnalyzeToolPerformance.test_memory_usage_with_repeated_analysis: Performance#test_memory_usage_with_repeated_analysis().
  TestUniversalAnalyzeToolIntegration: Integration#
  TestUniversalAnalyzeToolIntegration.temp_dir: Integration#temp_dir().
  TestUniversalAnalyzeToolIntegration.test_tool_with_realistic_python_file: Integration#test_tool_with_realistic_python_file().
  TestUniversalAnalyzeToolIntegration.test_tool_with_realistic_java_file: Integration#test_tool_with_realistic_java_file().
---
# Module: [`tests/integration/cli/test_universal_analyze_tool_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py)

## Classes
### `TestUniversalAnalyzeToolConfiguration`
- def: [`tests/integration/cli/test_universal_analyze_tool_extended.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L205)
- doc: Test UniversalAnalyzeTool configuration and initialization.
- signature: `class TestUniversalAnalyzeToolConfiguration:`
- members:
  - `test_tool_components_initialization(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L240) — Test that tool components are properly initialized.
  - `test_tool_initialization_with_invalid_project_root(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L223) — Test tool initialization with invalid project root.
  - `test_tool_initialization_with_none_project_root(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L217) — Test tool initialization with None project root.
  - `test_tool_initialization_with_valid_project_root(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L208) — Test tool initialization with valid project root.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`security_validator`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.security_validator), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.analysis_engine)

### `TestUniversalAnalyzeToolEdgeCases`
- def: [`tests/integration/cli/test_universal_analyze_tool_extended.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L20)
- doc: Test edge cases and error conditions in UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolEdgeCases:`
- members:
  - `temp_dir(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L24) — Create a temporary directory for testing.
  - `test_execute_with_binary_file(self, tool, temp_dir)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L54) — Test executing analysis on a binary file.
  - `test_execute_with_empty_file(self, tool, temp_dir)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L35) — Test executing analysis on an empty file.
  - `test_execute_with_invalid_arguments(self, tool)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L159) — Test executing with invalid arguments.
  - `test_execute_with_large_file(self, tool, temp_dir)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L73) — Test executing analysis on a large file.
  - `test_execute_with_malformed_syntax(self, tool, temp_dir)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L94) — Test executing analysis on files with malformed syntax.
  - `test_execute_with_nonexistent_file(self, tool)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L145) — Test executing analysis on a non-existent file.
  - `test_execute_with_path_traversal_attempt(self, tool)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L183) — Test executing with path traversal attempts.
  - `test_execute_with_unicode_content(self, tool, temp_dir)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L120) — Test executing analysis on files with Unicode content.
  - `tool(self, temp_dir)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L30) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

### `TestUniversalAnalyzeToolIntegration`
- def: [`tests/integration/cli/test_universal_analyze_tool_extended.py:350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L350)
- doc: Integration tests for UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolIntegration:`
- members:
  - `temp_dir(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L354) — Create a temporary directory for testing.
  - `test_tool_with_realistic_java_file(self, tool, temp_dir)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L417) — Test tool with realistic Java file.
  - `test_tool_with_realistic_python_file(self, tool, temp_dir)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L365) — Test tool with realistic Python file.
  - `tool(self, temp_dir)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L360) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool)

### `TestUniversalAnalyzeToolPerformance`
- def: [`tests/integration/cli/test_universal_analyze_tool_extended.py:254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L254)
- doc: Test UniversalAnalyzeTool performance characteristics.
- signature: `class TestUniversalAnalyzeToolPerformance:`
- members:
  - `temp_dir(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L258) — Create a temporary directory for testing.
  - `test_analysis_with_timeout_scenarios(self, tool, temp_dir)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L322) — Test analysis with potential timeout scenarios.
  - `test_concurrent_analysis(self, tool, temp_dir)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L269) — Test concurrent file analysis.
  - `test_memory_usage_with_repeated_analysis(self, tool, temp_dir)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L294) — Test memory usage with repeated analysis.
  - `tool(self, temp_dir)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_universal_analyze_tool_extended.py#L264) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

