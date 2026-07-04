---
title: 'Module: src/codegraphcontext/cli/cli_helpers.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/cli_helpers.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.cli_helpers`/
symbols:
  console: console.
  _initialize_services: _initialize_services().
  _run_index_with_progress: _run_index_with_progress().
  watch_helper: watch_helper().
  index_helper: index_helper().
  reindex_helper: reindex_helper().
  visualize_helper: visualize_helper().
  add_package_helper: add_package_helper().
  cypher_helper_visual: cypher_helper_visual().
  _fail_services_init: _fail_services_init().
  cypher_helper: cypher_helper().
  clean_helper: clean_helper().
  _kuzu_fallback_path: _kuzu_fallback_path().
  list_repos_helper: list_repos_helper().
  delete_helper: delete_helper().
  update_helper: update_helper().
  stats_helper: stats_helper().
  _print_call_resolution_diagnostics: _print_call_resolution_diagnostics().
  setup_scip_helper: setup_scip_helper().
  _print_query_exception: _print_query_exception().
  unwatch_helper: unwatch_helper().
  list_watching_helper: list_watching_helper().
  watch_helper.do_index: watch_helper().do_index().
  visualize_helper.open_browser: visualize_helper().open_browser().
---
# Module: [`src/codegraphcontext/cli/cli_helpers.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py)

## Functions
- `_fail_services_init()` — [`L44`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L44) — Abort the CLI command when database/services could not be initialized. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `_initialize_services(cli_context_flag: Optional[str] = None, cwd: Optional[Path] = None)` — [`L88`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L88) — Initializes and returns core service managers based on the resolved context. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `_kuzu_fallback_path(ctx: ResolvedContext)` — [`L49`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L49) — Derive a KùzuDB directory when falling back from another backend.
- `_print_call_resolution_diagnostics(graph_builder: GraphBuilder, limit: int = 5)` — [`L63`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L63)
- `_print_query_exception(e: Exception, query: str)` — [`L423`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L423) — Pretty-print a database query exception, surfacing the raw driver
- `_run_index_with_progress(graph_builder: GraphBuilder, path_obj: Path, is_dependency: bool = False, cgcignore_path: str = None)` — [`L202`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L202) — Internal helper to run indexing with a Live progress bar. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `add_package_helper(package_name: str, language: str, context: Optional[str] = None)` — [`L339`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L339) — Synchronously indexes a package. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `clean_helper(context: Optional[str] = None)` — [`L694`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L694) — Remove orphaned nodes and relationships from the database.
- `cypher_helper(query: str, context: Optional[str] = None)` — [`L467`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L467) — Executes a read-only Cypher query. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `cypher_helper_visual(query: str, context: Optional[str] = None)` — [`L498`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L498) — Executes a read-only Cypher query and visualizes the results. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `delete_helper(repo_path: str, context: Optional[str] = None)` — [`L404`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L404) — Deletes a repository from the graph.
- `do_index()` — [`L927`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L927)
- `index_helper(path: str, context: Optional[str] = None)` — [`L260`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L260) — Synchronously indexes a repository in a given context. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `list_repos_helper(context: Optional[str] = None)` — [`L374`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L374) — Lists all indexed repositories.
- `list_watching_helper()` — [`L974`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L974) — List all directories currently being watched.
- `open_browser()` — [`L614`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L614)
- `reindex_helper(path: str, context: Optional[str] = None)` — [`L632`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L632) — Force re-index by deleting and rebuilding the repository. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `setup_scip_helper()` — [`L983`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L983) — Diagnostic and setup helper for SCIP indexers.
- `stats_helper(path: str = None, context: Optional[str] = None)` — [`L748`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L748) — Show indexing statistics for a repository or overall.
- `unwatch_helper(path: str)` — [`L967`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L967) — Stop watching a directory.
- `update_helper(path: str, context: Optional[str] = None, quiet: bool = False)` — [`L677`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L677) — Update/refresh index for a path (alias for reindex).
- `visualize_helper(repo_path: Optional[str] = None, port: int = 8000, context: Optional[str] = None, cypher_query: Optional[str] = None)` — [`L528`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L528) — Generates an interactive visualization using the Playground UI. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `watch_helper(path: str, context: Optional[str] = None, use_polling: Optional[bool] = None)` — [`L853`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L853) — Watch a directory for changes and auto-update the graph (blocking mode). — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)

## Module values
- `console` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/cli_helpers.py#L41)

