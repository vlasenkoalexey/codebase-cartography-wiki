---
title: 'Module: compatibility_test/scripts/run_compatibility_test.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/run_compatibility_test.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts.run_compatibility_test`/
symbols:
  StandardizedCompatibilityTester.run_compatibility_test: StandardizedCompatibilityTester#run_compatibility_test().
  StandardizedCompatibilityTester.generate_report: StandardizedCompatibilityTester#generate_report().
  StandardizedCompatibilityTester.run_version_tests: StandardizedCompatibilityTester#run_version_tests().
  StandardizedCompatibilityTester.compare_outputs: StandardizedCompatibilityTester#compare_outputs().
  _load_mcp_tool_class: _load_mcp_tool_class().
  StandardizedCompatibilityTester._generate_cache_report_content: StandardizedCompatibilityTester#_generate_cache_report_content().
  StandardizedCompatibilityTester.setup_directories: StandardizedCompatibilityTester#setup_directories().
  StandardizedCompatibilityTester.cache_manager: StandardizedCompatibilityTester#cache_manager.
  StandardizedCompatibilityTester.compatibility_test_dir: StandardizedCompatibilityTester#compatibility_test_dir.
  StandardizedCompatibilityTester._execute_mcp_tool: StandardizedCompatibilityTester#_execute_mcp_tool().
  StandardizedCompatibilityTester.version_a: StandardizedCompatibilityTester#version_a.
  StandardizedCompatibilityTester.version_b: StandardizedCompatibilityTester#version_b.
  StandardizedCompatibilityTester.cache_reporter: StandardizedCompatibilityTester#cache_reporter.
  StandardizedCompatibilityTester.clear_cache: StandardizedCompatibilityTester#clear_cache.
  StandardizedCompatibilityTester.results_dir: StandardizedCompatibilityTester#results_dir.
  StandardizedCompatibilityTester.version_a_dir: StandardizedCompatibilityTester#version_a_dir.
  StandardizedCompatibilityTester.version_b_dir: StandardizedCompatibilityTester#version_b_dir.
  StandardizedCompatibilityTester.project_root: StandardizedCompatibilityTester#project_root.
  StandardizedCompatibilityTester._cleanup_test_directories: StandardizedCompatibilityTester#_cleanup_test_directories().
  StandardizedCompatibilityTester.load_test_cases: StandardizedCompatibilityTester#load_test_cases().
  StandardizedCompatibilityTester.enable_version: StandardizedCompatibilityTester#enable_version().
  StandardizedCompatibilityTester.execute_test_case: StandardizedCompatibilityTester#execute_test_case().
  StandardizedCompatibilityTester._generate_summary: StandardizedCompatibilityTester#_generate_summary().
  main: main().
  _compare_common_output_files: _compare_common_output_files().
  _compare_output_file: _compare_output_file().
  StandardizedCompatibilityTester.test_cases_file: StandardizedCompatibilityTester#test_cases_file.
  StandardizedCompatibilityTester.load_mcp_settings: StandardizedCompatibilityTester#load_mcp_settings().
  StandardizedCompatibilityTester.save_mcp_settings: StandardizedCompatibilityTester#save_mcp_settings().
  StandardizedCompatibilityTester._process_params: StandardizedCompatibilityTester#_process_params().
  StandardizedCompatibilityTester.test_cases: StandardizedCompatibilityTester#test_cases.
  _list_output_files: _list_output_files().
  StandardizedCompatibilityTester.mcp_settings_path: StandardizedCompatibilityTester#mcp_settings_path.
  StandardizedCompatibilityTester.test_results: StandardizedCompatibilityTester#test_results.
  _set_project_path_result: _set_project_path_result().
  _build_unified_diff: _build_unified_diff().
  _record_missing_output_files: _record_missing_output_files().
  StandardizedCompatibilityTester: StandardizedCompatibilityTester#
  StandardizedCompatibilityTester.wait_for_server_startup: StandardizedCompatibilityTester#wait_for_server_startup().
  StandardizedCompatibilityTester._format_identical_items: StandardizedCompatibilityTester#_format_identical_items().
  StandardizedCompatibilityTester._format_detailed_diffs: StandardizedCompatibilityTester#_format_detailed_diffs().
  StandardizedCompatibilityTester.__init__: StandardizedCompatibilityTester#__init__().
---
# Module: [`compatibility_test/scripts/run_compatibility_test.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py)

