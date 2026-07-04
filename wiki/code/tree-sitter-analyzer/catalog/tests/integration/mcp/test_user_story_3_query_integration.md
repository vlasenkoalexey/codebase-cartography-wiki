---
title: 'Module: tests/integration/mcp/test_user_story_3_query_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_user_story_3_query_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_user_story_3_query_integration`/TestUserStory3QueryIntegration#
symbols:
  TestUserStory3QueryIntegration.tools: tools().
  TestUserStory3QueryIntegration: ''
  TestUserStory3QueryIntegration.temp_project: temp_project().
  TestUserStory3QueryIntegration.test_03_query_code_java_methods: test_03_query_code_java_methods().
  TestUserStory3QueryIntegration.test_04_query_code_typescript_interfaces: test_04_query_code_typescript_interfaces().
  TestUserStory3QueryIntegration.test_05_query_code_python_classes: test_05_query_code_python_classes().
  TestUserStory3QueryIntegration.test_06_query_code_custom_query: test_06_query_code_custom_query().
  TestUserStory3QueryIntegration.test_07_query_with_filter: test_07_query_with_filter().
  TestUserStory3QueryIntegration.test_09_large_file_performance: test_09_large_file_performance().
  TestUserStory3QueryIntegration.test_11_file_output_optimization: test_11_file_output_optimization().
  TestUserStory3QueryIntegration.test_13_markdown_analysis: test_13_markdown_analysis().
---
# Module: [`tests/integration/mcp/test_user_story_3_query_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py)

## Classes
### `TestUserStory3QueryIntegration`
- def: [`tests/integration/mcp/test_user_story_3_query_integration.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L22)
- doc: User Story 3: クエリ実行統合テスト
- signature: `class TestUserStory3QueryIntegration:`
- members:
  - `temp_project(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L26) — テスト用プロジェクト構造を作成
  - `test_03_query_code_java_methods(self, tools, temp_project)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L534) — Javaメソッドクエリテスト
  - `test_04_query_code_typescript_interfaces(self, tools, temp_project)` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L557) — TypeScriptインターフェースクエリテスト
  - `test_05_query_code_python_classes(self, tools, temp_project)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L587) — Pythonクラスクエリテスト
  - `test_06_query_code_custom_query(self, tools, temp_project)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L616) — カスタムクエリテスト
  - `test_07_query_with_filter(self, tools, temp_project)` — [`L646`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L646) — フィルタ付きクエリテスト
  - `test_09_large_file_performance(self, tools, temp_project)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L668) — 大規模ファイルでのパフォーマンステスト
  - `test_11_file_output_optimization(self, tools, temp_project)` — [`L695`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L695) — ファイル出力とトークン最適化テスト
  - `test_13_markdown_analysis(self, tools, temp_project)` — [`L731`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L731) — Markdownファイル解析テスト
  - `tools(self, temp_project)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_3_query_integration.py#L525) — テスト用ツールインスタンスを作成
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool)

