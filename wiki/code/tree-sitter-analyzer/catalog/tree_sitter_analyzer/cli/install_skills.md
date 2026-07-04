---
title: 'Module: tree_sitter_analyzer/cli/install_skills.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/install_skills.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.install_skills`/
symbols:
  install_skills: install_skills().
  _bundled_skills_dir: _bundled_skills_dir().
  InstallReport: InstallReport#
  InstallReport.installed_count: InstallReport#installed_count.
  InstallReport.skipped_count: InstallReport#skipped_count.
  InstallReport.installed: InstallReport#installed.
  InstallReport.skipped: InstallReport#skipped.
  InstallReport.destination: InstallReport#destination.
  _COPY_IGNORE: _COPY_IGNORE.
  _resolve_target: _resolve_target().
---
# Module: [`tree_sitter_analyzer/cli/install_skills.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py)

## Classes
### `InstallReport`  ·  implements/extends _TypedDict
- def: [`tree_sitter_analyzer/cli/install_skills.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L15)
- signature: `class InstallReport(TypedDict):`
- members:
  - `destination` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L20)
  - `installed` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L18)
  - `installed_count` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L16)
  - `skipped` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L19)
  - `skipped_count` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L17)
- used by: [`install_skills`](install_skills.md#install_skills)

## Functions
- `_bundled_skills_dir()` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L23) — Return the absolute path to the bundled tsa-* skills directory.
- `_resolve_target(target_dir: Path | None, *, global_install: bool)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L33) — Return the .claude/skills/ directory to install into.
- `install_skills(target_dir: Path | None = None, *, global_install: bool = False)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L47) — Copy bundled tsa-* skills to *dest_skills_dir*.

## Module values
- `_COPY_IGNORE` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/install_skills.py#L30)

