---
title: 'Module: src/codegraphcontext/server.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/server.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.server`/
symbols:
  MCPServer.handle_tool_call: MCPServer#handle_tool_call().
  MCPServer.switch_context_tool: MCPServer#switch_context_tool().
  MCPServer.db_manager: MCPServer#db_manager.
  MCPServer._run_loop: MCPServer#_run_loop().
  MCPServer.code_finder: MCPServer#code_finder.
  MCPServer.code_watcher: MCPServer#code_watcher.
  MCPServer.graph_builder: MCPServer#graph_builder.
  MCPServer.add_code_to_graph_tool: MCPServer#add_code_to_graph_tool().
  MCPServer.shutdown: MCPServer#shutdown().
  MCPServer.job_manager: MCPServer#job_manager.
  MCPServer.add_package_to_graph_tool: MCPServer#add_package_to_graph_tool().
  MCPServer.run: MCPServer#run().
  MCPServer: MCPServer#
  _strip_workspace_prefix: _strip_workspace_prefix().
  MCPServer._load_disabled_tools: MCPServer#_load_disabled_tools().
  MCPServer.watch_directory_tool: MCPServer#watch_directory_tool().
  MCPServer.generate_report_tool: MCPServer#generate_report_tool().
  MCPServer.discover_codegraph_contexts_tool: MCPServer#discover_codegraph_contexts_tool().
  MCPServer._start_watcher_if: MCPServer#_start_watcher_if().
  MCPServer.tools: MCPServer#tools.
  MCPServer.list_indexed_repositories_tool: MCPServer#list_indexed_repositories_tool().
  _apply_response_token_limit: _apply_response_token_limit().
  MCPServer.disabled_tools: MCPServer#disabled_tools.
  MCPServer.resolved_context: MCPServer#resolved_context.
  MCPServer.cwd: MCPServer#cwd.
  MCPServer._init_tools: MCPServer#_init_tools().
  MCPServer.execute_cypher_query_tool: MCPServer#execute_cypher_query_tool().
  MCPServer.visualize_graph_query_tool: MCPServer#visualize_graph_query_tool().
  MCPServer.find_dead_code_tool: MCPServer#find_dead_code_tool().
  MCPServer.calculate_cyclomatic_complexity_tool: MCPServer#calculate_cyclomatic_complexity_tool().
  MCPServer.find_most_complex_functions_tool: MCPServer#find_most_complex_functions_tool().
  MCPServer.analyze_code_relationships_tool: MCPServer#analyze_code_relationships_tool().
  MCPServer.find_code_tool: MCPServer#find_code_tool().
  MCPServer.delete_repository_tool: MCPServer#delete_repository_tool().
  MCPServer.check_job_status_tool: MCPServer#check_job_status_tool().
  MCPServer.list_jobs_tool: MCPServer#list_jobs_tool().
  MCPServer.list_watched_paths_tool: MCPServer#list_watched_paths_tool().
  MCPServer.unwatch_directory_tool: MCPServer#unwatch_directory_tool().
  MCPServer.load_bundle_tool: MCPServer#load_bundle_tool().
  MCPServer.search_registry_bundles_tool: MCPServer#search_registry_bundles_tool().
  MCPServer.get_repository_stats_tool: MCPServer#get_repository_stats_tool().
  MCPServer.find_java_spring_endpoints_tool: MCPServer#find_java_spring_endpoints_tool().
  MCPServer.find_java_spring_beans_tool: MCPServer#find_java_spring_beans_tool().
  MCPServer.find_datasource_nodes_tool: MCPServer#find_datasource_nodes_tool().
  MCPServer._context_note_pending: MCPServer#_context_note_pending.
  MCPServer._stop_current_watcher: MCPServer#_stop_current_watcher().
  MCPServer.loop: MCPServer#loop.
  _strip_path_value: _strip_path_value().
  _teardown_db_manager: _teardown_db_manager().
  MCPServer.get_database_status: MCPServer#get_database_status().
  WORKSPACE_PREFIX: WORKSPACE_PREFIX.
  MCPServer.discovered_child_contexts: MCPServer#discovered_child_contexts.
  _is_path_key: _is_path_key().
  _CHARS_PER_TOKEN: _CHARS_PER_TOKEN.
  MCPServer._normalize_tool_name: MCPServer#_normalize_tool_name().
  MCPServer._get_version: MCPServer#_get_version().
  DEFAULT_EDIT_DISTANCE: DEFAULT_EDIT_DISTANCE.
  DEFAULT_FUZZY_SEARCH: DEFAULT_FUZZY_SEARCH.
  MCPServer.__init__: MCPServer#__init__().
