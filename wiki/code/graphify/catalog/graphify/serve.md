---
title: 'Module: graphify/serve.py'
type: catalog
provenance: extracted
module: graphify/serve.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.serve`/
symbols:
  _build_server._tool_triage_prs: _build_server()._tool_triage_prs().
  _score_nodes: _score_nodes().
  _query_graph_text: _query_graph_text().
  _build_server: _build_server().
  _build_http_app: _build_http_app().
  _query_terms: _query_terms().
  _load_graph: _load_graph().
  _normalize_context_filters: _normalize_context_filters().
  _find_node: _find_node().
  _build_server._tool_list_prs: _build_server()._tool_list_prs().
  _subgraph_to_text: _subgraph_to_text().
  _pick_seeds: _pick_seeds().
  _build_server.read_resource: _build_server().read_resource().
  _get_trigram_index: _get_trigram_index().
  _main: _main().
  _trigram_candidates: _trigram_candidates().
  _build_server._tool_get_pr_impact: _build_server()._tool_get_pr_impact().
  serve: serve().
  _search_tokens: _search_tokens().
  _community_header: _community_header().
  _build_server._load_ctx: _build_server()._load_ctx().
  _strip_diacritics: _strip_diacritics().
  _compute_idf: _compute_idf().
  _build_server._tool_get_neighbors: _build_server()._tool_get_neighbors().
  _node_search_text: _node_search_text().
  _infer_context_filters: _infer_context_filters().
  _resolve_context_filters: _resolve_context_filters().
  _trigrams: _trigrams().
  _bfs: _bfs().
  _build_server._select_graph: _build_server()._select_graph().
  _build_server._tool_query_graph: _build_server()._tool_query_graph().
  _build_server._tool_get_community: _build_server()._tool_get_community().
  _build_server._tool_shortest_path: _build_server()._tool_shortest_path().
  serve_http: serve_http().
  _filter_graph_by_context: _filter_graph_by_context().
  _communities_from_graph: _communities_from_graph().
  _ApiKeyMiddleware.__call__: _ApiKeyMiddleware#__call__().
  _build_server._tool_god_nodes: _build_server()._tool_god_nodes().
  _dfs: _dfs().
  _filter_blank_stdin: _filter_blank_stdin().
  _build_server._resolve_graph_path: _build_server()._resolve_graph_path().
  _build_server._tool_get_node: _build_server()._tool_get_node().
  _build_server.call_tool: _build_server().call_tool().
  _MCPASGIApp.__call__: _MCPASGIApp#__call__().
  _has_chinese: _has_chinese().
  _is_searchable: _is_searchable().
  _EXACT_MATCH_BONUS: _EXACT_MATCH_BONUS.
  _PREFIX_MATCH_BONUS: _PREFIX_MATCH_BONUS.
  _build_server._tool_graph_stats: _build_server()._tool_graph_stats().
  _ApiKeyMiddleware.app: _ApiKeyMiddleware#app.
  _segment_chinese: _segment_chinese().
  _QUERY_STOPWORDS: _QUERY_STOPWORDS.
  _SUBSTRING_MATCH_BONUS: _SUBSTRING_MATCH_BONUS.
  _SOURCE_MATCH_BONUS: _SOURCE_MATCH_BONUS.
  _filter_blank_stdin._relay: _filter_blank_stdin()._relay().
  _build_server._load_community_labels: _build_server()._load_community_labels().
  serve.main: serve().main().
  _MCPASGIApp: _MCPASGIApp#
  _MCPASGIApp._manager: _MCPASGIApp#_manager.
  _ApiKeyMiddleware: _ApiKeyMiddleware#
  _ApiKeyMiddleware._expected: _ApiKeyMiddleware#_expected.
  _build_http_app.lifespan: _build_http_app().lifespan().
  _CONTEXT_HINTS._CONTEXT_HINTS: _CONTEXT_HINTS._CONTEXT_HINTS.
  _CONTEXT_FILTER_ALIASES._CONTEXT_FILTER_ALIASES: _CONTEXT_FILTER_ALIASES._CONTEXT_FILTER_ALIASES.
  _build_server.list_tools: _build_server().list_tools().
  _build_server.list_resources: _build_server().list_resources().
  _MCPASGIApp.__init__: _MCPASGIApp#__init__().
  _ApiKeyMiddleware.__init__: _ApiKeyMiddleware#__init__().
---
# Module: [`graphify/serve.py`](../../../../../raw/code/graphify/graphify/serve.py)

## Classes
### `_ApiKeyMiddleware`
- def: [`graphify/serve.py:1370`](../../../../../raw/code/graphify/graphify/serve.py#L1370)
- doc: Pure-ASGI API-key gate for the HTTP transport.
- signature: `class _ApiKeyMiddleware:`
- members:
  - `app` — [`L1380`](../../../../../raw/code/graphify/graphify/serve.py#L1380)
- protocol/private: `__call__`[`L1383`](../../../../../raw/code/graphify/graphify/serve.py#L1383), `__init__`[`L1379`](../../../../../raw/code/graphify/graphify/serve.py#L1379), `_expected`[`L1381`](../../../../../raw/code/graphify/graphify/serve.py#L1381)
- used by: [`_build_http_app`](serve.md#_build_http_app)

### `_MCPASGIApp`
- def: [`graphify/serve.py:1354`](../../../../../raw/code/graphify/graphify/serve.py#L1354)
- doc: Raw-ASGI wrapper around the Streamable HTTP session manager.
- signature: `class _MCPASGIApp:`
- protocol/private: `__call__`[`L1366`](../../../../../raw/code/graphify/graphify/serve.py#L1366), `__init__`[`L1363`](../../../../../raw/code/graphify/graphify/serve.py#L1363), `_manager`[`L1364`](../../../../../raw/code/graphify/graphify/serve.py#L1364)
- used by: [`_build_http_app`](serve.md#_build_http_app)

## Functions
- `_bfs(G: nx.Graph, start_nodes: list[str], depth: int)` — [`L508`](../../../../../raw/code/graphify/graphify/serve.py#L508) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_build_http_app(graph_path: str, *, host: str = "127.0.0.1", port: int = 8080, api_key: str | None = None, path: str = "/mcp", json_response: bool = False, stateless: bool = False, session_timeout: float | None = 3600)` — [`L1411`](../../../../../raw/code/graphify/graphify/serve.py#L1411) — Build the Starlette ASGI app for the Streamable HTTP transport. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_build_server(graph_path: str)` — [`L758`](../../../../../raw/code/graphify/graphify/serve.py#L758) — Build the configured low-level MCP Server (shared by every transport). — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_communities_from_graph(G: nx.Graph)` — [`L65`](../../../../../raw/code/graphify/graphify/serve.py#L65) — Reconstruct community dict from community property stored on nodes.
- `_community_header(cid: int, community_name)` — [`L743`](../../../../../raw/code/graphify/graphify/serve.py#L743) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_compute_idf(G: nx.Graph, terms: list[str])` — [`L155`](../../../../../raw/code/graphify/graphify/serve.py#L155) — IDF weights for query terms, cached in G.graph['_idf_cache']. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_dfs(G: nx.Graph, start_nodes: list[str], depth: int)` — [`L538`](../../../../../raw/code/graphify/graphify/serve.py#L538)
- `_filter_blank_stdin()` — [`L713`](../../../../../raw/code/graphify/graphify/serve.py#L713) — Filter blank lines from stdin before MCP reads it.
- `_filter_graph_by_context(G: nx.Graph, context_filters: list[str] | None)` — [`L491`](../../../../../raw/code/graphify/graphify/serve.py#L491)
- `_find_node(G: nx.Graph, label: str)` — [`L657`](../../../../../raw/code/graphify/graphify/serve.py#L657) — Return node IDs whose label or ID matches the search term (diacritic-insensitive). — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_get_trigram_index(G: nx.Graph)` — [`L210`](../../../../../raw/code/graphify/graphify/serve.py#L210) — Lazily build and cache a trigram -> node-position postings map on the graph. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_has_chinese(text: str)` — [`L88`](../../../../../raw/code/graphify/graphify/serve.py#L88)
- `_infer_context_filters(question: str)` — [`L469`](../../../../../raw/code/graphify/graphify/serve.py#L469)
- `_is_searchable(term: str)` — [`L103`](../../../../../raw/code/graphify/graphify/serve.py#L103) — True if term is Chinese, non-English, or an English word longer than 2 chars.
- `_load_community_labels()` — [`L1247`](../../../../../raw/code/graphify/graphify/serve.py#L1247)
- `_load_ctx(path: str)` — [`L786`](../../../../../raw/code/graphify/graphify/serve.py#L786) — Return (G, communities) for a graph.json path, reusing a cached — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_load_graph(graph_path: str)` — [`L21`](../../../../../raw/code/graphify/graphify/serve.py#L21) — documented in [graphify-build](../../concepts/graphify-build.md)
- `_main(argv: list[str] | None = None)` — [`L1551`](../../../../../raw/code/graphify/graphify/serve.py#L1551) — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `_node_search_text(data: dict, nid: str)` — [`L187`](../../../../../raw/code/graphify/graphify/serve.py#L187) — Concatenate every field _score_nodes / _find_node match a query against, so
- `_normalize_context_filters(filters: list[str] | None)` — [`L453`](../../../../../raw/code/graphify/graphify/serve.py#L453) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_pick_seeds(scored: list[tuple[float, str]], max_k: int = 3, gap_ratio: float = 0.2, *, G: nx.Graph | None = None, terms: list[str] | None = None)` — [`L351`](../../../../../raw/code/graphify/graphify/serve.py#L351) — Select BFS seed nodes, stopping when score drops too far below the top. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_query_graph_text(G: nx.Graph, question: str, *, mode: str = "bfs", depth: int = 3, token_budget: int = 2000, context_filters: list[str] | None = None)` — [`L629`](../../../../../raw/code/graphify/graphify/serve.py#L629) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `_query_terms(question: str)` — [`L128`](../../../../../raw/code/graphify/graphify/serve.py#L128) — Split a query into searchable terms, segmenting Chinese text, then drop — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_relay()` — [`L727`](../../../../../raw/code/graphify/graphify/serve.py#L727)
- `_resolve_context_filters(question: str, explicit_filters: list[str] | None = None)` — [`L481`](../../../../../raw/code/graphify/graphify/serve.py#L481) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_resolve_graph_path(project_path)` — [`L816`](../../../../../raw/code/graphify/graphify/serve.py#L816) — Map an optional project_path to a concrete graph.json path. ``None``
- `_score_nodes(G: nx.Graph, terms: list[str])` — [`L286`](../../../../../raw/code/graphify/graphify/serve.py#L286) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `_search_tokens(text: str)` — [`L83`](../../../../../raw/code/graphify/graphify/serve.py#L83) — Split text into word tokens, stripping punctuation and diacritics. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_segment_chinese(text: str)` — [`L92`](../../../../../raw/code/graphify/graphify/serve.py#L92) — Segment Chinese text and keep the original term for exact matching.
- `_select_graph(project_path)` — [`L839`](../../../../../raw/code/graphify/graphify/serve.py#L839)
- `_strip_diacritics(text: str | None)` — [`L75`](../../../../../raw/code/graphify/graphify/serve.py#L75) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_subgraph_to_text(G: nx.Graph, nodes: set[str], edges: list[tuple], token_budget: int = 2000, *, seeds: list[str] | None = None)` — [`L564`](../../../../../raw/code/graphify/graphify/serve.py#L564) — Render subgraph as text, cutting at token_budget (approx 3 chars/token). — documented in [graphify-security](../../concepts/graphify-security.md)
- `_tool_get_community(arguments: dict)` — [`L1059`](../../../../../raw/code/graphify/graphify/serve.py#L1059) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_tool_get_neighbors(arguments: dict)` — [`L1031`](../../../../../raw/code/graphify/graphify/serve.py#L1031) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_tool_get_node(arguments: dict)` — [`L1014`](../../../../../raw/code/graphify/graphify/serve.py#L1014) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_tool_get_pr_impact(arguments: dict)` — [`L1162`](../../../../../raw/code/graphify/graphify/serve.py#L1162) — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_tool_god_nodes(arguments: dict)` — [`L1075`](../../../../../raw/code/graphify/graphify/serve.py#L1075) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_tool_graph_stats(_: dict)` — [`L1082`](../../../../../raw/code/graphify/graphify/serve.py#L1082)
- `_tool_list_prs(arguments: dict)` — [`L1149`](../../../../../raw/code/graphify/graphify/serve.py#L1149) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_tool_query_graph(arguments: dict)` — [`L985`](../../../../../raw/code/graphify/graphify/serve.py#L985)
- `_tool_shortest_path(arguments: dict)` — [`L1094`](../../../../../raw/code/graphify/graphify/serve.py#L1094)
- `_tool_triage_prs(arguments: dict)` — [`L1192`](../../../../../raw/code/graphify/graphify/serve.py#L1192) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_trigram_candidates(G: nx.Graph, needles: list[str], *, guard_frac: float = 0.1)` — [`L234`](../../../../../raw/code/graphify/graphify/serve.py#L234) — Node IDs whose text could contain any `needle` as a substring, via the — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `_trigrams(text: str)` — [`L180`](../../../../../raw/code/graphify/graphify/serve.py#L180) — Character trigrams of `text`; for <3-char text the whole string is the key.
- `call_tool(name: str, arguments: dict)` — [`L1320`](../../../../../raw/code/graphify/graphify/serve.py#L1320)
- `lifespan(_app)` — [`L1476`](../../../../../raw/code/graphify/graphify/serve.py#L1476)
- `list_resources()` — [`L1257`](../../../../../raw/code/graphify/graphify/serve.py#L1257)
- `list_tools()` — [`L848`](../../../../../raw/code/graphify/graphify/serve.py#L848)
- `main()` — [`L1346`](../../../../../raw/code/graphify/graphify/serve.py#L1346)
- `read_resource(uri: AnyUrl)` — [`L1268`](../../../../../raw/code/graphify/graphify/serve.py#L1268) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `serve(graph_path: str | None = None)` — [`L1335`](../../../../../raw/code/graphify/graphify/serve.py#L1335) — Start the MCP server over stdio (the default, per-developer transport). — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `serve_http(graph_path: str | None = None, *, host: str = "127.0.0.1", port: int = 8080, api_key: str | None = None, path: str = "/mcp", json_response: bool = False, stateless: bool = False, session_timeout: float | None = 3600)` — [`L1493`](../../../../../raw/code/graphify/graphify/serve.py#L1493) — Start the MCP server over Streamable HTTP (MCP spec 2025-03-26). — documented in [graphify-paths](../../concepts/graphify-paths.md)

## Module values
- `_CONTEXT_FILTER_ALIASES` — [`L415`](../../../../../raw/code/graphify/graphify/serve.py#L415)
- `_CONTEXT_HINTS` — [`L405`](../../../../../raw/code/graphify/graphify/serve.py#L405)
- `_EXACT_MATCH_BONUS` — [`L149`](../../../../../raw/code/graphify/graphify/serve.py#L149)
- `_PREFIX_MATCH_BONUS` — [`L150`](../../../../../raw/code/graphify/graphify/serve.py#L150)
- `_QUERY_STOPWORDS` — [`L117`](../../../../../raw/code/graphify/graphify/serve.py#L117)
- `_SOURCE_MATCH_BONUS` — [`L152`](../../../../../raw/code/graphify/graphify/serve.py#L152)
- `_SUBSTRING_MATCH_BONUS` — [`L151`](../../../../../raw/code/graphify/graphify/serve.py#L151)

