---
title: 'Module: tests/unit/mcp/test_gitignore_detector_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_gitignore_detector_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_gitignore_detector_comprehensive`/TestGitignoreDetector
symbols:
  TestGitignoreDetectorInitialization.test_detector_initialization: Initialization#test_detector_initialization().
  TestGitignoreDetectorInitialization.test_get_default_detector: Initialization#test_get_default_detector().
  TestGitignoreDetectorBasicFunctionality.detector: BasicFunctionality#detector().
  TestGitignoreDetectorFileDiscovery.detector: FileDiscovery#detector().
  TestGitignoreDetectorPatternAnalysis.detector: PatternAnalysis#detector().
  TestGitignoreDetectorSearchDirectoryAnalysis.detector: SearchDirectoryAnalysis#detector().
  TestGitignoreDetectorFileAnalysis.detector: FileAnalysis#detector().
  TestGitignoreDetectorDetectionInfo.detector: DetectionInfo#detector().
  TestGitignoreDetectorIntegration.detector: Integration#detector().
  TestGitignoreDetectorInitialization: Initialization#
  TestGitignoreDetectorBasicFunctionality: BasicFunctionality#
  TestGitignoreDetectorBasicFunctionality.temp_project: BasicFunctionality#temp_project().
  TestGitignoreDetectorBasicFunctionality.test_should_use_no_ignore_non_root_search: BasicFunctionality#test_should_use_no_ignore_non_root_search().
  TestGitignoreDetectorBasicFunctionality.test_should_use_no_ignore_multiple_roots: BasicFunctionality#test_should_use_no_ignore_multiple_roots().
  TestGitignoreDetectorBasicFunctionality.test_should_use_no_ignore_no_project_root: BasicFunctionality#test_should_use_no_ignore_no_project_root().
  TestGitignoreDetectorBasicFunctionality.test_should_use_no_ignore_valid_root_search: BasicFunctionality#test_should_use_no_ignore_valid_root_search().
  TestGitignoreDetectorBasicFunctionality.test_should_use_no_ignore_with_exception_handling: BasicFunctionality#test_should_use_no_ignore_with_exception_handling().
  TestGitignoreDetectorFileDiscovery: FileDiscovery#
  TestGitignoreDetectorFileDiscovery.temp_project_with_gitignore: FileDiscovery#temp_project_with_gitignore().
  TestGitignoreDetectorFileDiscovery.test_find_gitignore_files_single_file: FileDiscovery#test_find_gitignore_files_single_file().
  TestGitignoreDetectorFileDiscovery.test_find_gitignore_files_multiple_levels: FileDiscovery#test_find_gitignore_files_multiple_levels().
  TestGitignoreDetectorFileDiscovery.test_find_gitignore_files_no_files: FileDiscovery#test_find_gitignore_files_no_files().
  TestGitignoreDetectorFileDiscovery.test_find_gitignore_files_depth_limit: FileDiscovery#test_find_gitignore_files_depth_limit().
  TestGitignoreDetectorPatternAnalysis: PatternAnalysis#
  TestGitignoreDetectorPatternAnalysis.temp_project_with_source_code: PatternAnalysis#temp_project_with_source_code().
  TestGitignoreDetectorPatternAnalysis.test_has_interfering_patterns_with_source_directories: PatternAnalysis#test_has_interfering_patterns_with_source_directories().
  TestGitignoreDetectorPatternAnalysis.test_has_interfering_patterns_with_comments: PatternAnalysis#test_has_interfering_patterns_with_comments().
  TestGitignoreDetectorPatternAnalysis.test_has_interfering_patterns_with_empty_lines: PatternAnalysis#test_has_interfering_patterns_with_empty_lines().
  TestGitignoreDetectorPatternAnalysis.test_has_interfering_patterns_file_read_error: PatternAnalysis#test_has_interfering_patterns_file_read_error().
  TestGitignoreDetectorPatternAnalysis.test_is_interfering_pattern_directory_patterns: PatternAnalysis#test_is_interfering_pattern_directory_patterns().
  TestGitignoreDetectorPatternAnalysis.test_is_interfering_pattern_non_interfering: PatternAnalysis#test_is_interfering_pattern_non_interfering().
  TestGitignoreDetectorPatternAnalysis.test_is_interfering_pattern_leading_slash: PatternAnalysis#test_is_interfering_pattern_leading_slash().
  TestGitignoreDetectorPatternAnalysis.test_is_interfering_pattern_source_directory_names: PatternAnalysis#test_is_interfering_pattern_source_directory_names().
  TestGitignoreDetectorSearchDirectoryAnalysis: SearchDirectoryAnalysis#
  TestGitignoreDetectorSearchDirectoryAnalysis.temp_project_structure: SearchDirectoryAnalysis#temp_project_structure().
  TestGitignoreDetectorSearchDirectoryAnalysis.test_is_search_dir_affected_by_pattern_exact_match: SearchDirectoryAnalysis#test_is_search_dir_affected_by_pattern_exact_match().
  TestGitignoreDetectorSearchDirectoryAnalysis.test_is_search_dir_affected_by_pattern_subdirectory: SearchDirectoryAnalysis#test_is_search_dir_affected_by_pattern_subdirectory().
  TestGitignoreDetectorSearchDirectoryAnalysis.test_is_search_dir_affected_by_pattern_unrelated: SearchDirectoryAnalysis#test_is_search_dir_affected_by_pattern_unrelated().
  TestGitignoreDetectorSearchDirectoryAnalysis.test_is_search_dir_affected_by_pattern_path_resolution_error: SearchDirectoryAnalysis#test_is_search_dir_affected_by_pattern_path_resolution_error().
  TestGitignoreDetectorFileAnalysis: FileAnalysis#
  TestGitignoreDetectorFileAnalysis.temp_directory_with_files: FileAnalysis#temp_directory_with_files().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_with_searchable_files: FileAnalysis#test_directory_has_searchable_files_with_searchable_files().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_no_searchable_files: FileAnalysis#test_directory_has_searchable_files_no_searchable_files().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_empty_directory: FileAnalysis#test_directory_has_searchable_files_empty_directory().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_nested_structure: FileAnalysis#test_directory_has_searchable_files_nested_structure().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_permission_error: FileAnalysis#test_directory_has_searchable_files_permission_error().
  TestGitignoreDetectorFileAnalysis.test_directory_has_searchable_files_case_insensitive_extensions: FileAnalysis#test_directory_has_searchable_files_case_insensitive_extensions().
  TestGitignoreDetectorDetectionInfo: DetectionInfo#
  TestGitignoreDetectorDetectionInfo.test_get_detection_info_non_root_search: DetectionInfo#test_get_detection_info_non_root_search().
  TestGitignoreDetectorDetectionInfo.test_get_detection_info_no_project_root: DetectionInfo#test_get_detection_info_no_project_root().
  TestGitignoreDetectorDetectionInfo.test_get_detection_info_no_gitignore_files: DetectionInfo#test_get_detection_info_no_gitignore_files().
  TestGitignoreDetectorDetectionInfo.test_get_detection_info_with_interfering_patterns: DetectionInfo#test_get_detection_info_with_interfering_patterns().
  TestGitignoreDetectorDetectionInfo.test_get_detection_info_exception_handling: DetectionInfo#test_get_detection_info_exception_handling().
  TestGitignoreDetectorDetectionInfo.test_get_interfering_patterns_file_read_error: DetectionInfo#test_get_interfering_patterns_file_read_error().
  TestGitignoreDetectorIntegration: Integration#
  TestGitignoreDetectorIntegration.test_real_world_scenario_node_project: Integration#test_real_world_scenario_node_project().
  TestGitignoreDetectorIntegration.test_real_world_scenario_java_project: Integration#test_real_world_scenario_java_project().
  TestGitignoreDetectorIntegration.test_real_world_scenario_python_project: Integration#test_real_world_scenario_python_project().
  TestGitignoreDetectorIntegration.test_complex_gitignore_hierarchy: Integration#test_complex_gitignore_hierarchy().
  TestGitignoreDetectorIntegration.test_performance_with_large_directory_structure: Integration#test_performance_with_large_directory_structure().
