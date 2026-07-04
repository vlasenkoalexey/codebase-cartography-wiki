---
title: 'Module: tests/unit/mcp/test_utils/test_gitignore_detector.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_gitignore_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_gitignore_detector`/Test
symbols:
  TestIntegration.test_full_detection_workflow: Integration#test_full_detection_workflow().
  TestGitignoreDetectorInit.test_initialization: GitignoreDetectorInit#test_initialization().
  TestShouldUseNoIgnore.test_non_root_directory_search: ShouldUseNoIgnore#test_non_root_directory_search().
  TestShouldUseNoIgnore.test_no_project_root: ShouldUseNoIgnore#test_no_project_root().
  TestShouldUseNoIgnore.test_root_search_no_gitignore: ShouldUseNoIgnore#test_root_search_no_gitignore().
  TestShouldUseNoIgnore.test_root_search_with_interfering_gitignore: ShouldUseNoIgnore#test_root_search_with_interfering_gitignore().
  TestShouldUseNoIgnore.test_root_search_with_non_interfering_gitignore: ShouldUseNoIgnore#test_root_search_with_non_interfering_gitignore().
  TestShouldUseNoIgnore.test_exception_handling: ShouldUseNoIgnore#test_exception_handling().
  TestFindGitignoreFiles.test_find_gitignore_in_current_dir: FindGitignoreFiles#test_find_gitignore_in_current_dir().
  TestFindGitignoreFiles.test_find_multiple_gitignores: FindGitignoreFiles#test_find_multiple_gitignores().
  TestFindGitignoreFiles.test_temp_directory_only_current: FindGitignoreFiles#test_temp_directory_only_current().
  TestHasInterferingPatterns.test_no_interfering_patterns: HasInterferingPatterns#test_no_interfering_patterns().
  TestHasInterferingPatterns.test_with_interfering_directory_pattern: HasInterferingPatterns#test_with_interfering_directory_pattern().
  TestHasInterferingPatterns.test_with_source_directory_pattern: HasInterferingPatterns#test_with_source_directory_pattern().
  TestHasInterferingPatterns.test_with_comments_and_empty_lines: HasInterferingPatterns#test_with_comments_and_empty_lines().
  TestHasInterferingPatterns.test_exception_handling: HasInterferingPatterns#test_exception_handling().
  TestIsInterferingPattern.test_directory_pattern_with_slash: IsInterferingPattern#test_directory_pattern_with_slash().
  TestIsInterferingPattern.test_source_directory_pattern: IsInterferingPattern#test_source_directory_pattern().
  TestIsInterferingPattern.test_non_source_directory_pattern: IsInterferingPattern#test_non_source_directory_pattern().
  TestIsInterferingPattern.test_absolute_path_pattern: IsInterferingPattern#test_absolute_path_pattern().
  TestIsInterferingPattern.test_pattern_with_slash_in_middle: IsInterferingPattern#test_pattern_with_slash_in_middle().
  TestIsSearchDirAffectedByPattern.test_search_dir_same_as_pattern_dir: IsSearchDirAffectedByPattern#test_search_dir_same_as_pattern_dir().
  TestIsSearchDirAffectedByPattern.test_search_dir_subdirectory_of_pattern: IsSearchDirAffectedByPattern#test_search_dir_subdirectory_of_pattern().
  TestIsSearchDirAffectedByPattern.test_search_dir_not_affected: IsSearchDirAffectedByPattern#test_search_dir_not_affected().
  TestIsSearchDirAffectedByPattern.test_nonexistent_paths: IsSearchDirAffectedByPattern#test_nonexistent_paths().
  TestDirectoryHasSearchableFiles.test_directory_with_searchable_files: DirectoryHasSearchableFiles#test_directory_with_searchable_files().
  TestDirectoryHasSearchableFiles.test_directory_without_searchable_files: DirectoryHasSearchableFiles#test_directory_without_searchable_files().
  TestDirectoryHasSearchableFiles.test_empty_directory: DirectoryHasSearchableFiles#test_empty_directory().
  TestDirectoryHasSearchableFiles.test_exception_handling: DirectoryHasSearchableFiles#test_exception_handling().
  TestGetDetectionInfo.test_no_interference_detected: GetDetectionInfo#test_no_interference_detected().
  TestGetDetectionInfo.test_interference_detected: GetDetectionInfo#test_interference_detected().
  TestGetDetectionInfo.test_non_root_search: GetDetectionInfo#test_non_root_search().
  TestGetDetectionInfo.test_no_project_root: GetDetectionInfo#test_no_project_root().
  TestGetDetectionInfo.test_nonexistent_project_root: GetDetectionInfo#test_nonexistent_project_root().
  TestGetInterferingPatterns.test_no_interfering_patterns: GetInterferingPatterns#test_no_interfering_patterns().
  TestGetInterferingPatterns.test_with_interfering_patterns: GetInterferingPatterns#test_with_interfering_patterns().
  TestGetInterferingPatterns.test_filters_comments_and_empty_lines: GetInterferingPatterns#test_filters_comments_and_empty_lines().
  TestGetDefaultDetector.test_returns_gitignore_detector_instance: GetDefaultDetector#test_returns_gitignore_detector_instance().
  TestIntegration.test_real_world_scenario: Integration#test_real_world_scenario().
  TestGetDefaultDetector.test_returns_same_instance: GetDefaultDetector#test_returns_same_instance().
  TestGitignoreDetectorInit: GitignoreDetectorInit#
  TestShouldUseNoIgnore: ShouldUseNoIgnore#
  TestFindGitignoreFiles: FindGitignoreFiles#
  TestHasInterferingPatterns: HasInterferingPatterns#
  TestIsInterferingPattern: IsInterferingPattern#
  TestIsSearchDirAffectedByPattern: IsSearchDirAffectedByPattern#
  TestDirectoryHasSearchableFiles: DirectoryHasSearchableFiles#
  TestGetDetectionInfo: GetDetectionInfo#
  TestGetInterferingPatterns: GetInterferingPatterns#
  TestGetDefaultDetector: GetDefaultDetector#
  TestIntegration: Integration#
