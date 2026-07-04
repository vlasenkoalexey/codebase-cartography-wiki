---
title: 'Module: scripts/sync_version_minimal.py'
type: catalog
provenance: extracted
module: scripts/sync_version_minimal.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.sync_version_minimal`/
symbols:
  check_versions: check_versions().
  main: main().
  get_version_from_pyproject: get_version_from_pyproject().
  get_essential_version_files: get_essential_version_files().
  update_version_in_file: update_version_in_file().
  update_mcp_server_version: update_mcp_server_version().
---
# Module: [`scripts/sync_version_minimal.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py)

## Functions
- `check_versions(check_only: bool = False)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L120) — Check and optionally update essential version numbers only
- `get_essential_version_files()` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L46) — Get only essential files that need version synchronization
- `get_version_from_pyproject()` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L23) — Get current version from pyproject.toml
- `main()` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L164) — Main function
- `update_mcp_server_version(new_version: str, *, check_only: bool = False)` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L91) — Update [tool.mcp].server_version in pyproject.toml.
- `update_version_in_file(file_path: Path, new_version: str, *, check_only: bool = False)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/scripts/sync_version_minimal.py#L56) — Update version in a single file

