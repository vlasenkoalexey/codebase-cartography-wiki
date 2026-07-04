---
title: 'Module: understand-anything-plugin/skills/understand-domain/extract-domain-context.py'
type: catalog
provenance: extracted
module: understand-anything-plugin/skills/understand-domain/extract-domain-context.py
status: fresh
symbol_base: scip-python python understand-anything 0.0.0 `understand-anything-plugin.skills.understand-domain.extract-domain-context`/
symbols:
  scan_file_tree._walk: scan_file_tree()._walk().
  main: main().
  extract_file_signatures: extract_file_signatures().
  scan_file_tree: scan_file_tree().
  detect_entry_points: detect_entry_points().
  MAX_OUTPUT_BYTES: MAX_OUTPUT_BYTES.
  extract_metadata: extract_metadata().
  _truncate_to_fit: _truncate_to_fit().
  MAX_ENTRY_POINTS: MAX_ENTRY_POINTS.
  MAX_FILES_TOTAL: MAX_FILES_TOTAL.
  is_ignored: is_ignored().
  MAX_FILE_TREE_DEPTH: MAX_FILE_TREE_DEPTH.
  MAX_FILES_PER_DIR: MAX_FILES_PER_DIR.
  MAX_SAMPLED_FILES: MAX_SAMPLED_FILES.
  MAX_LINES_PER_FILE: MAX_LINES_PER_FILE.
  SOURCE_EXTENSIONS: SOURCE_EXTENSIONS.
  SKIP_DIRS: SKIP_DIRS.
  METADATA_FILES: METADATA_FILES.
  parse_gitignore: parse_gitignore().
  extract_file_signatures.priority_score: extract_file_signatures().priority_score().
  ENTRY_POINT_PATTERNS.ENTRY_POINT_PATTERNS: ENTRY_POINT_PATTERNS.ENTRY_POINT_PATTERNS.
---
# Module: [`understand-anything-plugin/skills/understand-domain/extract-domain-context.py`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py)

## Functions
- `_truncate_to_fit(context: dict[str, Any])` — [`L343`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L343) — Progressively trim context sections to stay under MAX_OUTPUT_BYTES.
- `_walk(dir_path: Path, depth: int)` — [`L159`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L159)
- `detect_entry_points(root: Path, file_paths: list[str])` — [`L197`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L197) — Scan source files for entry point patterns.
- `extract_file_signatures(root: Path, file_paths: list[str])` — [`L244`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L244) — Extract exports and imports from each file (lightweight).
- `extract_metadata(root: Path)` — [`L306`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L306) — Read project metadata files.
- `is_ignored(rel_path: str, gitignore_patterns: list[re.Pattern[str]])` — [`L141`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L141) — Check if a relative path matches any gitignore pattern.
- `main()` — [`L376`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L376)
- `parse_gitignore(project_root: Path)` — [`L119`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L119) — Parse .gitignore into a list of compiled regex patterns.
- `priority_score(path: str)` — [`L257`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L257)
- `scan_file_tree(root: Path, gitignore_patterns: list[re.Pattern[str]], max_depth: int = MAX_FILE_TREE_DEPTH)` — [`L151`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L151) — Return a flat list of relative file paths (source files only).

## Module values
- `ENTRY_POINT_PATTERNS` — [`L70`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L70)
- `MAX_ENTRY_POINTS` — [`L29`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L29)
- `MAX_FILES_PER_DIR` — [`L25`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L25)
- `MAX_FILES_TOTAL` — [`L26`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L26)
- `MAX_FILE_TREE_DEPTH` — [`L24`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L24)
- `MAX_LINES_PER_FILE` — [`L28`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L28)
- `MAX_OUTPUT_BYTES` — [`L30`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L30)
- `MAX_SAMPLED_FILES` — [`L27`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L27)
- `METADATA_FILES` — [`L60`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L60)
- `SKIP_DIRS` — [`L51`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L51)
- `SOURCE_EXTENSIONS` — [`L33`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-domain/extract-domain-context.py#L33)

