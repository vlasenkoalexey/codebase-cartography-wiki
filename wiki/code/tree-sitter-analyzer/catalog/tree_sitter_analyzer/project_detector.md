---
title: 'Module: tree_sitter_analyzer/project_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/project_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.project_detector`/
symbols:
  ProjectRootDetector: ProjectRootDetector#
  detect_project_root: detect_project_root().
  ProjectRootDetector.detect_from_file: ProjectRootDetector#detect_from_file().
  ProjectRootDetector._traverse_upward: ProjectRootDetector#_traverse_upward().
  logger: logger.
  ProjectRootDetector._record_dir_candidates: ProjectRootDetector#_record_dir_candidates().
  ProjectRootDetector._find_markers_in_dir: ProjectRootDetector#_find_markers_in_dir().
  result: result.
  ProjectRootDetector.get_fallback_root: ProjectRootDetector#get_fallback_root().
  ProjectRootDetector.detect_from_cwd: ProjectRootDetector#detect_from_cwd().
  ProjectRootDetector._calculate_score: ProjectRootDetector#_calculate_score().
  _has_high_priority_marker: _has_high_priority_marker().
  test_path: test_path.
  _marker_exists_in_dir: _marker_exists_in_dir().
  PROJECT_MARKERS: PROJECT_MARKERS.
  ProjectRootDetector.max_depth: ProjectRootDetector#max_depth.
  _HIGH_PRIORITY_PROJECT_MARKERS._HIGH_PRIORITY_PROJECT_MARKERS: _HIGH_PRIORITY_PROJECT_MARKERS._HIGH_PRIORITY_PROJECT_MARKERS.
  ProjectRootDetector.__init__: ProjectRootDetector#__init__().
---
# Module: [`tree_sitter_analyzer/project_detector.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py)

## Classes
### `ProjectRootDetector`
- def: [`tree_sitter_analyzer/project_detector.py:104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L104)
- doc: Intelligent project root directory detection.
- signature: `class ProjectRootDetector:`
- members:
  - `__init__(self, max_depth: int = 10)` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L107) — Initialize project root detector.
  - `_calculate_score(self, markers: list[str])` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L244) — Calculate a score for project root candidates based on markers found.
  - `_find_markers_in_dir(self, directory: str)` — [`L223`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L223) — Find project markers in a directory.
  - `_record_dir_candidates(self, current_dir: str, candidates: list[tuple[str, int, list[str]]])` — [`L199`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L199) — Score the markers in ``current_dir``; short-circuit on high priority.
  - `_traverse_upward(self, start_dir: str)` — [`L156`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L156) — Traverse upward from start directory looking for project markers.
  - `detect_from_cwd(self)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L143) — Detect project root from current working directory.
  - `detect_from_file(self, file_path: str)` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L116) — Detect project root from a file path.
  - `get_fallback_root(self, file_path: str)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L281) — Get fallback project root when detection fails.
  - `max_depth` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L114)
- uses (calls/refs, reference-scoped): [`logger`](project_detector.md#logger), [`_has_high_priority_marker`](project_detector.md#_has_high_priority_marker), [`PROJECT_MARKERS`](project_detector.md#PROJECT_MARKERS), [`_marker_exists_in_dir`](project_detector.md#_marker_exists_in_dir)
- used by: [`detect_project_root`](project_detector.md#detect_project_root)  (24 test-only)

## Functions
- `_has_high_priority_marker(markers_found: list[str])` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L30) — Return True iff any high-priority marker is in ``markers_found``.
- `_marker_exists_in_dir(dir_path: Path, marker: str)` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L38) — Return True iff ``marker`` exists in ``dir_path``.
- `detect_project_root(file_path: str | None = None, explicit_root: str | None = None)` — [`L306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L306) — Unified project root detection with priority handling.

## Module values
- `PROJECT_MARKERS` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L50)
- `_HIGH_PRIORITY_PROJECT_MARKERS` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L18)
- `logger` — [`L11`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L11)
- `result` — [`L360`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L360)
- `test_path` — [`L359`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/project_detector.py#L359)

