---
title: 'Module: tests/integration/test_phase7_end_to_end.py'
type: catalog
provenance: extracted
module: tests/integration/test_phase7_end_to_end.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_phase7_end_to_end`/TestPhase7EndToEnd#
symbols:
  TestPhase7EndToEnd._verify_performance_requirements: _verify_performance_requirements().
  TestPhase7EndToEnd.test_complete_enterprise_workflow: test_complete_enterprise_workflow().
  TestPhase7EndToEnd.test_error_recovery_and_resilience: test_error_recovery_and_resilience().
  TestPhase7EndToEnd._analyze_project_overview: _analyze_project_overview().
  TestPhase7EndToEnd._analyze_java_components: _analyze_java_components().
  TestPhase7EndToEnd._analyze_python_components: _analyze_python_components().
  TestPhase7EndToEnd._verify_integration_quality: _verify_integration_quality().
  TestPhase7EndToEnd._simulate_code_investigation: _simulate_code_investigation().
  TestPhase7EndToEnd._simulate_bug_analysis: _simulate_bug_analysis().
  TestPhase7EndToEnd._simulate_refactoring_analysis: _simulate_refactoring_analysis().
  TestPhase7EndToEnd.test_real_world_development_workflow: test_real_world_development_workflow().
  TestPhase7EndToEnd._analyze_language_details: _analyze_language_details().
  TestPhase7EndToEnd.enterprise_project: enterprise_project().
  TestPhase7EndToEnd._analyze_javascript_components: _analyze_javascript_components().
  TestPhase7EndToEnd._verify_security_compliance: _verify_security_compliance().
  TestPhase7EndToEnd.test_performance_under_load: test_performance_under_load().
  TestPhase7EndToEnd._create_java_enterprise_structure: _create_java_enterprise_structure().
  TestPhase7EndToEnd._create_python_enterprise_structure: _create_python_enterprise_structure().
  TestPhase7EndToEnd._create_javascript_enterprise_structure: _create_javascript_enterprise_structure().
  TestPhase7EndToEnd._create_config_and_docs: _create_config_and_docs().
  TestPhase7EndToEnd: ''
---
# Module: [`tests/integration/test_phase7_end_to_end.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py)

## Classes
### `TestPhase7EndToEnd`
- def: [`tests/integration/test_phase7_end_to_end.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L42)
- doc: Phase 7 エンドツーエンド統合テスト
- signature: `class TestPhase7EndToEnd:`
- members:
  - `_analyze_java_components(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L192) — Java コンポーネント分析
  - `_analyze_javascript_components(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L259) — JavaScript コンポーネント分析
  - `_analyze_language_details(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L172) — 各言語の詳細分析
  - `_analyze_project_overview(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L129) — プロジェクト全体の概要分析
  - `_analyze_python_components(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L225) — Python コンポーネント分析
  - `_create_config_and_docs(self, project_root: Path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L77) — 設定ファイルとドキュメント作成
  - `_create_java_enterprise_structure(self, project_root: Path)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L65) — エンタープライズJavaプロジェクト構造
  - `_create_javascript_enterprise_structure(self, project_root: Path)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L73) — エンタープライズJavaScriptプロジェクト構造
  - `_create_python_enterprise_structure(self, project_root: Path)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L69) — エンタープライズPythonプロジェクト構造
  - `_simulate_bug_analysis(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L525) — バグ修正のためのコード分析シミュレーション
  - `_simulate_code_investigation(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L478`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L478) — 新機能開発のためのコード調査シミュレーション
  - `_simulate_refactoring_analysis(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L578`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L578) — リファクタリングのための影響範囲調査シミュレーション
  - `_verify_integration_quality(self, server: TreeSitterAnalyzerMCPServer, project_path: str, overview_results: dict, detailed_results: dict)` — [`L367`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L367) — 統合品質検証
  - `_verify_performance_requirements(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L319) — パフォーマンス要件検証
  - `_verify_security_compliance(self, server: TreeSitterAnalyzerMCPServer, project_path: str)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L280) — セキュリティコンプライアンス検証
  - `enterprise_project(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L46) — エンタープライズ規模のテストプロジェクト作成
  - `test_complete_enterprise_workflow(self, enterprise_project)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L82) — 完全なエンタープライズワークフローテスト
  - `test_error_recovery_and_resilience(self, enterprise_project)` — [`L646`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L646) — エラー回復と回復力テスト
  - `test_performance_under_load(self, enterprise_project)` — [`L626`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L626) — 負荷下でのパフォーマンステスト
  - `test_real_world_development_workflow(self, enterprise_project)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_end_to_end.py#L441) — 実世界の開発ワークフローシミュレーション
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`SearchContentTool`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`QueryTool`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`AnalysisError`](../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`set_project_path`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`execute`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute)  (5 test-only)