---
# Module: [`tests/unit/mcp/test_utils/test_gitignore_detector.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py)

## Classes
### `TestDirectoryHasSearchableFiles`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:283`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L283)
- doc: Tests for _directory_has_searchable_files method.
- signature: `class TestDirectoryHasSearchableFiles:`
- members:
  - `test_directory_with_searchable_files(self, tmp_path)` — [`L286`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L286) — Test directory with searchable files.
  - `test_directory_without_searchable_files(self, tmp_path)` — [`L296`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L296) — Test directory without searchable files.
  - `test_empty_directory(self, tmp_path)` — [`L306`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L306) — Test empty directory.
  - `test_exception_handling(self, tmp_path)` — [`L312`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L312) — Test exception handling.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_directory_has_searchable_files`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._directory_has_searchable_files)

### `TestFindGitignoreFiles`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L84)
- doc: Tests for _find_gitignore_files method.
- signature: `class TestFindGitignoreFiles:`
- members:
  - `test_find_gitignore_in_current_dir(self, tmp_path)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L87) — Test finding .gitignore in current directory.
  - `test_find_multiple_gitignores(self, tmp_path)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L97) — Test finding multiple .gitignore files.
  - `test_temp_directory_only_current(self, tmp_path)` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L120) — Test that temp directories only check current directory.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_find_gitignore_files`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._find_gitignore_files)

### `TestGetDefaultDetector`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:407`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L407)
- doc: Tests for get_default_detector function.
- signature: `class TestGetDefaultDetector:`
- members:
  - `test_returns_gitignore_detector_instance(self)` — [`L410`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L410) — Test that function returns GitignoreDetector instance.
  - `test_returns_same_instance(self)` — [`L415`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L415) — Test that function returns singleton instance.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`get_default_detector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#get_default_detector)

### `TestGetDetectionInfo`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:321`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L321)
- doc: Tests for get_detection_info method.
- signature: `class TestGetDetectionInfo:`
- members:
  - `test_interference_detected(self, tmp_path)` — [`L334`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L334) — Test when interference is detected.
  - `test_no_interference_detected(self, tmp_path)` — [`L324`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L324) — Test when no interference is detected.
  - `test_no_project_root(self)` — [`L358`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L358) — Test with no project root.
  - `test_non_root_search(self, tmp_path)` — [`L350`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L350) — Test with non-root search.
  - `test_nonexistent_project_root(self)` — [`L366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L366) — Test with nonexistent project root.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`get_detection_info`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.get_detection_info)

### `TestGetInterferingPatterns`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:374`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L374)
- doc: Tests for _get_interfering_patterns method.
- signature: `class TestGetInterferingPatterns:`
- members:
  - `test_filters_comments_and_empty_lines(self, tmp_path)` — [`L395`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L395) — Test that comments and empty lines are filtered.
  - `test_no_interfering_patterns(self, tmp_path)` — [`L377`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L377) — Test with no interfering patterns.
  - `test_with_interfering_patterns(self, tmp_path)` — [`L386`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L386) — Test with interfering patterns.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_get_interfering_patterns`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._get_interfering_patterns)

### `TestGitignoreDetectorInit`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L17)
- doc: Tests for GitignoreDetector initialization.
- signature: `class TestGitignoreDetectorInit:`
- members:
  - `test_initialization(self)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L20) — Test that GitignoreDetector initializes correctly.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`common_ignore_patterns`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.common_ignore_patterns)

