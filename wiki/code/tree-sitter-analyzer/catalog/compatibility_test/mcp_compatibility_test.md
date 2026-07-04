---
title: 'Module: compatibility_test/mcp_compatibility_test.py'
type: catalog
provenance: extracted
module: compatibility_test/mcp_compatibility_test.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.mcp_compatibility_test`/
symbols:
  MCPCompatibilityTester.test_basic_functionality: MCPCompatibilityTester#test_basic_functionality().
  MCPCompatibilityTester.run_compatibility_test: MCPCompatibilityTester#run_compatibility_test().
  main: main().
  MCPCompatibilityTester.enable_version: MCPCompatibilityTester#enable_version().
  MCPCompatibilityTester.verify_tools_configuration: MCPCompatibilityTester#verify_tools_configuration().
  MCPCompatibilityTester.save_results: MCPCompatibilityTester#save_results().
  MCPCompatibilityTester.load_mcp_settings: MCPCompatibilityTester#load_mcp_settings().
  MCP_TOOLS: MCP_TOOLS.
  MCPCompatibilityTester.save_mcp_settings: MCPCompatibilityTester#save_mcp_settings().
  MCPCompatibilityTester.generate_report: MCPCompatibilityTester#generate_report().
  MCPCompatibilityTester.project_root: MCPCompatibilityTester#project_root.
  MCPCompatibilityTester.mcp_settings_path: MCPCompatibilityTester#mcp_settings_path.
  VERSIONS: VERSIONS.
  MCPCompatibilityTester: MCPCompatibilityTester#
  MCPCompatibilityTester.test_set_project_path: MCPCompatibilityTester#test_set_project_path().
  MCPCompatibilityTester.test_list_files: MCPCompatibilityTester#test_list_files().
  MCPCompatibilityTester.test_check_code_scale: MCPCompatibilityTester#test_check_code_scale().
  MCPCompatibilityTester.test_analyze_code_structure: MCPCompatibilityTester#test_analyze_code_structure().
  MCPCompatibilityTester.test_query_code: MCPCompatibilityTester#test_query_code().
  MCPCompatibilityTester.test_extract_code_section: MCPCompatibilityTester#test_extract_code_section().
  MCPCompatibilityTester.test_find_and_grep: MCPCompatibilityTester#test_find_and_grep().
  MCPCompatibilityTester.test_search_content: MCPCompatibilityTester#test_search_content().
  MCPCompatibilityTester.__init__: MCPCompatibilityTester#__init__().
  MCPCompatibilityTester.results: MCPCompatibilityTester#results.
---
# Module: [`compatibility_test/mcp_compatibility_test.py`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py)

## Classes
### `MCPCompatibilityTester`
- def: [`compatibility_test/mcp_compatibility_test.py:29`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L29)
- signature: `class MCPCompatibilityTester:`
- members:
  - `enable_version(self, version: str)` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L57) — 指定されたバージョンを有効化し、他を無効化する
  - `generate_report(self, results: dict[str, Any])` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L244) — テスト結果レポートの生成
  - `load_mcp_settings(self)` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L38) — mcp_settings.jsonを読み込む
  - `run_compatibility_test(self)` — [`L215`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L215) — 互換性テストの実行
  - `save_mcp_settings(self, settings: dict[str, Any])` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L47) — mcp_settings.jsonを保存する
  - `save_results(self, results: dict[str, Any])` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L281) — 結果をファイルに保存
  - `test_analyze_code_structure(self)` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L151) — analyze_code_structureツールのテスト
  - `test_basic_functionality(self, version: str)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L90) — 基本機能のテスト
  - `test_check_code_scale(self)` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L139) — check_code_scaleツールのテスト
  - `test_extract_code_section(self)` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L175) — extract_code_sectionツールのテスト
  - `test_find_and_grep(self)` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L191) — find_and_grepツールのテスト
  - `test_list_files(self)` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L131) — list_filesツールのテスト
  - `test_query_code(self)` — [`L163`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L163) — query_codeツールのテスト
  - `test_search_content(self)` — [`L203`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L203) — search_contentツールのテスト
  - `test_set_project_path(self)` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L123) — set_project_pathツールのテスト
  - `verify_tools_configuration(self, version: str)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L79) — 指定されたバージョンのツール設定を確認する
  - `mcp_settings_path` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L32)
  - `project_root` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L31)
  - `results` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L36)
- protocol/private: `__init__`[`L30`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L30)
- uses (calls/refs, reference-scoped): [`MCP_TOOLS`](mcp_compatibility_test.md#MCP_TOOLS), [`VERSIONS`](mcp_compatibility_test.md#VERSIONS)
- used by: [`main`](mcp_compatibility_test.md#main)

## Functions
- `main()` — [`L305`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L305) — メイン実行関数

## Module values
- `MCP_TOOLS` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L14)
- `VERSIONS` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/compatibility_test/mcp_compatibility_test.py#L26)