---
# Module: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py)

## Classes
### `TestGitignoreDetectorBasicFunctionality`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L52)
- doc: Test basic Gitignore detector functionality.
- signature: `class TestGitignoreDetectorBasicFunctionality:`
- members:
  - `detector(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L56) — Create a detector instance.
  - `temp_project(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L61) — Create a temporary project directory.
  - `test_should_use_no_ignore_multiple_roots(self, detector)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L76) — Test that multiple root searches don't trigger no-ignore.
  - `test_should_use_no_ignore_no_project_root(self, detector)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L85) — Test that searches without project root don't trigger no-ignore.
  - `test_should_use_no_ignore_non_root_search(self, detector)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L67) — Test that non-root searches don't trigger no-ignore.
  - `test_should_use_no_ignore_valid_root_search(self, detector, temp_project)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L94) — Test valid root search without gitignore.
  - `test_should_use_no_ignore_with_exception_handling(self, detector)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L102) — Test exception handling in should_use_no_ignore.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorDetectionInfo`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L528)
- doc: Test Gitignore detector detection info functionality.
- signature: `class TestGitignoreDetectorDetectionInfo:`
- members:
  - `detector(self)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L532) — Create a detector instance.
  - `test_get_detection_info_exception_handling(self, detector)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L594) — Test detection info exception handling.
  - `test_get_detection_info_no_gitignore_files(self, detector)` — [`L558`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L558) — Test detection info when no .gitignore files exist.
  - `test_get_detection_info_no_project_root(self, detector)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L548) — Test detection info without project root.
  - `test_get_detection_info_non_root_search(self, detector)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L536) — Test detection info for non-root search.
  - `test_get_detection_info_with_interfering_patterns(self, detector)` — [`L570`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L570) — Test detection info with interfering patterns.
  - `test_get_interfering_patterns_file_read_error(self, detector)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L604) — Test handling of file read errors in pattern extraction.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorFileAnalysis`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L422)
