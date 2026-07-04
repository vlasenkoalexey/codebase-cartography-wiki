---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.change_impact_git`/_
symbols:
  _get_changed_files: get_changed_files().
  _get_untracked_files: get_untracked_files().
  _run_git: run_git().
  _get_diff_stat: get_diff_stat().
  _with_pathspec: with_pathspec().
  _normalize_scope_paths: normalize_scope_paths().
  _split_git_lines: split_git_lines().
  _unique_preserve_order: unique_preserve_order().
  _filter_excluded_paths: filter_excluded_paths().
  _path_is_excluded: path_is_excluded().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py)

## Functions
- `_filter_excluded_paths(paths: list[str])` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L25) — Drop paths that live inside tool-owned cache directories (K6).
- `_get_changed_files(mode: str, project_root: str | None, scope_paths: list[str] | None = None)` — [`L99`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L99) — Get list of changed file paths from git diff.
- `_get_diff_stat(mode: str, project_root: str | None, scope_paths: list[str] | None = None)` — [`L127`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L127) — Get diff stat summary from git.
- `_get_untracked_files(project_root: str | None, scope_paths: list[str] | None = None)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L83) — Get untracked files that are not ignored by git.
- `_normalize_scope_paths(scope_paths: list[str] | None)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L68) — Normalize optional git pathspecs while preserving caller order.
- `_path_is_excluded(path: str)` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L10) — Return True when ``path`` lies inside a tool-owned / cache directory.
- `_run_git(args: list[str], cwd: str | None = None)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L34) — Run a git subprocess and return (returncode, stdout).
- `_split_git_lines(output: str)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L51) — Split git output into non-empty path lines.
- `_unique_preserve_order(paths: list[str])` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L56) — Return paths without duplicates while preserving git output order.
- `_with_pathspec(args: list[str], scope_paths: list[str] | None)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_git.py#L75) — Append git pathspec arguments when the caller requests scoped output.

