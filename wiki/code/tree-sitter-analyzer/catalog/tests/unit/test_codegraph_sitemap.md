---
title: 'Module: tests/unit/test_codegraph_sitemap.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_sitemap.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_sitemap`/
symbols:
  TestSitemapTool._make_tool: TestSitemapTool#_make_tool().
  indexed_project: indexed_project().
  large_indexed_project: large_indexed_project().
  test_sitemap_builders_normalize_cached_slash_paths: test_sitemap_builders_normalize_cached_slash_paths().
  TestSitemapOutputBudget._make_tool: TestSitemapOutputBudget#_make_tool().
  TestSitemapCLI._run_cli: TestSitemapCLI#_run_cli().
  TestSitemapFileLimitTruncation._tool: TestSitemapFileLimitTruncation#_tool().
  TestSitemapTool.test_full_mode: TestSitemapTool#test_full_mode().
  TestSitemapTool.test_api_mode: TestSitemapTool#test_api_mode().
  TestSitemapTool.test_module_mode: TestSitemapTool#test_module_mode().
  TestSitemapTool.test_flat_mode: TestSitemapTool#test_flat_mode().
  TestSitemapTool.test_language_filter: TestSitemapTool#test_language_filter().
  TestSitemapTool.test_directory_filter: TestSitemapTool#test_directory_filter().
  TestSitemapTool.test_empty_cache: TestSitemapTool#test_empty_cache().
  TestSitemapTool.test_tool_definition: TestSitemapTool#test_tool_definition().
  TestSitemapTool.test_validate_arguments_bad_mode: TestSitemapTool#test_validate_arguments_bad_mode().
  TestSitemapOutputBudget.test_flat_mode_capped_by_default: TestSitemapOutputBudget#test_flat_mode_capped_by_default().
  TestSitemapOutputBudget.test_api_mode_capped_by_default: TestSitemapOutputBudget#test_api_mode_capped_by_default().
  TestSitemapOutputBudget.test_max_symbols_param_expands_list: TestSitemapOutputBudget#test_max_symbols_param_expands_list().
  TestSitemapOutputBudget.test_small_project_not_truncated: TestSitemapOutputBudget#test_small_project_not_truncated().
  TestSitemapFileLimitTruncation.test_file_limit_sets_truncated_in_all_modes: TestSitemapFileLimitTruncation#test_file_limit_sets_truncated_in_all_modes().
  TestSitemapFileLimitTruncation.test_truncation_note_absent_when_complete: TestSitemapFileLimitTruncation#test_truncation_note_absent_when_complete().
  TestSitemapFileLimitTruncation.test_non_positive_budget_rejected: TestSitemapFileLimitTruncation#test_non_positive_budget_rejected().
  TestSitemapCLI.test_cli_smoke: TestSitemapCLI#test_cli_smoke().
  TestSitemapCLI.test_cli_api_mode: TestSitemapCLI#test_cli_api_mode().
  TestSitemapCLI.test_cli_module_mode: TestSitemapCLI#test_cli_module_mode().
  TestSitemapCLI.test_cli_max_symbols_flag_truncates: TestSitemapCLI#test_cli_max_symbols_flag_truncates().
  TestSitemapTool: TestSitemapTool#
  TestSitemapOutputBudget: TestSitemapOutputBudget#
  TestSitemapCLI: TestSitemapCLI#
  TestSitemapFileLimitTruncation: TestSitemapFileLimitTruncation#
---
# Module: [`tests/unit/test_codegraph_sitemap.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py)

## Classes
### `TestSitemapCLI`
- def: [`tests/unit/test_codegraph_sitemap.py:255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L255)
- signature: `class TestSitemapCLI:`
- members:
  - `test_cli_api_mode(self, indexed_project, monkeypatch)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L286)
  - `test_cli_max_symbols_flag_truncates(self, large_indexed_project, monkeypatch)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L297) — F3 CLI parity: --codegraph-sitemap-max-symbols bounds the output.
  - `test_cli_module_mode(self, indexed_project, monkeypatch)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L292)
  - `test_cli_smoke(self, indexed_project, monkeypatch)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L280)
- protocol/private: `_run_cli`[`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L256)
- uses (calls/refs, reference-scoped): [`main`](../../tree_sitter_analyzer/cli_main.md#main)

### `TestSitemapFileLimitTruncation`
- def: [`tests/unit/test_codegraph_sitemap.py:335`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L335)
- doc: Codex P2 #337 + reviewer P3s: the max_files LIMIT must also flag
- signature: `class TestSitemapFileLimitTruncation:`
- members:
  - `test_file_limit_sets_truncated_in_all_modes(self, large_indexed_project)` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L347) — When more files exist than max_files, EVERY mode must report
  - `test_non_positive_budget_rejected(self, indexed_project)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L371) — max_symbols / max_files < 1 must raise, not silently negative-slice
  - `test_truncation_note_absent_when_complete(self, indexed_project)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L362) — A complete response must NOT carry an empty truncation_note (reviewer
- protocol/private: `_tool`[`L339`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L339)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.execute), [`CodeGraphSitemapTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool)

### `TestSitemapOutputBudget`
- def: [`tests/unit/test_codegraph_sitemap.py:169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L169)
- doc: F3: bound sitemap symbol output so large repos don't emit a wall of text.
- signature: `class TestSitemapOutputBudget:`
- members:
  - `test_api_mode_capped_by_default(self, large_indexed_project)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L198)
  - `test_flat_mode_capped_by_default(self, large_indexed_project)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L180)
  - `test_max_symbols_param_expands_list(self, large_indexed_project)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L211)
  - `test_small_project_not_truncated(self, indexed_project)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L226)
- protocol/private: `_make_tool`[`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L172)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.execute), [`CodeGraphSitemapTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool)

### `TestSitemapTool`
- def: [`tests/unit/test_codegraph_sitemap.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L47)
- signature: `class TestSitemapTool:`
- members:
  - `test_api_mode(self, indexed_project)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L68)
  - `test_directory_filter(self, indexed_project)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L106)
  - `test_empty_cache(self, tmp_path)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L115)
  - `test_flat_mode(self, indexed_project)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L89)
  - `test_full_mode(self, indexed_project)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L57)
  - `test_language_filter(self, indexed_project)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L97)
  - `test_module_mode(self, indexed_project)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L79)
  - `test_tool_definition(self, indexed_project)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L124)
  - `test_validate_arguments_bad_mode(self, indexed_project)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L130)
- protocol/private: `_make_tool`[`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L48)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.execute), [`CodeGraphSitemapTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.validate_arguments), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.get_tool_definition)

## Functions
- `indexed_project(tmp_path)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L11)
- `large_indexed_project(tmp_path)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L137) — A project whose symbol count exceeds the default max_symbols cap.
- `test_sitemap_builders_normalize_cached_slash_paths(tmp_path)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_sitemap.py#L232)

