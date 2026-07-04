---
title: 'Module: tests/unit/test_test_gap_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_test_gap_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_test_gap_tool`/
symbols:
  TestFilePathScoping.test_target_file_scopes_analyzer_totals: TestFilePathScoping#test_target_file_scopes_analyzer_totals().
  TestPackageScopeCollectFiles.test_package_symbols_included_in_scan: TestPackageScopeCollectFiles#test_package_symbols_included_in_scan().
  TestPackageScopeCollectFiles.test_tests_dir_does_not_count_as_production: TestPackageScopeCollectFiles#test_tests_dir_does_not_count_as_production().
  TestPackageScopeCollectFiles.test_test_files_still_used_for_naming_coverage: TestPackageScopeCollectFiles#test_test_files_still_used_for_naming_coverage().
  TestFilePathScoping.test_target_file_default_none_is_project_wide: TestFilePathScoping#test_target_file_default_none_is_project_wide().
  TestFilePathScoping.test_target_file_found_beyond_max_files_walk_order: TestFilePathScoping#test_target_file_found_beyond_max_files_walk_order().
  tool: tool().
  TestCodeGraphTestGapTool.test_validate_no_mode: TestCodeGraphTestGapTool#test_validate_no_mode().
  TestCodeGraphTestGapTool.test_validate_invalid_mode: TestCodeGraphTestGapTool#test_validate_invalid_mode().
  TestCodeGraphTestGapTool.test_validate_file_mode_no_path: TestCodeGraphTestGapTool#test_validate_file_mode_no_path().
  TestCodeGraphTestGapTool.test_execute_no_project_root: TestCodeGraphTestGapTool#test_execute_no_project_root().
  TestPackageScopeCollectFiles.test_max_files_cap_counts_production_files_only: TestPackageScopeCollectFiles#test_max_files_cap_counts_production_files_only().
  TestPackageScopeCollectFiles.test_non_prod_dirs_excluded_from_production: TestPackageScopeCollectFiles#test_non_prod_dirs_excluded_from_production().
  TestPackageScopeCollectFiles._make_project: TestPackageScopeCollectFiles#_make_project().
  TestFilePathScoping._two_file_project: TestFilePathScoping#_two_file_project().
  TestPackageScopeCollectFiles.test_tests_collected_after_production_cap_reached: TestPackageScopeCollectFiles#test_tests_collected_after_production_cap_reached().
  TestFilePathScoping.test_file_path_honored_in_gaps_mode: TestFilePathScoping#test_file_path_honored_in_gaps_mode().
  project_with_code: project_with_code().
  TestCodeGraphTestGapTool: TestCodeGraphTestGapTool#
  TestCodeGraphTestGapTool.test_tool_definition: TestCodeGraphTestGapTool#test_tool_definition().
  TestCodeGraphTestGapTool.test_schema_has_modes: TestCodeGraphTestGapTool#test_schema_has_modes().
  TestCodeGraphTestGapTool.test_output_format_defaults_to_toon: TestCodeGraphTestGapTool#test_output_format_defaults_to_toon().
  TestCodeGraphTestGapTool.test_default_output_is_toon_formatted: TestCodeGraphTestGapTool#test_default_output_is_toon_formatted().
  TestCodeGraphTestGapTool.test_execute_summary: TestCodeGraphTestGapTool#test_execute_summary().
  TestCodeGraphTestGapTool.test_execute_gaps: TestCodeGraphTestGapTool#test_execute_gaps().
  TestCodeGraphTestGapTool.test_execute_gaps_toon_strips_bulk: TestCodeGraphTestGapTool#test_execute_gaps_toon_strips_bulk().
  TestCodeGraphTestGapTool.test_execute_file_mode: TestCodeGraphTestGapTool#test_execute_file_mode().
  TestCodeGraphTestGapTool.test_execute_empty_project: TestCodeGraphTestGapTool#test_execute_empty_project().
  TestPackageScopeCollectFiles: TestPackageScopeCollectFiles#
  TestFilePathScoping: TestFilePathScoping#
---
# Module: [`tests/unit/test_test_gap_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py)

## Classes
### `TestCodeGraphTestGapTool`
- def: [`tests/unit/test_test_gap_tool.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L32)
- signature: `class TestCodeGraphTestGapTool:`
- members:
  - `test_default_output_is_toon_formatted(self, tool, project_with_code)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L52)
  - `test_execute_empty_project(self, tool, tmp_path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L117)
  - `test_execute_file_mode(self, tool, project_with_code)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L100)
  - `test_execute_gaps(self, tool, project_with_code)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L81)
  - `test_execute_gaps_toon_strips_bulk(self, tool, project_with_code)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L91) — Issue #439: in TOON mode the gaps list lives only in toon_content.
  - `test_execute_no_project_root(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L111)
  - `test_execute_summary(self, tool, project_with_code)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L73)
  - `test_output_format_defaults_to_toon(self, tool)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L45)
  - `test_schema_has_modes(self, tool)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L38)
  - `test_tool_definition(self, tool)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L33)
  - `test_validate_file_mode_no_path(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L67)
  - `test_validate_invalid_mode(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L62)
  - `test_validate_no_mode(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L58)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestFilePathScoping`
- def: [`tests/unit/test_test_gap_tool.py:220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L220)
- doc: Issue #693: file_path must scope the analysis, not be a silent no-op.
- signature: `class TestFilePathScoping:`
- members:
  - `_two_file_project(self, tmp_path)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L223) — Two production files with distinct symbol counts, no matching tests.
  - `test_file_path_honored_in_gaps_mode(self, tool, tmp_path)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L261) — #693 core: file_path in the default (gaps) mode scopes the result —
  - `test_target_file_default_none_is_project_wide(self, tmp_path)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L252) — Omitting target_file keeps the existing project-wide behavior.
  - `test_target_file_found_beyond_max_files_walk_order(self, tmp_path)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L277) — Codex #713 P2: a scoped target later than max_files in walk order must
  - `test_target_file_scopes_analyzer_totals(self, tmp_path)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L237) — analyze_coverage_gaps(target_file=...) counts only that file's symbols.
- uses (calls/refs, reference-scoped): (6 test-only callers)

### `TestPackageScopeCollectFiles`
- def: [`tests/unit/test_test_gap_tool.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L124)
- doc: Issue #457: max_files cap must not let test dirs crowd out the package tree.
- signature: `class TestPackageScopeCollectFiles:`
- members:
  - `_make_project(self, tmp_path)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L127) — Multi-package project with a tests/ dir that sorts before pkg/.
  - `test_max_files_cap_counts_production_files_only(self, tmp_path)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L146) — max_files cap must be reached only by production files.
  - `test_non_prod_dirs_excluded_from_production(self, tmp_path)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L205) — corpus/, examples/, benchmarks/ are treated as non-production dirs.
  - `test_package_symbols_included_in_scan(self, tmp_path)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L181) — pkg/sub/module.py symbols must appear in production count even when
  - `test_test_files_still_used_for_naming_coverage(self, tmp_path)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L196) — Tests inside tests/ are still scanned for naming-convention matching
  - `test_tests_collected_after_production_cap_reached(self, tmp_path)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L161) — Codex P2 (#479): the production cap must not stop the walk.
  - `test_tests_dir_does_not_count_as_production(self, tmp_path)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L189) — Files inside tests/ are never counted as production symbols.
- uses (calls/refs, reference-scoped): (5 test-only callers)

## Functions
- `project_with_code(tmp_path)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L17)
- `tool(tmp_path)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_tool.py#L10)

