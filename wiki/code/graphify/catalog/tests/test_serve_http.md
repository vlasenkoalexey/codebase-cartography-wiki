---
title: 'Module: tests/test_serve_http.py'
type: catalog
provenance: extracted
module: tests/test_serve_http.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_serve_http`/
symbols:
  _graph_file: _graph_file().
  test_tools_list_over_http: test_tools_list_over_http().
  _MCP_HEADERS: _MCP_HEADERS.
  _client: _client().
  _INIT_BODY: _INIT_BODY.
  test_app_builds_and_initialize_succeeds: test_app_builds_and_initialize_succeeds().
  test_unknown_path_is_404: test_unknown_path_is_404().
  test_api_key_missing_is_401: test_api_key_missing_is_401().
  test_api_key_wrong_is_401: test_api_key_wrong_is_401().
  test_api_key_bearer_ok: test_api_key_bearer_ok().
  test_api_key_x_api_key_header_ok: test_api_key_x_api_key_header_ok().
  test_blank_api_key_means_no_auth: test_blank_api_key_means_no_auth().
  test_api_key_bearer_scheme_case_insensitive: test_api_key_bearer_scheme_case_insensitive().
  test_custom_mount_path: test_custom_mount_path().
  test_project_path_routes_to_that_projects_graph: test_project_path_routes_to_that_projects_graph().
  test_stateless_mode_initialize: test_stateless_mode_initialize().
  test_stateless_with_timeout_does_not_raise: test_stateless_with_timeout_does_not_raise().
  test_session_timeout_zero_disables: test_session_timeout_zero_disables().
  test_bad_project_path_errors_without_killing_server: test_bad_project_path_errors_without_killing_server().
  test_project_path_is_optional_on_every_tool: test_project_path_is_optional_on_every_tool().
  _init_session: _init_session().
  _call_tool: _call_tool().
  test_cli_defaults_to_stdio: test_cli_defaults_to_stdio().
  test_cli_http_passes_flags: test_cli_http_passes_flags().
  test_cli_api_key_from_env: test_cli_api_key_from_env().
  SAMPLE_GRAPH: SAMPLE_GRAPH.
  _project_with_graph: _project_with_graph().
---
# Module: [`tests/test_serve_http.py`](../../../../../raw/code/graphify/tests/test_serve_http.py)

## Functions
- `_call_tool(client, headers, name, arguments, rid)` — [`L194`](../../../../../raw/code/graphify/tests/test_serve_http.py#L194)
- `_client(app)` — [`L55`](../../../../../raw/code/graphify/tests/test_serve_http.py#L55)
- `_graph_file(tmp_path: Path)` — [`L49`](../../../../../raw/code/graphify/tests/test_serve_http.py#L49)
- `_init_session(client)` — [`L186`](../../../../../raw/code/graphify/tests/test_serve_http.py#L186)
- `_project_with_graph(tmp_path, node_count: int)` — [`L173`](../../../../../raw/code/graphify/tests/test_serve_http.py#L173) — Create ``<proj>/graphify-out/graph.json`` and return the project dir.
- `test_api_key_bearer_ok(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_serve_http.py#L98)
- `test_api_key_bearer_scheme_case_insensitive(tmp_path)` — [`L129`](../../../../../raw/code/graphify/tests/test_serve_http.py#L129)
- `test_api_key_missing_is_401(tmp_path)` — [`L79`](../../../../../raw/code/graphify/tests/test_serve_http.py#L79)
- `test_api_key_wrong_is_401(tmp_path)` — [`L87`](../../../../../raw/code/graphify/tests/test_serve_http.py#L87)
- `test_api_key_x_api_key_header_ok(tmp_path)` — [`L110`](../../../../../raw/code/graphify/tests/test_serve_http.py#L110)
- `test_app_builds_and_initialize_succeeds(tmp_path)` — [`L61`](../../../../../raw/code/graphify/tests/test_serve_http.py#L61)
- `test_bad_project_path_errors_without_killing_server(tmp_path)` — [`L230`](../../../../../raw/code/graphify/tests/test_serve_http.py#L230) — A missing project graph is a tool error, not a process exit — the server
- `test_blank_api_key_means_no_auth(tmp_path)` — [`L121`](../../../../../raw/code/graphify/tests/test_serve_http.py#L121)
- `test_cli_api_key_from_env(monkeypatch)` — [`L296`](../../../../../raw/code/graphify/tests/test_serve_http.py#L296)
- `test_cli_defaults_to_stdio(monkeypatch)` — [`L268`](../../../../../raw/code/graphify/tests/test_serve_http.py#L268)
- `test_cli_http_passes_flags(monkeypatch)` — [`L279`](../../../../../raw/code/graphify/tests/test_serve_http.py#L279)
- `test_custom_mount_path(tmp_path)` — [`L140`](../../../../../raw/code/graphify/tests/test_serve_http.py#L140)
- `test_project_path_is_optional_on_every_tool(tmp_path)` — [`L203`](../../../../../raw/code/graphify/tests/test_serve_http.py#L203) — Multi-project support is additive: every tool gains an optional
- `test_project_path_routes_to_that_projects_graph(tmp_path)` — [`L217`](../../../../../raw/code/graphify/tests/test_serve_http.py#L217) — One running server answers against the default graph when project_path is
- `test_session_timeout_zero_disables(tmp_path)` — [`L259`](../../../../../raw/code/graphify/tests/test_serve_http.py#L259)
- `test_stateless_mode_initialize(tmp_path)` — [`L242`](../../../../../raw/code/graphify/tests/test_serve_http.py#L242)
- `test_stateless_with_timeout_does_not_raise(tmp_path)` — [`L249`](../../../../../raw/code/graphify/tests/test_serve_http.py#L249)
- `test_tools_list_over_http(tmp_path)` — [`L149`](../../../../../raw/code/graphify/tests/test_serve_http.py#L149) — A full initialize -> tools/list round trip works over the HTTP transport.
- `test_unknown_path_is_404(tmp_path)` — [`L72`](../../../../../raw/code/graphify/tests/test_serve_http.py#L72)

## Module values
- `SAMPLE_GRAPH` — [`L21`](../../../../../raw/code/graphify/tests/test_serve_http.py#L21)
- `_INIT_BODY` — [`L32`](../../../../../raw/code/graphify/tests/test_serve_http.py#L32)
- `_MCP_HEADERS` — [`L43`](../../../../../raw/code/graphify/tests/test_serve_http.py#L43)

