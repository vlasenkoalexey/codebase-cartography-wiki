---
title: 'Module: tests/integration/mcp/test_user_story_2_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_user_story_2_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_user_story_2_integration`/
symbols:
  TestUserStory2Integration.extract_tool: TestUserStory2Integration#extract_tool().
  TestUserStory2Integration.list_files_tool: TestUserStory2Integration#list_files_tool().
  TestUserStory2Integration.search_tool: TestUserStory2Integration#search_tool().
  TestUserStory2Integration.test_error_handling_invalid_paths: TestUserStory2Integration#test_error_handling_invalid_paths().
  pytestmark: pytestmark.
  TestUserStory2Integration: TestUserStory2Integration#
  TestUserStory2Integration.temp_project: TestUserStory2Integration#temp_project().
  TestUserStory2Integration.test_extract_code_section_basic: TestUserStory2Integration#test_extract_code_section_basic().
  TestUserStory2Integration.test_extract_code_section_json_format: TestUserStory2Integration#test_extract_code_section_json_format().
  TestUserStory2Integration.test_list_files_basic_search: TestUserStory2Integration#test_list_files_basic_search().
  TestUserStory2Integration.test_list_files_advanced_filtering: TestUserStory2Integration#test_list_files_advanced_filtering().
  TestUserStory2Integration.test_list_files_count_only: TestUserStory2Integration#test_list_files_count_only().
  TestUserStory2Integration.test_search_content_basic: TestUserStory2Integration#test_search_content_basic().
  TestUserStory2Integration.test_search_content_regex_pattern: TestUserStory2Integration#test_search_content_regex_pattern().
  TestUserStory2Integration.test_search_content_count_only: TestUserStory2Integration#test_search_content_count_only().
  TestUserStory2Integration.test_search_content_total_only: TestUserStory2Integration#test_search_content_total_only().
  TestUserStory2Integration.test_workflow_file_discovery_and_analysis: TestUserStory2Integration#test_workflow_file_discovery_and_analysis().
  TestUserStory2Integration.test_workflow_todo_analysis: TestUserStory2Integration#test_workflow_todo_analysis().
  TestUserStory2Integration.test_workflow_configuration_analysis: TestUserStory2Integration#test_workflow_configuration_analysis().
  TestUserStory2Integration.test_performance_large_search: TestUserStory2Integration#test_performance_large_search().
  TestUserStory2Integration.test_file_output_integration: TestUserStory2Integration#test_file_output_integration().
---
# Module: [`tests/integration/mcp/test_user_story_2_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py)

## Classes
### `TestUserStory2Integration`
- def: [`tests/integration/mcp/test_user_story_2_integration.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L27)
- doc: User Story 2: 高度な解析ツール統合テスト
- signature: `class TestUserStory2Integration:`
- members:
  - `extract_tool(self, temp_project)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L404) — ReadPartialTool インスタンス
  - `list_files_tool(self, temp_project)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L409) — ListFilesTool インスタンス
  - `search_tool(self, temp_project)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L414) — SearchContentTool インスタンス
  - `temp_project(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L31) — テスト用プロジェクト構造を作成
  - `test_error_handling_invalid_paths(self, extract_tool, list_files_tool, search_tool)` — [`L730`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L730) — T010-14: エラーハンドリングテスト - 無効なパス
  - `test_extract_code_section_basic(self, extract_tool)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L419) — T010-1: extract_code_section基本機能テスト
  - `test_extract_code_section_json_format(self, extract_tool)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L439) — T010-2: extract_code_section JSON形式出力テスト
  - `test_file_output_integration(self, search_tool, extract_tool, temp_project)` — [`L761`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L761) — T010-15: ファイル出力統合テスト
  - `test_list_files_advanced_filtering(self, list_files_tool)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L474) — T010-4: list_files高度フィルタリングテスト
  - `test_list_files_basic_search(self, list_files_tool)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L458) — T010-3: list_files基本検索テスト
  - `test_list_files_count_only(self, list_files_tool)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L495) — T010-5: list_filesカウントモードテスト
  - `test_performance_large_search(self, search_tool)` — [`L706`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L706) — T010-13: パフォーマンステスト - 大規模検索
  - `test_search_content_basic(self, search_tool)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L510) — T010-6: search_content基本検索テスト
  - `test_search_content_count_only(self, search_tool)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L551) — T010-8: search_contentカウントモードテスト
  - `test_search_content_regex_pattern(self, search_tool)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L528) — T010-7: search_content正規表現パターンテスト
  - `test_search_content_total_only(self, search_tool)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L564) — T010-9: search_content合計モードテスト
  - `test_workflow_configuration_analysis(self, list_files_tool, search_tool, extract_tool)` — [`L658`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L658) — T010-12: ワークフロー統合テスト - 設定ファイル分析
  - `test_workflow_file_discovery_and_analysis(self, list_files_tool, search_tool, extract_tool)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L575) — T010-10: ワークフロー統合テスト - ファイル発見→検索→抽出
  - `test_workflow_todo_analysis(self, search_tool, extract_tool)` — [`L621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L621) — T010-11: ワークフロー統合テスト - TODO分析
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

## Module values
- `pytestmark` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_2_integration.py#L24)

