---
title: 'Module: upload_to_pypi.py'
type: catalog
provenance: extracted
module: upload_to_pypi.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 upload_to_pypi/
symbols:
  main: main().
  get_version: get_version().
  get_version_from_package: get_version_from_package().
  get_version_from_pyproject: get_version_from_pyproject().
  check_git_status: check_git_status().
  check_git_tag: check_git_tag().
  check_packages: check_packages().
  check_pypi_version: check_pypi_version().
  run_tests: run_tests().
  upload_with_uv: upload_with_uv().
---
# Module: [`upload_to_pypi.py`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py)

## Functions
- `check_git_status()` — [`L73`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L73) — Check if git repo is clean
- `check_git_tag(version: str)` — [`L90`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L90) — Check if git tag exists for version
- `check_packages(version: str)` — [`L109`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L109) — Check if packages are built
- `check_pypi_version(version: str)` — [`L138`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L138) — Check if version already exists on PyPI
- `get_version()` — [`L57`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L57) — Get version using multiple methods
- `get_version_from_package()` — [`L46`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L46) — Get version from package __init__.py
- `get_version_from_pyproject()` — [`L14`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L14) — Get version from pyproject.toml
- `main()` — [`L339`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L339) — Main function
- `run_tests()` — [`L200`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L200) — Run tests before upload
- `upload_with_uv()` — [`L220`](../../../../raw/code/tree-sitter-analyzer/upload_to_pypi.py#L220) — Upload using uv

