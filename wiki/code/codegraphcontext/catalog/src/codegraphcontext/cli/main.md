---
title: 'Module: src/codegraphcontext/cli/main.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/main.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.main`/
symbols:
  console: console.
  _load_credentials: _load_credentials().
  doctor: doctor().
  app: app.
  hook_status: hook_status().
  context_list: context_list().
  bundle_import: bundle_import().
  delete: delete().
  analyze_app: analyze_app.
  _write_datasource_graph: _write_datasource_graph().
  mcp_start: mcp_start().
  find_by_name: find_by_name().
  find_by_pattern: find_by_pattern().
  find_by_type: find_by_type().
  analyze_callers: analyze_callers().
  analyze_chain: analyze_chain().
  analyze_dependencies: analyze_dependencies().
  analyze_inheritance_tree: analyze_inheritance_tree().
  analyze_complexity: analyze_complexity().
  analyze_overrides: analyze_overrides().
  bundle_export: bundle_export().
  bundle_load: bundle_load().
  index: index().
  find_app: find_app.
  mcp_tools: mcp_tools().
  hook_install: hook_install().
  hook_uninstall: hook_uninstall().
  report: report().
  analyze_calls: analyze_calls().
  query_graph: query_graph().
  context_app: context_app.
  registry_app: registry_app.
  context_create: context_create().
  config_app: config_app.
  bundle_app: bundle_app.
  registry_download: registry_download().
  find_by_variable: find_by_variable().
  find_by_content_search: find_by_content_search().
  find_by_decorator_search: find_by_decorator_search().
  find_by_argument_search: find_by_argument_search().
  analyze_kotlin_call_audit: analyze_kotlin_call_audit().
  analyze_dead_code: analyze_dead_code().
  analyze_variable_usage: analyze_variable_usage().
  main: main().
  datasource_cassandra: datasource_cassandra().
  datasource_redis: datasource_redis().
  mcp_app: mcp_app.
  hook_app: hook_app.
  datasource_app: datasource_app.
  list_repositories: list_repositories().
  watch: watch().
  config_reset: config_reset().
  config_db: config_db().
  bundle_merge: bundle_merge().
  update: update().
  clean: clean().
  stats: stats().
  visualize: visualize().
  add_package: add_package().
  unwatch: unwatch().
  watching: watching().
  cypher_legacy: cypher_legacy().
  visualize_abbrev: visualize_abbrev().
  version_cmd: version_cmd().
  datasource_mysql: datasource_mysql().
  neo4j_app: neo4j_app.
  api_app: api_app.
  mcp_setup: mcp_setup().
  neo4j_setup: neo4j_setup().
  analyze_complexity._render_complexity_table: analyze_complexity()._render_complexity_table().
  mcp_setup_alias: mcp_setup_alias().
  neo4j_setup_alias: neo4j_setup_alias().
  context_delete: context_delete().
  context_mode: context_mode().
  context_default: context_default().
  config_set: config_set().
  export_shortcut: export_shortcut().
  load_shortcut: load_shortcut().
  api_start: api_start().
  registry_list: registry_list().
  registry_search: registry_search().
  registry_request: registry_request().
  setup_scip: setup_scip().
  index_abbrev: index_abbrev().
  list_abbrev: list_abbrev().
  delete_abbrev: delete_abbrev().
  watch_abbrev: watch_abbrev().
  _load_credentials._append_source: _load_credentials()._append_source().
  _configure_library_loggers: _configure_library_loggers().
  _confirm_bundle_clear: _confirm_bundle_clear().
  config_show: config_show().
  registry_callback: registry_callback().
  help: help().
  get_version: get_version().
  bundle_merge._read_bytes: bundle_merge()._read_bytes().
  analyze_complexity._is_file_path: analyze_complexity()._is_file_path().
---
# Module: [`src/codegraphcontext/cli/main.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py)