## Classes
### `StandardizedCompatibilityTester`
- def: [`compatibility_test/scripts/run_compatibility_test.py:156`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L156)
- signature: `class StandardizedCompatibilityTester:`
- members:
  - `_cleanup_test_directories(self)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L210) — テスト結果とレポートディレクトリをクリーンアップ
  - `_execute_mcp_tool(self, tool_name: str, params: dict[str, Any])` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L384) — 実際のMCPツールを実行
  - `_format_detailed_diffs(self, detailed_diffs: dict[str, str])` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L599) — 詳細差分をフォーマット
  - `_format_identical_items(self, identical_files: list[str])` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L593) — 一致項目をフォーマット
  - `_generate_cache_report_content(self)` — [`L610`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L610) — キャッシュレポートコンテンツを生成
  - `_generate_summary(self, version_a_results: dict[str, Any], version_b_results: dict[str, Any], comparison_results: dict[str, Any])` — [`L575`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L575) — 総評を生成
  - `_process_params(self, params: dict[str, Any])` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L399) — パラメータの{PROJECT_ROOT}などを実際の値に置換
  - `compare_outputs(self)` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L464) — バージョン間の出力を比較
  - `enable_version(self, version: str)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L292) — 指定されたバージョンを有効化し、他を無効化する
  - `execute_test_case(self, tool_name: str, test_case: dict[str, Any], output_dir: Path)` — [`L330`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L330) — 個別のテストケースを実行
  - `generate_report(self, version_a_results: dict[str, Any], version_b_results: dict[str, Any], comparison_results: dict[str, Any])` — [`L495`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L495) — 比較レポートを生成
  - `load_mcp_settings(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L273) — mcp_settings.jsonを読み込む
  - `load_test_cases(self)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L263) — テストケースを読み込み
  - `run_compatibility_test(self)` — [`L634`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L634) — 互換性テストの実行
  - `run_version_tests(self, version: str, output_dir: Path)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L409) — 指定されたバージョンでテストを実行
  - `save_mcp_settings(self, settings: dict[str, Any])` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L282) — mcp_settings.jsonを保存する
  - `setup_directories(self)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L199) — 必要なディレクトリを作成（既存ファイルのクリーンアップを含む）
  - `wait_for_server_startup(self, timeout: int = 10)` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L325) — MCPサーバーの起動を待機
  - `cache_manager` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L176)
  - `cache_reporter` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L177)
  - `clear_cache` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L178)
  - `compatibility_test_dir` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L169)
  - `mcp_settings_path` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L170)
  - `project_root` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L166)
  - `results_dir` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L181)
  - `test_cases` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L187)
  - `test_cases_file` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L186)
  - `test_results` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L190)
  - `version_a` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L164)
  - `version_a_dir` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L182)
  - `version_b` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L165)
  - `version_b_dir` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L183)
- protocol/private: `__init__`[`L157`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L157)
- uses (calls/refs, reference-scoped): [`get_cache_stats`](../utils/cache_manager.md#CacheManager.get_cache_stats), [`_load_mcp_tool_class`](run_compatibility_test.md#_load_mcp_tool_class), [`clear_all_caches`](../utils/cache_manager.md#CacheManager.clear_all_caches), [`generate_cache_report`](../utils/cache_reporter.md#CacheReporter.generate_cache_report), [`CacheManager`](../utils/cache_manager.md#CacheManager), [`CacheReporter`](../utils/cache_reporter.md#CacheReporter), [`_compare_common_output_files`](run_compatibility_test.md#_compare_common_output_files), [`_list_output_files`](run_compatibility_test.md#_list_output_files), [`format_report_for_markdown`](../utils/cache_reporter.md#CacheReporter.format_report_for_markdown), [`_record_missing_output_files`](run_compatibility_test.md#_record_missing_output_files), [`_set_project_path_result`](run_compatibility_test.md#_set_project_path_result)
- used by: [`main`](run_compatibility_test.md#main)

## Functions
- `_build_unified_diff(content_a: str, content_b: str, filename: str, version_a: str, version_b: str)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L127)
- `_compare_common_output_files(comparison_results: dict[str, Any], common_files: set[str], version_a_dir: Path, version_b_dir: Path, version_a: str, version_b: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L83)
- `_compare_output_file(comparison_results: dict[str, Any], file_a: Path, file_b: Path, filename: str, version_a: str, version_b: str)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L102)
- `_list_output_files(output_dir: Path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L77)
- `_load_mcp_tool_class(tool_name: str)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L38)
- `_record_missing_output_files(comparison_results: dict[str, Any], version_a_files: set[str], version_b_files: set[str], version_a: str, version_b: str)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L143)
- `_set_project_path_result(params: dict[str, Any])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L31)
- `main()` — [`L696`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/run_compatibility_test.py#L696) — メイン実行関数

