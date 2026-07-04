---
title: 'Module: scripts/sync_version.py'
type: catalog
provenance: extracted
module: scripts/sync_version.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.sync_version`/
symbols:
  VersionSynchronizer.sync_all_versions: VersionSynchronizer#sync_all_versions().
  VersionSynchronizer.check_version_consistency: VersionSynchronizer#check_version_consistency().
  main: main().
  VersionSynchronizer.get_current_version: VersionSynchronizer#get_current_version().
  VersionSynchronizer.project_root: VersionSynchronizer#project_root.
  VersionSynchronizer.version_patterns: VersionSynchronizer#version_patterns.
  VersionSynchronizer: VersionSynchronizer#
  VersionSynchronizer.update_file_versions: VersionSynchronizer#update_file_versions().
  VersionSynchronizer.__init__: VersionSynchronizer#__init__().
---
# Module: [`scripts/sync_version.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py)

## Classes
### `VersionSynchronizer`
- def: [`scripts/sync_version.py:14`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L14)
- signature: `class VersionSynchronizer:`
- members:
  - `check_version_consistency(self)` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L118) — Check if all versions are consistent
  - `get_current_version(self)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L42) — Get the current version from pyproject.toml
  - `sync_all_versions(self, target_version: str = None)` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L97) — Synchronize all version numbers across the project
  - `update_file_versions(self, file_path: Path, patterns: list[tuple[str, str]], target_version: str)` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L57) — Update version numbers in a specific file
  - `project_root` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L16)
  - `version_patterns` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L17)
- protocol/private: `__init__`[`L15`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L15)
- used by: [`main`](sync_version.md#main)

## Functions
- `main()` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version.py#L164)

