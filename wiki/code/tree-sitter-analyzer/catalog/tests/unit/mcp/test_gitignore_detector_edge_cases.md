---
title: 'Module: tests/unit/mcp/test_gitignore_detector_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_gitignore_detector_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_gitignore_detector_edge_cases`/TestGitignoreDetector
symbols:
  TestGitignoreDetectorConcurrencyEdgeCases.get_detector: ConcurrencyEdgeCases#get_detector().
  TestGitignoreDetectorErrorHandling.detector: ErrorHandling#detector().
  TestGitignoreDetectorBoundaryConditions.detector: BoundaryConditions#detector().
  TestGitignoreDetectorSpecialCharacters.detector: SpecialCharacters#detector().
  TestGitignoreDetectorPerformanceEdgeCases.detector: PerformanceEdgeCases#detector().
  TestGitignoreDetectorConcurrencyEdgeCases.detector: ConcurrencyEdgeCases#detector().
  TestGitignoreDetectorConcurrencyEdgeCases.test_get_default_detector_thread_safety: ConcurrencyEdgeCases#test_get_default_detector_thread_safety().
  TestGitignoreDetectorConcurrencyEdgeCases.test_file_operations_with_concurrent_modifications: ConcurrencyEdgeCases#test_file_operations_with_concurrent_modifications().
  TestGitignoreDetectorMemoryEdgeCases.detector: MemoryEdgeCases#detector().
  TestGitignoreDetectorConcurrencyEdgeCases.modify_file: ConcurrencyEdgeCases#modify_file().
  TestGitignoreDetectorErrorHandling: ErrorHandling#
  TestGitignoreDetectorErrorHandling.test_should_use_no_ignore_with_invalid_project_root: ErrorHandling#test_should_use_no_ignore_with_invalid_project_root().
  TestGitignoreDetectorErrorHandling.test_find_gitignore_files_with_permission_error: ErrorHandling#test_find_gitignore_files_with_permission_error().
  TestGitignoreDetectorErrorHandling.test_find_gitignore_files_with_os_error: ErrorHandling#test_find_gitignore_files_with_os_error().
  TestGitignoreDetectorErrorHandling.test_has_interfering_patterns_with_encoding_error: ErrorHandling#test_has_interfering_patterns_with_encoding_error().
  TestGitignoreDetectorErrorHandling.test_has_interfering_patterns_with_file_not_found: ErrorHandling#test_has_interfering_patterns_with_file_not_found().
  TestGitignoreDetectorErrorHandling.test_directory_has_searchable_files_with_broken_symlinks: ErrorHandling#test_directory_has_searchable_files_with_broken_symlinks().
  TestGitignoreDetectorErrorHandling.test_directory_has_searchable_files_with_circular_symlinks: ErrorHandling#test_directory_has_searchable_files_with_circular_symlinks().
  TestGitignoreDetectorBoundaryConditions: BoundaryConditions#
  TestGitignoreDetectorBoundaryConditions.test_should_use_no_ignore_with_empty_roots: BoundaryConditions#test_should_use_no_ignore_with_empty_roots().
  TestGitignoreDetectorBoundaryConditions.test_should_use_no_ignore_with_dot_slash_root: BoundaryConditions#test_should_use_no_ignore_with_dot_slash_root().
  TestGitignoreDetectorBoundaryConditions.test_find_gitignore_files_at_filesystem_root: BoundaryConditions#test_find_gitignore_files_at_filesystem_root().
  TestGitignoreDetectorBoundaryConditions.test_find_gitignore_files_with_very_deep_path: BoundaryConditions#test_find_gitignore_files_with_very_deep_path().
  TestGitignoreDetectorBoundaryConditions.test_has_interfering_patterns_with_empty_gitignore: BoundaryConditions#test_has_interfering_patterns_with_empty_gitignore().
  TestGitignoreDetectorBoundaryConditions.test_has_interfering_patterns_with_only_comments: BoundaryConditions#test_has_interfering_patterns_with_only_comments().
  TestGitignoreDetectorBoundaryConditions.test_has_interfering_patterns_with_only_whitespace: BoundaryConditions#test_has_interfering_patterns_with_only_whitespace().
  TestGitignoreDetectorBoundaryConditions.test_is_interfering_pattern_with_empty_pattern: BoundaryConditions#test_is_interfering_pattern_with_empty_pattern().
  TestGitignoreDetectorBoundaryConditions.test_is_interfering_pattern_with_whitespace_pattern: BoundaryConditions#test_is_interfering_pattern_with_whitespace_pattern().
  TestGitignoreDetectorBoundaryConditions.test_directory_has_searchable_files_with_zero_byte_files: BoundaryConditions#test_directory_has_searchable_files_with_zero_byte_files().
  TestGitignoreDetectorBoundaryConditions.test_directory_has_searchable_files_with_hidden_files: BoundaryConditions#test_directory_has_searchable_files_with_hidden_files().
  TestGitignoreDetectorSpecialCharacters: SpecialCharacters#
  TestGitignoreDetectorSpecialCharacters.test_has_interfering_patterns_with_unicode_patterns: SpecialCharacters#test_has_interfering_patterns_with_unicode_patterns().
  TestGitignoreDetectorSpecialCharacters.test_has_interfering_patterns_with_special_regex_chars: SpecialCharacters#test_has_interfering_patterns_with_special_regex_chars().
  TestGitignoreDetectorSpecialCharacters.test_directory_has_searchable_files_with_unicode_filenames: SpecialCharacters#test_directory_has_searchable_files_with_unicode_filenames().
  TestGitignoreDetectorSpecialCharacters.test_is_interfering_pattern_with_escaped_characters: SpecialCharacters#test_is_interfering_pattern_with_escaped_characters().
  TestGitignoreDetectorPerformanceEdgeCases: PerformanceEdgeCases#
  TestGitignoreDetectorPerformanceEdgeCases.test_has_interfering_patterns_with_very_large_gitignore: PerformanceEdgeCases#test_has_interfering_patterns_with_very_large_gitignore().
  TestGitignoreDetectorPerformanceEdgeCases.test_directory_has_searchable_files_with_many_files: PerformanceEdgeCases#test_directory_has_searchable_files_with_many_files().
  TestGitignoreDetectorPerformanceEdgeCases.test_find_gitignore_files_with_many_directories: PerformanceEdgeCases#test_find_gitignore_files_with_many_directories().
  TestGitignoreDetectorPerformanceEdgeCases.test_is_search_dir_affected_by_pattern_with_long_paths: PerformanceEdgeCases#test_is_search_dir_affected_by_pattern_with_long_paths().
  TestGitignoreDetectorConcurrencyEdgeCases: ConcurrencyEdgeCases#
  TestGitignoreDetectorMemoryEdgeCases: MemoryEdgeCases#
  TestGitignoreDetectorMemoryEdgeCases.test_memory_usage_with_large_directory_scan: MemoryEdgeCases#test_memory_usage_with_large_directory_scan().
  TestGitignoreDetectorMemoryEdgeCases.test_pattern_matching_with_many_patterns: MemoryEdgeCases#test_pattern_matching_with_many_patterns().
  TestGitignoreDetectorMemoryEdgeCases.test_get_detection_info_memory_efficiency: MemoryEdgeCases#test_get_detection_info_memory_efficiency().
