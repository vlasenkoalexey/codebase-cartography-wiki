---
title: 'Module: tests/unit/core/test_project_detector.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_project_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_project_detector`/
symbols:
  normalize_path_for_comparison: normalize_path_for_comparison().
  TestUnifiedDetectProjectRoot.test_fallback_to_file_directory: TestUnifiedDetectProjectRoot#test_fallback_to_file_directory().
  TestProjectRootDetector.temp_dir: TestProjectRootDetector#temp_dir.
  TestProjectRootDetector.test_detect_from_git_repo: TestProjectRootDetector#test_detect_from_git_repo().
  TestProjectRootDetector.test_detect_from_python_project: TestProjectRootDetector#test_detect_from_python_project().
  TestProjectRootDetector.test_detect_from_javascript_project: TestProjectRootDetector#test_detect_from_javascript_project().
  TestProjectRootDetector.test_detect_from_java_project: TestProjectRootDetector#test_detect_from_java_project().
  TestProjectRootDetector.test_multiple_markers_priority: TestProjectRootDetector#test_multiple_markers_priority().
  TestProjectRootDetector.test_fallback_behavior: TestProjectRootDetector#test_fallback_behavior().
  TestProjectRootDetector.test_no_markers_found: TestProjectRootDetector#test_no_markers_found().
  TestProjectRootDetector.test_max_depth_limit: TestProjectRootDetector#test_max_depth_limit().
  TestProjectRootDetector.test_invalid_explicit_root: TestProjectRootDetector#test_invalid_explicit_root().
  TestUnifiedDetectProjectRoot.test_explicit_root_priority: TestUnifiedDetectProjectRoot#test_explicit_root_priority().
  TestUnifiedDetectProjectRoot.test_auto_detection_from_file: TestUnifiedDetectProjectRoot#test_auto_detection_from_file().
  TestUnifiedDetectProjectRoot.test_invalid_explicit_root: TestUnifiedDetectProjectRoot#test_invalid_explicit_root().
  TestUnifiedDetectProjectRoot.temp_dir: TestUnifiedDetectProjectRoot#temp_dir.
  TestProjectDetectorEdge.test_detect_from_file_with_file_input: TestProjectDetectorEdge#test_detect_from_file_with_file_input().
  TestProjectDetectorEdge.test_detect_from_file_empty_path: TestProjectDetectorEdge#test_detect_from_file_empty_path().
  TestProjectDetectorEdge.test_traverse_upward_finds_best_candidate: TestProjectDetectorEdge#test_traverse_upward_finds_best_candidate().
  TestProjectDetectorEdge.test_calculate_score_weights: TestProjectDetectorEdge#test_calculate_score_weights().
  TestProjectDetectorEdge.test_detect_from_cwd_exception_handling: TestProjectDetectorEdge#test_detect_from_cwd_exception_handling().
  TestProjectDetectorEdge.test_detect_from_file_exception_handling: TestProjectDetectorEdge#test_detect_from_file_exception_handling().
  TestProjectDetectorEdge.test_traverse_candidates_without_high_priority: TestProjectDetectorEdge#test_traverse_candidates_without_high_priority().
  TestProjectDetectorEdge.test_find_markers_with_glob_patterns: TestProjectDetectorEdge#test_find_markers_with_glob_patterns().
  TestProjectDetectorEdge.test_find_markers_oserror: TestProjectDetectorEdge#test_find_markers_oserror().
  TestProjectDetectorEdge.test_calculate_score_medium_and_low_priority: TestProjectDetectorEdge#test_calculate_score_medium_and_low_priority().
  TestProjectDetectorEdge.test_get_fallback_root_existing_directory: TestProjectDetectorEdge#test_get_fallback_root_existing_directory().
  TestProjectDetectorEdge.test_get_fallback_root_empty_string: TestProjectDetectorEdge#test_get_fallback_root_empty_string().
  TestProjectDetectorEdge.test_get_fallback_root_nonexistent_path: TestProjectDetectorEdge#test_get_fallback_root_nonexistent_path().
  TestProjectDetectorEdge.test_get_fallback_root_exception_returns_cwd: TestProjectDetectorEdge#test_get_fallback_root_exception_returns_cwd().
  TestProjectRootDetector.teardown_method: TestProjectRootDetector#teardown_method().
  TestUnifiedDetectProjectRoot.teardown_method: TestUnifiedDetectProjectRoot#teardown_method().
  TestProjectDetectorEdge.test_detect_project_root_falls_back_to_cwd: TestProjectDetectorEdge#test_detect_project_root_falls_back_to_cwd().
  TestProjectDetectorEdge.test_detect_project_root_no_args_no_markers: TestProjectDetectorEdge#test_detect_project_root_no_args_no_markers().
  TestProjectRootDetector: TestProjectRootDetector#
  TestProjectRootDetector.setup_method: TestProjectRootDetector#setup_method().
  TestUnifiedDetectProjectRoot: TestUnifiedDetectProjectRoot#
  TestUnifiedDetectProjectRoot.setup_method: TestUnifiedDetectProjectRoot#setup_method().
  TestProjectDetectorEdge: TestProjectDetectorEdge#
---
# Module: [`tests/unit/core/test_project_detector.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py)

