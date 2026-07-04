---
title: 'Module: src/codegraphcontext/core/bundle_registry.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/bundle_registry.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.bundle_registry`/
symbols:
  BundleRegistry.fetch_available_bundles: BundleRegistry#fetch_available_bundles().
  RegistryUnavailableError: RegistryUnavailableError#
  BundleRegistry: BundleRegistry#
  BundleRegistry.find_bundle_download_info: BundleRegistry#find_bundle_download_info().
  logger: logger.
  _github_headers: _github_headers().
  _get_manifest_url: _get_manifest_url().
  BundleRegistry.download_file: BundleRegistry#download_file().
---
# Module: [`src/codegraphcontext/core/bundle_registry.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py)

## Classes
### `BundleRegistry`
- def: [`src/codegraphcontext/core/bundle_registry.py:28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L28)
- doc: Core logic for interacting with the CodeGraphContext bundle registry.
- signature: `class BundleRegistry:`
- members:
  - `download_file(url: str, output_path: Path, progress_callback=None)` — [`L131`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L131) — Download a file from a URL to a local path.
  - `fetch_available_bundles()` — [`L35`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L35) — Fetch all available bundles from the Hugging Face raw dataset registry manifest.
  - `find_bundle_download_info(name: str)` — [`L87`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L87) — Find a download URL and metadata for a bundle by name.
- uses (calls/refs, reference-scoped): [`RegistryUnavailableError`](bundle_registry.md#RegistryUnavailableError), [`_get_manifest_url`](bundle_registry.md#_get_manifest_url), [`_github_headers`](bundle_registry.md#_github_headers), [`logger`](bundle_registry.md#logger)
- used by: [`load_bundle`](../tools/handlers/management_handlers.md#load_bundle), [`search_registry_bundles`](../tools/handlers/management_handlers.md#search_registry_bundles), [`fetch_available_bundles`](../cli/registry_commands.md#fetch_available_bundles)

### `RegistryUnavailableError`  ·  implements/extends RuntimeError
- def: [`src/codegraphcontext/core/bundle_registry.py:10`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L10)
- doc: Raised when the remote bundle registry cannot be reached.
- signature: `class RegistryUnavailableError(RuntimeError):`
- used by: [`search_registry_bundles`](../tools/handlers/management_handlers.md#search_registry_bundles), [`fetch_available_bundles`](bundle_registry.md#BundleRegistry.fetch_available_bundles), [`fetch_available_bundles`](../cli/registry_commands.md#fetch_available_bundles), [`list_bundles`](../cli/registry_commands.md#list_bundles), [`search_bundles`](../cli/registry_commands.md#search_bundles)

## Functions
- `_get_manifest_url()` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L23)
- `_github_headers()` — [`L14`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L14) — Return GitHub API headers, including auth token if available.

## Module values
- `logger` — [`L7`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/bundle_registry.py#L7)

