---
title: 'Module: tests/unit/security/test_mcp_security.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_mcp_security.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_mcp_security`/
symbols:
  TestInputValidation.test_file_path_validation: TestInputValidation#test_file_path_validation().
  TestInputValidation.test_long_path_attack: TestInputValidation#test_long_path_attack().
  TestSecurityBestPractices.test_concurrent_request_handling: TestSecurityBestPractices#test_concurrent_request_handling().
  TestInputValidation.test_null_byte_injection: TestInputValidation#test_null_byte_injection().
  TestInputValidation.test_special_character_injection: TestInputValidation#test_special_character_injection().
  TestProjectBoundaryProtection.test_path_traversal_prevention: TestProjectBoundaryProtection#test_path_traversal_prevention().
  TestSecurityBestPractices.test_input_sanitization: TestSecurityBestPractices#test_input_sanitization().
  TestSecurityBestPractices.test_resource_limits: TestSecurityBestPractices#test_resource_limits().
  TestSecurityBestPractices.test_timeout_protection: TestSecurityBestPractices#test_timeout_protection().
  security_validator: security_validator().
  TestInputValidation.test_directory_path_validation: TestInputValidation#test_directory_path_validation().
  TestInputValidation.test_unicode_normalization_attack: TestInputValidation#test_unicode_normalization_attack().
  TestProjectBoundaryProtection.test_absolute_path_restriction: TestProjectBoundaryProtection#test_absolute_path_restriction().
  TestProjectBoundaryProtection.test_symlink_traversal_prevention: TestProjectBoundaryProtection#test_symlink_traversal_prevention().
  TestProjectBoundaryProtection.test_project_root_enforcement: TestProjectBoundaryProtection#test_project_root_enforcement().
  TestInformationLeakagePrevention.test_error_message_sanitization: TestInformationLeakagePrevention#test_error_message_sanitization().
  TestInformationLeakagePrevention.test_stack_trace_filtering: TestInformationLeakagePrevention#test_stack_trace_filtering().
  TestInformationLeakagePrevention.test_file_content_filtering: TestInformationLeakagePrevention#test_file_content_filtering().
  TestSecurityConfiguration.test_security_headers_and_metadata: TestSecurityConfiguration#test_security_headers_and_metadata().
  safe_project_structure: safe_project_structure().
  malicious_paths: malicious_paths().
  TestInputValidation: TestInputValidation#
  TestProjectBoundaryProtection: TestProjectBoundaryProtection#
  TestInformationLeakagePrevention: TestInformationLeakagePrevention#
  TestSecurityBestPractices: TestSecurityBestPractices#
  TestSecurityBestPractices.test_security_validator_initialization: TestSecurityBestPractices#test_security_validator_initialization().
  TestSecurityConfiguration: TestSecurityConfiguration#
  TestSecurityConfiguration.test_default_security_settings: TestSecurityConfiguration#test_default_security_settings().
---
# Module: [`tests/unit/security/test_mcp_security.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py)

## Classes
### `TestInformationLeakagePrevention`
- def: [`tests/unit/security/test_mcp_security.py:238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L238)
- doc: 情報漏洩防止の確認
- signature: `class TestInformationLeakagePrevention:`
- members:
  - `test_error_message_sanitization(self, safe_project_structure)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L242) — エラーメッセージのサニタイゼーション
  - `test_file_content_filtering(self, tmp_path)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L254) — ファイル内容のフィルタリング
  - `test_stack_trace_filtering(self, safe_project_structure)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L248) — スタックトレースのフィルタリング
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestInputValidation`
- def: [`tests/unit/security/test_mcp_security.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L81)
- doc: 入力検証の包括的テスト
- signature: `class TestInputValidation:`
- members:
  - `test_directory_path_validation(self, safe_project_structure, malicious_paths)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L97) — ディレクトリパス検証テスト
  - `test_file_path_validation(self, safe_project_structure, malicious_paths)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L85) — ファイルパス検証テスト
  - `test_long_path_attack(self, safe_project_structure)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L141) — 長いパス攻撃の防御テスト
  - `test_null_byte_injection(self, safe_project_structure)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L105) — ヌルバイト注入攻撃の防御テスト
  - `test_special_character_injection(self, safe_project_structure)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L152) — 特殊文字注入攻撃の防御テスト
  - `test_unicode_normalization_attack(self, safe_project_structure)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L129) — Unicode正規化攻撃の防御テスト
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`ValidationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ValidationError)  (2 test-only)

### `TestProjectBoundaryProtection`
- def: [`tests/unit/security/test_mcp_security.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L179)
- doc: プロジェクト境界保護の検証
- signature: `class TestProjectBoundaryProtection:`
- members:
  - `test_absolute_path_restriction(self, safe_project_structure)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L210) — 絶対パス制限テスト
  - `test_path_traversal_prevention(self, safe_project_structure)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L183) — パストラバーサル攻撃の防御テスト
  - `test_project_root_enforcement(self, safe_project_structure)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L232) — プロジェクトルート強制テスト
  - `test_symlink_traversal_prevention(self, tmp_path)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L226) — シンボリックリンクトラバーサル防御テスト
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute)  (3 test-only)

### `TestSecurityBestPractices`
- def: [`tests/unit/security/test_mcp_security.py:260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L260)
- doc: セキュリティベストプラクティスの適用確認
- signature: `class TestSecurityBestPractices:`
- members:
  - `test_concurrent_request_handling(self, safe_project_structure)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L336) — 同時リクエスト処理の確認
  - `test_input_sanitization(self, safe_project_structure)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L271) — 入力サニタイゼーションの確認
  - `test_resource_limits(self, safe_project_structure)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L295) — リソース制限の確認
  - `test_security_validator_initialization(self, security_validator)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L263) — セキュリティバリデーターの初期化確認
  - `test_timeout_protection(self, safe_project_structure)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L316) — タイムアウト保護の確認
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`ValidationError`](../../../tree_sitter_analyzer/_exceptions_core.md#ValidationError)

### `TestSecurityConfiguration`
- def: [`tests/unit/security/test_mcp_security.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L360)
- doc: セキュリティ設定の確認
- signature: `class TestSecurityConfiguration:`
- members:
  - `test_default_security_settings(self, security_validator)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L363) — デフォルトセキュリティ設定の確認
  - `test_security_headers_and_metadata(self)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L380) — セキュリティヘッダーとメタデータの確認
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool)

## Functions
- `malicious_paths()` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L63) — 悪意のあるパス例
- `safe_project_structure(tmp_path)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L45) — 安全なプロジェクト構造
- `security_validator()` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_mcp_security.py#L39) — セキュリティバリデーター

