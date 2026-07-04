---
title: 'Module: scripts/check_patch_coverage.py'
type: catalog
provenance: extracted
module: scripts/check_patch_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.check_patch_coverage`/
symbols:
  main: main().
  print_report: print_report().
  missing_patch_coverage: missing_patch_coverage().
  PatchCoverageMiss: PatchCoverageMiss#
  parse_added_lines: parse_added_lines().
  normalize_coverage_files: normalize_coverage_files().
  HUNK_RE: HUNK_RE.
  DEFAULT_PATHS: DEFAULT_PATHS.
  PatchCoverageMiss.path: PatchCoverageMiss#path.
  PatchCoverageMiss.line: PatchCoverageMiss#line.
  PatchCoverageMiss.reason: PatchCoverageMiss#reason.
  load_coverage: load_coverage().
  normalize_repo_path: normalize_repo_path().
  is_tracked_python_source: is_tracked_python_source().
  git_diff: git_diff().
  build_parser: build_parser().
---
# Module: [`scripts/check_patch_coverage.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py)

## Classes
### `PatchCoverageMiss`
- def: [`scripts/check_patch_coverage.py:27`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L27)
- doc: A missing coverage finding on a PR-added line.
- signature: `class PatchCoverageMiss:`
- members:
  - `line` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L31)
  - `path` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L30)
  - `reason` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L32)
- used by: [`print_report`](check_patch_coverage.md#print_report), [`missing_patch_coverage`](check_patch_coverage.md#missing_patch_coverage)

## Functions
- `build_parser()` — [`L194`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L194)
- `git_diff(project_root: Path, base: str, pathspecs: list[str], worktree: bool)` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L158) — Return unified diff text for the PR patch or current worktree.
- `is_tracked_python_source(path: str)` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L114) — Return true for package source paths covered by Codecov patch gate.
- `load_coverage(path: Path)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L70) — Load a coverage.py JSON report.
- `main(argv: list[str] | None = None)` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L234)
- `missing_patch_coverage(added_lines: dict[str, set[int]], coverage_data: dict[str, Any], project_root: Path)` — [`L119`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L119) — Find added executable lines and branch source lines missing coverage.
- `normalize_coverage_files(coverage_data: dict[str, Any], project_root: Path)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L79) — Return coverage file entries keyed by repo-relative POSIX path.
- `normalize_repo_path(path: str, project_root: Path)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L103) — Normalize absolute or relative paths to repo-relative POSIX form.
- `parse_added_lines(diff_text: str)` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L35) — Return added destination line numbers by path from unified diff text.
- `print_report(misses: list[PatchCoverageMiss])` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L179) — Print a human-readable gate result.

## Module values
- `DEFAULT_PATHS` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L23)
- `HUNK_RE` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_patch_coverage.py#L22)