### `TestHasInterferingPatterns`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L136)
- doc: Tests for _has_interfering_patterns method.
- signature: `class TestHasInterferingPatterns:`
- members:
  - `test_exception_handling(self, tmp_path)` — [`L179`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L179) — Test exception handling when reading gitignore.
  - `test_no_interfering_patterns(self, tmp_path)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L139) — Test with non-interfering patterns.
  - `test_with_comments_and_empty_lines(self, tmp_path)` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L170) — Test that comments and empty lines are ignored.
  - `test_with_interfering_directory_pattern(self, tmp_path)` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L148) — Test with interfering directory pattern.
  - `test_with_source_directory_pattern(self, tmp_path)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L161) — Test with source directory pattern.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_has_interfering_patterns`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._has_interfering_patterns)

### `TestIntegration`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:422`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L422)
- doc: Integration tests for GitignoreDetector.
- signature: `class TestIntegration:`
- members:
  - `test_full_detection_workflow(self, tmp_path)` — [`L425`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L425) — Test complete detection workflow.
  - `test_real_world_scenario(self, tmp_path)` — [`L458`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L458) — Test real-world scenario with typical .gitignore.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`should_use_no_ignore`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.should_use_no_ignore), [`get_detection_info`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.get_detection_info)

### `TestIsInterferingPattern`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:195`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L195)
- doc: Tests for _is_interfering_pattern method.
- signature: `class TestIsInterferingPattern:`
- members:
  - `test_absolute_path_pattern(self, tmp_path)` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L222) — Test absolute path pattern.
  - `test_directory_pattern_with_slash(self, tmp_path)` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L198) — Test directory pattern with slash.
  - `test_non_source_directory_pattern(self, tmp_path)` — [`L210`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L210) — Test non-source directory pattern.
  - `test_pattern_with_slash_in_middle(self, tmp_path)` — [`L228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L228) — Test pattern with slash in middle.
  - `test_source_directory_pattern(self, tmp_path)` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L204) — Test source directory patterns.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_is_interfering_pattern`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._is_interfering_pattern)

### `TestIsSearchDirAffectedByPattern`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:235`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L235)
- doc: Tests for _is_search_dir_affected_by_pattern method.
- signature: `class TestIsSearchDirAffectedByPattern:`
- members:
  - `test_nonexistent_paths(self, tmp_path)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L272) — Test with nonexistent paths.
  - `test_search_dir_not_affected(self, tmp_path)` — [`L259`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L259) — Test when search dir is not affected.
  - `test_search_dir_same_as_pattern_dir(self, tmp_path)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L238) — Test when search dir is same as pattern dir.
  - `test_search_dir_subdirectory_of_pattern(self, tmp_path)` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L247) — Test when search dir is subdirectory of pattern.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`_is_search_dir_affected_by_pattern`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector._is_search_dir_affected_by_pattern)

### `TestShouldUseNoIgnore`
- def: [`tests/unit/mcp/test_utils/test_gitignore_detector.py:29`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L29)
- doc: Tests for should_use_no_ignore method.
- signature: `class TestShouldUseNoIgnore:`
- members:
  - `test_exception_handling(self, tmp_path)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L74) — Test that exceptions are handled gracefully.
  - `test_no_project_root(self)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L38) — Test that missing project root returns False.
  - `test_non_root_directory_search(self)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L32) — Test that non-root directory search returns False.
  - `test_root_search_no_gitignore(self, tmp_path)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L44) — Test root search without .gitignore returns False.
  - `test_root_search_with_interfering_gitignore(self, tmp_path)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L50) — Test root search with interfering .gitignore returns True.
  - `test_root_search_with_non_interfering_gitignore(self, tmp_path)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_gitignore_detector.py#L64) — Test root search with non-interfering .gitignore returns False.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`should_use_no_ignore`](../../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.should_use_no_ignore)

