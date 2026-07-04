---
title: 'Module: tests/integration/mcp/test_user_story_4_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_user_story_4_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_user_story_4_integration`/TestUserStory4Integration#
symbols:
  TestUserStory4Integration.mcp_server: mcp_server().
  TestUserStory4Integration: ''
  TestUserStory4Integration.temp_project: temp_project().
  TestUserStory4Integration.test_set_project_path_basic: test_set_project_path_basic().
  TestUserStory4Integration.test_set_project_path_validation: test_set_project_path_validation().
  TestUserStory4Integration.test_find_and_grep_tool_basic: test_find_and_grep_tool_basic().
  TestUserStory4Integration.test_find_and_grep_two_stage_search: test_find_and_grep_two_stage_search().
  TestUserStory4Integration.test_find_and_grep_optimization_features: test_find_and_grep_optimization_features().
  TestUserStory4Integration.test_code_file_resource_access: test_code_file_resource_access().
  TestUserStory4Integration.test_code_file_resource_security: test_code_file_resource_security().
  TestUserStory4Integration.test_project_stats_resource_overview: test_project_stats_resource_overview().
  TestUserStory4Integration.test_project_stats_resource_languages: test_project_stats_resource_languages().
  TestUserStory4Integration.test_project_stats_resource_files: test_project_stats_resource_files().
  TestUserStory4Integration.test_integrated_workflow_scenario_1: test_integrated_workflow_scenario_1().
  TestUserStory4Integration.test_integrated_workflow_scenario_2: test_integrated_workflow_scenario_2().
  TestUserStory4Integration.test_integrated_workflow_scenario_3: test_integrated_workflow_scenario_3().
  TestUserStory4Integration.test_error_handling_integration: test_error_handling_integration().
  TestUserStory4Integration.test_performance_integration: test_performance_integration().
  TestUserStory4Integration.test_concurrent_access_integration: test_concurrent_access_integration().
---
# Module: [`tests/integration/mcp/test_user_story_4_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py)

## Classes
### `TestUserStory4Integration`
- def: [`tests/integration/mcp/test_user_story_4_integration.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L27)
- doc: User Story 4: 統合ワークフロー・プロジェクト管理の統合テスト
- signature: `class TestUserStory4Integration:`
- members:
  - `mcp_server(self, temp_project)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L183) — MCPサーバーインスタンスを作成
  - `temp_project(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L31) — テスト用プロジェクト構造を作成
  - `test_code_file_resource_access(self, mcp_server, temp_project)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L308) — T017: code_file リソースアクセステスト
  - `test_code_file_resource_security(self, mcp_server, temp_project)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L326) — code_file リソースのセキュリティテスト
  - `test_concurrent_access_integration(self, mcp_server, temp_project)` — [`L624`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L624) — 並行アクセス統合テスト
  - `test_error_handling_integration(self, mcp_server, temp_project)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L567) — 統合エラーハンドリングテスト
  - `test_find_and_grep_optimization_features(self, mcp_server, temp_project)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L285) — find_and_grep ツールの最適化機能テスト
  - `test_find_and_grep_tool_basic(self, mcp_server, temp_project)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L217) — T016: find_and_grep ツールの基本機能テスト
  - `test_find_and_grep_two_stage_search(self, mcp_server, temp_project)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L253) — find_and_grep ツールの2段階検索テスト
  - `test_integrated_workflow_scenario_1(self, mcp_server, temp_project)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L422) — 統合ワークフローシナリオ1: プロジェクト分析→検索→詳細確認
  - `test_integrated_workflow_scenario_2(self, mcp_server, temp_project)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L463) — 統合ワークフローシナリオ2: 言語別分析→特定言語検索→複雑度確認
  - `test_integrated_workflow_scenario_3(self, mcp_server, temp_project)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L508) — 統合ワークフローシナリオ3: プロジェクト変更→境界更新→再分析
  - `test_performance_integration(self, mcp_server, temp_project)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L591) — パフォーマンス統合テスト
  - `test_project_stats_resource_files(self, mcp_server, temp_project)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L394) — project_stats リソースのファイル統計テスト
  - `test_project_stats_resource_languages(self, mcp_server, temp_project)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L368) — project_stats リソースの言語統計テスト
  - `test_project_stats_resource_overview(self, mcp_server, temp_project)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L346) — project_stats リソースの概要統計テスト
  - `test_set_project_path_basic(self, mcp_server, temp_project)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L188) — T015: set_project_path の基本機能テスト
  - `test_set_project_path_validation(self, mcp_server)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_4_integration.py#L202) — set_project_path の検証機能テスト
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