## Classes
### `TestProjectDetectorEdge`
- def: [`tests/unit/core/test_project_detector.py:332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L332)
- doc: Coverage boost for project_detector.py uncovered paths (72.67% → 80%+).
- signature: `class TestProjectDetectorEdge:`
- members:
  - `test_calculate_score_medium_and_low_priority(self)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L437) — Medium and low priority markers score correctly.
  - `test_calculate_score_weights(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L371) — _calculate_score returns weighted scores for different markers.
  - `test_detect_from_cwd_exception_handling(self, monkeypatch)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L379) — detect_from_cwd handles OSError gracefully.
  - `test_detect_from_file_empty_path(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L350) — detect_project_root with empty/NONE path returns None.
  - `test_detect_from_file_exception_handling(self, monkeypatch, tmp_path)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L390) — detect_from_file handles exceptions gracefully.
  - `test_detect_from_file_with_file_input(self, tmp_path)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L335) — detect_project_root with a file path → uses parent directory.
  - `test_detect_project_root_falls_back_to_cwd(self, tmp_path)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L480) — detect_project_root falls back to cwd when file_path has no markers.
  - `test_detect_project_root_no_args_no_markers(self, monkeypatch, tmp_path)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L489) — detect_project_root returns None when cwd has no markers.
  - `test_find_markers_oserror(self, monkeypatch)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L425) — _find_markers_in_dir handles OSError gracefully.
  - `test_find_markers_with_glob_patterns(self, tmp_path)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L416) — Glob markers like *.sln are matched correctly.
  - `test_get_fallback_root_empty_string(self)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L455) — get_fallback_root with empty string returns cwd.
  - `test_get_fallback_root_exception_returns_cwd(self, monkeypatch)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L471) — get_fallback_root returns cwd when an unexpected exception occurs.
  - `test_get_fallback_root_existing_directory(self, tmp_path)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L447) — get_fallback_root returns the directory itself for an existing dir.
  - `test_get_fallback_root_nonexistent_path(self)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L463) — get_fallback_root with nonexistent path returns cwd.
  - `test_traverse_candidates_without_high_priority(self, tmp_path)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L402) — Non-high-priority markers trigger candidate sorting path.
  - `test_traverse_upward_finds_best_candidate(self, tmp_path)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L357) — Multiple directories with different markers — picks highest score.
- uses (calls/refs, reference-scoped): [`ProjectRootDetector`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector), [`detect_project_root`](../../../tree_sitter_analyzer/project_detector.md#detect_project_root), [`detect_from_file`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.detect_from_file), [`_traverse_upward`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector._traverse_upward), [`_find_markers_in_dir`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector._find_markers_in_dir), [`get_fallback_root`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.get_fallback_root), [`detect_from_cwd`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.detect_from_cwd), [`_calculate_score`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector._calculate_score)

### `TestProjectRootDetector`
- def: [`tests/unit/core/test_project_detector.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L75)
- doc: Test cases for ProjectRootDetector class
- signature: `class TestProjectRootDetector:`
- members:
  - `setup_method(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L78) — Set up test fixtures
  - `teardown_method(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L82) — Clean up test fixtures
  - `test_detect_from_git_repo(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L86) — Test detection from git repository
  - `test_detect_from_java_project(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L128) — Test detection from Java project
  - `test_detect_from_javascript_project(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L114) — Test detection from JavaScript project
  - `test_detect_from_python_project(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L100) — Test detection from Python project
  - `test_fallback_behavior(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L182) — Test fallback behavior
  - `test_invalid_explicit_root(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L213) — Test behavior with invalid explicit root
  - `test_max_depth_limit(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L170) — Test max depth limit
  - `test_multiple_markers_priority(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L142) — Test priority when multiple markers are found
  - `test_no_markers_found(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L157) — Test behavior when no markers are found
  - `temp_dir` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L80)
- uses (calls/refs, reference-scoped): [`ProjectRootDetector`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector), [`detect_project_root`](../../../tree_sitter_analyzer/project_detector.md#detect_project_root), [`detect_from_file`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.detect_from_file), [`get_fallback_root`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.get_fallback_root)  (1 test-only)

### `TestUnifiedDetectProjectRoot`
- def: [`tests/unit/core/test_project_detector.py:237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L237)
- doc: Test cases for unified detect_project_root function
- signature: `class TestUnifiedDetectProjectRoot:`
- members:
  - `setup_method(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L240) — Set up test fixtures
  - `teardown_method(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L244) — Clean up test fixtures
  - `test_auto_detection_from_file(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L268) — Test auto detection from file
  - `test_explicit_root_priority(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L248) — Test that explicit root takes priority
  - `test_fallback_to_file_directory(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L285) — Test fallback to file directory
  - `test_invalid_explicit_root(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L308) — Test behavior with invalid explicit root
  - `temp_dir` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L242)
- uses (calls/refs, reference-scoped): [`ProjectRootDetector`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector), [`detect_project_root`](../../../tree_sitter_analyzer/project_detector.md#detect_project_root), [`detect_from_file`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.detect_from_file), [`get_fallback_root`](../../../tree_sitter_analyzer/project_detector.md#ProjectRootDetector.get_fallback_root)  (1 test-only)

## Functions
- `normalize_path_for_comparison(path_str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_project_detector.py#L21) — Normalize path for comparison, handling platform-specific differences.