- doc: Test Gitignore detector file analysis functionality.
- signature: `class TestGitignoreDetectorFileAnalysis:`
- members:
  - `detector(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L426) — Create a detector instance.
  - `temp_directory_with_files(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L431) — Create a temporary directory with various file types.
  - `test_directory_has_searchable_files_case_insensitive_extensions(self, detector)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L513) — Test detection with case-insensitive file extensions.
  - `test_directory_has_searchable_files_empty_directory(self, detector)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L476) — Test detection in empty directory.
  - `test_directory_has_searchable_files_nested_structure(self, detector)` — [`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L485) — Test detection of searchable files in nested structure.
  - `test_directory_has_searchable_files_no_searchable_files(self, detector)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L462) — Test detection when directory has no searchable files.
  - `test_directory_has_searchable_files_permission_error(self, detector)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L499) — Test handling of permission errors during file scanning.
  - `test_directory_has_searchable_files_with_searchable_files(self, detector, temp_directory_with_files)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L454) — Test detection of searchable files in directory.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorFileDiscovery`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L113)
- doc: Test Gitignore detector file discovery functionality.
- signature: `class TestGitignoreDetectorFileDiscovery:`
- members:
  - `detector(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L117) — Create a detector instance.
  - `temp_project_with_gitignore(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L122) — Create a temporary project with .gitignore files.
  - `test_find_gitignore_files_depth_limit(self, detector)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L180) — Test that .gitignore file search respects depth limit.
  - `test_find_gitignore_files_multiple_levels(self, detector)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L148) — Test finding .gitignore files at multiple levels.
  - `test_find_gitignore_files_no_files(self, detector)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L163) — Test finding .gitignore files when none exist.
  - `test_find_gitignore_files_single_file(self, detector, temp_project_with_gitignore)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L139) — Test finding single .gitignore file.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorInitialization`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L18)
