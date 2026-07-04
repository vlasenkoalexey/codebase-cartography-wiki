---
title: 'Module: tests/integration/mcp/test_user_story_3_extract_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_user_story_3_extract_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_user_story_3_extract_integration`/TestUserStory3ExtractIntegration#
symbols:
  TestUserStory3ExtractIntegration.tools: tools().
  TestUserStory3ExtractIntegration: ''
  TestUserStory3ExtractIntegration.temp_project: temp_project().
  TestUserStory3ExtractIntegration.test_01_extract_code_section_basic: test_01_extract_code_section_basic().
  TestUserStory3ExtractIntegration.test_02_extract_code_section_json_format: test_02_extract_code_section_json_format().
  TestUserStory3ExtractIntegration.test_08_extract_and_query_workflow: test_08_extract_and_query_workflow().
  TestUserStory3ExtractIntegration.test_10_multi_language_consistency: test_10_multi_language_consistency().
  TestUserStory3ExtractIntegration.test_12_error_handling_integration: test_12_error_handling_integration().
  TestUserStory3ExtractIntegration.test_14_concurrent_operations: test_14_concurrent_operations().
  TestUserStory3ExtractIntegration.test_15_comprehensive_workflow: test_15_comprehensive_workflow().
  TestUserStory3ExtractIntegration.test_16_tool_definitions: test_16_tool_definitions().
  TestUserStory3ExtractIntegration.test_17_memory_efficiency: test_17_memory_efficiency().
---
# Module: [`tests/integration/mcp/test_user_story_3_extract_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py)

## Classes
### `TestUserStory3ExtractIntegration`
- def: [`tests/integration/mcp/test_user_story_3_extract_integration.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L23)
- doc: User Story 3: 精密コード抽出・クロスカット統合テスト
- signature: `class TestUserStory3ExtractIntegration:`
- members:
  - `temp_project(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L27) — テスト用プロジェクト構造を作成
  - `test_01_extract_code_section_basic(self, tools, temp_project)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L459) — 基本的なコード抽出機能のテスト
  - `test_02_extract_code_section_json_format(self, tools, temp_project)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L480) — JSON形式でのコード抽出テスト
  - `test_08_extract_and_query_workflow(self, tools, temp_project)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L505) — 抽出→クエリのワークフローテスト
  - `test_10_multi_language_consistency(self, tools, temp_project)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L543) — 多言語での一貫性テスト
  - `test_12_error_handling_integration(self, tools, temp_project)` — [`L589`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L589) — エラーハンドリング統合テスト
  - `test_14_concurrent_operations(self, tools, temp_project)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L619) — 並行操作テスト
  - `test_15_comprehensive_workflow(self, tools, temp_project)` — [`L659`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L659) — 包括的ワークフローテスト
  - `test_16_tool_definitions(self, tools)` — [`L720`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L720) — ツール定義の検証テスト
  - `test_17_memory_efficiency(self, tools, temp_project)` — [`L741`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L741) — メモリ効率性テスト
  - `tools(self, temp_project)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_extract_integration.py#L450) — テスト用ツールインスタンスを作成
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

