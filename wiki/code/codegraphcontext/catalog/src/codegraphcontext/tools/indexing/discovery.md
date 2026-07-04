---
title: 'Module: src/codegraphcontext/tools/indexing/discovery.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/discovery.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.discovery`/
symbols:
  discover_files_to_index: discover_files_to_index().
  safe_walk: safe_walk().
  safe_walk.onerror: safe_walk().onerror().
  _GENERIC_EXTENSIONS._GENERIC_EXTENSIONS: _GENERIC_EXTENSIONS._GENERIC_EXTENSIONS.
  _GENERIC_FILENAMES._GENERIC_FILENAMES: _GENERIC_FILENAMES._GENERIC_FILENAMES.
---
# Module: [`src/codegraphcontext/tools/indexing/discovery.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py)

## Functions
- `discover_files_to_index(path: Path, cgcignore_path: Optional[str] = None, supported_extensions: Optional[Set[str]] = None)` — [`L82`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py#L82) — Returns (files, ignore_root). *ignore_root* is used for .cgcignore relative matching. — documented in [codegraphcontext-cli-cli_helpers](../../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `onerror(err: OSError)` — [`L44`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py#L44)
- `safe_walk(path: Path, spec: Optional[Any] = None, ignore_dirs: Optional[Set[str]] = None, ignore_root: Optional[Path] = None)` — [`L21`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py#L21) — Recursively find files under path while:

## Module values
- `_GENERIC_EXTENSIONS` — [`L14`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py#L14)
- `_GENERIC_FILENAMES` — [`L18`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/discovery.py#L18)

