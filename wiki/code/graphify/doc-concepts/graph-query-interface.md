---
title: The query / path / explain interface
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The query / path / explain interface

## Definition
Instead of grepping files, you ask the graph. Three commands form the read interface: **`query "<question>"`** returns the relevant subgraph for a natural-language question, **`path "A" "B"`** returns the shortest relationship path between two nodes, and **`explain "Node"`** describes a node and its neighborhood. Queries are scoped and compact — the always-on install nudges assistants to prefer `graphify query` over reading the full report or raw files.

## In graphify (grounded)
The query engine lives in `serve.py` and is shared by CLI and MCP:
- **query** — [`_query_graph_text`](../catalog/graphify/serve.md#_query_graph_text) / [`_tool_query_graph`](../catalog/graphify/serve.md#_build_server._tool_query_graph), which score candidate nodes ([`_score_nodes`](../catalog/graphify/serve.md#_score_nodes)) and expand a subgraph via BFS/DFS ([`_bfs`](../catalog/graphify/serve.md#_bfs) / [`_dfs`](../catalog/graphify/serve.md#_dfs), the `--dfs`/`--budget` flags).
- **path** — [`_tool_shortest_path`](../catalog/graphify/serve.md#_build_server._tool_shortest_path).
- **explain** — the node lookup [`_tool_get_node`](../catalog/graphify/serve.md#_build_server._tool_get_node) / [`_tool_get_neighbors`](../catalog/graphify/serve.md#_build_server._tool_get_neighbors).
- Node-name resolution for a fuzzy query (e.g. `"UserService"`) draws on symbol resolution / path proximity — see [`disambiguate_ambiguous_candidates`](../catalog/graphify/paths.md#disambiguate_ambiguous_candidates) in `paths.py`.
- Every `query`/`path`/`explain` call is logged as JSON Lines (`~/.cache/graphify-queries.log`); the RFC in [node-summaries](node-summaries.md) proposes attaching summaries to the nodes these commands return.

## Why it matters / when it applies
This is graphify's comprehension payoff and its point of comparison with other tools: a scoped subgraph answer costs a fraction of the tokens of reading raw files (see [token-benchmark](token-benchmark.md)), and it routes the assistant to the right ten nodes instead of a whole-repo grep.

## Connections
- Code concepts: [serve](../concepts/graphify-serve.md), [paths](../concepts/graphify-paths.md), [symbol_resolution](../concepts/graphify-symbol_resolution.md)
- Module catalogs: [serve](../catalog/graphify/serve.md), [paths](../catalog/graphify/paths.md)
- Related doc-concepts: [mcp-server](mcp-server.md), [god-nodes-report](god-nodes-report.md), [token-benchmark](token-benchmark.md), [always-on-graph](always-on-graph.md)

## Source
Extracted from `README.md` ("Common commands", "Using the graph directly") (kept in place).
