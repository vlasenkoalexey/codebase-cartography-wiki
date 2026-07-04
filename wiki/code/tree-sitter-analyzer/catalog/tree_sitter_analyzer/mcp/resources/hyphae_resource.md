---
title: 'Module: tree_sitter_analyzer/mcp/resources/hyphae_resource.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/resources/hyphae_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.resources.hyphae_resource`/
symbols:
  read_hyphae_resource: read_hyphae_resource().
  is_hyphae_resource_uri: is_hyphae_resource_uri().
  uri_from_selector: uri_from_selector().
  selector_from_uri: selector_from_uri().
  _RESOURCE_SCHEME: _RESOURCE_SCHEME.
  _item_to_dict: _item_to_dict().
---
# Module: [`tree_sitter_analyzer/mcp/resources/hyphae_resource.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py)

## Functions
- `_item_to_dict(item: Any)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L62) — Convert a Hyphae result item to a serialisable dict.
- `is_hyphae_resource_uri(uri: str)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L16) — True when *uri* matches the ``tsa://hyphae/`` scheme.
- `read_hyphae_resource(uri: str, project_root: str | None)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L31) — Execute the Hyphae selector encoded in *uri* and return the result.
- `selector_from_uri(uri: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L21) — Extract and URL-decode the selector from a ``tsa://hyphae/`` URI.
- `uri_from_selector(selector: str)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L26) — Build a ``tsa://hyphae/`` URI for *selector*.

## Module values
- `_RESOURCE_SCHEME` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/hyphae_resource.py#L13)