---
# Module: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py)

## Classes
### `TestGitignoreDetectorBoundaryConditions`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L146)
- doc: Test Gitignore detector boundary conditions.
- signature: `class TestGitignoreDetectorBoundaryConditions:`
- members:
  - `detector(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L150) — Create a detector instance.
  - `test_directory_has_searchable_files_with_hidden_files(self, detector)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L292) — Test searchable file detection with hidden files.
  - `test_directory_has_searchable_files_with_zero_byte_files(self, detector)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L278) — Test searchable file detection with zero-byte files.
  - `test_find_gitignore_files_at_filesystem_root(self, detector)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L173) — Test finding .gitignore files at filesystem root.
  - `test_find_gitignore_files_with_very_deep_path(self, detector)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L190) — Test finding .gitignore files with very deep path.
  - `test_has_interfering_patterns_with_empty_gitignore(self, detector)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L209) — Test pattern detection with empty .gitignore file.
  - `test_has_interfering_patterns_with_only_comments(self, detector)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L222) — Test pattern detection with .gitignore containing only comments.
  - `test_has_interfering_patterns_with_only_whitespace(self, detector)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L243) — Test pattern detection with .gitignore containing only whitespace.
  - `test_is_interfering_pattern_with_empty_pattern(self, detector)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L256) — Test pattern interference detection with empty pattern.
  - `test_is_interfering_pattern_with_whitespace_pattern(self, detector)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L265) — Test pattern interference detection with whitespace-only pattern.
  - `test_should_use_no_ignore_with_dot_slash_root(self, detector)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L163) — Test should_use_no_ignore with './' root.
  - `test_should_use_no_ignore_with_empty_roots(self, detector)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L154) — Test should_use_no_ignore with empty roots list.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorConcurrencyEdgeCases`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L489)
- doc: Test Gitignore detector concurrency edge cases.
- signature: `class TestGitignoreDetectorConcurrencyEdgeCases:`
- members:
  - `detector(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L493) — Create a detector instance.
  - `get_detector()` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L503)
  - `modify_file()` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L530)
  - `test_file_operations_with_concurrent_modifications(self, detector)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L520) — Test file operations with concurrent file modifications.
  - `test_get_default_detector_thread_safety(self)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L497) — Test that get_default_detector is thread-safe.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`get_default_detector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#get_default_detector)

### `TestGitignoreDetectorErrorHandling`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L20)
- doc: Test Gitignore detector error handling.
- signature: `class TestGitignoreDetectorErrorHandling:`
- members:
  - `detector(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L24) — Create a detector instance.
  - `test_directory_has_searchable_files_with_broken_symlinks(self, detector)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L106) — Test searchable file detection with broken symlinks.
  - `test_directory_has_searchable_files_with_circular_symlinks(self, detector)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L124) — Test searchable file detection with circular symlinks.
  - `test_find_gitignore_files_with_os_error(self, detector)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L66) — Test finding .gitignore files with OS errors.
  - `test_find_gitignore_files_with_permission_error(self, detector)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L47) — Test finding .gitignore files with permission errors.
  - `test_has_interfering_patterns_with_encoding_error(self, detector)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L78) — Test pattern detection with encoding errors.
  - `test_has_interfering_patterns_with_file_not_found(self, detector)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L94) — Test pattern detection with non-existent file.
  - `test_should_use_no_ignore_with_invalid_project_root(self, detector)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L28) — Test should_use_no_ignore with invalid project root.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorMemoryEdgeCases`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:552`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L552)
- doc: Test Gitignore detector memory edge cases.
- signature: `class TestGitignoreDetectorMemoryEdgeCases:`
- members:
  - `detector(self)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L556) — Create a detector instance.
  - `test_get_detection_info_memory_efficiency(self, detector)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L604) — Test get_detection_info memory efficiency.
  - `test_memory_usage_with_large_directory_scan(self, detector)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L563) — Test memory usage with large directory scan.
  - `test_pattern_matching_with_many_patterns(self, detector)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L582) — Test pattern matching with many patterns.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorPerformanceEdgeCases`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L400)