- doc: Test Gitignore detector initialization.
- signature: `class TestGitignoreDetectorInitialization:`
- members:
  - `test_detector_initialization(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L21) — Test detector initialization with default patterns.
  - `test_get_default_detector(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L43) — Test getting default detector instance.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector), [`get_default_detector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#get_default_detector), [`common_ignore_patterns`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector.common_ignore_patterns)

### `TestGitignoreDetectorIntegration`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:620`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L620)
- doc: Test Gitignore detector integration scenarios.
- signature: `class TestGitignoreDetectorIntegration:`
- members:
  - `detector(self)` — [`L624`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L624) — Create a detector instance.
  - `test_complex_gitignore_hierarchy(self, detector)` — [`L749`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L749) — Test complex .gitignore file hierarchy.
  - `test_performance_with_large_directory_structure(self, detector)` — [`L776`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L776) — Test performance with large directory structure.
  - `test_real_world_scenario_java_project(self, detector)` — [`L670`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L670) — Test real-world scenario with Java project structure.
  - `test_real_world_scenario_node_project(self, detector)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L628) — Test real-world scenario with Node.js project structure.
  - `test_real_world_scenario_python_project(self, detector)` — [`L705`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L705) — Test real-world scenario with Python project structure.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorPatternAnalysis`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L199)
- doc: Test Gitignore detector pattern analysis functionality.
- signature: `class TestGitignoreDetectorPatternAnalysis:`
- members:
  - `detector(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L203) — Create a detector instance.
  - `temp_project_with_source_code(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L208) — Create a temporary project with source code.
  - `test_has_interfering_patterns_file_read_error(self, detector, temp_project_with_source_code)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L269) — Test handling of file read errors.
  - `test_has_interfering_patterns_with_comments(self, detector, temp_project_with_source_code)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L243) — Test that comments in .gitignore are ignored.
  - `test_has_interfering_patterns_with_empty_lines(self, detector, temp_project_with_source_code)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L256) — Test that empty lines in .gitignore are ignored.
  - `test_has_interfering_patterns_with_source_directories(self, detector, temp_project_with_source_code)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L230) — Test detection of interfering patterns for source directories.
  - `test_is_interfering_pattern_directory_patterns(self, detector, temp_project_with_source_code)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L286) — Test detection of interfering directory patterns.
  - `test_is_interfering_pattern_leading_slash(self, detector, temp_project_with_source_code)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L310) — Test handling of patterns with leading slash.
  - `test_is_interfering_pattern_non_interfering(self, detector, temp_project_with_source_code)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L298) — Test detection of non-interfering patterns.
  - `test_is_interfering_pattern_source_directory_names(self, detector, temp_project_with_source_code)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L322) — Test detection of source directory name patterns.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

### `TestGitignoreDetectorSearchDirectoryAnalysis`
- def: [`tests/unit/mcp/test_gitignore_detector_comprehensive.py:341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L341)
- doc: Test Gitignore detector search directory analysis.
- signature: `class TestGitignoreDetectorSearchDirectoryAnalysis:`
- members:
  - `detector(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L345) — Create a detector instance.
  - `temp_project_structure(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L350) — Create a temporary project with nested structure.
  - `test_is_search_dir_affected_by_pattern_exact_match(self, detector, temp_project_structure)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L365) — Test search directory affected by pattern - exact match.
  - `test_is_search_dir_affected_by_pattern_path_resolution_error(self, detector, temp_project_structure)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L405) — Test handling of path resolution errors.
  - `test_is_search_dir_affected_by_pattern_subdirectory(self, detector, temp_project_structure)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L377) — Test search directory affected by pattern - subdirectory.
  - `test_is_search_dir_affected_by_pattern_unrelated(self, detector, temp_project_structure)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_gitignore_detector_comprehensive.py#L389) — Test search directory not affected by pattern - unrelated.
- uses (calls/refs, reference-scoped): [`GitignoreDetector`](../../../tree_sitter_analyzer/mcp/utils/gitignore_detector.md#GitignoreDetector)