---
# Module: [`src/codegraphcontext/server.py`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py)

## Classes
### `MCPServer`
- def: [`src/codegraphcontext/server.py:138`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L138)
- doc: The main MCP Server class.
- signature: `class MCPServer:`
- members:
  - `__init__(self, loop=None, cwd: Path | None = None)` — [`L150`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L150) — Initializes the MCP server and its components.
  - `_init_tools(self)` — [`L205`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L205) — Defines the complete tool manifest for the LLM.
  - `_load_disabled_tools(self)` — [`L234`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L234) — Load disabled tool names from `<cwd>/mcp.json` config.
  - `_normalize_tool_name(self, name: Any)` — [`L216`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L216) — Normalize tool names from mcp.json to internal tool identifiers.
  - `_start_watcher_if(self, should_start: bool)` — [`L444`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L444) — Start the (new) code watcher when the previous one was running.
  - `_stop_current_watcher(self)` — [`L432`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L432) — Stop the active code watcher (if any). Returns whether it was running.
  - `add_code_to_graph_tool(self, **args)` — [`L334`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L334) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `add_package_to_graph_tool(self, **args)` — [`L343`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L343) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `analyze_code_relationships_tool(self, **args)` — [`L310`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L310)
  - `calculate_cyclomatic_complexity_tool(self, **args)` — [`L304`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L304)
  - `check_job_status_tool(self, **args)` — [`L322`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L322)
  - `delete_repository_tool(self, **args)` — [`L319`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L319)
  - `discover_codegraph_contexts_tool(self, **args)` — [`L404`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L404)
  - `execute_cypher_query_tool(self, **args)` — [`L295`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L295)
  - `find_code_tool(self, **args)` — [`L313`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L313)
  - `find_datasource_nodes_tool(self, **args)` — [`L401`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L401)
  - `find_dead_code_tool(self, **args)` — [`L301`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L301)
  - `find_java_spring_beans_tool(self, **args)` — [`L398`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L398)
  - `find_java_spring_endpoints_tool(self, **args)` — [`L395`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L395)
  - `find_most_complex_functions_tool(self, **args)` — [`L307`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L307)
  - `generate_report_tool(self, **args)` — [`L370`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L370)
  - `get_database_status(self)` — [`L287`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L287) — Returns the current connection status of the Neo4j database.
  - `get_repository_stats_tool(self, **args)` — [`L367`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L367)
  - `handle_tool_call(self, tool_name: str, args: Dict[str, Any])` — [`L575`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L575) — Routes a tool call from the AI assistant to the appropriate handler function. — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `list_indexed_repositories_tool(self, **args)` — [`L316`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L316)
  - `list_jobs_tool(self)` — [`L325`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L325)
  - `list_watched_paths_tool(self, **args)` — [`L328`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L328)
  - `load_bundle_tool(self, **args)` — [`L361`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L361)
  - `run(self)` — [`L643`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L643) — Runs the main server loop, listening for JSON-RPC requests from stdin. — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `search_registry_bundles_tool(self, **args)` — [`L364`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L364)
  - `shutdown(self)` — [`L750`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L750) — Gracefully shuts down the server and its components. — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `switch_context_tool(self, **args)` — [`L453`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L453) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `unwatch_directory_tool(self, **args)` — [`L331`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L331)
  - `visualize_graph_query_tool(self, **args)` — [`L298`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L298)
  - `watch_directory_tool(self, **args)` — [`L352`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L352)
  - `code_finder` — [`L199`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L199) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `code_watcher` — [`L200`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L200) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `cwd` — [`L159`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L159)
  - `db_manager` — [`L171`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L171) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `disabled_tools` — [`L162`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L162)
  - `discovered_child_contexts` — [`L160`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L160)
  - `graph_builder` — [`L198`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L198) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `job_manager` — [`L186`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L186) — documented in [codegraphcontext-server](../../../concepts/codegraphcontext-server.md)
  - `loop` — [`L195`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L195)
  - `resolved_context` — [`L166`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L166)
  - `tools` — [`L210`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L210)
