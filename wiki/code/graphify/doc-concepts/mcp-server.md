---
title: The MCP graph server
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The MCP graph server

## Definition
graphify can expose the graph as an MCP server so an assistant gets structured, repeated tool-call access rather than shelling out per query. It serves the tools `query_graph`, `get_node`, `get_neighbors`, `shortest_path`, `list_prs`, `get_pr_impact`, and `triage_prs`. The default `--transport stdio` spawns one local server per developer; `--transport http` serves the same tools over MCP Streamable HTTP so a single shared process (with `--api-key`, `--host 0.0.0.0`) can serve a whole team.

## In graphify (grounded)
- The server is `serve.py`: [`serve`](../catalog/graphify/serve.md#serve) (stdio) and [`serve_http`](../catalog/graphify/serve.md#serve_http) (HTTP), with the HTTP app built by [`_build_http_app`](../catalog/graphify/serve.md#_build_http_app) and guarded by [`_ApiKeyMiddleware`](../catalog/graphify/serve.md#_ApiKeyMiddleware.__init__).
- Each advertised MCP tool is a `_tool_*` handler: [`_tool_query_graph`](../catalog/graphify/serve.md#_build_server._tool_query_graph), [`_tool_get_node`](../catalog/graphify/serve.md#_build_server._tool_get_node), [`_tool_get_neighbors`](../catalog/graphify/serve.md#_build_server._tool_get_neighbors), [`_tool_shortest_path`](../catalog/graphify/serve.md#_build_server._tool_shortest_path), [`_tool_list_prs`](../catalog/graphify/serve.md#_build_server._tool_list_prs), [`_tool_get_pr_impact`](../catalog/graphify/serve.md#_build_server._tool_get_pr_impact), [`_tool_triage_prs`](../catalog/graphify/serve.md#_build_server._tool_triage_prs).
- The graph file is loaded through [`_load_graph`](../catalog/graphify/serve.md#_load_graph) after path validation ([`validate_graph_path`](../catalog/graphify/security.md#validate_graph_path)).

## Why it matters / when it applies
The MCP surface is how graphify becomes a persistent tool an agent reaches for automatically, and the HTTP transport is what lets a team point every IDE at one graph URL instead of each running graphify locally — the same query engine, exposed as protocol tools.

## Connections
- Code concepts: [serve](../concepts/graphify-serve.md), [security](../concepts/graphify-security.md)
- Module catalogs: [serve](../catalog/graphify/serve.md), [security](../catalog/graphify/security.md)
- Related doc-concepts: [graph-query-interface](graph-query-interface.md), [pr-dashboard](pr-dashboard.md), [security-validation](security-validation.md)

## Source
Extracted from `README.md` ("Using the graph directly", "Shared HTTP server") and `ARCHITECTURE.md` (kept in place).
