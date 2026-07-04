---
title: 'Module: src/codegraphcontext/cli/registry_commands.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/registry_commands.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.registry_commands`/
symbols:
  console: console.
  download_bundle: download_bundle().
  load_bundle_command: load_bundle_command().
  fetch_available_bundles: fetch_available_bundles().
  list_bundles: list_bundles().
  search_bundles: search_bundles().
  request_bundle: request_bundle().
  GITHUB_ORG: GITHUB_ORG.
  GITHUB_REPO: GITHUB_REPO.
  _get_base_package_name: _get_base_package_name().
---
# Module: [`src/codegraphcontext/cli/registry_commands.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py)

## Functions
- `_get_base_package_name(bundle_name: str)` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L30) — Extract base package name from full bundle name.
- `download_bundle(name: str, output_dir: Optional[str] = None, auto_load: bool = False)` — [`L195`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L195) — Download a bundle from the registry.
- `fetch_available_bundles()` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L21) — Fetch all available bundles from the Hugging Face registry (delegates to core BundleRegistry).
- `list_bundles(verbose: bool = False, unique: bool = False)` — [`L62`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L62) — Display all available bundles in a table.
- `load_bundle_command(bundle_name: str, clear_existing: bool = False)` — [`L386`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L386) — Load a bundle (for MCP tool integration).
- `request_bundle(repo_url: str, wait: bool = False)` — [`L353`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L353) — Request on-demand generation of a bundle.
- `search_bundles(query: str)` — [`L140`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L140) — Search for bundles matching the query.

## Module values
- `GITHUB_ORG` — [`L17`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L17)
- `GITHUB_REPO` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L18)
- `console` — [`L15`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/registry_commands.py#L15)

