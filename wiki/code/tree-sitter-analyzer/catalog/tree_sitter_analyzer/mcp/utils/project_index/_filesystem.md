---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._filesystem`/
symbols:
  describe_dir: describe_dir().
  extract_readme_excerpt: extract_readme_excerpt().
  compute_language_distribution: compute_language_distribution().
  find_entry_points: find_entry_points().
  build_top_level_structure: build_top_level_structure().
  extract_module_descriptions: extract_module_descriptions().
  scan_subdir_descriptions: scan_subdir_descriptions().
  collect_root_key_files: collect_root_key_files().
  list_files: list_files().
  _scan_subdir_entry_points: _scan_subdir_entry_points().
  _ARTIFACT_DIRS._ARTIFACT_DIRS: _ARTIFACT_DIRS._ARTIFACT_DIRS.
  _build_dir_entry: _build_dir_entry().
  read_module_docstring: read_module_docstring().
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py)

## Functions
- `_build_dir_entry(name: str, count: int, sub_counts: dict[str, dict[str, int]])` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L203) — Build a single ``top_level_structure[i]`` dict for ``name``.
- `_scan_subdir_entry_points(root_path: Path, subdir: Path)` — [`L154`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L154) — Return relative paths of entry-point files in ``subdir``.
- `build_top_level_structure(root_path: Path, all_files: list[str])` — [`L167`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L167) — Return depth-1 directory entries with file counts and depth-2 breakdown.
- `collect_root_key_files(root_path: Path)` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L120) — Return key files (LICENSE/README/etc.) living at project root.
- `compute_language_distribution(all_files: list[str])` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L101) — Derive ``{language: count}`` from file extensions.
- `describe_dir(dir_path: Path, dir_name: str)` — [`L267`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L267) — Return a short description for a directory.
- `extract_module_descriptions(root_path: Path, top_dirs: list[str])` — [`L304`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L304) — Return a mapping of relative directory path → short description.
- `extract_readme_excerpt(root_path: Path)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L224) — Extract the first meaningful paragraph from README.md (max 200 chars).
- `find_entry_points(root_path: Path)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L128) — Scan the project root (up to 3 levels) for known entry-point files.
- `list_files(roots: list[str])` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L56) — Return absolute paths of all regular files under *roots*.
- `read_module_docstring(init_path: Path)` — [`L243`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L243) — Extract the module-level docstring from a Python __init__.py file.
- `scan_subdir_descriptions(top_name: str, top_path: Path, descriptions: dict[str, str])` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L285) — Populate ``descriptions`` with ``top/sub`` → ``desc`` mappings.

## Module values
- `_ARTIFACT_DIRS` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_filesystem.py#L31)