- protocol/private: `_context_note_pending`[`L161`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L161), `_get_version`[`L280`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L280), `_run_loop`[`L662`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L662)
- uses (calls/refs, reference-scoped): [`warning_logger`](utils/debug_log.md#warning_logger), [`error_logger`](utils/debug_log.md#error_logger), [`resolve_context`](cli/config_manager.md#resolve_context), [`get_database_manager`](core/__init__.md#get_database_manager), [`GraphBuilder`](tools/graph_builder.md#GraphBuilder), [`load_bundle`](tools/handlers/management_handlers.md#load_bundle), [`generate_report`](tools/report_generator.md#generate_report), [`load_config`](cli/config_manager.md#load_config), [`check_job_status`](tools/handlers/management_handlers.md#check_job_status), [`CONFIG_DIR`](cli/config_manager.md#CONFIG_DIR), [`CodeFinder`](tools/code_finder.md#CodeFinder), [`is_path_allowed`](utils/path_sandbox.md#is_path_allowed), [`database`](cli/config_manager.md#ResolvedContext.database), [`JobManager`](core/jobs.md#JobManager), [`list_jobs`](tools/handlers/management_handlers.md#list_jobs), [`search_registry_bundles`](tools/handlers/management_handlers.md#search_registry_bundles), [`cgcignore_path`](cli/config_manager.md#ResolvedContext.cgcignore_path), [`_default_global_db_path`](cli/config_manager.md#_default_global_db_path), [`_strip_workspace_prefix`](server.md#_strip_workspace_prefix), [`debug_logger`](utils/debug_log.md#debug_logger), [`mode`](cli/config_manager.md#ResolvedContext.mode), [`analyze_code_relationships`](tools/handlers/analysis_handlers.md#analyze_code_relationships), [`cleanup_old_jobs`](core/jobs.md#JobManager.cleanup_old_jobs), [`db_path`](cli/config_manager.md#ResolvedContext.db_path), [`delete_repository`](tools/handlers/management_handlers.md#delete_repository), [`execute_cypher_query`](tools/handlers/query_handlers.md#execute_cypher_query), [`find_code`](tools/handlers/analysis_handlers.md#find_code), [`find_dead_code`](tools/handlers/analysis_handlers.md#find_dead_code), [`find_most_complex_functions`](tools/handlers/analysis_handlers.md#find_most_complex_functions), [`get_repository_stats`](tools/handlers/management_handlers.md#get_repository_stats), [`discover_child_contexts`](cli/config_manager.md#discover_child_contexts), [`context_name`](cli/config_manager.md#ResolvedContext.context_name), [`add_code_to_graph`](tools/handlers/indexing_handlers.md#add_code_to_graph), [`add_package_to_graph`](tools/handlers/indexing_handlers.md#add_package_to_graph), [`calculate_cyclomatic_complexity`](tools/handlers/analysis_handlers.md#calculate_cyclomatic_complexity), [`find_datasource_nodes`](tools/handlers/analysis_handlers.md#find_datasource_nodes), [`find_java_spring_beans`](tools/handlers/analysis_handlers.md#find_java_spring_beans), [`find_java_spring_endpoints`](tools/handlers/analysis_handlers.md#find_java_spring_endpoints), [`list_indexed_repositories`](tools/handlers/management_handlers.md#list_indexed_repositories), [`visualize_graph_query`](tools/handlers/query_handlers.md#visualize_graph_query)  (+13 more)
- used by: [`call_tool`](api/router.md#call_tool), [`execute_query`](api/router.md#execute_query), [`get_status`](api/router.md#get_status), [`index_repository`](api/router.md#index_repository), [`list_repositories`](api/router.md#list_repositories), [`list_tools`](api/router.md#list_tools), [`mcp_start`](cli/main.md#mcp_start), [`get_server`](api/router.md#get_server), [`handle_call_tool`](api/mcp_sse.md#handle_call_tool), [`mcp_tools`](cli/main.md#mcp_tools), [`_server_instance`](api/router.md#_server_instance._server_instance), [`handle_list_tools`](api/mcp_sse.md#handle_list_tools)

## Functions
- `_apply_response_token_limit(tool_name: str, text: str)` — [`L94`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L94) — Truncate *text* to the configured token budget and append a notice. — documented in [codegraphcontext-cli-config_manager](../../../concepts/codegraphcontext-cli-config_manager.md)
- `_is_path_key(key: str)` — [`L59`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L59) — Check if a dict key represents a file path field.
- `_strip_path_value(value)` — [`L70`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L70) — Strip /workspace/ prefix from a single string value.
- `_strip_workspace_prefix(obj)` — [`L77`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L77) — Recursively strip /workspace/ prefix from path values in results.
- `_teardown_db_manager(db_manager)` — [`L51`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L51) — Release DB resources; stop FalkorDB Lite worker when switching contexts.

## Module values
- `DEFAULT_EDIT_DISTANCE` — [`L45`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L45)
- `DEFAULT_FUZZY_SEARCH` — [`L46`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L46)
- `WORKSPACE_PREFIX` — [`L48`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L48)
- `_CHARS_PER_TOKEN` — [`L91`](../../../../../../raw/code/codegraphcontext/src/codegraphcontext/server.py#L91)

