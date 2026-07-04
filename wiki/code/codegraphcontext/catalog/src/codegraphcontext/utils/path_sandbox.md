---
title: 'Module: src/codegraphcontext/utils/path_sandbox.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/utils/path_sandbox.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.utils.path_sandbox`/
symbols:
  is_path_allowed: is_path_allowed().
  is_safe_download_url: is_safe_download_url().
  clamp_discovery_depth: clamp_discovery_depth().
  sanitize_bundle_filename: sanitize_bundle_filename().
  MAX_DISCOVERY_DEPTH: MAX_DISCOVERY_DEPTH.
  _ALLOWED_DOWNLOAD_HOST_SUFFIXES: _ALLOWED_DOWNLOAD_HOST_SUFFIXES.
  get_allowed_roots: get_allowed_roots().
  is_path_under_root: is_path_under_root().
---
# Module: [`src/codegraphcontext/utils/path_sandbox.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py)

## Functions
- `clamp_discovery_depth(max_depth: int)` — [`L85`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L85) — Clamp discovery depth to a safe range.
- `get_allowed_roots()` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L21) — Return directories under which paths may be indexed or loaded.
- `is_path_allowed(path: Path)` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L36) — True when *path* resolves under an allowed root. — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `is_path_under_root(path: Path, root: Path)` — [`L48`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L48) — True when *path* resolves under *root*.
- `is_safe_download_url(url: str)` — [`L71`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L71) — True when *url* uses HTTPS and points to an allowed registry host.
- `sanitize_bundle_filename(filename: str, default: str = "bundle.cgc")` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L57) — Return a safe basename for a downloaded bundle file.

## Module values
- `MAX_DISCOVERY_DEPTH` — [`L10`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L10)
- `_ALLOWED_DOWNLOAD_HOST_SUFFIXES` — [`L13`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_sandbox.py#L13)

