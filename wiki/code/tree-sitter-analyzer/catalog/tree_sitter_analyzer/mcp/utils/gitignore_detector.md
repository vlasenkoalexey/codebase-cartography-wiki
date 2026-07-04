---
title: 'Module: tree_sitter_analyzer/mcp/utils/gitignore_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/gitignore_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.gitignore_detector`/
symbols:
  GitignoreDetector: GitignoreDetector#
  get_default_detector: get_default_detector().
  GitignoreDetector.should_use_no_ignore: GitignoreDetector#should_use_no_ignore().
  GitignoreDetector._has_interfering_patterns: GitignoreDetector#_has_interfering_patterns().
  GitignoreDetector.get_detection_info: GitignoreDetector#get_detection_info().
  GitignoreDetector._is_interfering_pattern: GitignoreDetector#_is_interfering_pattern().
  GitignoreDetector._get_interfering_patterns: GitignoreDetector#_get_interfering_patterns().
  logger: logger.
  GitignoreDetector._is_search_dir_affected_by_pattern: GitignoreDetector#_is_search_dir_affected_by_pattern().
  GitignoreDetector.common_ignore_patterns: GitignoreDetector#common_ignore_patterns.
  GitignoreDetector._find_gitignore_files: GitignoreDetector#_find_gitignore_files().
  GitignoreDetector._directory_has_searchable_files: GitignoreDetector#_directory_has_searchable_files().
  _default_detector: _default_detector.
  _default_detector_lock: _default_detector_lock.
  GitignoreDetector.__init__: GitignoreDetector#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/utils/gitignore_detector.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py)

## Classes
### `GitignoreDetector`
- def: [`tree_sitter_analyzer/mcp/utils/gitignore_detector.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L17)
- doc: Detects .gitignore interference with file searches
- signature: `class GitignoreDetector:`
- members:
  - `_directory_has_searchable_files(self, directory: Path)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L224) — Check if directory contains files that users typically want to search
  - `_find_gitignore_files(self, project_path: Path)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L75) — Find .gitignore files in project hierarchy
  - `_get_interfering_patterns(self, gitignore_file: Path, gitignore_dir: Path, current_search_dir: Path)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L314) — Get list of interfering patterns from a gitignore file
  - `_has_interfering_patterns(self, gitignore_file: Path, gitignore_dir: Path, current_search_dir: Path)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L103) — Check if .gitignore file has patterns that might interfere with searches
  - `_is_interfering_pattern(self, pattern: str, gitignore_dir: Path, current_search_dir: Path)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L140) — Check if a gitignore pattern is likely to interfere with searches
  - `_is_search_dir_affected_by_pattern(self, search_dir: Path, pattern_dir: Path, gitignore_dir: Path)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L197) — Check if the search directory would be affected by a gitignore pattern
  - `get_detection_info(self, roots: list[str], project_root: str | None = None)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L252) — Get detailed information about gitignore detection
  - `should_use_no_ignore(self, roots: list[str], project_root: str | None = None)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L37) — Determine if --no-ignore should be used based on search context
  - `common_ignore_patterns` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L21)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L20)
- uses (calls/refs, reference-scoped): [`read_file_safe`](../../encoding_utils.md#read_file_safe), [`logger`](gitignore_detector.md#logger)
- used by: [`get_default_detector`](gitignore_detector.md#get_default_detector), [`_resolve_no_ignore`](../tools/list_files_tool.md#ListFilesTool._resolve_no_ignore), [`_resolve_no_ignore`](../tools/search_content_tool.md#SearchContentTool._resolve_no_ignore)  (54 test-only)

## Functions
- `get_default_detector()` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L347) — Get the default gitignore detector instance

## Module values
- `_default_detector` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L343)
- `_default_detector_lock` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L344)
- `logger` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/gitignore_detector.py#L14)