## Functions
- `_append_source(source_name: str, source_values: dict)` — [`L327`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L327)
- `_configure_library_loggers()` — [`L51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L51) — Configure third-party library loggers based on config setting.
- `_confirm_bundle_clear(clear: bool, yes: bool)` — [`L662`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L662) — Return True if import may proceed; False if user cancelled.
- `_is_file_path(value: str)` — [`L2538`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2538)
- `_load_credentials(cli_context_flag: Optional[str] = None)` — [`L294`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L294) — Loads configuration and credentials from various sources into environment variables. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `_read_bytes(p: Path)` — [`L818`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L818)
- `_render_complexity_table(results, title)` — [`L2543`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2543)
- `_write_datasource_graph(ingested: dict, context: Optional[str] = None)` — [`L3074`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L3074) — Shared helper: write ingested datasource dict to the active graph. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `add_package(package_name: str = typer.Argument(..., help="Name of the package to add."), language: str = typer.Argument(..., help="Language of the package."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1544`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1544) — Adds a package to the code graph.
- `analyze_callers(ctx: typer.Context, function: str = typer.Argument(..., help="Function name to analyze"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2187`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2187) — Show what functions call this function. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `analyze_calls(ctx: typer.Context, function: str = typer.Argument(..., help="Function name to analyze"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2131`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2131) — Show what functions this function calls (callees). — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_chain(ctx: typer.Context, from_func: str = typer.Argument(..., help="Starting function"), to_func: str = typer.Argument(..., help="Target function"), max_depth: int = typer.Option(5, "--depth", "-d", help="Maximum call chain depth"), from_file: Optional[str] = typer.Option(None, "--from-file", help="File for starting function"), to_file: Optional[str] = typer.Option(None, "--to-file", help="File for target function"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2245`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2245) — Show call chain between two functions. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `analyze_complexity(path: Optional[str] = typer.Argument(None, help="Function name or file path to analyze"), threshold: int = typer.Option(10, "--threshold", "-t", help="Complexity threshold for warnings"), limit: int = typer.Option(20, "--limit", "-l", help="Maximum results to show"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path to scope analysis"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2509`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2509) — Show cyclomatic complexity for functions. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `analyze_dead_code(path: Optional[str] = typer.Argument(None, help="Path to analyze (not yet implemented)"), exclude_decorators: Optional[str] = typer.Option(None, "--exclude", "-e", help="Comma-separated decorators to exclude"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2593`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2593) — Find potentially unused functions and classes. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_dependencies(ctx: typer.Context, target: str = typer.Argument(..., help="Module name"), show_external: bool = typer.Option(True, "--external/--no-external", help="Show external dependencies"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2378`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2378) — Show dependencies and imports for a module. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_inheritance_tree(ctx: typer.Context, class_name: str = typer.Argument(..., help="Class name"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2443`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2443) — Show inheritance hierarchy for a class. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_kotlin_call_audit(repo_path: Optional[str] = typer.Option(None, "--repo-path", "-r", help="Limit audit to paths under this repository root"), limit: int = typer.Option(20, "--limit", "-n", help="Maximum examples/top names to show"), json_output: bool = typer.Option(False, "--json", help="Print machine-readable JSON"), fail_on_ambiguity: bool = typer.Option(False, "--fail-on-ambiguity", help="Exit non-zero if any ambiguous Kotlin call groups are found"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2319`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2319) — Audit Kotlin function call edges for multi-target callsite ambiguity. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_overrides(ctx: typer.Context, function_name: str = typer.Argument(..., help="Function/method name to find implementations of"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2643`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2643) — Find all implementations of a function across different classes. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `analyze_variable_usage(variable_name: str = typer.Argument(..., help="Variable name to analyze"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2699`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2699) — Analyze where a variable is defined and used across the codebase. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `api_start(host: str = typer.Option("0.0.0.0", help="Host to bind the server to"), port: int = typer.Option(8000, help="Port to bind the server to"), reload: bool = typer.Option(False, help="Enable auto-reload (development only)"))` — [`L944`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L944) — Start the CGC Gateway HTTP API server.
- `bundle_export(output: str = typer.Argument(..., help="Output path for the .cgc bundle file"), repo: Optional[str] = typer.Option(None, "--repo", "-r", help="Specific repository path to export (default: export all)"), no_stats: bool = typer.Option(False, "--no-stats", help="Skip statistics generation"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L611`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L611) — Export the current graph to a portable .cgc bundle. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `bundle_import(bundle_file: str = typer.Argument(..., help="Path to the .cgc bundle file to import"), clear: bool = typer.Option(False, "--clear", help="Clear existing graph data before importing"), yes: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation when using --clear"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L682`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L682) — Import a .cgc bundle into the current database. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `bundle_load(bundle_name: str = typer.Argument(..., help="Bundle name or path to load (e.g., 'numpy' or 'numpy.cgc')"), clear: bool = typer.Option(False, "--clear", help="Clear existing graph data before loading"), yes: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation when using --clear"))` — [`L734`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L734) — Load a pre-indexed bundle (download if needed, then import). — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `bundle_merge(ancestor: str = typer.Argument(..., help="Common ancestor version of the bundle (%O)"), current: str = typer.Argument(..., help="Current branch version of the bundle (%A); also the merge result"), other: str = typer.Argument(..., help="Other branch version of the bundle (%B)"))` — [`L797`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L797) — Git merge driver for .cgc bundle files.
- `clean(context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1338`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1338) — Remove orphaned nodes and relationships from the database.
- `config_db(backend: str = typer.Argument(..., help="Database backend: 'neo4j', 'falkordb', 'falkordb-remote', 'kuzudb', or 'ladybugdb'"))` — [`L579`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L579) — Quickly switch the default database backend.
- `config_reset()` — [`L566`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L566) — Reset all configuration to default values.
- `config_set(key: str = typer.Argument(..., help="Configuration key to set"), value: str = typer.Argument(..., help="Value to set"))` — [`L549`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L549) — Set a configuration value.
- `config_show()` — [`L539`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L539) — Display current configuration settings.
- `context_create(name: str = typer.Argument(..., help="Name of the new context"), database: str = typer.Option(None, "--database", "--db", "-db", "-d", help=config_manager.DATABASE_CLI_HELP), db_path: str = typer.Option(None, "--db-path", help="Explicit path for the DB (defaults to ~/.codegraphcontext/contexts/<name>/db)"))` — [`L257`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L257) — Create a new logical context. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `context_default(name: str = typer.Argument(..., help="Name of the context to set as default"))` — [`L283`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L283) — Set the default named context (used when --context is omitted in named mode).
- `context_delete(name: str = typer.Argument(..., help="Name of the context to delete"))` — [`L268`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L268) — Delete a context from the registry.
- `context_list()` — [`L227`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L227) — List all available contexts and current mode. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `context_mode(mode: str = typer.Argument(..., help="Mode to switch to (global, per-repo, named)"))` — [`L276`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L276) — Set the system-wide context mode.
- `cypher_legacy(query: str = typer.Argument(..., help="The read-only Cypher query to execute."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2796`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2796) — [Deprecated] Use 'cgc query' instead.
- `datasource_cassandra(ctx: typer.Context, host: str = typer.Option(..., "--host", "-H", help="Cassandra contact point (comma-separated for multiple)"), port: int = typer.Option(9042, "--port", "-p", help="Cassandra native transport port"), keyspace: str = typer.Option(..., "--keyspace", "-k", help="Keyspace to ingest"), username: Optional[str] = typer.Option(None, "--user", "-u", help="Cassandra username"), password: Optional[str] = typer.Option(None, "--password", "-P", help="Cassandra password", hide_input=True), name: Optional[str] = typer.Option(None, "--name", "-n", help="Logical datasource name (default: cassandra-<keyspace>)"), env: str = typer.Option("production", "--env", "-e", help="Deployment environment label"), context: Optional[str] = typer.Option(None, "--context", "-c", help="CGC context to use"))` — [`L2998`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2998) — Ingest Cassandra keyspace schema (tables + columns) and write to the code graph. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `datasource_mysql(ctx: typer.Context, host: str = typer.Option(..., "--host", "-H", help="MySQL host / Aurora endpoint"), port: int = typer.Option(3306, "--port", "-p", help="MySQL port"), user: str = typer.Option(..., "--user", "-u", help="MySQL username"), password: str = typer.Option(..., "--password", "-P", help="MySQL password", hide_input=True), database: str = typer.Option(..., "--database", "-d", help="Database / schema name"), name: Optional[str] = typer.Option(None, "--name", "-n", help="Logical datasource name (default: mysql-<database>)"), env: str = typer.Option("production", "--env", "-e", help="Deployment environment label"), context: Optional[str] = typer.Option(None, "--context", "-c", help="CGC context to use"))` — [`L2961`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2961) — Ingest Aurora MySQL schema (tables + columns) and write to the code graph.
- `datasource_redis(ctx: typer.Context, host: str = typer.Option(..., "--host", "-H", help="Redis host"), port: int = typer.Option(6379, "--port", "-p", help="Redis port"), db: int = typer.Option(0, "--db", help="Redis database index"), password: Optional[str] = typer.Option(None, "--password", "-P", help="Redis AUTH password", hide_input=True), name: Optional[str] = typer.Option(None, "--name", "-n", help="Logical datasource name"), env: str = typer.Option("production", "--env", "-e", help="Deployment environment label"), max_keys: int = typer.Option(10000, "--max-keys", help="Maximum keys to scan (avoid full scan in large clusters)"), context: Optional[str] = typer.Option(None, "--context", "-c", help="CGC context to use"))` — [`L3036`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L3036) — Discover Redis key patterns and write to the code graph. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `delete(path: Optional[str] = typer.Argument(None, help="Path of the repository to delete from the code graph."), all_repos: bool = typer.Option(False, "--all", help="Delete all indexed repositories"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1377`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1377) — Deletes a repository from the code graph. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `delete_abbrev(path: Optional[str] = typer.Argument(None, help="Path to delete"), all_repos: bool = typer.Option(False, "--all", help="Delete all indexed repositories"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2827`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2827) — Shortcut for 'cgc delete'
- `doctor()` — [`L1052`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1052) — Run diagnostics to check system health and configuration. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `export_shortcut(output: str = typer.Argument(..., help="Output path for the .cgc bundle file"), repo: Optional[str] = typer.Option(None, "--repo", "-r", help="Specific repository path to export"), no_stats: bool = typer.Option(False, "--no-stats", help="Skip generating statistics in the bundle"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L910`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L910) — Shortcut for 'cgc bundle export'
- `find_by_argument_search(argument: str = typer.Argument(..., help="Argument/parameter name to search for"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2078`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2078) — Find functions that take a specific argument/parameter. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `find_by_content_search(query: str = typer.Argument(..., help="Text to search for in source code and docstrings"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1972`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1972) — Search code content (source and docstrings) using full-text index.
- `find_by_decorator_search(decorator: str = typer.Argument(..., help="Decorator name to search for"), file: Optional[str] = typer.Option(None, "--file", "-f", help="Specific file path"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2030`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2030) — Find functions with a specific decorator.
- `find_by_name(ctx: typer.Context, name: str = typer.Argument(..., help="Name to search for"), type: Optional[str] = typer.Option(None, "--type", "-t", help="Filter by type (function, class, file, module)"), fuzzy: Optional[bool] = typer.Option(None, "--fuzzy/--no-fuzzy", help="Enable/disable fuzzy matching for this command. Overrides the FUZZY_SEARCH config value (default: true)."), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1637`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1637) — Find code elements by name. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `find_by_pattern(ctx: typer.Context, pattern: str = typer.Argument(..., help="Substring pattern to search (fuzzy search fallback)"), case_sensitive: bool = typer.Option(False, "--case-sensitive", "-C", help="Case-sensitive search"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1774`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1774) — Find code elements using substring matching. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `find_by_type(ctx: typer.Context, element_type: str = typer.Argument(..., help="Type to search for (function, class, file, module)"), limit: int = typer.Option(50, "--limit", "-l", help="Maximum results to return"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1867`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1867) — Find all elements of a specific type. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `find_by_variable(name: str = typer.Argument(..., help="Variable name to search for"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1926`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1926) — Find variables by name.
- `get_version()` — [`L93`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L93) — Try to read version from the installed package metadata.
- `help(ctx: typer.Context)` — [`L2859`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2859) — Show the main help message and exit.
- `hook_install(path: str = typer.Argument(".", help="Path inside the Git repository"), force: bool = typer.Option(False, "--force", "-f", help="Replace existing non-CGC hook files"))` — [`L852`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L852) — Install CGC-managed Git hooks in the nearest repository. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `hook_status(path: str = typer.Argument(".", help="Path inside the Git repository"))` — [`L887`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L887) — Show whether CGC-managed Git hooks are installed. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `hook_uninstall(path: str = typer.Argument(".", help="Path inside the Git repository"))` — [`L873`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L873) — Remove CGC-managed Git hooks and local merge-driver config. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `index(path: Optional[str] = typer.Argument(None, help="Path to the directory or file to index. Defaults to the current directory."), force: bool = typer.Option(False, "--force", "-f", help="Force re-index (delete existing and rebuild)"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use (overrides mode/default)"))` — [`L1299`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1299) — Indexes a directory or file by adding it to the code graph. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `index_abbrev(path: Optional[str] = typer.Argument(None, help="Path to index"), force: bool = typer.Option(False, "--force", "-f", help="Force re-index (delete existing and rebuild)"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2811`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2811) — Shortcut for 'cgc index'
- `list_abbrev(context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2820`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2820) — Shortcut for 'cgc list'
- `list_repositories(context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1532`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1532) — List all indexed repositories.
- `load_shortcut(bundle_name: str = typer.Argument(..., help="Bundle name or path to load"), clear: bool = typer.Option(False, "--clear", help="Clear existing graph data before loading"), yes: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation when using --clear"))` — [`L920`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L920) — Shortcut for 'cgc bundle load'
- `main(ctx: typer.Context, database: Optional[str] = typer.Option(None, "--database", "--db", "-db", help="[Global] Temporarily override database backend (" + "|".join(config_manager.SUPPORTED_DATABASES) + ") for any command"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="[Global] Show results as interactive graph visualization in browser"), version_: bool = typer.Option(None, "--version", "-v", help="[Root-level only] Show version and exit", is_eager=True), help_: bool = typer.Option(None, "--help", "-h", help="[Root-level only] Show help and exit", is_eager=True), db_path: Optional[str] = typer.Option(None, "--path", "--db-path", help="[Global] Temporarily override database path (for local DBs like KuzuDB)"))` — [`L2872`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2872) — Main entry point for the cgc CLI application.
- `mcp_setup()` — [`L109`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L109) — Configure MCP Client (IDE/CLI Integration).
- `mcp_setup_alias()` — [`L189`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L189) — Shortcut for 'cgc mcp setup'
- `mcp_start()` — [`L126`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L126) — Start the CodeGraphContext MCP server. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `mcp_tools()` — [`L157`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L157) — List all available MCP tools.
- `neo4j_setup()` — [`L199`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L199) — Configure Neo4j Database Connection.
- `neo4j_setup_alias()` — [`L217`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L217) — Shortcut for 'cgc neo4j setup'
- `query_graph(ctx: typer.Context, query: str = typer.Argument(..., help="Cypher query to execute (read-only)"), visual: bool = typer.Option(False, "--visual", "--viz", "-V", help="Show results as interactive graph visualization"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2772`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2772) — Execute a custom Cypher query on the code graph. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `registry_callback(ctx: typer.Context)` — [`L963`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L963) — Browse and download bundles from the registry.
- `registry_download(name: str = typer.Argument(..., help="Bundle name to download (e.g., 'numpy')"), output_dir: Optional[str] = typer.Option(None, "--output", "-o", help="Output directory (default: current directory)"), load: bool = typer.Option(False, "--load", "-l", help="Automatically load the bundle after downloading"))` — [`L1005`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1005) — Download a bundle from the registry.
- `registry_list(verbose: bool = typer.Option(False, "--verbose", "-v", help="Show detailed information including download URLs"), unique: bool = typer.Option(False, "--unique", "-u", help="Show only one version per package (most recent)"))` — [`L969`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L969) — List all available bundles in the registry.
- `registry_request(repo_url: str = typer.Argument(..., help="GitHub repository URL to index"), wait: bool = typer.Option(False, "--wait", "-w", help="Wait for generation to complete (not yet implemented)"))` — [`L1030`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1030) — Request on-demand generation of a bundle.
- `registry_search(query: str = typer.Argument(..., help="Search query (matches name, repository, or description)"))` — [`L988`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L988) — Search for bundles in the registry.
- `report(output: Optional[str] = typer.Option(None, "--output", "-o", help="Output file path. Defaults to CGC_REPORT.md in the current directory."), java: bool = typer.Option(False, "--java", "-j", help="Include Spring/Maven Java sections."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1481`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1481) — Generate a CGC_REPORT.md with god nodes, complexity, cross-module connections, and suggested queries.
- `setup_scip()` — [`L1367`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1367) — Check availability of SCIP indexers and provide installation hints.
- `stats(path: Optional[str] = typer.Argument(None, help="Path to show stats for. Omit for overall stats."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1351`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1351) — Show indexing statistics.
- `unwatch(path: str = typer.Argument(..., help="Path to stop watching"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1595`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1595) — Stop watching a directory for changes.
- `update(path: Optional[str] = typer.Argument(None, help="Path to refresh. Defaults to current directory."), quiet: bool = typer.Option(False, "--quiet", "-q", help="Reduce output when running from automation"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use (overrides mode/default)"))` — [`L1321`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1321) — Refresh an existing repository index.
- `version_cmd()` — [`L2866`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2866) — Show the application version.
- `visualize(repo: Optional[str] = typer.Option(None, "--repo", "-r", help="Path to the repository to visualize."), port: int = typer.Option(8000, "--port", "-p", help="Port to run the visualizer server on."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1520`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1520) — Launches the interactive UI to visualize the code graph.
- `visualize_abbrev(repo: Optional[str] = typer.Argument(None, help="Path to the repository to visualize."), port: int = typer.Option(8000, "--port", "-p", help="Port to run the visualizer server on."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2836`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2836) — Shortcut for 'cgc visualize'
- `watch(path: str = typer.Argument(".", help="Path to the directory to watch. Defaults to current directory."), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"), poll: bool = typer.Option(False, "--poll", help="Use watchdog's polling observer for Docker bind mounts and network filesystems."))` — [`L1560`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1560) — Watch a directory for file changes and automatically update the code graph.
- `watch_abbrev(path: str = typer.Argument(".", help="Path to watch"), context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L2846`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2846) — Shortcut for 'cgc watch'
- `watching(context: Optional[str] = typer.Option(None, "--context", "-c", help="Specific context to use"))` — [`L1612`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1612) — List all directories currently being watched for changes.

## Module values
- `analyze_app` — [`L2127`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2127) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `api_app` — [`L940`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L940)
- `app` — [`L81`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L81) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `bundle_app` — [`L607`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L607) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `config_app` — [`L535`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L535) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `console` — [`L86`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L86) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `context_app` — [`L223`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L223) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `datasource_app` — [`L2956`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L2956)
- `find_app` — [`L1633`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L1633) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `hook_app` — [`L847`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L847)
- `mcp_app` — [`L105`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L105)
- `neo4j_app` — [`L195`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L195)
- `registry_app` — [`L932`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/main.py#L932) — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)

