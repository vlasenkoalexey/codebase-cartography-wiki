---
title: 'Module: tests/integration/test_phase7_security_integration.py'
type: catalog
provenance: extracted
module: tests/integration/test_phase7_security_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_phase7_security_integration`/
symbols:
  TestPhase7SecurityIntegration.test_security_policy_consistency: TestPhase7SecurityIntegration#test_security_policy_consistency().
  TestPhase7SecurityIntegration.test_path_traversal_protection_comprehensive: TestPhase7SecurityIntegration#test_path_traversal_protection_comprehensive().
  TestPhase7SecurityIntegration.test_malicious_query_protection: TestPhase7SecurityIntegration#test_malicious_query_protection().
  TestPhase7SecurityIntegration.test_unicode_normalization_attacks: TestPhase7SecurityIntegration#test_unicode_normalization_attacks().
  TestPhase7SecurityIntegration.test_concurrent_security_stress: TestPhase7SecurityIntegration#test_concurrent_security_stress().
  TestPhase7SecurityIntegration.test_sensitive_data_exposure_prevention: TestPhase7SecurityIntegration#test_sensitive_data_exposure_prevention().
  TestPhase7SecurityIntegration.test_information_leakage_prevention: TestPhase7SecurityIntegration#test_information_leakage_prevention().
  TestPhase7SecurityIntegration.test_comprehensive_security_validation: TestPhase7SecurityIntegration#test_comprehensive_security_validation().
  TestPhase7SecurityIntegration.test_security_under_load: TestPhase7SecurityIntegration#test_security_under_load().
  secure_test_project: secure_test_project().
  TestPhase7SecurityIntegration: TestPhase7SecurityIntegration#
---
# Module: [`tests/integration/test_phase7_security_integration.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py)

## Classes
### `TestPhase7SecurityIntegration`
- def: [`tests/integration/test_phase7_security_integration.py:82`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L82)
- doc: Phase 7 セキュリティ統合テスト
- signature: `class TestPhase7SecurityIntegration:`
- members:
  - `test_comprehensive_security_validation(self, secure_test_project)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L311) — 包括的セキュリティ検証テスト
  - `test_concurrent_security_stress(self, secure_test_project)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L211) — 同時セキュリティストレステスト
  - `test_information_leakage_prevention(self, secure_test_project)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L255) — 情報漏洩防止テスト
  - `test_malicious_query_protection(self, secure_test_project)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L122) — 悪意のあるクエリ保護テスト
  - `test_path_traversal_protection_comprehensive(self, secure_test_project)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L86) — 包括的パストラバーサル保護テスト
  - `test_security_policy_consistency(self, secure_test_project)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L233) — セキュリティポリシー一貫性テスト
  - `test_security_under_load(self, secure_test_project)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L279) — 負荷下でのセキュリティテスト
  - `test_sensitive_data_exposure_prevention(self, secure_test_project)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L184) — 機密データ露出防止テスト
  - `test_unicode_normalization_attacks(self, secure_test_project)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L164) — Unicode正規化攻撃テスト
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`SearchContentTool`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`ListFilesTool`](../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`AnalyzeCodeStructureTool`](../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FindAndGrepTool`](../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`set_project_path`](../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path)  (19 test-only)

## Functions
- `secure_test_project()` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_phase7_security_integration.py#L68) — セキュリティテスト用プロジェクト作成

