---
title: 'Module: graphify/mcp_ingest.py'
type: catalog
provenance: extracted
module: graphify/mcp_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.mcp_ingest`/
symbols:
  extract_mcp_config: extract_mcp_config().
  _emit_server: _emit_server().
  _detect_package_from_args: _detect_package_from_args().
  is_mcp_config_path: is_mcp_config_path().
  _make_id: _make_id().
  _add_node: _add_node().
  _add_edge: _add_edge().
  MCP_CONFIG_FILENAMES.MCP_CONFIG_FILENAMES: MCP_CONFIG_FILENAMES.MCP_CONFIG_FILENAMES.
  _MAX_BYTES: _MAX_BYTES.
  _MAX_SERVERS_PER_FILE: _MAX_SERVERS_PER_FILE.
  _NPM_PKG_RE: _NPM_PKG_RE.
  _PY_MCP_PKG_RE: _PY_MCP_PKG_RE.
  _ARG_FLAG_RE: _ARG_FLAG_RE.
  _strip_version: _strip_version().
---
# Module: [`graphify/mcp_ingest.py`](../../../../../raw/code/graphify/graphify/mcp_ingest.py)

## Functions
- `_add_edge(edges: list[dict[str, Any]], seen: set[tuple[str, str, str]], *, source: str, target: str, relation: str, source_file: str, line: int, context: str | None = None)` — [`L343`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L343) — Append an edge if (source, target, relation) is not already present.
- `_add_node(nodes: list[dict[str, Any]], seen: set[str], *, nid: str, label: str, kind: str, source_file: str, line: int)` — [`L319`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L319) — Append a node if not already present. ``kind`` is metadata, not file_type. — documented in [graphify-security](../../concepts/graphify-security.md)
- `_detect_package_from_args(args: list[Any])` — [`L284`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L284) — Return the first arg that looks like an npm or pypi package id, else None.
- `_emit_server(*, server_name: str, spec: dict[str, Any], file_nid: str, file_stem: str, source_file: str, nodes: list[dict[str, Any]], edges: list[dict[str, Any]], seen_node_ids: set[str], seen_edge_keys: set[tuple[str, str, str]])` — [`L169`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L169) — Emit nodes/edges for one entry under ``mcpServers``.
- `_make_id(*parts: str)` — [`L379`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L379) — Build a stable node ID via the single shared recipe (#1378).
- `_strip_version(pkg: str)` — [`L302`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L302) — Drop the ``@version`` suffix from an npm package id, preserving the scope.
- `extract_mcp_config(path: Path)` — [`L86`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L86) — Parse an MCP config file into Graphify nodes and edges. — documented in [graphify-extract](../../concepts/graphify-extract.md)
- `is_mcp_config_path(path: Path)` — [`L81`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L81) — Return True when ``path`` is a recognised MCP config filename.

## Module values
- `MCP_CONFIG_FILENAMES` — [`L70`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L70)
- `_ARG_FLAG_RE` — [`L281`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L281)
- `_MAX_BYTES` — [`L77`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L77)
- `_MAX_SERVERS_PER_FILE` — [`L78`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L78)
- `_NPM_PKG_RE` — [`L279`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L279)
- `_PY_MCP_PKG_RE` — [`L280`](../../../../../raw/code/graphify/graphify/mcp_ingest.py#L280)

