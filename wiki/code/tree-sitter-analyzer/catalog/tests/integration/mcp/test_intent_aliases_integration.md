---
title: 'Module: tests/integration/mcp/test_intent_aliases_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_intent_aliases_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_intent_aliases_integration`/
symbols:
  server: server().
  TestIntentAliasErrorHandling.test_alias_with_invalid_params_raises_error: TestIntentAliasErrorHandling#test_alias_with_invalid_params_raises_error().
  TestIntentAliasIntegration: TestIntentAliasIntegration#
  TestIntentAliasIntegration.temp_python_file: TestIntentAliasIntegration#temp_python_file().
  TestIntentAliasIntegration.test_locate_usage_alias_calls_search_content: TestIntentAliasIntegration#test_locate_usage_alias_calls_search_content().
  TestIntentAliasIntegration.test_map_structure_alias_calls_list_files: TestIntentAliasIntegration#test_map_structure_alias_calls_list_files().
  TestIntentAliasIntegration.test_extract_structure_alias_calls_analyze_code_structure: TestIntentAliasIntegration#test_extract_structure_alias_calls_analyze_code_structure().
  TestIntentAliasIntegration.test_original_tool_name_still_works: TestIntentAliasIntegration#test_original_tool_name_still_works().
  TestIntentAliasErrorHandling: TestIntentAliasErrorHandling#
  TestIntentAliasErrorHandling.test_unknown_alias_raises_error: TestIntentAliasErrorHandling#test_unknown_alias_raises_error().
  TestMultipleAliasesForSameTool: TestMultipleAliasesForSameTool#
  TestMultipleAliasesForSameTool.temp_dir: TestMultipleAliasesForSameTool#temp_dir().
  TestMultipleAliasesForSameTool.test_map_structure_and_discover_files_same_result: TestMultipleAliasesForSameTool#test_map_structure_and_discover_files_same_result().
  TestMultipleAliasesForSameTool.test_locate_usage_and_find_usage_same_result: TestMultipleAliasesForSameTool#test_locate_usage_and_find_usage_same_result().
  TestAliasWithAllToolParameters: TestAliasWithAllToolParameters#
  TestAliasWithAllToolParameters.temp_dir_with_files: TestAliasWithAllToolParameters#temp_dir_with_files().
  TestAliasWithAllToolParameters.test_locate_usage_supports_all_search_content_params: TestAliasWithAllToolParameters#test_locate_usage_supports_all_search_content_params().
  TestAliasWithAllToolParameters.test_map_structure_supports_all_list_files_params: TestAliasWithAllToolParameters#test_map_structure_supports_all_list_files_params().
---
# Module: [`tests/integration/mcp/test_intent_aliases_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py)

## Classes
### `TestAliasWithAllToolParameters`
- def: [`tests/integration/mcp/test_intent_aliases_integration.py:255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L255)
- doc: 测试 Alias 支持原始工具的所有参数
- signature: `class TestAliasWithAllToolParameters:`
- members:
  - `temp_dir_with_files(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L259) — Create temp directory with multiple files
  - `test_locate_usage_supports_all_search_content_params(self, server, temp_dir_with_files)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L274) — locate_usage 应该支持 search_content 的所有参数
  - `test_map_structure_supports_all_list_files_params(self, server, temp_dir_with_files)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L297) — map_structure 应该支持 list_files 的所有参数

### `TestIntentAliasErrorHandling`
- def: [`tests/integration/mcp/test_intent_aliases_integration.py:158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L158)
- doc: 测试 Intent Alias 的错误处理
- signature: `class TestIntentAliasErrorHandling:`
- members:
  - `test_alias_with_invalid_params_raises_error(self, server)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L168) — Alias + 无效参数应该返回错误
  - `test_unknown_alias_raises_error(self, server)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L162) — 未知的 alias 应该返回错误
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

### `TestIntentAliasIntegration`
- def: [`tests/integration/mcp/test_intent_aliases_integration.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L32)
- doc: 测试 Intent Alias 在 MCP Server 中的集成
- signature: `class TestIntentAliasIntegration:`
- members:
  - `temp_python_file(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L36) — Create a temporary Python file in an isolated directory.
  - `test_extract_structure_alias_calls_analyze_code_structure(self, server, temp_python_file)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L107) — extract_structure alias 应该调用 analyze_code_structure 工具
  - `test_locate_usage_alias_calls_search_content(self, server, temp_python_file)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L62) — locate_usage alias 应该调用 search_content 工具并返回正确格式
  - `test_map_structure_alias_calls_list_files(self, server, temp_python_file)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L86) — map_structure alias 应该调用 list_files 工具并返回正确格式
  - `test_original_tool_name_still_works(self, server, temp_python_file)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L129) — 原始工具名应该仍然有效（向后兼容）

### `TestMultipleAliasesForSameTool`
- def: [`tests/integration/mcp/test_intent_aliases_integration.py:176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L176)
- doc: 测试同一工具的多个 alias
- signature: `class TestMultipleAliasesForSameTool:`
- members:
  - `temp_dir(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L180) — Create temporary directory with files
  - `test_locate_usage_and_find_usage_same_result(self, server, temp_dir)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L223) — locate_usage 和 find_usage 应该返回相同结果
  - `test_map_structure_and_discover_files_same_result(self, server, temp_dir)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L193) — map_structure 和 discover_files 应该返回相同结果

## Functions
- `server()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_intent_aliases_integration.py#L22) — Session-scoped MCP server fixture.