- doc: Test Gitignore detector performance edge cases.
- signature: `class TestGitignoreDetectorPerformanceEdgeCases:`
- members:
  - `detector(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L404) — Create a detector instance.
  - `test_directory_has_searchable_files_with_many_files(self, detector)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L430) — Test searchable file detection with many files.
  - `test_find_gitignore_files_with_many_directories(self, detector)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L447) — Test finding .gitignore files with many directories.
  - `test_has_interfering_patterns_with_very_large_gitignore(self, detector)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L408) — Test pattern detection with very large .gitignore file.
  - `test_is_search_dir_affected_by_pattern_with_long_paths(self, detector)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L466) — Test search directory analysis with very long paths.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorSpecialCharacters`
- def: [`tests/unit/mcp/test_gitignore_detector_edge_cases.py:306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L306)
- doc: Test Gitignore detector with special characters.
- signature: `class TestGitignoreDetectorSpecialCharacters:`
- members:
  - `detector(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L310) — Create a detector instance.
  - `test_directory_has_searchable_files_with_unicode_filenames(self, detector)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L363) — Test searchable file detection with Unicode filenames.
  - `test_has_interfering_patterns_with_special_regex_chars(self, detector)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L338) — Test pattern detection with special regex characters.
  - `test_has_interfering_patterns_with_unicode_patterns(self, detector)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L314) — Test pattern detection with Unicode characters in patterns.
  - `test_is_interfering_pattern_with_escaped_characters(self, detector)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_edge_cases.py#L381) — Test pattern interference detection with escaped characters.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

